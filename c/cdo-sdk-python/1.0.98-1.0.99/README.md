# Comparing `tmp/cdo-sdk-python-1.0.98.tar.gz` & `tmp/cdo-sdk-python-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdo-sdk-python-1.0.98.tar", last modified: Tue Apr 23 10:12:59 2024, max compression
+gzip compressed data, was "cdo-sdk-python-1.0.99.tar", last modified: Tue Apr 23 16:16:53 2024, max compression
```

## Comparing `cdo-sdk-python-1.0.98.tar` & `cdo-sdk-python-1.0.99.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 10:12:59.193827 cdo-sdk-python-1.0.98/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3710 2024-04-23 10:12:59.193827 cdo-sdk-python-1.0.98/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    19643 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/README.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 10:12:59.169827 cdo-sdk-python-1.0.98/cdo_sdk_python/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8262 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 10:12:59.173827 cdo-sdk-python-1.0.98/cdo_sdk_python/api/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      899 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    47620 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/change_requests_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    28767 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/changelogs_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    56491 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/cloud_delivered_fmc_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    58557 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/connectors_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   306892 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/inventory_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    29653 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/meta_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)   114554 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/object_management_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    85076 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/remote_access_monitoring_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21766 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/search_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    65201 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/tenant_management_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12108 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/transactions_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    88351 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api/users_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25780 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api_client.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      652 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/api_response.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15728 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/configuration.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5960 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/exceptions.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 10:12:59.181827 cdo-sdk-python-1.0.98/cdo_sdk_python/models/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6866 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/__init__.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2573 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/api_token_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4405 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/asa_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3247 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/asa_failover_mate.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      817 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/asa_failover_mode.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2829 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/authentication_error.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2777 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/browser.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3957 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cd_fmc_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2915 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cd_fmc_object.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4212 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cd_fmc_result.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2925 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_region.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2970 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_region_list.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3682 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_token_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5385 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_transaction.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      824 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_transaction_status.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1396 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_transaction_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2836 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/change_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2765 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/change_request_create_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3633 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/change_request_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3825 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/changelog.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3600 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/changelog_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4457 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/client_device.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3859 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/common_api_error.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1093 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/config_state.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      962 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/conflict_detection_interval.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      871 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/conflict_detection_state.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1034 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/connectivity_state.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      900 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/connector_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3667 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/create_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10847 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/device.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3576 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/device_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2923 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/device_patch_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      886 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/device_role.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3582 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3335 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/entity.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1368 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/entity_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4295 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/event.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5099 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/ftd_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2630 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/ftd_registration_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4091 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/global_search_result.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3305 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/group_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6055 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/icmp4_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6373 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/icmp6_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4152 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/inventory.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4097 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/ios_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2771 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/issues_dto.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3295 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/json_web_key.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2941 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/jwk_set.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2898 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/labels.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3746 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/list_object_response.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2961 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/location.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      814 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/meraki_deployment_mode.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2709 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/meta.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4550 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/mfa_event.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3593 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/mfa_event_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2566 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/msp_add_tenant_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3061 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/network.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2579 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/network_object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7106 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5804 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/object_response.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2860 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/on_prem_fmc_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2765 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/os.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3096 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/override.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2726 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/policy.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3074 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/ports_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2980 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/public_key.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5950 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/ra_vpn_session.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3626 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/ra_vpn_session_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3374 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/reference_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4507 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3552 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3024 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc_public_key.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      876 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc_status.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5575 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/service_object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5970 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/service_object_value_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4175 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/shared_object_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6324 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/single_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3016 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/state_machine_details.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2885 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/state_machine_error.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      835 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/status.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2543 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/status_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3638 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/target.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2632 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/targets_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3496 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3576 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      886 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant_pay_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4856 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant_settings.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3966 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/unified_object_list_view.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3418 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/update_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2510 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/url_object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3477 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/user.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3001 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/user_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3560 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/user_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1003 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/models/user_role.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9220 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/cdo_sdk_python/rest.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 10:12:59.169827 cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3710 2024-04-23 10:12:59.000000 cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7698 2024-04-23 10:12:59.000000 cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-04-23 10:12:59.000000 cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       76 2024-04-23 10:12:59.000000 cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       15 2024-04-23 10:12:59.000000 cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1911 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/pyproject.toml
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       69 2024-04-23 10:12:59.193827 cdo-sdk-python-1.0.98/setup.cfg
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1203 2024-04-23 10:12:47.000000 cdo-sdk-python-1.0.98/setup.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 10:12:59.193827 cdo-sdk-python-1.0.98/test/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1394 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_api_token_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2145 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_asa_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_asa_failover_mate.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      742 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_asa_failover_mode.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1537 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_authentication_error.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1367 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_browser.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cd_fmc_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1656 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cd_fmc_object.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2733 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cd_fmc_result.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1411 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cdo_region.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1601 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cdo_region_list.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1680 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cdo_token_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2223 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cdo_transaction.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      777 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cdo_transaction_status.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      763 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cdo_transaction_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1638 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_change_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1670 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_change_request_create_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1815 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_change_request_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1286 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_change_requests_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_changelog.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2375 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_changelog_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      930 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_changelogs_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2124 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_client_device.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1840 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_cloud_delivered_fmc_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1496 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_common_api_error.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      713 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_config_state.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      812 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_conflict_detection_interval.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      791 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_conflict_detection_state.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      755 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_connectivity_state.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      727 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_connector_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      891 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_connectors_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2387 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_create_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4246 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_device.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4829 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_device_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1673 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_device_patch_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      706 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_device_role.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2241 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_duo_admin_panel_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1581 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_entity.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      706 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_entity_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1641 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_event.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2116 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_ftd_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1580 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_ftd_registration_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3885 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_global_search_result.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1559 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_group_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1431 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_icmp4_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1435 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_icmp6_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2735 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_inventory.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4407 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_inventory_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2107 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_ios_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1399 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_issues_dto.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1480 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_json_web_key.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1601 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_jwk_set.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1444 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_labels.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2746 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_list_object_response.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1404 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_location.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      777 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_meraki_deployment_mode.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1340 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_meta.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1031 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_meta_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2627 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_mfa_event.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2956 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_mfa_event_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1497 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_msp_add_tenant_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1413 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_network.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1524 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_network_object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1835 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1738 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_object_management_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2653 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_object_response.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1466 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_on_prem_fmc_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1302 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_os.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1470 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_override.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1384 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_policy.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1394 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_ports_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2171 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_public_key.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2451 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_ra_vpn_session.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2694 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_ra_vpn_session_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1478 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_reference_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1427 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_remote_access_monitoring_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2530 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_sdc.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2803 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_sdc_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2208 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_sdc_public_key.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      699 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_sdc_status.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      908 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_search_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1542 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_service_object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1785 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_service_object_value_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1770 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_shared_object_value.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1629 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_single_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1685 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_state_machine_details.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1521 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_state_machine_error.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      677 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_status.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1358 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_status_info.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1412 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_target.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1449 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_targets_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1567 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_tenant.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1530 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_tenant_management_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1853 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_tenant_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      728 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_tenant_pay_type.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1838 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_tenant_settings.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      810 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_transactions_api.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2357 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_unified_object_list_view.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1918 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_update_request.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1496 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_url_object_content.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1504 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_user.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1656 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_user_create_or_update_input.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1786 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_user_page.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      692 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_user_role.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1724 2024-04-23 10:12:42.000000 cdo-sdk-python-1.0.98/test/test_users_api.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 16:16:53.268671 cdo-sdk-python-1.0.99/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3710 2024-04-23 16:16:53.268671 cdo-sdk-python-1.0.99/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    19643 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/README.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 16:16:53.244671 cdo-sdk-python-1.0.99/cdo_sdk_python/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8262 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 16:16:53.248671 cdo-sdk-python-1.0.99/cdo_sdk_python/api/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      899 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    47620 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/change_requests_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    28767 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/changelogs_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    56491 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/cloud_delivered_fmc_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    58557 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/connectors_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   306892 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/inventory_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    29653 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/meta_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)   114554 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/object_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    85076 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/remote_access_monitoring_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    21766 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/search_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    65201 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/tenant_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12108 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/transactions_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    88351 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api/users_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25780 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api_client.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      652 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/api_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15728 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/configuration.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5960 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/exceptions.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 16:16:53.256671 cdo-sdk-python-1.0.99/cdo_sdk_python/models/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6866 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2573 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/api_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4405 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/asa_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3247 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/asa_failover_mate.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      817 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/asa_failover_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2829 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/authentication_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2777 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/browser.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3957 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cd_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2915 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cd_fmc_object.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4212 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cd_fmc_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2925 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_region.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2970 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_region_list.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3682 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5594 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_transaction.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      824 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_transaction_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1396 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_transaction_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2836 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/change_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2765 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/change_request_create_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3633 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/change_request_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3825 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/changelog.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3600 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/changelog_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4457 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/client_device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3859 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/common_api_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1093 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/config_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      962 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/conflict_detection_interval.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      871 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/conflict_detection_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1034 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/connectivity_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      900 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/connector_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3667 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/create_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10847 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3576 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/device_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2923 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/device_patch_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      886 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/device_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3582 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3335 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/entity.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1368 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/entity_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4295 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5099 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/ftd_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2630 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/ftd_registration_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4091 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/global_search_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3305 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/group_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6055 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/icmp4_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6373 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/icmp6_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4152 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/inventory.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4097 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/ios_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2771 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/issues_dto.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3295 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/json_web_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2941 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/jwk_set.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2898 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/labels.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3746 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/list_object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2961 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/location.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      814 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/meraki_deployment_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2709 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/meta.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4550 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/mfa_event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3593 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/mfa_event_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2566 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/msp_add_tenant_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3061 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/network.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2579 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/network_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7106 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5804 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2860 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/on_prem_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2765 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/os.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3096 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/override.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2726 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/policy.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3074 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/ports_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2980 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5950 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/ra_vpn_session.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3626 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/ra_vpn_session_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3374 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/reference_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4507 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3552 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3024 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc_public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      876 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5575 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/service_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5970 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/service_object_value_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4175 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/shared_object_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6324 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/single_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3016 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/state_machine_details.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2885 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/state_machine_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      835 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2543 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/status_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3638 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/target.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2632 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/targets_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3496 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3576 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      886 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant_pay_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4856 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant_settings.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3966 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/unified_object_list_view.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3418 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/update_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2510 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/url_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3477 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/user.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3001 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/user_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3560 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/user_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1003 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/models/user_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9220 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/cdo_sdk_python/rest.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 16:16:53.244671 cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3710 2024-04-23 16:16:53.000000 cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7698 2024-04-23 16:16:53.000000 cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2024-04-23 16:16:53.000000 cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       76 2024-04-23 16:16:53.000000 cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       15 2024-04-23 16:16:53.000000 cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1911 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/pyproject.toml
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       69 2024-04-23 16:16:53.268671 cdo-sdk-python-1.0.99/setup.cfg
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1203 2024-04-23 16:16:42.000000 cdo-sdk-python-1.0.99/setup.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2024-04-23 16:16:53.268671 cdo-sdk-python-1.0.99/test/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1394 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_api_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2145 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_asa_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_asa_failover_mate.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      742 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_asa_failover_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1537 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_authentication_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1367 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_browser.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cd_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1656 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cd_fmc_object.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2733 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cd_fmc_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1411 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cdo_region.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1601 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cdo_region_list.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1680 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cdo_token_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2223 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cdo_transaction.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      777 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cdo_transaction_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      763 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cdo_transaction_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1638 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_change_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1670 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_change_request_create_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1815 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_change_request_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1286 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_change_requests_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_changelog.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2375 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_changelog_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      930 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_changelogs_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2124 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_client_device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1840 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_cloud_delivered_fmc_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1496 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_common_api_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      713 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_config_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      812 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_conflict_detection_interval.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      791 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_conflict_detection_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      755 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_connectivity_state.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      727 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_connector_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      891 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_connectors_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2387 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_create_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4246 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_device.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4829 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_device_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1673 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_device_patch_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      706 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_device_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2241 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_duo_admin_panel_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1581 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_entity.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      706 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_entity_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1641 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2116 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_ftd_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1580 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_ftd_registration_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3885 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_global_search_result.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1559 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_group_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1431 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_icmp4_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1435 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_icmp6_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2735 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_inventory.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4407 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_inventory_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2107 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_ios_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1399 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_issues_dto.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1480 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_json_web_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1601 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_jwk_set.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1444 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_labels.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2746 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_list_object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1404 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_location.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      777 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_meraki_deployment_mode.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1340 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_meta.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1031 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_meta_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2627 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_mfa_event.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2956 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_mfa_event_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1497 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_msp_add_tenant_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1413 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_network.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1524 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_network_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1835 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1738 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_object_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2653 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_object_response.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1466 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_on_prem_fmc_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1302 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_os.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1470 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_override.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1384 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_policy.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1394 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_ports_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2171 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2451 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_ra_vpn_session.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2694 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_ra_vpn_session_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1478 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_reference_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1427 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_remote_access_monitoring_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2530 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_sdc.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2803 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_sdc_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2208 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_sdc_public_key.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      699 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_sdc_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      908 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_search_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1542 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_service_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1785 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_service_object_value_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1770 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_shared_object_value.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1629 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_single_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1685 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_state_machine_details.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1521 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_state_machine_error.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      677 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_status.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1358 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_status_info.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1412 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_target.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1449 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_targets_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1567 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_tenant.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1530 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_tenant_management_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1853 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_tenant_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      728 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_tenant_pay_type.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1838 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_tenant_settings.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      810 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_transactions_api.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2357 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_unified_object_list_view.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1918 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_update_request.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1496 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_url_object_content.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1504 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_user.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1656 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_user_create_or_update_input.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1786 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_user_page.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      692 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_user_role.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1724 2024-04-23 16:16:35.000000 cdo-sdk-python-1.0.99/test/test_users_api.py
```

### Comparing `cdo-sdk-python-1.0.98/PKG-INFO` & `cdo-sdk-python-1.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdo-sdk-python
-Version: 1.0.98
+Version: 1.0.99
 Summary: CDO API
 Home-page: UNKNOWN
 Author: CDO TAC
 Author-email: cdo.tac@cisco.com
 License: UNKNOWN
 Description: # Cisco Defense Orchestrator (CDO) Python SDK
         The CDO Python SDK facilitates automated interaction with the Cisco Defense Orchestrator (CDO) API, enabling developers to integrate Cisco's cloud-based security policy and device management into Python applications.
```

### Comparing `cdo-sdk-python-1.0.98/README.md` & `cdo-sdk-python-1.0.99/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # cdo-sdk-python
 Use the documentation to explore the endpoints CDO has to offer
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 0.1.0
-- Package version: 1.0.98
+- Package version: 1.0.99
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/__init__.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: cdo.tac@cisco.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.98"
+__version__ = "1.0.99"
 
 # import apis into sdk package
 from cdo_sdk_python.api.change_requests_api import ChangeRequestsApi
 from cdo_sdk_python.api.changelogs_api import ChangelogsApi
 from cdo_sdk_python.api.cloud_delivered_fmc_api import CloudDeliveredFMCApi
 from cdo_sdk_python.api.command_line_interface_api import CommandLineInterfaceApi
 from cdo_sdk_python.api.connectors_api import ConnectorsApi
```

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/__init__.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/change_requests_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/change_requests_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/changelogs_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/changelogs_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/cloud_delivered_fmc_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/cloud_delivered_fmc_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/connectors_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/connectors_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/inventory_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/inventory_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/meta_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/meta_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/object_management_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/object_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/remote_access_monitoring_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/remote_access_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/search_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/search_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/tenant_management_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/transactions_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api/users_api.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api/users_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api_client.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.98/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.99/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/api_response.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/api_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/configuration.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 0.1.0\n"\
-               "SDK Package Version: 1.0.98".\
+               "SDK Package Version: 1.0.99".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/exceptions.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/exceptions.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/__init__.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/api_token_info.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/api_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/asa_create_or_update_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/asa_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/asa_failover_mate.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/asa_failover_mate.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/asa_failover_mode.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/asa_failover_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/authentication_error.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/authentication_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/browser.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/browser.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cd_fmc_info.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cd_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cd_fmc_object.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cd_fmc_object.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cd_fmc_result.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cd_fmc_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_region.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_region.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_region_list.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_region_list.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_token_info.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_transaction.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,28 @@
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CdoTransaction(BaseModel):
     """
     CdoTransaction
     """ # noqa: E501
-    transaction_uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the asynchronous transaction triggered.", alias="transactionUid")
     tenant_uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the tenant that asynchronous transaction triggered on.", alias="tenantUid")
+    sort_key: Optional[StrictStr] = Field(default=None, description="DynamoDB sort key to provide us with efficient query capabilities.", alias="sortKey")
+    transaction_uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the asynchronous transaction triggered.", alias="transactionUid")
     entity_uid: Optional[StrictStr] = Field(default=None, description="The unique identifier of the entity that the asynchronous transaction is triggered on.", alias="entityUid")
     entity_url: Optional[StrictStr] = Field(default=None, description="A URL to access the entity that the asynchronous transaction is triggered on.", alias="entityUrl")
     transaction_polling_url: Optional[StrictStr] = Field(default=None, description="The URL to poll to track the progress of the transaction.", alias="transactionPollingUrl")
     submission_time: Optional[datetime] = Field(default=None, description="The time (UTC; represented using the RFC-3339 standard) at which the transaction was triggered", alias="submissionTime")
     last_updated_time: Optional[datetime] = Field(default=None, description="The time (UTC; represented using the RFC-3339 standard) at which the transaction status was last updated", alias="lastUpdatedTime")
     transaction_type: Optional[CdoTransactionType] = Field(default=None, alias="transactionType")
     cdo_transaction_status: Optional[CdoTransactionStatus] = Field(default=None, alias="cdoTransactionStatus")
     error_message: Optional[StrictStr] = Field(default=None, description="Transaction error message, if any", alias="errorMessage")
     error_details: Optional[Dict[str, StrictStr]] = Field(default=None, description="Transaction error details, if any", alias="errorDetails")
     expire_at: Optional[StrictInt] = Field(default=None, description="TTL attribute detailing the expiry time this item should be deleted", alias="expireAt")
-    __properties: ClassVar[List[str]] = ["transactionUid", "tenantUid", "entityUid", "entityUrl", "transactionPollingUrl", "submissionTime", "lastUpdatedTime", "transactionType", "cdoTransactionStatus", "errorMessage", "errorDetails", "expireAt"]
+    __properties: ClassVar[List[str]] = ["tenantUid", "sortKey", "transactionUid", "entityUid", "entityUrl", "transactionPollingUrl", "submissionTime", "lastUpdatedTime", "transactionType", "cdoTransactionStatus", "errorMessage", "errorDetails", "expireAt"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -91,16 +92,17 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "transactionUid": obj.get("transactionUid"),
             "tenantUid": obj.get("tenantUid"),
+            "sortKey": obj.get("sortKey"),
+            "transactionUid": obj.get("transactionUid"),
             "entityUid": obj.get("entityUid"),
             "entityUrl": obj.get("entityUrl"),
             "transactionPollingUrl": obj.get("transactionPollingUrl"),
             "submissionTime": obj.get("submissionTime"),
             "lastUpdatedTime": obj.get("lastUpdatedTime"),
             "transactionType": obj.get("transactionType"),
             "cdoTransactionStatus": obj.get("cdoTransactionStatus"),
```

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_transaction_status.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_transaction_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/cdo_transaction_type.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/cdo_transaction_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/change_request.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/change_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/change_request_create_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/change_request_create_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/change_request_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/change_request_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/changelog.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/changelog.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/changelog_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/changelog_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/client_device.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/client_device.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/common_api_error.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/common_api_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/config_state.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/config_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/conflict_detection_interval.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/conflict_detection_interval.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/conflict_detection_state.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/conflict_detection_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/connectivity_state.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/connectivity_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/connector_type.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/connector_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/create_request.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/create_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/device.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/device.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/device_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/device_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/device_patch_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/device_patch_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/device_role.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/device_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/duo_admin_panel_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/entity.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/entity.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/entity_type.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/entity_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/event.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/event.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/ftd_create_or_update_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/ftd_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/ftd_registration_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/ftd_registration_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/global_search_result.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/global_search_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/group_content.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/group_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/icmp4_value.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/icmp4_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/icmp6_value.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/icmp6_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/inventory.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/inventory.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/ios_create_or_update_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/ios_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/issues_dto.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/issues_dto.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/json_web_key.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/json_web_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/jwk_set.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/jwk_set.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/labels.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/labels.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/list_object_response.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/list_object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/location.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/location.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/meraki_deployment_mode.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/meraki_deployment_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/meta.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/meta.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/mfa_event.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/mfa_event.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/mfa_event_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/mfa_event_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/msp_add_tenant_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/msp_add_tenant_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/network.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/network.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/network_object_content.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/network_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/object_content.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/object_response.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/on_prem_fmc_info.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/on_prem_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/os.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/os.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/override.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/override.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/policy.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/policy.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/ports_value.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/ports_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/public_key.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/public_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/ra_vpn_session.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/ra_vpn_session.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/ra_vpn_session_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/ra_vpn_session_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/reference_info.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/reference_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc_public_key.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc_public_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/sdc_status.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/sdc_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/service_object_content.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/service_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/service_object_value_content.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/service_object_value_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/shared_object_value.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/shared_object_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/single_content.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/single_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/state_machine_details.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/state_machine_details.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/state_machine_error.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/state_machine_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/status.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/status_info.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/status_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/target.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/target.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/targets_request.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/targets_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant_pay_type.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant_pay_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/tenant_settings.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/tenant_settings.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/unified_object_list_view.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/unified_object_list_view.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/update_request.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/update_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/url_object_content.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/url_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/user.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/user.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/user_create_or_update_input.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/user_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/user_page.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/user_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/models/user_role.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/models/user_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python/rest.py` & `cdo-sdk-python-1.0.99/cdo_sdk_python/rest.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/PKG-INFO` & `cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdo-sdk-python
-Version: 1.0.98
+Version: 1.0.99
 Summary: CDO API
 Home-page: UNKNOWN
 Author: CDO TAC
 Author-email: cdo.tac@cisco.com
 License: UNKNOWN
 Description: # Cisco Defense Orchestrator (CDO) Python SDK
         The CDO Python SDK facilitates automated interaction with the Cisco Defense Orchestrator (CDO) API, enabling developers to integrate Cisco's cloud-based security policy and device management into Python applications.
```

### Comparing `cdo-sdk-python-1.0.98/cdo_sdk_python.egg-info/SOURCES.txt` & `cdo-sdk-python-1.0.99/cdo_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/pyproject.toml` & `cdo-sdk-python-1.0.99/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cdo_sdk_python"
-version = "1.0.98"
+version = "1.0.99"
 description = "CDO API"
 authors = ["CDO TAC <cdo.tac@cisco.com>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "CDO API"]
 include = ["cdo_sdk_python/py.typed"]
```

### Comparing `cdo-sdk-python-1.0.98/setup.py` & `cdo-sdk-python-1.0.99/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "cdo-sdk-python"
-VERSION = "1.0.98"
+VERSION = "1.0.99"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `cdo-sdk-python-1.0.98/test/test_api_token_info.py` & `cdo-sdk-python-1.0.99/test/test_api_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_asa_create_or_update_input.py` & `cdo-sdk-python-1.0.99/test/test_asa_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_asa_failover_mate.py` & `cdo-sdk-python-1.0.99/test/test_asa_failover_mate.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_asa_failover_mode.py` & `cdo-sdk-python-1.0.99/test/test_asa_failover_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_authentication_error.py` & `cdo-sdk-python-1.0.99/test/test_authentication_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_browser.py` & `cdo-sdk-python-1.0.99/test/test_browser.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cd_fmc_info.py` & `cdo-sdk-python-1.0.99/test/test_cd_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cd_fmc_object.py` & `cdo-sdk-python-1.0.99/test/test_cd_fmc_object.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cd_fmc_result.py` & `cdo-sdk-python-1.0.99/test/test_cd_fmc_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cdo_region.py` & `cdo-sdk-python-1.0.99/test/test_cdo_region.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cdo_region_list.py` & `cdo-sdk-python-1.0.99/test/test_cdo_region_list.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cdo_token_info.py` & `cdo-sdk-python-1.0.99/test/test_cdo_token_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cdo_transaction.py` & `cdo-sdk-python-1.0.99/test/test_cdo_transaction.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cdo_transaction_status.py` & `cdo-sdk-python-1.0.99/test/test_cdo_transaction_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cdo_transaction_type.py` & `cdo-sdk-python-1.0.99/test/test_cdo_transaction_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_change_request.py` & `cdo-sdk-python-1.0.99/test/test_change_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_change_request_create_input.py` & `cdo-sdk-python-1.0.99/test/test_change_request_create_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_change_request_page.py` & `cdo-sdk-python-1.0.99/test/test_change_request_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_change_requests_api.py` & `cdo-sdk-python-1.0.99/test/test_change_requests_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_changelog.py` & `cdo-sdk-python-1.0.99/test/test_changelog.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_changelog_page.py` & `cdo-sdk-python-1.0.99/test/test_changelog_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_changelogs_api.py` & `cdo-sdk-python-1.0.99/test/test_changelogs_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_client_device.py` & `cdo-sdk-python-1.0.99/test/test_client_device.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_cloud_delivered_fmc_api.py` & `cdo-sdk-python-1.0.99/test/test_cloud_delivered_fmc_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_common_api_error.py` & `cdo-sdk-python-1.0.99/test/test_common_api_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_config_state.py` & `cdo-sdk-python-1.0.99/test/test_config_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_conflict_detection_interval.py` & `cdo-sdk-python-1.0.99/test/test_conflict_detection_interval.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_conflict_detection_state.py` & `cdo-sdk-python-1.0.99/test/test_conflict_detection_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_connectivity_state.py` & `cdo-sdk-python-1.0.99/test/test_connectivity_state.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_connector_type.py` & `cdo-sdk-python-1.0.99/test/test_connector_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_connectors_api.py` & `cdo-sdk-python-1.0.99/test/test_connectors_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_create_request.py` & `cdo-sdk-python-1.0.99/test/test_create_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_device.py` & `cdo-sdk-python-1.0.99/test/test_device.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_device_page.py` & `cdo-sdk-python-1.0.99/test/test_device_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_device_patch_input.py` & `cdo-sdk-python-1.0.99/test/test_device_patch_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_device_role.py` & `cdo-sdk-python-1.0.99/test/test_device_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_duo_admin_panel_create_or_update_input.py` & `cdo-sdk-python-1.0.99/test/test_duo_admin_panel_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_entity.py` & `cdo-sdk-python-1.0.99/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_entity_type.py` & `cdo-sdk-python-1.0.99/test/test_entity_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_event.py` & `cdo-sdk-python-1.0.99/test/test_event.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_ftd_create_or_update_input.py` & `cdo-sdk-python-1.0.99/test/test_ftd_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_ftd_registration_input.py` & `cdo-sdk-python-1.0.99/test/test_ftd_registration_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_global_search_result.py` & `cdo-sdk-python-1.0.99/test/test_global_search_result.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_group_content.py` & `cdo-sdk-python-1.0.99/test/test_group_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_icmp4_value.py` & `cdo-sdk-python-1.0.99/test/test_icmp4_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_icmp6_value.py` & `cdo-sdk-python-1.0.99/test/test_icmp6_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_inventory.py` & `cdo-sdk-python-1.0.99/test/test_inventory.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_inventory_api.py` & `cdo-sdk-python-1.0.99/test/test_inventory_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_ios_create_or_update_input.py` & `cdo-sdk-python-1.0.99/test/test_ios_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_issues_dto.py` & `cdo-sdk-python-1.0.99/test/test_issues_dto.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_json_web_key.py` & `cdo-sdk-python-1.0.99/test/test_json_web_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_jwk_set.py` & `cdo-sdk-python-1.0.99/test/test_jwk_set.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_labels.py` & `cdo-sdk-python-1.0.99/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_list_object_response.py` & `cdo-sdk-python-1.0.99/test/test_list_object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_location.py` & `cdo-sdk-python-1.0.99/test/test_location.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_meraki_deployment_mode.py` & `cdo-sdk-python-1.0.99/test/test_meraki_deployment_mode.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_meta.py` & `cdo-sdk-python-1.0.99/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_meta_api.py` & `cdo-sdk-python-1.0.99/test/test_meta_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_mfa_event.py` & `cdo-sdk-python-1.0.99/test/test_mfa_event.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_mfa_event_page.py` & `cdo-sdk-python-1.0.99/test/test_mfa_event_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_msp_add_tenant_input.py` & `cdo-sdk-python-1.0.99/test/test_msp_add_tenant_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_network.py` & `cdo-sdk-python-1.0.99/test/test_network.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_network_object_content.py` & `cdo-sdk-python-1.0.99/test/test_network_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_object_content.py` & `cdo-sdk-python-1.0.99/test/test_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_object_management_api.py` & `cdo-sdk-python-1.0.99/test/test_object_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_object_response.py` & `cdo-sdk-python-1.0.99/test/test_object_response.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_on_prem_fmc_info.py` & `cdo-sdk-python-1.0.99/test/test_on_prem_fmc_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_os.py` & `cdo-sdk-python-1.0.99/test/test_os.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_override.py` & `cdo-sdk-python-1.0.99/test/test_override.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_policy.py` & `cdo-sdk-python-1.0.99/test/test_policy.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_ports_value.py` & `cdo-sdk-python-1.0.99/test/test_ports_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_public_key.py` & `cdo-sdk-python-1.0.99/test/test_public_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_ra_vpn_session.py` & `cdo-sdk-python-1.0.99/test/test_ra_vpn_session.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_ra_vpn_session_page.py` & `cdo-sdk-python-1.0.99/test/test_ra_vpn_session_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_reference_info.py` & `cdo-sdk-python-1.0.99/test/test_reference_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_remote_access_monitoring_api.py` & `cdo-sdk-python-1.0.99/test/test_remote_access_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_sdc.py` & `cdo-sdk-python-1.0.99/test/test_sdc.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_sdc_page.py` & `cdo-sdk-python-1.0.99/test/test_sdc_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_sdc_public_key.py` & `cdo-sdk-python-1.0.99/test/test_sdc_public_key.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_sdc_status.py` & `cdo-sdk-python-1.0.99/test/test_sdc_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_search_api.py` & `cdo-sdk-python-1.0.99/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_service_object_content.py` & `cdo-sdk-python-1.0.99/test/test_service_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_service_object_value_content.py` & `cdo-sdk-python-1.0.99/test/test_service_object_value_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_shared_object_value.py` & `cdo-sdk-python-1.0.99/test/test_shared_object_value.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_single_content.py` & `cdo-sdk-python-1.0.99/test/test_single_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_state_machine_details.py` & `cdo-sdk-python-1.0.99/test/test_state_machine_details.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_state_machine_error.py` & `cdo-sdk-python-1.0.99/test/test_state_machine_error.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_status.py` & `cdo-sdk-python-1.0.99/test/test_status.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_status_info.py` & `cdo-sdk-python-1.0.99/test/test_status_info.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_target.py` & `cdo-sdk-python-1.0.99/test/test_target.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_targets_request.py` & `cdo-sdk-python-1.0.99/test/test_targets_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_tenant.py` & `cdo-sdk-python-1.0.99/test/test_tenant.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_tenant_management_api.py` & `cdo-sdk-python-1.0.99/test/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_tenant_page.py` & `cdo-sdk-python-1.0.99/test/test_tenant_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_tenant_pay_type.py` & `cdo-sdk-python-1.0.99/test/test_tenant_pay_type.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_tenant_settings.py` & `cdo-sdk-python-1.0.99/test/test_tenant_settings.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_transactions_api.py` & `cdo-sdk-python-1.0.99/test/test_transactions_api.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_unified_object_list_view.py` & `cdo-sdk-python-1.0.99/test/test_unified_object_list_view.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_update_request.py` & `cdo-sdk-python-1.0.99/test/test_update_request.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_url_object_content.py` & `cdo-sdk-python-1.0.99/test/test_url_object_content.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_user.py` & `cdo-sdk-python-1.0.99/test/test_user.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_user_create_or_update_input.py` & `cdo-sdk-python-1.0.99/test/test_user_create_or_update_input.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_user_page.py` & `cdo-sdk-python-1.0.99/test/test_user_page.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_user_role.py` & `cdo-sdk-python-1.0.99/test/test_user_role.py`

 * *Files identical despite different names*

### Comparing `cdo-sdk-python-1.0.98/test/test_users_api.py` & `cdo-sdk-python-1.0.99/test/test_users_api.py`

 * *Files identical despite different names*

