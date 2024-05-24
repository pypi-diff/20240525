# Comparing `tmp/pulumi_gcp-7.9.0a1707891532.tar.gz` & `tmp/pulumi_gcp-7.9.0a1707934510.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gcp-7.9.0a1707891532.tar", last modified: Wed Feb 14 06:27:14 2024, max compression
+gzip compressed data, was "pulumi_gcp-7.9.0a1707934510.tar", last modified: Wed Feb 14 18:24:41 2024, max compression
```

## Comparing `pulumi_gcp-7.9.0a1707891532.tar` & `pulumi_gcp-7.9.0a1707934510.tar`

### file list

```diff
@@ -1,1600 +1,1606 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.471072 pulumi_gcp-7.9.0a1707891532/
--rw-r--r--   0 runner    (1000) runner    (1000)     2658 2024-02-14 06:27:14.471072 pulumi_gcp-7.9.0a1707891532/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2206 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.187074 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/
--rw-r--r--   0 runner    (1000) runner    (1000)   177687 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1412 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9248 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/_utilities.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.187074 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/
--rw-r--r--   0 runner    (1000) runner    (1000)      402 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5623 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/get_folder_service_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5943 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/get_organization_service_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5676 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/get_project_service_account.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.191074 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/
--rw-r--r--   0 runner    (1000) runner    (1000)      941 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   282019 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24042 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_level.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43195 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_level_condition.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17512 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_levels.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17970 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30941 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30645 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26936 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36134 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/authorized_orgs_desc.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9604 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/egress_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16969 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/gcp_user_access_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4313 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/get_access_policy_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9677 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/ingress_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   278709 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    61112 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15316 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter_egress_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15898 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter_ingress_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14658 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter_resource.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17283 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeters.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.195073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34459 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/domain.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30064 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/domain_trust.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29784 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/peering.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.195073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/
--rw-r--r--   0 runner    (1000) runner    (1000)      476 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51111 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    66057 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/backup.py
--rw-r--r--   0 runner    (1000) runner    (1000)   102559 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3658 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/get_locations.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4802 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/get_supported_database_flags.py
--rw-r--r--   0 runner    (1000) runner    (1000)    77098 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    66492 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24091 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/user.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.199073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/
--rw-r--r--   0 runner    (1000) runner    (1000)      801 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18414 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25661 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47003 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36799 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36503 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32915 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33403 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33107 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29621 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30283 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38470 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38174 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34620 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5637 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/get_api_config_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4626 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/get_api_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6053 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/get_gateway_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15285 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.203073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/
--rw-r--r--   0 runner    (1000) runner    (1000)     1082 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    62041 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16584 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/addons_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21256 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/endpoint_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13977 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16176 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_group_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11022 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_keystore.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17533 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_references.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32118 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32188 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31892 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28298 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19637 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/flowhook.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4950 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/get_environment_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48509 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16105 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/instance_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22871 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/keystores_aliases_key_cert_file.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21233 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/keystores_aliases_pkcs12.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38071 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/keystores_aliases_self_signed_cert.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17284 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/nat_address.py
--rw-r--r--   0 runner    (1000) runner    (1000)    58078 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/organization.py
--rw-r--r--   0 runner    (1000) runner    (1000)    58816 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20091 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/sharedflow.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17432 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/sharedflow_deployment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18475 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/sync_authorization.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30888 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/target_server.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.203073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/
--rw-r--r--   0 runner    (1000) runner    (1000)      637 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   130694 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33757 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/application.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14461 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/application_url_dispatch_rules.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21628 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/domain_mapping.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19993 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/engine_split_traffic.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20171 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/firewall_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)   103553 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/flexible_app_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5845 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/get_default_service_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)   128868 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16504 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/service_network_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    78316 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/standard_app_version.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.207073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/
--rw-r--r--   0 runner    (1000) runner    (1000)      551 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39733 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12891 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/get_repository.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6662 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/get_repository_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    68122 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79897 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38306 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38010 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34363 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13732 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/vpcsc_config.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.207073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17190 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18696 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    75350 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/workload.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.207073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/
--rw-r--r--   0 runner    (1000) runner    (1000)      384 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3229 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5472 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/get_management_server.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22551 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/management_server.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5637 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.211073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/
--rw-r--r--   0 runner    (1000) runner    (1000)      498 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7611 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37479 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/app_connection.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28680 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/app_connector.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32606 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/app_gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8366 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/get_app_connection.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7399 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/get_app_connector.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8498 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/get_app_gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13049 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.211073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/
--rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7136 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20110 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/catalog.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22662 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/database.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7540 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28984 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/table.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.215073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/
--rw-r--r--   0 runner    (1000) runner    (1000)     1128 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   244520 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41635 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/app_profile.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18775 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/bi_reservation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35458 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/capacity_commitment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51356 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41522 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41226 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37635 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    60016 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/data_transfer_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    93465 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47311 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_access.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30436 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30148 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26608 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7706 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_connection_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14673 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_dataset.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4902 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_dataset_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5843 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_default_service_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5938 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_table_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41592 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41292 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36513 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    52957 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/job.py
--rw-r--r--   0 runner    (1000) runner    (1000)   255005 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33713 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/reservation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19719 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/reservation_assignment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    62143 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/routine.py
--rw-r--r--   0 runner    (1000) runner    (1000)    94232 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/table.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.219073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/
--rw-r--r--   0 runner    (1000) runner    (1000)      672 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10040 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28326 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40509 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40213 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36504 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7354 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/get_data_exchange_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8456 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/get_listing_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51138 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43998 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43702 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40078 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8828 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.219073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/
--rw-r--r--   0 runner    (1000) runner    (1000)      486 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4122 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25066 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37929 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37633 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33972 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6356 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/get_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3647 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.223073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/
--rw-r--r--   0 runner    (1000) runner    (1000)      662 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19577 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32810 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/gc_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4703 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/get_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5422 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/get_table_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44231 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30171 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29883 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25402 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16740 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27766 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32066 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31778 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27369 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.223073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/
--rw-r--r--   0 runner    (1000) runner    (1000)      532 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32072 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25813 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/account_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25525 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/account_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21082 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/account_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37713 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/budget.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4196 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/get_account_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30032 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11095 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/project_info.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17103 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/sub_account.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.227073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/
--rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24798 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21918 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34809 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34513 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30879 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5553 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/get_attestor_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24943 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33779 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.227073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17661 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35476 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/blockchain_nodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18573 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.231073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/
--rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   299965 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    94291 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/authority.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29875 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43451 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43151 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38162 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    77464 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40659 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44022 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43722 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38460 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15845 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/get_authority.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6337 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/get_ca_pool_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6573 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/get_certificate_template_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   340846 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.231073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/
--rw-r--r--   0 runner    (1000) runner    (1000)      548 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32339 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    55995 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48354 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate_issuance_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26306 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate_map.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39930 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate_map_entry.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27726 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/dns_authorization.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7108 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/get_certificate_map.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35579 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31648 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/trust_config.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.235073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/
--rw-r--r--   0 runner    (1000) runner    (1000)      442 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14491 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36829 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/folder_feed.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7758 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/get_resources_search_all.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35922 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/organization_feed.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17392 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36666 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/project_feed.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.235073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/
--rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   137743 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42084 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/bitbucket_server_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15944 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/get_trigger.py
--rw-r--r--   0 runner    (1000) runner    (1000)   225287 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   117612 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/trigger.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34889 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/worker_pool.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.239073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/
--rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27301 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42980 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36229 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35933 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32314 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6230 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/get_connection_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26571 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34655 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/repository.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.239073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/
--rw-r--r--   0 runner    (1000) runner    (1000)      395 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73447 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    60999 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/automation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    59060 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/delivery_pipeline.py
--rw-r--r--   0 runner    (1000) runner    (1000)    71706 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    61882 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/target.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.239073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    55255 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54973 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    53215 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/registration.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.243073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17556 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   105256 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39396 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39100 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35501 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22130 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/get_function.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7045 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/get_function_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27072 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.243073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/
--rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50435 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56632 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37941 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37645 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34032 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10158 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/get_function.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6627 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/get_function_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    78989 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.243073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/
--rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15802 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4949 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/get_group_lookup.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4017 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/get_group_memberships.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3889 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/get_groups.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34005 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26135 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/group_membership.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34253 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.243073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudids/
--rw-r--r--   0 runner    (1000) runner    (1000)      293 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudids/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29139 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudids/endpoint.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.247073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/
--rw-r--r--   0 runner    (1000) runner    (1000)      540 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   151702 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20754 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/domain_mapping.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3946 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/get_locations.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7096 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/get_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6386 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/get_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36491 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36195 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32774 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   218998 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51753 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/service.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.251073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/
--rw-r--r--   0 runner    (1000) runner    (1000)      672 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   187467 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16263 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_job.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6177 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_job_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19047 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6325 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    94482 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36011 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35715 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32229 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   305215 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   122373 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36507 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36211 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32657 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.251073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/
--rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23942 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47962 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/job.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23249 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.251073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/
--rw-r--r--   0 runner    (1000) runner    (1000)      468 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16152 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6225 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/get_queue_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15120 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28588 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36131 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35835 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32315 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.255073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/
--rw-r--r--   0 runner    (1000) runner    (1000)      406 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    99394 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26828 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/environment.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6588 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/get_environment.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5202 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/get_image_versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)   174163 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.295073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/
--rw-r--r--   0 runner    (1000) runner    (1000)     7157 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)  1782395 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    69103 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/address.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28085 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/attached_disk.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34486 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/autoscaler.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38009 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29038 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28742 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25107 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15701 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_signed_url_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)   115842 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30549 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30249 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25183 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14473 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_signed_url_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15539 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ca_external_account_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)   125906 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11579 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_async_replication.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37347 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37051 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33569 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17392 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_resource_policy_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36846 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/external_vpn_gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)    86318 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24166 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14702 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall_policy_association.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39504 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall_policy_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)   163739 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/forwarding_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9548 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_address.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9412 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_addresses.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8218 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_bucket.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5035 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_bucket_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19889 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5058 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7653 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5789 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_default_service_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23302 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_disk.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6568 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_disk_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19872 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_forwarding_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9072 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_global_address.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14924 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_global_forwarding_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6763 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_hc_vpn_gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11484 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_health_check.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17518 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_image.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5296 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_image_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26947 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8410 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17840 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_group_manager.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6914 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10377 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_serial_port.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28709 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4290 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_lbip_ranges.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5194 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_machine_image_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5602 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_machine_types.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10059 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_netblock_ip_ranges.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6428 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_network.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9202 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_network_endpoint_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9187 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_network_peering.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3879 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_networks.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5404 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_node_types.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6680 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16235 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_disk.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6871 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_disk_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7838 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_instance_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26604 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_instance_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11507 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_network_endpoint_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8720 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_ssl_certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5140 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_regions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8688 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_reservation.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8634 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_resource_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7542 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_router.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15123 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_router_nat.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7165 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_router_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14668 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_snapshot.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5373 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_snapshot_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8436 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_ssl_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9887 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_subnetwork.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7146 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_subnetwork_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5967 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_vpn_gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5028 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_zones.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46556 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_address.py
--rw-r--r--   0 runner    (1000) runner    (1000)   123521 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_forwarding_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19354 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_network_endpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24237 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_network_endpoint_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32352 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ha_vpn_gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)    64860 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/health_check.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37549 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/http_health_check.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37631 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/https_health_check.py
--rw-r--r--   0 runner    (1000) runner    (1000)    64495 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39988 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39688 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34811 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   138514 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)   104489 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_from_machine_image.py
--rw-r--r--   0 runner    (1000) runner    (1000)   108292 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_from_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29444 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    90779 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_group_manager.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19549 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_group_named_port.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45437 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45137 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40197 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14743 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)   114861 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    91102 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/interconnect_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29542 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42094 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41794 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36770 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31373 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/managed_ssl_certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31587 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/manged_ssl_certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49506 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47904 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24719 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_edge_security_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26113 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_endpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39103 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_endpoint_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24588 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_endpoint_list.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23274 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_firewall_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16090 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_firewall_policy_association.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48923 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_firewall_policy_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31315 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_peering.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24026 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_peering_routes_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47934 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/node_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34771 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/node_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19254 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/organization_security_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17439 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/organization_security_policy_association.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36253 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/organization_security_policy_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)  2161410 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31265 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/packet_mirroring.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38513 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/per_instance_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11105 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/project_default_network_tier.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12368 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/project_metadata.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11295 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/project_metadata_item.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21510 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/public_advertised_prefix.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26246 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/public_delegated_prefix.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30819 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_autoscaler.py
--rw-r--r--   0 runner    (1000) runner    (1000)   103124 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35572 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35272 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30080 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49853 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_commitment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    94526 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35035 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34739 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31197 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18589 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_resource_policy_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    68736 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_health_check.py
--rw-r--r--   0 runner    (1000) runner    (1000)   100511 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_instance_group_manager.py
--rw-r--r--   0 runner    (1000) runner    (1000)    99684 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_instance_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24559 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_endpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)    59782 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_endpoint_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25742 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_firewall_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18277 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_firewall_policy_association.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51746 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_firewall_policy_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39872 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_per_instance_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43767 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_security_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56088 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_security_policy_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35408 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_ssl_certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38275 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_ssl_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25236 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_target_http_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30828 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_target_https_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29474 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_target_tcp_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50697 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_url_map.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33148 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/reservation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42779 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/resource_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    55715 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/route.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28301 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37869 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_interface.py
--rw-r--r--   0 runner    (1000) runner    (1000)    85077 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_nat.py
--rw-r--r--   0 runner    (1000) runner    (1000)    77487 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_peer.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7485 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_status.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43362 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/security_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36750 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/security_scan_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49486 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/service_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8862 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/shared_vpc_host_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14551 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/shared_vpc_service_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    58994 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33571 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33275 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29725 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32154 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ssl_certificate.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37953 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ssl_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    85485 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46961 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46661 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41679 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31856 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_grpc_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30140 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_http_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    62591 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_https_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36259 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32453 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34378 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_ssl_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26504 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_tcp_proxy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46569 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/url_map.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25574 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/vpn_gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)    70394 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/vpn_tunnel.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.295073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/
--rw-r--r--   0 runner    (1000) runner    (1000)      285 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7050 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/__init__.pyi
--rw-r--r--   0 runner    (1000) runner    (1000)     1060 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22238 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/vars.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.303073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/
--rw-r--r--   0 runner    (1000) runner    (1000)      845 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   600135 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    69374 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/attached_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    72030 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/aws_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    81694 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/aws_node_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19942 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/azure_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)    70105 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/azure_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    57326 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/azure_node_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)   279872 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6954 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_attached_install_manifest.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4969 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_attached_versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5537 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_aws_versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5591 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_azure_versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45764 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13014 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_engine_versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6992 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_registry_image.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5353 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_registry_repository.py
--rw-r--r--   0 runner    (1000) runner    (1000)    71054 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/node_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)   816314 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13113 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/registry.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.303073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/
--rw-r--r--   0 runner    (1000) runner    (1000)      488 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12213 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5317 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/get_note_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34903 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34381 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34085 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30533 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27191 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/occurence.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11707 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.303073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/
--rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    78007 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56215 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/connection_profile.py
--rw-r--r--   0 runner    (1000) runner    (1000)    74814 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30742 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/private_connection.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.307073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/
--rw-r--r--   0 runner    (1000) runner    (1000)     1075 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38976 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    53170 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19453 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35856 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35560 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31948 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6067 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_entry_group_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4319 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_policy_tag_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6121 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_tag_template_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5906 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_taxonomy_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37077 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23795 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30506 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30210 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26615 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42303 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26575 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36022 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35726 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32097 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22192 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35399 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35103 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31525 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.311073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/
--rw-r--r--   0 runner    (1000) runner    (1000)      390 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    55942 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    82846 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/flex_template_job.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73885 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/job.py
--rw-r--r--   0 runner    (1000) runner    (1000)    52474 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    53478 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/pipeline.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.311073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/
--rw-r--r--   0 runner    (1000) runner    (1000)      576 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34924 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6296 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/get_repository_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32946 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42341 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12653 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12367 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9714 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33380 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_release_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36323 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_workflow_config.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.311073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/
--rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5960 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6848 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/get_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    87460 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6586 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.315073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/
--rw-r--r--   0 runner    (1000) runner    (1000)      484 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   933314 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   923651 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27571 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_deidentify_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35713 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_inspect_template.py
--rw-r--r--   0 runner    (1000) runner    (1000)    70172 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_job_trigger.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32375 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_stored_info_type.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.323073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/
--rw-r--r--   0 runner    (1000) runner    (1000)     1084 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   156246 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44110 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39437 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39141 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35635 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    62154 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36890 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36594 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33037 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7409 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_asset_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6423 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_datascan_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5944 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_lake_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7027 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_task_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6745 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_zone_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34258 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35389 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35093 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31604 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   151703 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43345 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38803 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38507 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35018 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38657 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37466 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37170 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33681 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.327073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/
--rw-r--r--   0 runner    (1000) runner    (1000)     1317 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   484209 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26124 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40390 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40094 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36384 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35832 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31708 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31420 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27600 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7390 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_autoscaling_policy_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5252 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_cluster_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5153 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_job_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6086 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_metastore_federation_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6728 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_metastore_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51519 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22591 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22303 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18579 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40549 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31716 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31420 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27676 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    75736 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37860 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37564 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33871 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   479237 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49930 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/workflow_template.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.327073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/
--rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1580 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18429 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/data_store_index.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1272 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.331073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/
--rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   155999 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56219 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/connection_profile.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4742 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/get_static_ips.py
--rw-r--r--   0 runner    (1000) runner    (1000)   159316 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30420 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/private_connection.py
--rw-r--r--   0 runner    (1000) runner    (1000)    93405 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/stream.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.331073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/
--rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5485 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38681 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/deployment.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4298 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.335073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/
--rw-r--r--   0 runner    (1000) runner    (1000)      682 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   359244 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51525 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/agent.py
--rw-r--r--   0 runner    (1000) runner    (1000)    59765 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_agent.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42569 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_entity_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23390 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_environment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    89400 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_flow.py
--rw-r--r--   0 runner    (1000) runner    (1000)    61023 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_intent.py
--rw-r--r--   0 runner    (1000) runner    (1000)   117816 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_page.py
--rw-r--r--   0 runner    (1000) runner    (1000)    65620 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_security_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39972 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_test_case.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21622 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33624 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_webhook.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23675 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/entity_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22854 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/fulfillment.py
--rw-r--r--   0 runner    (1000) runner    (1000)    53663 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/intent.py
--rw-r--r--   0 runner    (1000) runner    (1000)   354624 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.335073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/
--rw-r--r--   0 runner    (1000) runner    (1000)      396 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9839 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38865 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/chat_engine.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33707 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/data_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11781 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36238 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/search_engine.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.339073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/
--rw-r--r--   0 runner    (1000) runner    (1000)      749 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    77085 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34693 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/dns_managed_zone_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34397 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/dns_managed_zone_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30773 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/dns_managed_zone_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6498 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_keys.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6927 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_managed_zone.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5627 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_managed_zone_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3339 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_managed_zones.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6349 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_record_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)    72515 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/managed_zone.py
--rw-r--r--   0 runner    (1000) runner    (1000)    93949 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28798 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36656 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/record_set.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24533 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/response_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24717 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/response_policy_rule.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.339073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/
--rw-r--r--   0 runner    (1000) runner    (1000)      392 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46548 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73456 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47703 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/node_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45257 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41330 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/vpn_connection.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.339073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgenetwork/
--rw-r--r--   0 runner    (1000) runner    (1000)      314 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgenetwork/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27306 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgenetwork/network.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38158 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgenetwork/subnet.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.343073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/
--rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11735 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19766 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/consumers_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19470 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/consumers_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15889 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/consumers_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4635 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/get_service_consumers_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4120 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/get_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8875 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26194 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20006 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19710 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16163 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.343073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/
--rw-r--r--   0 runner    (1000) runner    (1000)      526 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40920 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18534 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/contact.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19761 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_processor.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11609 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_processor_default_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46736 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_warehouse_document_schema.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23684 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_warehouse_location.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39048 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.343073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/
--rw-r--r--   0 runner    (1000) runner    (1000)      397 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16072 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27670 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/channel.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17677 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/google_channel_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13749 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50550 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/trigger.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.347072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/
--rw-r--r--   0 runner    (1000) runner    (1000)      412 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13374 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41339 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/backup.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9762 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/get_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44179 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22344 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33829 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/snapshot.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.351072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/
--rw-r--r--   0 runner    (1000) runner    (1000)      898 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    62510 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33532 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/android_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29858 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/apple_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30026 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/database_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30523 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/extensions_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7950 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_android_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4146 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_android_app_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7235 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_apple_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4771 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_apple_app_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6780 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_hosting_channel.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5882 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_web_app.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8652 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_web_app_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29881 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_channel.py
--rw-r--r--   0 runner    (1000) runner    (1000)    63239 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_custom_domain.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31109 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_release.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19917 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_site.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22292 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)    60521 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11532 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11766 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/storage_bucket.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27242 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/web_app.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.351072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/
--rw-r--r--   0 runner    (1000) runner    (1000)      360 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4530 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3442 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19962 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/release.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14830 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/ruleset.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.351072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/
--rw-r--r--   0 runner    (1000) runner    (1000)      435 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8943 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25817 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/backup_schedule.py
--rw-r--r--   0 runner    (1000) runner    (1000)    60264 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/database.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22651 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/document.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24838 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/field.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26145 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/index.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8646 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.355073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/
--rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16936 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33742 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/access_approval_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3911 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/get_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7719 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/get_organization_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27770 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_audit_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21788 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26423 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23948 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33162 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/organization_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20796 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.355073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/
--rw-r--r--   0 runner    (1000) runner    (1000)      687 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    61945 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56487 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36803 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36507 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32909 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6429 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/get_backup_plan_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6472 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/get_restore_plan_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    60450 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    61826 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46008 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45712 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43049 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.359073 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/
--rw-r--r--   0 runner    (1000) runner    (1000)     1008 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   143274 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50189 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36149 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35853 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32327 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40796 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_membership.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21958 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/fleet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6263 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/get_feature_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6528 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/get_membership_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5199 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/get_scope_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37327 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31744 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37195 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36899 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33322 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27726 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_rbac_role_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32999 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/namespace.py
--rw-r--r--   0 runner    (1000) runner    (1000)   135813 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24458 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33207 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32911 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29419 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36133 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_rbac_role_binding.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.363072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/
--rw-r--r--   0 runner    (1000) runner    (1000)      488 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   270681 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    92350 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/bare_metal_admin_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)   115514 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/bare_metal_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    55754 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/bare_metal_node_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)   271480 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)   101373 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/v_mware_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54120 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/v_mware_node_pool.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.367072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/
--rw-r--r--   0 runner    (1000) runner    (1000)     1212 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44045 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32022 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34698 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34402 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30763 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16887 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27037 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26749 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23195 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36128 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27943 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27655 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24050 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    91875 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27772 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27484 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23896 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5687 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_consent_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4495 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_dataset_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4760 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_dicom_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4705 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_fhir_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4796 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_hl7_v2_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45620 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27933 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27645 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24074 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42833 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.371072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/
--rw-r--r--   0 runner    (1000) runner    (1000)      690 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42062 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14232 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/access_boundary_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14130 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/deny_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4693 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7430 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_testable_permissions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6838 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_workload_identity_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10419 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_workload_identity_pool_provider.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50341 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38392 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workforce_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    80073 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workforce_pool_provider.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26343 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workload_identity_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    82297 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workload_identity_pool_provider.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.379072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/
--rw-r--r--   0 runner    (1000) runner    (1000)     1960 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46518 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45409 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45109 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40029 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49071 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_version_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48771 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_version_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43691 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_version_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18867 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/brand.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14805 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6751 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_app_engine_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7807 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_app_engine_version_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4533 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_client.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4542 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_tunnel_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6251 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_tunnel_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5970 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4467 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7045 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_region_backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5735 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_type_app_engine_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4760 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_type_compute_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37708 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37430 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37130 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32260 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43447 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43147 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38109 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42326 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_backend_service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42026 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_backend_service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36925 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37075 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36775 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31968 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45810 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_region_backend_service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45510 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_region_backend_service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40283 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_region_backend_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41639 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_app_enging_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41339 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_app_enging_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36259 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_app_enging_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38330 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_compute_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38030 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_compute_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32992 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_compute_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.379072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/
--rw-r--r--   0 runner    (1000) runner    (1000)      639 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54374 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31573 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19839 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/default_supported_idp_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23913 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/inbound_saml_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20468 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/oauth_idp_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    58306 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14728 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/project_default_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19914 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22529 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant_default_supported_idp_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26741 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant_inbound_saml_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23189 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant_oauth_idp_config.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.379072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/
--rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    99714 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    94953 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/connection.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28367 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/endpoint_attachment.py
--rw-r--r--   0 runner    (1000) runner    (1000)   104747 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.383072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/
--rw-r--r--   0 runner    (1000) runner    (1000)      984 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25017 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42081 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32326 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32034 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27584 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19508 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4194 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_crypto_key_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4546 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_key_ring_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10407 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_crypto_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8536 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_crypto_key_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5654 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_key_ring.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6467 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_secret.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8238 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_secret_asymmetric.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5557 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_secret_ciphertext.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13173 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32312 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32020 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27129 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25985 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_import_job.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26682 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18345 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/secret_ciphertext.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.391072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/
--rw-r--r--   0 runner    (1000) runner    (1000)     1063 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    69922 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29395 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/billing_account_bucket_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16560 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/billing_account_exclusion.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33271 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/billing_account_sink.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29710 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_bucket_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17486 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_exclusion.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22592 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36342 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_sink.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8803 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_folder_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9127 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_organization_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9930 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_project_cmek_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8857 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_project_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7668 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_sink.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27365 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/linked_dataset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22526 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/log_view.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49850 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/metric.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30594 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_bucket_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16999 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_exclusion.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22855 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    36209 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_sink.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73434 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33478 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/project_bucket_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17151 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/project_exclusion.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40692 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/project_sink.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.391072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21481 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    72167 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20654 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.391072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/
--rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19753 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    57669 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19085 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.391072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/migrationcenter/
--rw-r--r--   0 runner    (1000) runner    (1000)      290 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/migrationcenter/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28554 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/migrationcenter/group.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.391072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/
--rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      997 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32424 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/engine_model.py
--rw-r--r--   0 runner    (1000) runner    (1000)      850 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.395072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/
--rw-r--r--   0 runner    (1000) runner    (1000)      876 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   198035 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    55809 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/alert_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22711 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/custom_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15805 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/dashboard.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27445 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/generic_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10143 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_app_engine_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11613 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_cluster_istio_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10953 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_istio_canonical_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10393 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_mesh_istio_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13197 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_notification_channel.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7746 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_secret_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3343 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_uptime_check_i_ps.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20933 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    53485 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/metric_descriptor.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14285 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/monitored_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54137 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/notification_channel.py
--rw-r--r--   0 runner    (1000) runner    (1000)   202734 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48822 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/slo.py
--rw-r--r--   0 runner    (1000) runner    (1000)    65572 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/uptime_check_config.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.399072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/
--rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27916 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    69744 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/active_directory.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37872 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/backup_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25143 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/backup_vault.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28948 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/kmsconfig.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26936 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47080 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/storage_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    76885 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/volume.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28236 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/volume_snapshot.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.399072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/
--rw-r--r--   0 runner    (1000) runner    (1000)      429 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29593 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27871 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/hub.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28193 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48531 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/policy_based_route.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40939 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/service_connection_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46701 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/spoke.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.399072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/
--rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9967 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50597 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/connectivity_test.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9502 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.403072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/
--rw-r--r--   0 runner    (1000) runner    (1000)      786 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43917 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34008 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12566 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12280 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30567 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34493 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/authorization_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37157 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/client_tls_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33212 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/gateway_security_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41480 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/gateway_security_policy_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5877 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/get_address_group_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47826 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34288 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/security_profile.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48752 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/server_tls_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30415 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/tls_inspection_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22134 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/url_list.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.407072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/
--rw-r--r--   0 runner    (1000) runner    (1000)      621 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   227395 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38732 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/edge_cache_keyset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79230 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/edge_cache_origin.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79616 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/edge_cache_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    43279 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/endpoint_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    72946 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/gateway.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41337 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/grpc_route.py
--rw-r--r--   0 runner    (1000) runner    (1000)    54489 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/http_route.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28067 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/mesh.py
--rw-r--r--   0 runner    (1000) runner    (1000)   225271 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25439 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/service_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32737 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/tcp_route.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24434 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/tls_route.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.407072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/
--rw-r--r--   0 runner    (1000) runner    (1000)      698 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    78670 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27301 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/environment.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6570 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/get_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6508 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/get_runtime_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)   110638 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37546 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37250 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33686 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9877 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/location.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73825 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48639 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37356 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37060 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33513 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.411072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/
--rw-r--r--   0 runner    (1000) runner    (1000)      850 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27088 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32619 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/access_approval_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19509 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/folder.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4291 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_active_folder.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7632 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_billing_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3997 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_client_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4060 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_client_open_id_user_info.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8019 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_folder.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4255 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_folders.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8978 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7165 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_organization.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7722 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16592 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_audit_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16906 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22838 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_custom_role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26495 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24139 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27401 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31607 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39100 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/project.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.411072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/
--rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32256 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32833 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/custom_constraint.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30184 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28439 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.415072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/
--rw-r--r--   0 runner    (1000) runner    (1000)      412 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   276549 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49415 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/guest_policies.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48624 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/os_policy_assignment.py
--rw-r--r--   0 runner    (1000) runner    (1000)   268681 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56679 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/patch_deployment.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.415072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/oslogin/
--rw-r--r--   0 runner    (1000) runner    (1000)      299 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/oslogin/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15038 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/oslogin/ssh_public_key.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.419072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/
--rw-r--r--   0 runner    (1000) runner    (1000)      815 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30598 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37409 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/access_approval_settings.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24011 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/api_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18815 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/default_service_accounts.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3877 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7571 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_organization_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4266 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_project.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6357 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_project_service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27921 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_audit_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26971 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24089 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_custom_role.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26679 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24155 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33115 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/organization_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38345 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18178 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11811 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/service_identity.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13736 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/usage_export_bucket.py
--rw-r--r--   0 runner    (1000) runner    (1000)   177463 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/provider.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.423072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47687 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5339 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_schema_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12745 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_subscription.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5115 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_subscription_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7616 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_topic.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5288 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_topic_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15992 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/lite_reservation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20733 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/lite_subscription.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24370 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/lite_topic.py
--rw-r--r--   0 runner    (1000) runner    (1000)    73454 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21028 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33701 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33405 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29896 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    96340 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28498 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28210 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24792 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39318 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33546 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33250 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29758 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pulumi-plugin.json
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/py.typed
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.423072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/
--rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12646 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41151 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/enterprise_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13613 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.423072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/
--rw-r--r--   0 runner    (1000) runner    (1000)      389 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35210 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42706 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20700 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/get_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)   110464 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    51908 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.423072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/resourcemanager/
--rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/resourcemanager/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20758 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/resourcemanager/lien.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.427072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/
--rw-r--r--   0 runner    (1000) runner    (1000)      551 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2812 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11505 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28737 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28441 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24883 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3965 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/get_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4913 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/get_config_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5495 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/get_variable.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1914 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20869 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/variable.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.427072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/
--rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14169 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9390 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5335 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7288 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret_version.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6600 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret_version_access.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4398 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secrets.py
--rw-r--r--   0 runner    (1000) runner    (1000)    37934 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    63500 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33965 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33669 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30111 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28835 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_version.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.431072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/
--rw-r--r--   0 runner    (1000) runner    (1000)      483 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8374 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6706 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/get_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34040 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12739 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12453 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9820 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7546 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.431072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/
--rw-r--r--   0 runner    (1000) runner    (1000)      808 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    56998 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23202 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/event_threat_detection_custom_module.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30777 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/folder_custom_module.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4743 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/get_source_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24444 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24144 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21511 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23588 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/mute_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23159 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/notification_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30991 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/organization_custom_module.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50876 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31027 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/project_custom_module.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16672 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15456 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15164 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12551 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.435072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/
--rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    62934 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    60544 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38883 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/posture.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39152 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/posture_deployment.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.435072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/
--rw-r--r--   0 runner    (1000) runner    (1000)      630 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5822 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28176 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/account.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7330 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10519 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_access_token.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9400 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_id_token.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7464 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_jwt.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6872 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4176 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33323 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33025 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28204 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34106 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/key.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4840 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.439072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/
--rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5280 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26938 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/endpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3807 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/get_namespace_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3765 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/get_service_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24574 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30934 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30638 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27008 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3484 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17475 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31004 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30708 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27112 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.439072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/
--rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21364 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/connection.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4989 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/get_peered_dns_domain.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17760 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/peered_dns_domain.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.439072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceusage/
--rw-r--r--   0 runner    (1000) runner    (1000)      308 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceusage/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25710 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceusage/consumer_quota_override.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.439072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/
--rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5858 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5418 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/get_repository.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5575 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/get_repository_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7347 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17379 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33255 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32959 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29417 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.443072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/
--rw-r--r--   0 runner    (1000) runner    (1000)      680 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15489 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    40672 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30537 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30249 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26699 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5877 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/get_database_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8560 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/get_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4998 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/get_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44934 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28179 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27891 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24341 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21770 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.447072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/
--rw-r--r--   0 runner    (1000) runner    (1000)      734 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    96354 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29144 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/database.py
--rw-r--r--   0 runner    (1000) runner    (1000)    82112 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/database_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7395 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_backup_run.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4906 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_ca_certs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6068 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15844 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5492 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database_instance_latest_recovery_time.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8386 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database_instances.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4502 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_databases.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4161 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_tiers.py
--rw-r--r--   0 runner    (1000) runner    (1000)   222768 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    38286 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/source_representation_instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21704 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/ssl_cert.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29237 2024-02-14 06:27:03.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/user.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.451072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/
--rw-r--r--   0 runner    (1000) runner    (1000)     1143 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   112185 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    79166 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19591 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_access_control.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16986 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_acl.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35665 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35365 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30467 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    60815 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_object.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23856 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/default_object_access_control.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11844 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/default_object_acl.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14658 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4086 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    15521 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket_object.py
--rw-r--r--   0 runner    (1000) runner    (1000)    14364 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket_object_content.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13659 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_object_signed_url.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_project_service_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5078 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_transfer_project_service_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5619 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_transfer_project_servie_account.py
--rw-r--r--   0 runner    (1000) runner    (1000)    18959 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/hmac_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29007 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/insights_report_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29832 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/notification.py
--rw-r--r--   0 runner    (1000) runner    (1000)    23899 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/object_access_control.py
--rw-r--r--   0 runner    (1000) runner    (1000)    16538 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/object_acl.py
--rw-r--r--   0 runner    (1000) runner    (1000)   136267 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    21503 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/transfer_agent_pool.py
--rw-r--r--   0 runner    (1000) runner    (1000)    42104 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/transfer_job.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.455072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/
--rw-r--r--   0 runner    (1000) runner    (1000)      771 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5272 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6945 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4105 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_key_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6434 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_value.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4205 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_value_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    17043 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/location_tag_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3476 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    13189 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    27379 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29684 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29388 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25893 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20870 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30000 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29704 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    26175 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.455072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19253 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5482 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/get_tensorflow_versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5641 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/get_v2_accelerator_types.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5310 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/get_v2_runtime_versions.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49672 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/node.py
--rw-r--r--   0 runner    (1000) runner    (1000)    19368 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    66390 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/v2_vm.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.459072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/
--rw-r--r--   0 runner    (1000) runner    (1000)     1361 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)   111680 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31005 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_dataset.py
--rw-r--r--   0 runner    (1000) runner    (1000)    48840 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12649 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12363 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9710 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32250 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_group.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34336 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_group_feature.py
--rw-r--r--   0 runner    (1000) runner    (1000)    49005 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_online_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    52559 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_online_store_featureview.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41678 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41123 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33802 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_feature.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29267 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    28971 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    25156 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33329 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    33033 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29388 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47065 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_index.py
--rw-r--r--   0 runner    (1000) runner    (1000)    45676 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_index_endpoint.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22785 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_metadata_store.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35236 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_tensorboard.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5845 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_endpoint_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5307 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_featurestore_entitytype_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6471 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_featurestore_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10085 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_index.py
--rw-r--r--   0 runner    (1000) runner    (1000)   127978 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.463072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/
--rw-r--r--   0 runner    (1000) runner    (1000)      872 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29805 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    22633 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44825 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/external_access_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)    24317 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/external_address.py
--rw-r--r--   0 runner    (1000) runner    (1000)     5670 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9820 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_external_access_rule.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7147 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_external_address.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6722 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_network.py
--rw-r--r--   0 runner    (1000) runner    (1000)    11243 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_network_peering.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9141 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_network_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4486 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_nsx_credentials.py
--rw-r--r--   0 runner    (1000) runner    (1000)     8697 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_private_cloud.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9603 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_subnet.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4614 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_vcenter_credentials.py
--rw-r--r--   0 runner    (1000) runner    (1000)    20499 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/network.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46136 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/network_peering.py
--rw-r--r--   0 runner    (1000) runner    (1000)    39741 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/network_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50143 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    32985 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/private_cloud.py
--rw-r--r--   0 runner    (1000) runner    (1000)    29446 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/subnet.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.467072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/
--rw-r--r--   0 runner    (1000) runner    (1000)      368 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2243 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35848 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/connector.py
--rw-r--r--   0 runner    (1000) runner    (1000)    10282 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/get_connector.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.467072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/
--rw-r--r--   0 runner    (1000) runner    (1000)      483 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34835 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     6374 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/get_instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    50450 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12432 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    12146 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)     9513 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31638 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/outputs.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.467072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workflows/
--rw-r--r--   0 runner    (1000) runner    (1000)      293 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workflows/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    47036 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workflows/workflow.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.471072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/
--rw-r--r--   0 runner    (1000) runner    (1000)      752 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)    44520 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/_inputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7026 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/get_workstation_config_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)     7529 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/get_workstation_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    41027 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/outputs.py
--rw-r--r--   0 runner    (1000) runner    (1000)    46165 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation.py
--rw-r--r--   0 runner    (1000) runner    (1000)    55283 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_cluster.py
--rw-r--r--   0 runner    (1000) runner    (1000)   110355 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34386 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    34090 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    30352 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config_iam_policy.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35877 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_iam_binding.py
--rw-r--r--   0 runner    (1000) runner    (1000)    35581 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_iam_member.py
--rw-r--r--   0 runner    (1000) runner    (1000)    31945 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_iam_policy.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 06:27:14.471072 pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2658 2024-02-14 06:27:14.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)    60507 2024-02-14 06:27:14.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-02-14 06:27:14.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-02-14 06:27:14.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-02-14 06:27:14.000000 pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-02-14 06:27:04.000000 pulumi_gcp-7.9.0a1707891532/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-02-14 06:27:14.471072 pulumi_gcp-7.9.0a1707891532/setup.cfg
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.696762 pulumi_gcp-7.9.0a1707934510/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2658 2024-02-14 18:24:41.696762 pulumi_gcp-7.9.0a1707934510/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2206 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.444758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/
+-rw-r--r--   0 runner    (1000) runner    (1000)   178791 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1412 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9248 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/_utilities.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.448758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/
+-rw-r--r--   0 runner    (1000) runner    (1000)      402 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5623 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/get_folder_service_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5943 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/get_organization_service_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5676 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/get_project_service_account.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.452758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/
+-rw-r--r--   0 runner    (1000) runner    (1000)      941 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   282019 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24042 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_level.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43195 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_level_condition.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17512 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_levels.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17970 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30941 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30645 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26936 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36134 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/authorized_orgs_desc.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9604 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/egress_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16969 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/gcp_user_access_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4313 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/get_access_policy_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9677 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/ingress_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   278709 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    61112 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15316 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter_egress_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15898 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter_ingress_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14658 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter_resource.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17283 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeters.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.452758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34459 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/domain.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30064 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/domain_trust.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29784 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/peering.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.452758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/
+-rw-r--r--   0 runner    (1000) runner    (1000)      476 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51111 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    66057 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/backup.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   102559 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3658 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/get_locations.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4802 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/get_supported_database_flags.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    77098 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    66492 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24091 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/user.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.456758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/
+-rw-r--r--   0 runner    (1000) runner    (1000)      801 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18414 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25661 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47003 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36799 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36503 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32915 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33403 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33107 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29621 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30283 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38470 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38174 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34620 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5637 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/get_api_config_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4626 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/get_api_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6053 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/get_gateway_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15285 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.460759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1082 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    62041 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16584 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/addons_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21256 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/endpoint_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13977 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16176 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_group_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11022 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_keystore.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17533 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_references.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32118 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32188 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31892 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28298 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19637 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/flowhook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4950 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/get_environment_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48509 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16105 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/instance_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22871 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/keystores_aliases_key_cert_file.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21233 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/keystores_aliases_pkcs12.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38071 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/keystores_aliases_self_signed_cert.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17284 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/nat_address.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    58078 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/organization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    58816 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20091 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/sharedflow.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17432 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/sharedflow_deployment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18475 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/sync_authorization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30888 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/target_server.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.460759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/
+-rw-r--r--   0 runner    (1000) runner    (1000)      637 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   130694 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33757 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/application.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14461 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/application_url_dispatch_rules.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21628 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/domain_mapping.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19993 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/engine_split_traffic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20171 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/firewall_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   103553 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/flexible_app_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5845 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/get_default_service_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   128868 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16504 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/service_network_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    78316 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/standard_app_version.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.464758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/
+-rw-r--r--   0 runner    (1000) runner    (1000)      551 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39733 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12891 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/get_repository.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6662 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/get_repository_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    68122 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79897 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38306 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38010 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34363 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13732 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/vpcsc_config.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.464758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17190 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18696 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    75350 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/workload.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.464758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/
+-rw-r--r--   0 runner    (1000) runner    (1000)      384 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3229 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5472 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/get_management_server.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22551 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/management_server.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5637 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.464758 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/
+-rw-r--r--   0 runner    (1000) runner    (1000)      498 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7611 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37479 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/app_connection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28680 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/app_connector.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32606 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/app_gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8366 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/get_app_connection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7399 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/get_app_connector.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8498 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/get_app_gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13049 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.468759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/
+-rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7136 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20110 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/catalog.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22662 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/database.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7540 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28984 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/table.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.472759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1128 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   244520 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41635 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/app_profile.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18775 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/bi_reservation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35458 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/capacity_commitment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51356 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41522 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41226 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37635 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    60016 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/data_transfer_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    93465 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47311 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_access.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30436 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30148 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26608 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7706 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_connection_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14673 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_dataset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4902 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_dataset_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5843 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_default_service_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5938 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_table_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41592 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41292 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36513 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    52957 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   255005 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33713 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/reservation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19719 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/reservation_assignment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    62143 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/routine.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    94232 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/table.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.472759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/
+-rw-r--r--   0 runner    (1000) runner    (1000)      672 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10040 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28326 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40509 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40213 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36504 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7354 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/get_data_exchange_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8456 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/get_listing_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51138 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43998 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43702 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40078 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8828 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.476759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/
+-rw-r--r--   0 runner    (1000) runner    (1000)      486 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4122 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25066 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37929 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37633 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33972 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6356 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/get_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3647 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.476759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/
+-rw-r--r--   0 runner    (1000) runner    (1000)      662 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19577 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32810 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/gc_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4703 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/get_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5422 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/get_table_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44231 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30171 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29883 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25402 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16740 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27766 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32066 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31778 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27369 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.480759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/
+-rw-r--r--   0 runner    (1000) runner    (1000)      532 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32072 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25813 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/account_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25525 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/account_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21082 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/account_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37713 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/budget.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4196 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/get_account_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30032 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11095 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/project_info.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17103 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/sub_account.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.480759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/
+-rw-r--r--   0 runner    (1000) runner    (1000)      505 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24798 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21918 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34809 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34513 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30879 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5553 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/get_attestor_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24943 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33779 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.480759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17661 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35476 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/blockchain_nodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18573 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.484759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/
+-rw-r--r--   0 runner    (1000) runner    (1000)      788 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   299965 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    94291 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/authority.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29875 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43451 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43151 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38162 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    77464 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40659 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44022 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43722 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38460 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15845 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/get_authority.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6337 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/get_ca_pool_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6573 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/get_certificate_template_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   340846 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.484759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/
+-rw-r--r--   0 runner    (1000) runner    (1000)      548 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32339 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    55995 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48354 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate_issuance_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26306 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate_map.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39930 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate_map_entry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27726 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/dns_authorization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7108 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/get_certificate_map.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35579 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31648 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/trust_config.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.488759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/
+-rw-r--r--   0 runner    (1000) runner    (1000)      442 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14491 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36829 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/folder_feed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7758 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/get_resources_search_all.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35922 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/organization_feed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17392 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36666 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/project_feed.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.488759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/
+-rw-r--r--   0 runner    (1000) runner    (1000)      430 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   137743 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42084 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/bitbucket_server_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15944 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/get_trigger.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   225287 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   117612 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/trigger.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34889 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/worker_pool.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.488759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      519 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27301 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42980 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36229 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35933 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32314 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6230 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/get_connection_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26571 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34655 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/repository.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.492759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/
+-rw-r--r--   0 runner    (1000) runner    (1000)      576 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    75939 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    60999 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/automation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    59060 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/delivery_pipeline.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12690 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/delivery_pipeline_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12404 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/delivery_pipeline_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9691 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/delivery_pipeline_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6413 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/get_delivery_pipeline_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73300 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    61882 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/target.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.492759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    55255 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54973 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    53215 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/registration.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.492759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17556 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   105256 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39396 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39100 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35501 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22130 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/get_function.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7045 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/get_function_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27072 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.496759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      511 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50435 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56632 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37941 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37645 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34032 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10158 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/get_function.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6627 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/get_function_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    78989 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.496759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/
+-rw-r--r--   0 runner    (1000) runner    (1000)      462 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15802 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4949 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/get_group_lookup.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4017 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/get_group_memberships.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3889 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/get_groups.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34005 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26135 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/group_membership.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34253 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.496759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudids/
+-rw-r--r--   0 runner    (1000) runner    (1000)      293 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudids/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29139 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudids/endpoint.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.496759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/
+-rw-r--r--   0 runner    (1000) runner    (1000)      540 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   151702 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20754 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/domain_mapping.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3946 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/get_locations.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7096 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/get_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6386 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/get_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36491 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36195 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32774 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   218998 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51753 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/service.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.500759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      672 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   187467 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16263 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6177 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_job_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19047 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6325 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    94482 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36011 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35715 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32229 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   305215 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   122373 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36507 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36211 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32657 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.500759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/
+-rw-r--r--   0 runner    (1000) runner    (1000)      333 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23942 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47962 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23249 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.504759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/
+-rw-r--r--   0 runner    (1000) runner    (1000)      468 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16152 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6225 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/get_queue_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15120 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28588 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36131 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35835 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32315 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.504759 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/
+-rw-r--r--   0 runner    (1000) runner    (1000)      406 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    99394 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26828 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/environment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6588 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/get_environment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5202 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/get_image_versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   174163 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.540760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/
+-rw-r--r--   0 runner    (1000) runner    (1000)     7198 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)  1789464 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    69103 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/address.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28085 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/attached_disk.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34486 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/autoscaler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38009 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29038 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28742 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25107 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15701 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_signed_url_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   115842 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30549 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30249 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25183 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14473 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_signed_url_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15539 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ca_external_account_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   125906 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11579 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_async_replication.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37347 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37051 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33569 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17392 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_resource_policy_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36846 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/external_vpn_gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    86318 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24166 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14702 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall_policy_association.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39504 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall_policy_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   163739 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/forwarding_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9548 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_address.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9412 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_addresses.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8218 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_bucket.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5035 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_bucket_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19889 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5058 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7653 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5789 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_default_service_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23302 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_disk.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6568 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_disk_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19872 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_forwarding_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9072 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_global_address.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14924 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_global_forwarding_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6763 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_hc_vpn_gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11484 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_health_check.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17518 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_image.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5296 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_image_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26947 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8410 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17840 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_group_manager.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6914 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10377 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_serial_port.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28709 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4290 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_lbip_ranges.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5194 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_machine_image_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5602 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_machine_types.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10059 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_netblock_ip_ranges.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6428 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_network.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9202 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_network_endpoint_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9187 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_network_peering.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3879 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_networks.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5404 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_node_types.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6680 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16235 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_disk.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6871 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_disk_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7838 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_instance_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26604 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_instance_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11507 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_network_endpoint_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8720 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_ssl_certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5140 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_regions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8688 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_reservation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8634 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_resource_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7542 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_router.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15123 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_router_nat.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7165 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_router_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14668 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_snapshot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5373 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_snapshot_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8436 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_ssl_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9887 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_subnetwork.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7146 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_subnetwork_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5967 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_vpn_gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5028 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_zones.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46556 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_address.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   123521 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_forwarding_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19354 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_network_endpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24237 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_network_endpoint_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32352 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ha_vpn_gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    64860 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/health_check.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37549 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/http_health_check.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37631 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/https_health_check.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    64495 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39988 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39688 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34811 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   138514 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   104489 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_from_machine_image.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   108292 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_from_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29444 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    90779 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_group_manager.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19106 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_group_membership.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19549 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_group_named_port.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45437 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45137 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40197 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14743 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   114861 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    91102 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/interconnect_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29542 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42094 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41794 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36770 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31373 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/managed_ssl_certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31587 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/manged_ssl_certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49506 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47904 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24719 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_edge_security_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26113 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_endpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39103 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_endpoint_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24588 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_endpoint_list.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23274 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_firewall_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16090 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_firewall_policy_association.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48923 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_firewall_policy_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31315 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_peering.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24026 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_peering_routes_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47934 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/node_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34771 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/node_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19254 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/organization_security_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17439 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/organization_security_policy_association.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36253 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/organization_security_policy_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)  2170406 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31265 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/packet_mirroring.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38513 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/per_instance_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11105 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/project_default_network_tier.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12368 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/project_metadata.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11295 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/project_metadata_item.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21510 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/public_advertised_prefix.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26246 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/public_delegated_prefix.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30819 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_autoscaler.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   103124 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35572 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35272 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30080 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49853 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_commitment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    94526 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35035 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34739 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31197 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18589 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_resource_policy_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    68736 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_health_check.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   100511 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_instance_group_manager.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    99684 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_instance_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24559 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_endpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    59782 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_endpoint_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25742 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_firewall_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18277 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_firewall_policy_association.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51746 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_firewall_policy_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39872 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_per_instance_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43767 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_security_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56088 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_security_policy_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35408 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_ssl_certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38275 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_ssl_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25236 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_target_http_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30828 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_target_https_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29474 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_target_tcp_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50697 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_url_map.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33148 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/reservation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42779 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/resource_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    55715 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/route.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28301 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37869 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_interface.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    85077 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_nat.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    77487 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_peer.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7485 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_status.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43362 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/security_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36750 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/security_scan_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49486 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/service_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8862 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/shared_vpc_host_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14551 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/shared_vpc_service_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    58994 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33571 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33275 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29725 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32154 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ssl_certificate.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37953 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ssl_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    85485 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46961 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46661 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41679 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31856 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_grpc_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30140 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_http_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    62591 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_https_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36259 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32453 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34378 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_ssl_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26504 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_tcp_proxy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46569 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/url_map.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25574 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/vpn_gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    70394 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/vpn_tunnel.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.544760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/
+-rw-r--r--   0 runner    (1000) runner    (1000)      285 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7201 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/__init__.pyi
+-rw-r--r--   0 runner    (1000) runner    (1000)     1060 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22699 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/vars.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.548760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/
+-rw-r--r--   0 runner    (1000) runner    (1000)      845 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   600135 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    69374 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/attached_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    72030 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/aws_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    81694 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/aws_node_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19942 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/azure_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    70105 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/azure_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    57326 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/azure_node_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   279872 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6954 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_attached_install_manifest.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4969 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_attached_versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5537 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_aws_versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5591 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_azure_versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45764 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13014 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_engine_versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6992 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_registry_image.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5353 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_registry_repository.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    71054 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/node_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   816314 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13113 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/registry.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.548760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/
+-rw-r--r--   0 runner    (1000) runner    (1000)      488 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12213 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5317 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/get_note_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34903 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34381 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34085 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30533 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27191 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/occurence.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11707 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.548760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/
+-rw-r--r--   0 runner    (1000) runner    (1000)      382 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    78007 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56215 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/connection_profile.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    74814 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30742 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/private_connection.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.552760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1075 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38976 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    53170 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19453 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35856 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35560 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31948 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6067 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_entry_group_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4319 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_policy_tag_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6121 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_tag_template_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5906 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_taxonomy_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37077 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23795 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30506 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30210 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26615 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42303 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26575 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36022 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35726 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32097 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22192 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35399 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35103 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31525 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.556760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/
+-rw-r--r--   0 runner    (1000) runner    (1000)      390 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    55942 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    82846 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/flex_template_job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73885 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    52474 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    53478 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/pipeline.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.556760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/
+-rw-r--r--   0 runner    (1000) runner    (1000)      576 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34924 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6296 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/get_repository_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32946 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42341 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12653 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12367 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9714 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33380 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_release_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36323 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_workflow_config.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.556760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/
+-rw-r--r--   0 runner    (1000) runner    (1000)      377 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5960 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6848 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/get_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    87460 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6586 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.560760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/
+-rw-r--r--   0 runner    (1000) runner    (1000)      484 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   933314 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   923651 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27571 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_deidentify_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35713 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_inspect_template.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    70172 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_job_trigger.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32375 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_stored_info_type.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.564760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1084 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   156246 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44110 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39437 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39141 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35635 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    62154 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36890 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36594 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33037 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7409 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_asset_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6423 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_datascan_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5944 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_lake_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7027 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_task_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6745 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_zone_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34258 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35389 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35093 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31604 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   151703 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43345 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38803 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38507 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35018 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38657 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37466 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37170 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33681 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.572760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1317 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   484209 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26124 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40390 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40094 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36384 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35832 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31708 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31420 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27600 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7390 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_autoscaling_policy_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5252 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_cluster_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5153 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_job_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6086 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_metastore_federation_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6728 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_metastore_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51519 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22591 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22303 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18579 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40549 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31716 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31420 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27676 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    75736 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37860 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37564 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33871 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   479237 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49930 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/workflow_template.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.572760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/
+-rw-r--r--   0 runner    (1000) runner    (1000)      346 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1580 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18429 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/data_store_index.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1272 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.572760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/
+-rw-r--r--   0 runner    (1000) runner    (1000)      434 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   155999 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56219 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/connection_profile.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4742 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/get_static_ips.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   159316 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30420 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/private_connection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    93405 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/stream.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.572760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/
+-rw-r--r--   0 runner    (1000) runner    (1000)      340 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5485 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38681 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/deployment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4298 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.576760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/
+-rw-r--r--   0 runner    (1000) runner    (1000)      682 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   359244 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51525 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/agent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    59765 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_agent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42569 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_entity_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23390 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_environment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    89400 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_flow.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    61023 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_intent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   117816 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_page.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    65620 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_security_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39972 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_test_case.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21622 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33624 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_webhook.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23675 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/entity_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22854 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/fulfillment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    53663 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/intent.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   354624 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.576760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/
+-rw-r--r--   0 runner    (1000) runner    (1000)      396 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9839 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38865 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/chat_engine.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33707 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/data_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11781 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36238 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/search_engine.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.580760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/
+-rw-r--r--   0 runner    (1000) runner    (1000)      749 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    77085 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34693 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/dns_managed_zone_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34397 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/dns_managed_zone_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30773 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/dns_managed_zone_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6498 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_keys.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6927 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_managed_zone.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5627 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_managed_zone_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3339 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_managed_zones.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6349 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_record_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    72515 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/managed_zone.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    93949 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28798 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36656 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/record_set.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24533 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/response_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24717 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/response_policy_rule.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.580760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/
+-rw-r--r--   0 runner    (1000) runner    (1000)      392 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46548 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73456 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47703 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/node_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45257 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41330 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/vpn_connection.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.580760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgenetwork/
+-rw-r--r--   0 runner    (1000) runner    (1000)      314 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgenetwork/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27306 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgenetwork/network.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38158 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgenetwork/subnet.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.584760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/
+-rw-r--r--   0 runner    (1000) runner    (1000)      635 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11735 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19766 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/consumers_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19470 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/consumers_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15889 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/consumers_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4635 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/get_service_consumers_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4120 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/get_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8875 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26194 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20006 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19710 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16163 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.584760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/
+-rw-r--r--   0 runner    (1000) runner    (1000)      526 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40920 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18534 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/contact.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19761 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_processor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11609 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_processor_default_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46736 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_warehouse_document_schema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23684 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_warehouse_location.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39048 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.584760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/
+-rw-r--r--   0 runner    (1000) runner    (1000)      397 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16072 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27670 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/channel.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17677 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/google_channel_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13749 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50550 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/trigger.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.588760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/
+-rw-r--r--   0 runner    (1000) runner    (1000)      412 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13374 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41339 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/backup.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9762 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/get_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44179 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22344 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33829 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/snapshot.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.588760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/
+-rw-r--r--   0 runner    (1000) runner    (1000)      938 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    62358 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33532 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/android_app.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34509 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/app_check_service_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29858 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/apple_app.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30026 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/database_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30523 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/extensions_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7950 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_android_app.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4146 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_android_app_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7235 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_apple_app.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4771 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_apple_app_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6780 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_hosting_channel.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5882 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_web_app.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8652 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_web_app_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29881 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_channel.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    63239 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_custom_domain.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31109 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_release.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19917 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_site.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22292 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    60449 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11532 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11766 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/storage_bucket.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27242 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/web_app.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.592760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/
+-rw-r--r--   0 runner    (1000) runner    (1000)      360 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4530 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3442 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19962 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/release.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14830 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/ruleset.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.592760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/
+-rw-r--r--   0 runner    (1000) runner    (1000)      435 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8943 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25817 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/backup_schedule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    60264 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/database.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22651 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/document.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24838 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/field.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26145 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/index.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8646 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.592760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/
+-rw-r--r--   0 runner    (1000) runner    (1000)      569 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16936 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33742 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/access_approval_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3911 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/get_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7719 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/get_organization_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27770 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_audit_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21788 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26423 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23948 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33162 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/organization_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20796 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.596760 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/
+-rw-r--r--   0 runner    (1000) runner    (1000)      687 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    61945 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56487 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36803 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36507 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32909 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6429 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/get_backup_plan_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6472 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/get_restore_plan_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    60450 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    61826 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46008 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45712 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43049 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.600761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1008 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   143274 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50189 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36149 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35853 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32327 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40796 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_membership.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21958 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/fleet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6263 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/get_feature_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6528 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/get_membership_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5199 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/get_scope_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37327 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31744 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37195 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36899 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33322 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27726 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_rbac_role_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32999 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/namespace.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   135813 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24458 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33207 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32911 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29419 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36133 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_rbac_role_binding.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.600761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/
+-rw-r--r--   0 runner    (1000) runner    (1000)      488 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   270681 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    92350 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/bare_metal_admin_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   115514 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/bare_metal_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    55754 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/bare_metal_node_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   271480 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   101373 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/v_mware_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54120 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/v_mware_node_pool.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.608761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1212 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44045 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32022 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34698 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34402 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30763 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16887 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27037 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26749 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23195 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36128 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27943 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27655 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24050 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    91875 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27772 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27484 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23896 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5687 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_consent_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4495 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_dataset_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4760 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_dicom_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4705 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_fhir_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4796 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_hl7_v2_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45620 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27933 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27645 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24074 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42833 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.608761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/
+-rw-r--r--   0 runner    (1000) runner    (1000)      690 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42062 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14232 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/access_boundary_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14130 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/deny_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4693 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7430 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_testable_permissions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6838 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_workload_identity_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10419 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_workload_identity_pool_provider.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50341 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38392 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workforce_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    80073 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workforce_pool_provider.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26343 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workload_identity_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    82297 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workload_identity_pool_provider.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.616761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1960 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46518 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45409 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45109 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40029 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49071 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_version_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48771 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_version_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43691 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_version_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18867 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/brand.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14805 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6751 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_app_engine_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7807 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_app_engine_version_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4533 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_client.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4542 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_tunnel_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6251 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_tunnel_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5970 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4467 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7045 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_region_backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5735 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_type_app_engine_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4760 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_type_compute_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37708 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37430 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37130 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32260 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43447 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43147 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38109 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42326 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_backend_service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42026 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_backend_service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36925 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37075 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36775 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31968 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45810 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_region_backend_service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45510 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_region_backend_service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40283 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_region_backend_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41639 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_app_enging_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41339 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_app_enging_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36259 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_app_enging_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38330 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_compute_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38030 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_compute_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32992 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_compute_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.616761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/
+-rw-r--r--   0 runner    (1000) runner    (1000)      639 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54374 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31573 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19839 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/default_supported_idp_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23913 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/inbound_saml_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20468 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/oauth_idp_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    58306 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14728 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/project_default_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19914 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22529 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant_default_supported_idp_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26741 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant_inbound_saml_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23189 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant_oauth_idp_config.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.616761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/
+-rw-r--r--   0 runner    (1000) runner    (1000)      375 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    99714 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    94953 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/connection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28367 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/endpoint_attachment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   104747 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.620761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/
+-rw-r--r--   0 runner    (1000) runner    (1000)      984 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25017 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42081 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32326 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32034 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27584 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19508 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4194 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_crypto_key_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4546 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_key_ring_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10407 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_crypto_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8536 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_crypto_key_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5654 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_key_ring.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6467 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_secret.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8238 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_secret_asymmetric.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5557 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_secret_ciphertext.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13173 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32312 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32020 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27129 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25985 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_import_job.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26682 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18345 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/secret_ciphertext.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.624761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1063 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    69922 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29395 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/billing_account_bucket_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16560 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/billing_account_exclusion.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33271 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/billing_account_sink.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29710 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_bucket_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17486 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_exclusion.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22592 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36342 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_sink.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8803 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_folder_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9127 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_organization_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9930 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_project_cmek_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8857 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_project_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7668 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_sink.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27365 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/linked_dataset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22526 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/log_view.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49850 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/metric.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30594 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_bucket_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16999 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_exclusion.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22855 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    36209 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_sink.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73434 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33478 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/project_bucket_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17151 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/project_exclusion.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40692 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/project_sink.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.624761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21481 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    72167 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20654 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.628761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/
+-rw-r--r--   0 runner    (1000) runner    (1000)      338 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19753 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    57669 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19085 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.628761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/migrationcenter/
+-rw-r--r--   0 runner    (1000) runner    (1000)      290 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/migrationcenter/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28554 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/migrationcenter/group.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.628761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/
+-rw-r--r--   0 runner    (1000) runner    (1000)      342 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      997 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32424 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/engine_model.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      850 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.632761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/
+-rw-r--r--   0 runner    (1000) runner    (1000)      876 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   198035 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    55809 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/alert_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22711 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/custom_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15805 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/dashboard.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27445 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/generic_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10143 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_app_engine_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11613 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_cluster_istio_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10953 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_istio_canonical_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10393 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_mesh_istio_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13197 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_notification_channel.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7746 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_secret_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3343 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_uptime_check_i_ps.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20933 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    53485 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/metric_descriptor.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14285 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/monitored_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54137 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/notification_channel.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   202734 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48822 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/slo.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    65572 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/uptime_check_config.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.632761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/
+-rw-r--r--   0 runner    (1000) runner    (1000)      509 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27916 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    69744 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/active_directory.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37872 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/backup_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25143 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/backup_vault.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28948 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/kmsconfig.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26936 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47080 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/storage_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    76885 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/volume.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28236 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/volume_snapshot.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.632761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/
+-rw-r--r--   0 runner    (1000) runner    (1000)      429 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29593 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27871 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/hub.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28193 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48531 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/policy_based_route.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40939 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/service_connection_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46701 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/spoke.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.632761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/
+-rw-r--r--   0 runner    (1000) runner    (1000)      347 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9967 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50597 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/connectivity_test.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9502 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.636761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/
+-rw-r--r--   0 runner    (1000) runner    (1000)      786 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43917 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34008 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12566 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12280 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30567 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34493 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/authorization_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37157 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/client_tls_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33212 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/gateway_security_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41480 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/gateway_security_policy_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5877 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/get_address_group_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47826 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34288 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/security_profile.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48752 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/server_tls_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30415 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/tls_inspection_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22134 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/url_list.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.640761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/
+-rw-r--r--   0 runner    (1000) runner    (1000)      621 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   227395 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38732 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/edge_cache_keyset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79230 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/edge_cache_origin.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79616 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/edge_cache_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    43279 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/endpoint_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    72946 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/gateway.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41337 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/grpc_route.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    54489 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/http_route.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28067 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/mesh.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   225271 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25439 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/service_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32737 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/tcp_route.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24434 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/tls_route.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.640761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/
+-rw-r--r--   0 runner    (1000) runner    (1000)      698 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    78670 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27301 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/environment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6570 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/get_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6508 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/get_runtime_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   110638 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37546 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37250 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33686 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9877 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/location.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73825 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48639 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37356 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37060 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33513 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.644761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/
+-rw-r--r--   0 runner    (1000) runner    (1000)      850 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27088 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32619 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/access_approval_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19509 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/folder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4291 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_active_folder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7632 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_billing_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3997 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_client_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4060 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_client_open_id_user_info.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8019 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_folder.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4255 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_folders.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8978 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7165 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_organization.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7722 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16592 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_audit_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16906 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22838 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_custom_role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26495 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24139 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27401 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31607 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39100 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/project.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.644761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/
+-rw-r--r--   0 runner    (1000) runner    (1000)      369 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32256 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32833 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/custom_constraint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30184 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28439 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.648761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/
+-rw-r--r--   0 runner    (1000) runner    (1000)      412 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   276549 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49415 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/guest_policies.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48624 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/os_policy_assignment.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   268681 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56679 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/patch_deployment.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.648761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/oslogin/
+-rw-r--r--   0 runner    (1000) runner    (1000)      299 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/oslogin/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15038 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/oslogin/ssh_public_key.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.652761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/
+-rw-r--r--   0 runner    (1000) runner    (1000)      815 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30598 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37409 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/access_approval_settings.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24011 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/api_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18815 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/default_service_accounts.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3877 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7571 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_organization_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4266 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_project.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6357 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_project_service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27921 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_audit_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26971 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24089 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_custom_role.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26679 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24155 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33115 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/organization_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38345 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18178 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11811 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/service_identity.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13736 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/usage_export_bucket.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   181078 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/provider.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.652761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/
+-rw-r--r--   0 runner    (1000) runner    (1000)      964 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47687 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5339 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_schema_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12745 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_subscription.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5115 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_subscription_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7616 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_topic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5288 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_topic_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15992 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/lite_reservation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20733 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/lite_subscription.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24370 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/lite_topic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    73454 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21028 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33701 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33405 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29896 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    96340 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28498 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28210 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24792 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39318 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33546 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33250 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29758 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       40 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pulumi-plugin.json
+-rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.656761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/
+-rw-r--r--   0 runner    (1000) runner    (1000)      344 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12646 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41151 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/enterprise_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13613 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.656761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/
+-rw-r--r--   0 runner    (1000) runner    (1000)      389 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35210 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42706 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20700 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/get_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   110464 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    51908 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.656761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/resourcemanager/
+-rw-r--r--   0 runner    (1000) runner    (1000)      289 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/resourcemanager/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20758 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/resourcemanager/lien.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.656761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/
+-rw-r--r--   0 runner    (1000) runner    (1000)      551 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2812 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11505 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28737 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28441 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24883 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3965 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/get_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4913 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/get_config_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5495 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/get_variable.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1914 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20869 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/variable.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.660761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/
+-rw-r--r--   0 runner    (1000) runner    (1000)      631 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14169 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9390 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5335 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7288 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret_version.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6600 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret_version_access.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4398 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secrets.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    37934 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    63500 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33965 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33669 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30111 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28835 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_version.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.660761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/
+-rw-r--r--   0 runner    (1000) runner    (1000)      483 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8374 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6706 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/get_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34040 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12739 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12453 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9820 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7546 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.664761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/
+-rw-r--r--   0 runner    (1000) runner    (1000)      808 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    56998 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23202 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/event_threat_detection_custom_module.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30777 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/folder_custom_module.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4743 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/get_source_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24444 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24144 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21511 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23588 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/mute_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23159 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/notification_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30991 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/organization_custom_module.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50876 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31027 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/project_custom_module.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16672 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15456 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15164 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12551 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.664761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/
+-rw-r--r--   0 runner    (1000) runner    (1000)      371 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    62934 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    60544 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38883 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/posture.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39742 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/posture_deployment.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.664761 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/
+-rw-r--r--   0 runner    (1000) runner    (1000)      630 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5822 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28176 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7330 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10519 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_access_token.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9400 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_id_token.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7464 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_jwt.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6872 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4176 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33323 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33025 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28204 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34106 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4840 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.668762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/
+-rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5280 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26938 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/endpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3807 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/get_namespace_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3765 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/get_service_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24574 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30934 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30638 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27008 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3484 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17475 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31004 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30708 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27112 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.668762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/
+-rw-r--r--   0 runner    (1000) runner    (1000)      365 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21364 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/connection.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4989 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/get_peered_dns_domain.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17760 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/peered_dns_domain.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.668762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceusage/
+-rw-r--r--   0 runner    (1000) runner    (1000)      308 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceusage/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25710 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceusage/consumer_quota_override.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.668762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/
+-rw-r--r--   0 runner    (1000) runner    (1000)      523 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5858 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5418 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/get_repository.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5575 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/get_repository_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7347 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17379 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33255 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32959 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29417 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.672762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/
+-rw-r--r--   0 runner    (1000) runner    (1000)      680 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15489 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    40672 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30537 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30249 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26699 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5877 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/get_database_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8560 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/get_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4998 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/get_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44934 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28179 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27891 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24341 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21770 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.676762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/
+-rw-r--r--   0 runner    (1000) runner    (1000)      734 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    96354 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29144 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/database.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    82112 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/database_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7395 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_backup_run.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4906 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_ca_certs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6068 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15844 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5492 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database_instance_latest_recovery_time.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8386 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database_instances.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4502 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_databases.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4161 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_tiers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   222768 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    38286 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/source_representation_instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21704 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/ssl_cert.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29237 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/user.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.680762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1143 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   112185 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    79166 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19591 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_access_control.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16986 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_acl.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35665 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35365 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30467 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    60815 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_object.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23856 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/default_object_access_control.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11844 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/default_object_acl.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14658 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4086 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    15521 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket_object.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    14364 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket_object_content.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13659 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_object_signed_url.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12841 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_project_service_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5078 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_transfer_project_service_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5619 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_transfer_project_servie_account.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    18959 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/hmac_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29007 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/insights_report_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29832 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/notification.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    23899 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/object_access_control.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    16538 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/object_acl.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   136267 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    21503 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/transfer_agent_pool.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    42104 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/transfer_job.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.680762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/
+-rw-r--r--   0 runner    (1000) runner    (1000)      771 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5272 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6945 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4105 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_key_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6434 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_value.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4205 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_value_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    17043 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/location_tag_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3476 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    13189 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    27379 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29684 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29388 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25893 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20870 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30000 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29704 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    26175 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.684762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19253 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5482 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/get_tensorflow_versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5641 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/get_v2_accelerator_types.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5310 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/get_v2_runtime_versions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49672 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/node.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    19368 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    66390 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/v2_vm.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.688762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1361 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   111680 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31005 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_dataset.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    48840 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12649 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12363 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9710 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32250 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_group.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34336 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_group_feature.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    49005 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_online_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    52559 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_online_store_featureview.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41678 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41123 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33802 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_feature.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29267 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    28971 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    25156 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33329 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    33033 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29388 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47065 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_index.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    45676 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_index_endpoint.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22785 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_metadata_store.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35236 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_tensorboard.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5845 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_endpoint_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5307 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_featurestore_entitytype_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6471 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_featurestore_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10085 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_index.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   127978 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.692762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/
+-rw-r--r--   0 runner    (1000) runner    (1000)      872 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29805 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    22633 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44825 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/external_access_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    24317 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/external_address.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     5670 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9820 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_external_access_rule.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7147 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_external_address.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6722 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_network.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    11243 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_network_peering.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9141 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_network_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4486 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_nsx_credentials.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     8697 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_private_cloud.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9603 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_subnet.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4614 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_vcenter_credentials.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    20499 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/network.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46136 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/network_peering.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    39741 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/network_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50143 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    32985 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/private_cloud.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    29446 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/subnet.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.692762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/
+-rw-r--r--   0 runner    (1000) runner    (1000)      368 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2243 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35848 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/connector.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    10282 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/get_connector.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3512 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.692762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/
+-rw-r--r--   0 runner    (1000) runner    (1000)      483 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34835 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     6374 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/get_instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    50182 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12432 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    12146 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     9513 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31638 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/outputs.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.692762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workflows/
+-rw-r--r--   0 runner    (1000) runner    (1000)      293 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workflows/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    47036 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workflows/workflow.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.696762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/
+-rw-r--r--   0 runner    (1000) runner    (1000)      752 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    44520 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/_inputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7026 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/get_workstation_config_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     7529 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/get_workstation_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    41027 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/outputs.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    46165 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    55283 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_cluster.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   110355 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34386 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    34090 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    30352 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config_iam_policy.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35877 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_iam_binding.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    35581 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_iam_member.py
+-rw-r--r--   0 runner    (1000) runner    (1000)    31945 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_iam_policy.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 18:24:41.696762 pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2658 2024-02-14 18:24:41.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)    60828 2024-02-14 18:24:41.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-02-14 18:24:41.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       49 2024-02-14 18:24:41.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-02-14 18:24:41.000000 pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      676 2024-02-14 18:24:24.000000 pulumi_gcp-7.9.0a1707934510/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-02-14 18:24:41.696762 pulumi_gcp-7.9.0a1707934510/setup.cfg
```

### Comparing `pulumi_gcp-7.9.0a1707891532/PKG-INFO` & `pulumi_gcp-7.9.0a1707934510/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gcp
-Version: 7.9.0a1707891532
+Version: 7.9.0a1707934510
 Summary: A Pulumi package for creating and managing Google Cloud Platform resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-gcp
 Keywords: pulumi,gcp
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_gcp Version: 7.9.0a1707891532 Summary: A
+Metadata-Version: 2.1 Name: pulumi_gcp Version: 7.9.0a1707934510 Summary: A
 Pulumi package for creating and managing Google Cloud Platform resources.
 License: Apache-2.0 Project-URL: Homepage, https://pulumi.io Project-URL:
 Repository, https://github.com/pulumi/pulumi-gcp Keywords: pulumi,gcp Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist:
 parver>=0.2.1 Requires-Dist: pulumi<4.0.0,>=3.0.0 Requires-Dist: semver>=2.8.1
 [![Actions Status](https://github.com/pulumi/pulumi-gcp/workflows/master/
 badge.svg)](https://github.com/pulumi/pulumi-gcp/actions) [![Slack](http://
```

### Comparing `pulumi_gcp-7.9.0a1707891532/README.md` & `pulumi_gcp-7.9.0a1707934510/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1643,14 +1643,38 @@
   "fqn": "pulumi_gcp.clouddeploy",
   "classes": {
    "gcp:clouddeploy/deliveryPipeline:DeliveryPipeline": "DeliveryPipeline"
   }
  },
  {
   "pkg": "gcp",
+  "mod": "clouddeploy/deliveryPipelineIamBinding",
+  "fqn": "pulumi_gcp.clouddeploy",
+  "classes": {
+   "gcp:clouddeploy/deliveryPipelineIamBinding:DeliveryPipelineIamBinding": "DeliveryPipelineIamBinding"
+  }
+ },
+ {
+  "pkg": "gcp",
+  "mod": "clouddeploy/deliveryPipelineIamMember",
+  "fqn": "pulumi_gcp.clouddeploy",
+  "classes": {
+   "gcp:clouddeploy/deliveryPipelineIamMember:DeliveryPipelineIamMember": "DeliveryPipelineIamMember"
+  }
+ },
+ {
+  "pkg": "gcp",
+  "mod": "clouddeploy/deliveryPipelineIamPolicy",
+  "fqn": "pulumi_gcp.clouddeploy",
+  "classes": {
+   "gcp:clouddeploy/deliveryPipelineIamPolicy:DeliveryPipelineIamPolicy": "DeliveryPipelineIamPolicy"
+  }
+ },
+ {
+  "pkg": "gcp",
   "mod": "clouddeploy/target",
   "fqn": "pulumi_gcp.clouddeploy",
   "classes": {
    "gcp:clouddeploy/target:Target": "Target"
   }
  },
  {
@@ -2243,14 +2267,22 @@
   "fqn": "pulumi_gcp.compute",
   "classes": {
    "gcp:compute/instanceGroupManager:InstanceGroupManager": "InstanceGroupManager"
   }
  },
  {
   "pkg": "gcp",
+  "mod": "compute/instanceGroupMembership",
+  "fqn": "pulumi_gcp.compute",
+  "classes": {
+   "gcp:compute/instanceGroupMembership:InstanceGroupMembership": "InstanceGroupMembership"
+  }
+ },
+ {
+  "pkg": "gcp",
   "mod": "compute/instanceGroupNamedPort",
   "fqn": "pulumi_gcp.compute",
   "classes": {
    "gcp:compute/instanceGroupNamedPort:InstanceGroupNamedPort": "InstanceGroupNamedPort"
   }
  },
  {
@@ -4155,14 +4187,22 @@
   "fqn": "pulumi_gcp.firebase",
   "classes": {
    "gcp:firebase/androidApp:AndroidApp": "AndroidApp"
   }
  },
  {
   "pkg": "gcp",
+  "mod": "firebase/appCheckServiceConfig",
+  "fqn": "pulumi_gcp.firebase",
+  "classes": {
+   "gcp:firebase/appCheckServiceConfig:AppCheckServiceConfig": "AppCheckServiceConfig"
+  }
+ },
+ {
+  "pkg": "gcp",
   "mod": "firebase/appleApp",
   "fqn": "pulumi_gcp.firebase",
   "classes": {
    "gcp:firebase/appleApp:AppleApp": "AppleApp"
   }
  },
  {
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/_utilities.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/get_folder_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/get_folder_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/get_organization_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/get_organization_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accessapproval/get_project_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accessapproval/get_project_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_level.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_level.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_level_condition.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_level_condition.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_levels.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_levels.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/access_policy_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/access_policy_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/authorized_orgs_desc.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/authorized_orgs_desc.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/egress_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/egress_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/gcp_user_access_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/gcp_user_access_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/get_access_policy_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/get_access_policy_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/ingress_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/ingress_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter_egress_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter_egress_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter_ingress_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter_ingress_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeter_resource.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeter_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/accesscontextmanager/service_perimeters.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/accesscontextmanager/service_perimeters.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/domain.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/domain_trust.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/domain_trust.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/activedirectory/peering.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/activedirectory/peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/backup.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/get_locations.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/get_locations.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/get_supported_database_flags.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/get_supported_database_flags.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/alloydb/user.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/alloydb/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_config_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_config_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/api_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/api_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/gateway_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/gateway_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/get_api_config_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/get_api_config_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/get_api_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/get_api_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/get_gateway_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/get_gateway_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigateway/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigateway/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/addons_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/addons_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/endpoint_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/endpoint_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_group_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_group_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_keystore.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_keystore.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/env_references.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/env_references.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/environment_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/environment_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/flowhook.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/flowhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/get_environment_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/get_environment_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/instance_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/instance_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/keystores_aliases_key_cert_file.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/keystores_aliases_key_cert_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/keystores_aliases_pkcs12.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/keystores_aliases_pkcs12.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/keystores_aliases_self_signed_cert.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/keystores_aliases_self_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/nat_address.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/nat_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/organization.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/sharedflow.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/sharedflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/sharedflow_deployment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/sharedflow_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/sync_authorization.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/sync_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/apigee/target_server.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/apigee/target_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/application.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/application_url_dispatch_rules.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/application_url_dispatch_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/domain_mapping.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/domain_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/engine_split_traffic.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/engine_split_traffic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/firewall_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/flexible_app_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/flexible_app_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/get_default_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/get_default_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/service_network_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/service_network_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/appengine/standard_app_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/appengine/standard_app_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/get_repository.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/get_repository_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/get_repository_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/repository_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/repository_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/artifactregistry/vpcsc_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/artifactregistry/vpcsc_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/assuredworkloads/workload.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/assuredworkloads/workload.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/get_management_server.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/get_management_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/management_server.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/management_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/backupdisasterrecovery/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/backupdisasterrecovery/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/app_connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/app_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/app_connector.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/app_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/app_gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/app_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/get_app_connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/get_app_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/get_app_connector.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/get_app_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/get_app_gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/get_app_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/beyondcorp/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/beyondcorp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/catalog.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/catalog.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/database.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/biglake/table.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/biglake/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/app_profile.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/app_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/bi_reservation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/bi_reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/capacity_commitment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/capacity_commitment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/connection_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/connection_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/data_transfer_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/data_transfer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_access.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/dataset_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/dataset_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_connection_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_connection_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_dataset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_dataset_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_dataset_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_default_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_default_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/get_table_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/get_table_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/reservation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/reservation_assignment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/reservation_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/routine.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/routine.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquery/table.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/data_exchange_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/get_data_exchange_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/get_data_exchange_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/get_listing_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/get_listing_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/listing_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/listing_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigqueryanalyticshub/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigqueryanalyticshub/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/data_policy_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/data_policy_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/get_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/get_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigquerydatapolicy/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigquerydatapolicy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/gc_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/gc_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/get_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/get_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/get_table_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/get_table_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/bigtable/table_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/bigtable/table_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/account_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/account_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/account_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/account_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/account_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/account_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/budget.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/budget.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/get_account_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/get_account_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/project_info.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/project_info.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/billing/sub_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/billing/sub_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/attestor_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/attestor_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/get_attestor_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/get_attestor_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/binaryauthorization/policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/binaryauthorization/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/blockchain_nodes.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/blockchain_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/blockchainnodeengine/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/blockchainnodeengine/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/authority.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/authority.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/ca_pool_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/ca_pool_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/certificate_template_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/certificate_template_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/get_authority.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/get_authority.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/get_ca_pool_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/get_ca_pool_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/get_certificate_template_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/get_certificate_template_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificateauthority/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificateauthority/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate_issuance_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate_issuance_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate_map.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/certificate_map_entry.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/certificate_map_entry.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/dns_authorization.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/dns_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/get_certificate_map.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/get_certificate_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/certificatemanager/trust_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/certificatemanager/trust_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/folder_feed.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/folder_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/get_resources_search_all.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/get_resources_search_all.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/organization_feed.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/organization_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudasset/project_feed.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudasset/project_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/bitbucket_server_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/bitbucket_server_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/get_trigger.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/get_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/trigger.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuild/worker_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuild/worker_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/connection_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/connection_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/get_connection_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/get_connection_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudbuildv2/repository.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudbuildv2/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     'AutomationRulePromoteReleaseRuleArgs',
     'AutomationSelectorArgs',
     'AutomationSelectorTargetArgs',
     'DeliveryPipelineConditionArgs',
     'DeliveryPipelineConditionPipelineReadyConditionArgs',
     'DeliveryPipelineConditionTargetsPresentConditionArgs',
     'DeliveryPipelineConditionTargetsTypeConditionArgs',
+    'DeliveryPipelineIamBindingConditionArgs',
+    'DeliveryPipelineIamMemberConditionArgs',
     'DeliveryPipelineSerialPipelineArgs',
     'DeliveryPipelineSerialPipelineStageArgs',
     'DeliveryPipelineSerialPipelineStageDeployParameterArgs',
     'DeliveryPipelineSerialPipelineStageStrategyArgs',
     'DeliveryPipelineSerialPipelineStageStrategyCanaryArgs',
     'DeliveryPipelineSerialPipelineStageStrategyCanaryCanaryDeploymentArgs',
     'DeliveryPipelineSerialPipelineStageStrategyCanaryCanaryDeploymentPostdeployArgs',
@@ -465,14 +467,92 @@
 
     @status.setter
     def status(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "status", value)
 
 
 @pulumi.input_type
+class DeliveryPipelineIamBindingConditionArgs:
+    def __init__(__self__, *,
+                 expression: pulumi.Input[str],
+                 title: pulumi.Input[str],
+                 description: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "expression", expression)
+        pulumi.set(__self__, "title", title)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+
+    @property
+    @pulumi.getter
+    def expression(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "expression")
+
+    @expression.setter
+    def expression(self, value: pulumi.Input[str]):
+        pulumi.set(self, "expression", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+
+@pulumi.input_type
+class DeliveryPipelineIamMemberConditionArgs:
+    def __init__(__self__, *,
+                 expression: pulumi.Input[str],
+                 title: pulumi.Input[str],
+                 description: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "expression", expression)
+        pulumi.set(__self__, "title", title)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+
+    @property
+    @pulumi.getter
+    def expression(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "expression")
+
+    @expression.setter
+    def expression(self, value: pulumi.Input[str]):
+        pulumi.set(self, "expression", value)
+
+    @property
+    @pulumi.getter
+    def title(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "title")
+
+    @title.setter
+    def title(self, value: pulumi.Input[str]):
+        pulumi.set(self, "title", value)
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "description")
+
+    @description.setter
+    def description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "description", value)
+
+
+@pulumi.input_type
 class DeliveryPipelineSerialPipelineArgs:
     def __init__(__self__, *,
                  stages: Optional[pulumi.Input[Sequence[pulumi.Input['DeliveryPipelineSerialPipelineStageArgs']]]] = None):
         """
         :param pulumi.Input[Sequence[pulumi.Input['DeliveryPipelineSerialPipelineStageArgs']]] stages: Each stage specifies configuration for a `Target`. The ordering of this list defines the promotion flow.
         """
         if stages is not None:
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/automation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/automation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/delivery_pipeline.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/delivery_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     'AutomationRulePromoteReleaseRule',
     'AutomationSelector',
     'AutomationSelectorTarget',
     'DeliveryPipelineCondition',
     'DeliveryPipelineConditionPipelineReadyCondition',
     'DeliveryPipelineConditionTargetsPresentCondition',
     'DeliveryPipelineConditionTargetsTypeCondition',
+    'DeliveryPipelineIamBindingCondition',
+    'DeliveryPipelineIamMemberCondition',
     'DeliveryPipelineSerialPipeline',
     'DeliveryPipelineSerialPipelineStage',
     'DeliveryPipelineSerialPipelineStageDeployParameter',
     'DeliveryPipelineSerialPipelineStageStrategy',
     'DeliveryPipelineSerialPipelineStageStrategyCanary',
     'DeliveryPipelineSerialPipelineStageStrategyCanaryCanaryDeployment',
     'DeliveryPipelineSerialPipelineStageStrategyCanaryCanaryDeploymentPostdeploy',
@@ -507,14 +509,68 @@
         """
         True if the targets are all a comparable type. For example this is true if all targets are GKE clusters. This is false if some targets are Cloud Run targets and others are GKE clusters.
         """
         return pulumi.get(self, "status")
 
 
 @pulumi.output_type
+class DeliveryPipelineIamBindingCondition(dict):
+    def __init__(__self__, *,
+                 expression: str,
+                 title: str,
+                 description: Optional[str] = None):
+        pulumi.set(__self__, "expression", expression)
+        pulumi.set(__self__, "title", title)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+
+    @property
+    @pulumi.getter
+    def expression(self) -> str:
+        return pulumi.get(self, "expression")
+
+    @property
+    @pulumi.getter
+    def title(self) -> str:
+        return pulumi.get(self, "title")
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[str]:
+        return pulumi.get(self, "description")
+
+
+@pulumi.output_type
+class DeliveryPipelineIamMemberCondition(dict):
+    def __init__(__self__, *,
+                 expression: str,
+                 title: str,
+                 description: Optional[str] = None):
+        pulumi.set(__self__, "expression", expression)
+        pulumi.set(__self__, "title", title)
+        if description is not None:
+            pulumi.set(__self__, "description", description)
+
+    @property
+    @pulumi.getter
+    def expression(self) -> str:
+        return pulumi.get(self, "expression")
+
+    @property
+    @pulumi.getter
+    def title(self) -> str:
+        return pulumi.get(self, "title")
+
+    @property
+    @pulumi.getter
+    def description(self) -> Optional[str]:
+        return pulumi.get(self, "description")
+
+
+@pulumi.output_type
 class DeliveryPipelineSerialPipeline(dict):
     def __init__(__self__, *,
                  stages: Optional[Sequence['outputs.DeliveryPipelineSerialPipelineStage']] = None):
         """
         :param Sequence['DeliveryPipelineSerialPipelineStageArgs'] stages: Each stage specifies configuration for a `Target`. The ordering of this list defines the promotion flow.
         """
         if stages is not None:
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddeploy/target.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddeploy/target.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/clouddomains/registration.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/clouddomains/registration.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/function_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/function_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/get_function.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/get_function.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/get_function_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/get_function_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctions/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctions/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/function_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/function_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/get_function.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/get_function.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/get_function_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/get_function_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudfunctionsv2/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudfunctionsv2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/get_group_lookup.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/get_group_lookup.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/get_group_memberships.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/get_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/get_groups.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/group_membership.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudidentity/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudidentity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudids/endpoint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudids/endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/domain_mapping.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/domain_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/get_locations.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/get_locations.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/get_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/get_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/get_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrun/service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrun/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_job_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_job_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/get_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/get_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/job_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/job_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudrunv2/service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudrunv2/service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudscheduler/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudscheduler/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/get_queue_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/get_queue_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/cloudtasks/queue_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/cloudtasks/queue_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/environment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/get_environment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/get_image_versions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/get_image_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/composer/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/composer/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 from .image_iam_member import *
 from .image_iam_policy import *
 from .instance import *
 from .instance_from_machine_image import *
 from .instance_from_template import *
 from .instance_group import *
 from .instance_group_manager import *
+from .instance_group_membership import *
 from .instance_group_named_port import *
 from .instance_iam_binding import *
 from .instance_iam_member import *
 from .instance_iam_policy import *
 from .instance_settings import *
 from .instance_template import *
 from .interconnect_attachment import *
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6119,30 +6119,47 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class InstanceConfidentialInstanceConfigArgs:
     def __init__(__self__, *,
-                 enable_confidential_compute: pulumi.Input[bool]):
+                 confidential_instance_type: Optional[pulumi.Input[str]] = None,
+                 enable_confidential_compute: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        :param pulumi.Input[str] confidential_instance_type: Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        """
+        return pulumi.get(self, "confidential_instance_type")
+
+    @confidential_instance_type.setter
+    def confidential_instance_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "confidential_instance_type", value)
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> pulumi.Input[bool]:
+    def enable_confidential_compute(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
 
     @enable_confidential_compute.setter
-    def enable_confidential_compute(self, value: pulumi.Input[bool]):
+    def enable_confidential_compute(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_confidential_compute", value)
 
 
 @pulumi.input_type
 class InstanceFromMachineImageAdvancedMachineFeaturesArgs:
     def __init__(__self__, *,
                  enable_nested_virtualization: Optional[pulumi.Input[bool]] = None,
@@ -6568,30 +6585,51 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class InstanceFromMachineImageConfidentialInstanceConfigArgs:
     def __init__(__self__, *,
-                 enable_confidential_compute: pulumi.Input[bool]):
+                 confidential_instance_type: Optional[pulumi.Input[str]] = None,
+                 enable_confidential_compute: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled.
+        :param pulumi.Input[str] confidential_instance_type: Specifies which confidential computing technology to use.
+               								This could be one of the following values: SEV, SEV_SNP.
+               								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specifies which confidential computing technology to use.
+        								This could be one of the following values: SEV, SEV_SNP.
+        								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        """
+        return pulumi.get(self, "confidential_instance_type")
+
+    @confidential_instance_type.setter
+    def confidential_instance_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "confidential_instance_type", value)
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> pulumi.Input[bool]:
+    def enable_confidential_compute(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defines whether the instance should have confidential compute enabled.
+        Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
         return pulumi.get(self, "enable_confidential_compute")
 
     @enable_confidential_compute.setter
-    def enable_confidential_compute(self, value: pulumi.Input[bool]):
+    def enable_confidential_compute(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_confidential_compute", value)
 
 
 @pulumi.input_type
 class InstanceFromMachineImageGuestAcceleratorArgs:
     def __init__(__self__, *,
                  count: pulumi.Input[int],
@@ -8098,30 +8136,51 @@
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class InstanceFromTemplateConfidentialInstanceConfigArgs:
     def __init__(__self__, *,
-                 enable_confidential_compute: pulumi.Input[bool]):
+                 confidential_instance_type: Optional[pulumi.Input[str]] = None,
+                 enable_confidential_compute: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled.
+        :param pulumi.Input[str] confidential_instance_type: Specifies which confidential computing technology to use.
+               								This could be one of the following values: SEV, SEV_SNP.
+               								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
+        """
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        Specifies which confidential computing technology to use.
+        								This could be one of the following values: SEV, SEV_SNP.
+        								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        """
+        return pulumi.get(self, "confidential_instance_type")
+
+    @confidential_instance_type.setter
+    def confidential_instance_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "confidential_instance_type", value)
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> pulumi.Input[bool]:
+    def enable_confidential_compute(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defines whether the instance should have confidential compute enabled.
+        Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
         return pulumi.get(self, "enable_confidential_compute")
 
     @enable_confidential_compute.setter
-    def enable_confidential_compute(self, value: pulumi.Input[bool]):
+    def enable_confidential_compute(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_confidential_compute", value)
 
 
 @pulumi.input_type
 class InstanceFromTemplateGuestAcceleratorArgs:
     def __init__(__self__, *,
                  count: pulumi.Input[int],
@@ -11354,30 +11413,47 @@
     def visible_core_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "visible_core_count", value)
 
 
 @pulumi.input_type
 class InstanceTemplateConfidentialInstanceConfigArgs:
     def __init__(__self__, *,
-                 enable_confidential_compute: pulumi.Input[bool]):
+                 confidential_instance_type: Optional[pulumi.Input[str]] = None,
+                 enable_confidential_compute: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[str] confidential_instance_type: Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        """
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        return pulumi.get(self, "confidential_instance_type")
+
+    @confidential_instance_type.setter
+    def confidential_instance_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "confidential_instance_type", value)
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> pulumi.Input[bool]:
+    def enable_confidential_compute(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
 
     @enable_confidential_compute.setter
-    def enable_confidential_compute(self, value: pulumi.Input[bool]):
+    def enable_confidential_compute(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_confidential_compute", value)
 
 
 @pulumi.input_type
 class InstanceTemplateDiskArgs:
     def __init__(__self__, *,
                  auto_delete: Optional[pulumi.Input[bool]] = None,
@@ -19172,30 +19248,47 @@
     def visible_core_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "visible_core_count", value)
 
 
 @pulumi.input_type
 class RegionInstanceTemplateConfidentialInstanceConfigArgs:
     def __init__(__self__, *,
-                 enable_confidential_compute: pulumi.Input[bool]):
+                 confidential_instance_type: Optional[pulumi.Input[str]] = None,
+                 enable_confidential_compute: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[str] confidential_instance_type: Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled on AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        """
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[pulumi.Input[str]]:
         """
-        :param pulumi.Input[bool] enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        return pulumi.get(self, "confidential_instance_type")
+
+    @confidential_instance_type.setter
+    def confidential_instance_type(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "confidential_instance_type", value)
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> pulumi.Input[bool]:
+    def enable_confidential_compute(self) -> Optional[pulumi.Input[bool]]:
         """
-        Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines whether the instance should have confidential compute enabled on AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
 
     @enable_confidential_compute.setter
-    def enable_confidential_compute(self, value: pulumi.Input[bool]):
+    def enable_confidential_compute(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_confidential_compute", value)
 
 
 @pulumi.input_type
 class RegionInstanceTemplateDiskArgs:
     def __init__(__self__, *,
                  auto_delete: Optional[pulumi.Input[bool]] = None,
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/address.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/address.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/attached_disk.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/attached_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/autoscaler.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/autoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_bucket_signed_url_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_bucket_signed_url_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/backend_service_signed_url_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/backend_service_signed_url_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ca_external_account_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ca_external_account_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_async_replication.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_async_replication.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/disk_resource_policy_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/disk_resource_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/external_vpn_gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/external_vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall_policy_association.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall_policy_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/firewall_policy_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/firewall_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/forwarding_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_address.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_addresses.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_addresses.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_bucket.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_bucket_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_bucket_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_default_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_default_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_disk.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_disk_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_disk_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_forwarding_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_global_address.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_global_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_global_forwarding_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_global_forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_hc_vpn_gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_hc_vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_health_check.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_health_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_image.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_image_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_image_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_group_manager.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_group_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_serial_port.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_serial_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_instance_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_instance_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_lbip_ranges.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_lbip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_machine_image_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_machine_image_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_machine_types.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_machine_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_netblock_ip_ranges.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_netblock_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_network.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_network_endpoint_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_network_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_network_peering.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_network_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_networks.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_node_types.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_node_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_disk.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_disk_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_disk_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_instance_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_instance_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_instance_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_instance_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_network_endpoint_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_network_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_region_ssl_certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_region_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_regions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_reservation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_resource_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_resource_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_router.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_router.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_router_nat.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_router_nat.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_router_status.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_router_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_snapshot.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_snapshot_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_snapshot_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_ssl_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_ssl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_subnetwork.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_subnetwork.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_subnetwork_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_subnetwork_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_vpn_gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/get_zones.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/get_zones.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_address.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_forwarding_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_network_endpoint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_network_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/global_network_endpoint_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/global_network_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ha_vpn_gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ha_vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/health_check.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/health_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/http_health_check.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/http_health_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/https_health_check.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/https_health_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/image_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/image_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_from_machine_image.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_from_machine_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_from_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_from_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_group_manager.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_group_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_group_named_port.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_group_named_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/instance_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/instance_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/interconnect_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/interconnect_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/machine_image_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/machine_image_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/managed_ssl_certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/managed_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/manged_ssl_certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/manged_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_edge_security_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_edge_security_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_endpoint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_endpoint_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_endpoint_list.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_endpoint_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_firewall_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_firewall_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_firewall_policy_association.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_firewall_policy_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_firewall_policy_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_firewall_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_peering.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/network_peering_routes_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/network_peering_routes_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/node_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/node_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/node_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/organization_security_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/organization_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/organization_security_policy_association.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/organization_security_policy_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/organization_security_policy_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/organization_security_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -6151,40 +6151,55 @@
 
 
 @pulumi.output_type
 class InstanceConfidentialInstanceConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "enableConfidentialCompute":
+        if key == "confidentialInstanceType":
+            suggest = "confidential_instance_type"
+        elif key == "enableConfidentialCompute":
             suggest = "enable_confidential_compute"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in InstanceConfidentialInstanceConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         InstanceConfidentialInstanceConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         InstanceConfidentialInstanceConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 enable_confidential_compute: bool):
+                 confidential_instance_type: Optional[str] = None,
+                 enable_confidential_compute: Optional[bool] = None):
         """
-        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        :param str confidential_instance_type: Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[str]:
+        """
+        Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        """
+        return pulumi.get(self, "confidential_instance_type")
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> bool:
+    def enable_confidential_compute(self) -> Optional[bool]:
         """
-        Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
 
 
 @pulumi.output_type
 class InstanceFromMachineImageAdvancedMachineFeatures(dict):
     @staticmethod
@@ -6607,40 +6622,59 @@
 
 
 @pulumi.output_type
 class InstanceFromMachineImageConfidentialInstanceConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "enableConfidentialCompute":
+        if key == "confidentialInstanceType":
+            suggest = "confidential_instance_type"
+        elif key == "enableConfidentialCompute":
             suggest = "enable_confidential_compute"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in InstanceFromMachineImageConfidentialInstanceConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         InstanceFromMachineImageConfidentialInstanceConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         InstanceFromMachineImageConfidentialInstanceConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 enable_confidential_compute: bool):
+                 confidential_instance_type: Optional[str] = None,
+                 enable_confidential_compute: Optional[bool] = None):
         """
-        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled.
+        :param str confidential_instance_type: Specifies which confidential computing technology to use.
+               								This could be one of the following values: SEV, SEV_SNP.
+               								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[str]:
+        """
+        Specifies which confidential computing technology to use.
+        								This could be one of the following values: SEV, SEV_SNP.
+        								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        """
+        return pulumi.get(self, "confidential_instance_type")
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> bool:
+    def enable_confidential_compute(self) -> Optional[bool]:
         """
-        Defines whether the instance should have confidential compute enabled.
+        Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
         return pulumi.get(self, "enable_confidential_compute")
 
 
 @pulumi.output_type
 class InstanceFromMachineImageGuestAccelerator(dict):
     def __init__(__self__, *,
@@ -8130,40 +8164,59 @@
 
 
 @pulumi.output_type
 class InstanceFromTemplateConfidentialInstanceConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "enableConfidentialCompute":
+        if key == "confidentialInstanceType":
+            suggest = "confidential_instance_type"
+        elif key == "enableConfidentialCompute":
             suggest = "enable_confidential_compute"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in InstanceFromTemplateConfidentialInstanceConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         InstanceFromTemplateConfidentialInstanceConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         InstanceFromTemplateConfidentialInstanceConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 enable_confidential_compute: bool):
+                 confidential_instance_type: Optional[str] = None,
+                 enable_confidential_compute: Optional[bool] = None):
         """
-        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled.
+        :param str confidential_instance_type: Specifies which confidential computing technology to use.
+               								This could be one of the following values: SEV, SEV_SNP.
+               								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[str]:
+        """
+        Specifies which confidential computing technology to use.
+        								This could be one of the following values: SEV, SEV_SNP.
+        								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        """
+        return pulumi.get(self, "confidential_instance_type")
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> bool:
+    def enable_confidential_compute(self) -> Optional[bool]:
         """
-        Defines whether the instance should have confidential compute enabled.
+        Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
         return pulumi.get(self, "enable_confidential_compute")
 
 
 @pulumi.output_type
 class InstanceFromTemplateGuestAccelerator(dict):
     def __init__(__self__, *,
@@ -11417,40 +11470,55 @@
 
 
 @pulumi.output_type
 class InstanceTemplateConfidentialInstanceConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "enableConfidentialCompute":
+        if key == "confidentialInstanceType":
+            suggest = "confidential_instance_type"
+        elif key == "enableConfidentialCompute":
             suggest = "enable_confidential_compute"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in InstanceTemplateConfidentialInstanceConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         InstanceTemplateConfidentialInstanceConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         InstanceTemplateConfidentialInstanceConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 enable_confidential_compute: bool):
+                 confidential_instance_type: Optional[str] = None,
+                 enable_confidential_compute: Optional[bool] = None):
         """
-        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        :param str confidential_instance_type: Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[str]:
+        """
+        Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        """
+        return pulumi.get(self, "confidential_instance_type")
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> bool:
+    def enable_confidential_compute(self) -> Optional[bool]:
         """
-        Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines whether the instance should have confidential compute enabled with AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
 
 
 @pulumi.output_type
 class InstanceTemplateDisk(dict):
     @staticmethod
@@ -19226,40 +19294,55 @@
 
 
 @pulumi.output_type
 class RegionInstanceTemplateConfidentialInstanceConfig(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "enableConfidentialCompute":
+        if key == "confidentialInstanceType":
+            suggest = "confidential_instance_type"
+        elif key == "enableConfidentialCompute":
             suggest = "enable_confidential_compute"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in RegionInstanceTemplateConfidentialInstanceConfig. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         RegionInstanceTemplateConfidentialInstanceConfig.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         RegionInstanceTemplateConfidentialInstanceConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 enable_confidential_compute: bool):
+                 confidential_instance_type: Optional[str] = None,
+                 enable_confidential_compute: Optional[bool] = None):
         """
-        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        :param str confidential_instance_type: Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled on AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
-        pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+        if confidential_instance_type is not None:
+            pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
+        if enable_confidential_compute is not None:
+            pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
+
+    @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> Optional[str]:
+        """
+        Defines the confidential computing technology the instance uses. SEV is an AMD feature. One of the following values: `SEV`, `SEV_SNP`. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM. If `SEV_SNP`, currently `min_cpu_platform` has to be set to `"AMD Milan"` or this will fail to create the VM.
+        """
+        return pulumi.get(self, "confidential_instance_type")
 
     @property
     @pulumi.getter(name="enableConfidentialCompute")
-    def enable_confidential_compute(self) -> bool:
+    def enable_confidential_compute(self) -> Optional[bool]:
         """
-        Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
+        Defines whether the instance should have confidential compute enabled on AMD SEV. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
 
 
 @pulumi.output_type
 class RegionInstanceTemplateDisk(dict):
     @staticmethod
@@ -40963,25 +41046,40 @@
         """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class GetInstanceConfidentialInstanceConfigResult(dict):
     def __init__(__self__, *,
+                 confidential_instance_type: str,
                  enable_confidential_compute: bool):
         """
-        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled.
+        :param str confidential_instance_type: Specifies which confidential computing technology to use.
+               								This could be one of the following values: SEV, SEV_SNP.
+               								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
+        pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
         pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
 
     @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> str:
+        """
+        Specifies which confidential computing technology to use.
+        								This could be one of the following values: SEV, SEV_SNP.
+        								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        """
+        return pulumi.get(self, "confidential_instance_type")
+
+    @property
     @pulumi.getter(name="enableConfidentialCompute")
     def enable_confidential_compute(self) -> bool:
         """
-        Defines whether the instance should have confidential compute enabled.
+        Defines whether the instance should have confidential compute enabled. Field will be deprecated in a future release
         """
         return pulumi.get(self, "enable_confidential_compute")
 
 
 @pulumi.output_type
 class GetInstanceGroupManagerAllInstancesConfigResult(dict):
     def __init__(__self__, *,
@@ -42350,21 +42448,36 @@
         """
         return pulumi.get(self, "visible_core_count")
 
 
 @pulumi.output_type
 class GetInstanceTemplateConfidentialInstanceConfigResult(dict):
     def __init__(__self__, *,
+                 confidential_instance_type: str,
                  enable_confidential_compute: bool):
         """
+        :param str confidential_instance_type: Specifies which confidential computing technology to use.
+               								This could be one of the following values: SEV, SEV_SNP.
+               								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
         :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
+        pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
         pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
 
     @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> str:
+        """
+        Specifies which confidential computing technology to use.
+        								This could be one of the following values: SEV, SEV_SNP.
+        								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        """
+        return pulumi.get(self, "confidential_instance_type")
+
+    @property
     @pulumi.getter(name="enableConfidentialCompute")
     def enable_confidential_compute(self) -> bool:
         """
         Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
 
@@ -43968,21 +44081,36 @@
         """
         return pulumi.get(self, "visible_core_count")
 
 
 @pulumi.output_type
 class GetRegionInstanceTemplateConfidentialInstanceConfigResult(dict):
     def __init__(__self__, *,
+                 confidential_instance_type: str,
                  enable_confidential_compute: bool):
         """
+        :param str confidential_instance_type: Specifies which confidential computing technology to use.
+               								This could be one of the following values: SEV, SEV_SNP.
+               								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
         :param bool enable_confidential_compute: Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
+        pulumi.set(__self__, "confidential_instance_type", confidential_instance_type)
         pulumi.set(__self__, "enable_confidential_compute", enable_confidential_compute)
 
     @property
+    @pulumi.getter(name="confidentialInstanceType")
+    def confidential_instance_type(self) -> str:
+        """
+        Specifies which confidential computing technology to use.
+        								This could be one of the following values: SEV, SEV_SNP.
+        								If SEV_SNP, min_cpu_platform = "AMD Milan" is currently required.
+        """
+        return pulumi.get(self, "confidential_instance_type")
+
+    @property
     @pulumi.getter(name="enableConfidentialCompute")
     def enable_confidential_compute(self) -> bool:
         """
         Defines whether the instance should have confidential compute enabled. `on_host_maintenance` has to be set to TERMINATE or this will fail to create the VM.
         """
         return pulumi.get(self, "enable_confidential_compute")
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/packet_mirroring.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/packet_mirroring.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/per_instance_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/per_instance_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/project_default_network_tier.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/project_default_network_tier.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/project_metadata.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/project_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/project_metadata_item.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/project_metadata_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/public_advertised_prefix.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/public_advertised_prefix.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/public_delegated_prefix.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/public_delegated_prefix.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_autoscaler.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_autoscaler.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_commitment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_commitment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_disk_resource_policy_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_disk_resource_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_health_check.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_health_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_instance_group_manager.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_instance_group_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_instance_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_instance_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_endpoint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_endpoint_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_firewall_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_firewall_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_firewall_policy_association.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_firewall_policy_association.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_network_firewall_policy_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_network_firewall_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_per_instance_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_per_instance_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_security_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_security_policy_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_security_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_ssl_certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_ssl_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_ssl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_target_http_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_target_http_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_target_https_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_target_https_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_target_tcp_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_target_tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/region_url_map.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/region_url_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/reservation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/resource_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/resource_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/route.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/route.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_interface.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_nat.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_nat.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_peer.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_peer.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/router_status.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/router_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/security_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/security_scan_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/security_scan_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/service_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/service_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/shared_vpc_host_project.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/shared_vpc_host_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/shared_vpc_service_project.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/shared_vpc_service_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/snapshot_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/snapshot_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ssl_certificate.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ssl_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/ssl_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/ssl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/subnetwork_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/subnetwork_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_grpc_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_grpc_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_http_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_http_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_https_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_https_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_ssl_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_ssl_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/target_tcp_proxy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/target_tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/url_map.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/url_map.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/vpn_gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/vpn_gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/compute/vpn_tunnel.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/compute/vpn_tunnel.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/__init__.pyi` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 accessContextManagerCustomEndpoint: Optional[str]
 
 accessToken: Optional[str]
 
 activeDirectoryCustomEndpoint: Optional[str]
 
+addTerraformAttributionLabel: Optional[bool]
+
 alloydbCustomEndpoint: Optional[str]
 
 apiGatewayCustomEndpoint: Optional[str]
 
 apigeeCustomEndpoint: Optional[str]
 
 apikeysCustomEndpoint: Optional[str]
@@ -162,14 +164,16 @@
 
 essentialContactsCustomEndpoint: Optional[str]
 
 eventarcCustomEndpoint: Optional[str]
 
 filestoreCustomEndpoint: Optional[str]
 
+firebaseAppCheckCustomEndpoint: Optional[str]
+
 firebaseCustomEndpoint: Optional[str]
 
 firebaseDatabaseCustomEndpoint: Optional[str]
 
 firebaseExtensionsCustomEndpoint: Optional[str]
 
 firebaseHostingCustomEndpoint: Optional[str]
@@ -306,14 +310,16 @@
 
 storageTransferCustomEndpoint: Optional[str]
 
 tagsCustomEndpoint: Optional[str]
 
 tagsLocationCustomEndpoint: Optional[str]
 
+terraformAttributionLabelAdditionStrategy: Optional[str]
+
 tpuCustomEndpoint: Optional[str]
 
 tpuV2CustomEndpoint: Optional[str]
 
 universeDomain: Optional[str]
 
 userProjectOverride: Optional[bool]
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/config/vars.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/config/vars.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,18 @@
         return __config__.get('accessToken')
 
     @property
     def active_directory_custom_endpoint(self) -> Optional[str]:
         return __config__.get('activeDirectoryCustomEndpoint')
 
     @property
+    def add_terraform_attribution_label(self) -> Optional[bool]:
+        return __config__.get_bool('addTerraformAttributionLabel')
+
+    @property
     def alloydb_custom_endpoint(self) -> Optional[str]:
         return __config__.get('alloydbCustomEndpoint')
 
     @property
     def api_gateway_custom_endpoint(self) -> Optional[str]:
         return __config__.get('apiGatewayCustomEndpoint')
 
@@ -325,14 +329,18 @@
         return __config__.get('eventarcCustomEndpoint')
 
     @property
     def filestore_custom_endpoint(self) -> Optional[str]:
         return __config__.get('filestoreCustomEndpoint')
 
     @property
+    def firebase_app_check_custom_endpoint(self) -> Optional[str]:
+        return __config__.get('firebaseAppCheckCustomEndpoint')
+
+    @property
     def firebase_custom_endpoint(self) -> Optional[str]:
         return __config__.get('firebaseCustomEndpoint')
 
     @property
     def firebase_database_custom_endpoint(self) -> Optional[str]:
         return __config__.get('firebaseDatabaseCustomEndpoint')
 
@@ -613,14 +621,18 @@
         return __config__.get('tagsCustomEndpoint')
 
     @property
     def tags_location_custom_endpoint(self) -> Optional[str]:
         return __config__.get('tagsLocationCustomEndpoint')
 
     @property
+    def terraform_attribution_label_addition_strategy(self) -> Optional[str]:
+        return __config__.get('terraformAttributionLabelAdditionStrategy')
+
+    @property
     def tpu_custom_endpoint(self) -> Optional[str]:
         return __config__.get('tpuCustomEndpoint')
 
     @property
     def tpu_v2_custom_endpoint(self) -> Optional[str]:
         return __config__.get('tpuV2CustomEndpoint')
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/attached_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/attached_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/aws_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/aws_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/aws_node_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/aws_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/azure_client.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/azure_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/azure_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/azure_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/azure_node_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/azure_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_attached_install_manifest.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_attached_install_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_attached_versions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_attached_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_aws_versions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_aws_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_azure_versions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_azure_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_engine_versions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_engine_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_registry_image.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/get_registry_repository.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/get_registry_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/node_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/container/registry.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/container/registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/get_note_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/get_note_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/note_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/note_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/occurence.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/occurence.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/containeranalysis/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/containeranalysis/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/connection_profile.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/connection_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/databasemigrationservice/private_connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/databasemigrationservice/private_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/entry_group_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/entry_group_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_entry_group_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_entry_group_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_policy_tag_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_policy_tag_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_tag_template_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_tag_template_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/get_taxonomy_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/get_taxonomy_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/policy_tag_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/policy_tag_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/tag_template_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/tag_template_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datacatalog/taxonomy_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datacatalog/taxonomy_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/flex_template_job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/flex_template_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataflow/pipeline.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataflow/pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/get_repository_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/get_repository_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_release_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_release_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataform/repository_workflow_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataform/repository_workflow_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/get_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/get_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datafusion/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datafusion/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_deidentify_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_deidentify_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_inspect_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_inspect_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_job_trigger.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_job_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataloss/prevention_stored_info_type.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataloss/prevention_stored_info_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/asset_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/asset_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/datascan_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/datascan_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_asset_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_asset_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_datascan_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_datascan_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_lake_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_lake_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_task_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_task_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/get_zone_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/get_zone_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/lake_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/lake_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/task_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/task_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataplex/zone_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataplex/zone_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/autoscaling_policy_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/autoscaling_policy_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/cluster_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/cluster_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_autoscaling_policy_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_autoscaling_policy_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_cluster_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_cluster_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_job_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_job_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_metastore_federation_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_metastore_federation_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/get_metastore_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/get_metastore_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/job_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/job_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_federation_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_federation_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/metastore_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/metastore_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dataproc/workflow_template.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dataproc/workflow_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/data_store_index.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/data_store_index.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastore/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastore/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/connection_profile.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/connection_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/get_static_ips.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/get_static_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/private_connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/private_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/datastream/stream.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/datastream/stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/deployment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/deploymentmanager/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/deploymentmanager/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/agent.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_agent.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_entity_type.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_entity_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_environment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_flow.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_flow.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_intent.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_intent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_page.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_security_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_security_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_test_case.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_test_case.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/cx_webhook.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/cx_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/entity_type.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/entity_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/fulfillment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/fulfillment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/intent.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/intent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/diagflow/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/diagflow/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/chat_engine.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/chat_engine.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/data_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/data_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/discoveryengine/search_engine.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/discoveryengine/search_engine.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/dns_managed_zone_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/dns_managed_zone_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/dns_managed_zone_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/dns_managed_zone_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/dns_managed_zone_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/dns_managed_zone_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_keys.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_managed_zone.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_managed_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_managed_zone_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_managed_zone_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_managed_zones.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_managed_zones.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/get_record_set.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/get_record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/managed_zone.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/managed_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/record_set.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/response_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/response_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/dns/response_policy_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/dns/response_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/node_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgecontainer/vpn_connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgecontainer/vpn_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgenetwork/network.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgenetwork/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/edgenetwork/subnet.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/edgenetwork/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/consumers_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/consumers_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/consumers_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/consumers_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/consumers_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/consumers_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/get_service_consumers_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/get_service_consumers_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/get_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/get_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/endpoints/service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/endpoints/service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/contact.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/contact.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_processor.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_processor.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_processor_default_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_processor_default_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_warehouse_document_schema.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_warehouse_document_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/document_ai_warehouse_location.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/document_ai_warehouse_location.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/essentialcontacts/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/essentialcontacts/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/channel.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/google_channel_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/google_channel_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/eventarc/trigger.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/eventarc/trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/backup.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/backup.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/get_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/filestore/snapshot.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/filestore/snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from .. import _utilities
 import typing
 # Export this package's modules as members:
 from .android_app import *
+from .app_check_service_config import *
 from .apple_app import *
 from .database_instance import *
 from .extensions_instance import *
 from .get_android_app import *
 from .get_android_app_config import *
 from .get_apple_app import *
 from .get_apple_app_config import *
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -898,19 +898,19 @@
         pulumi.set(self, "path", value)
 
 
 @pulumi.input_type
 class HostingCustomDomainIssueArgs:
     def __init__(__self__, *,
                  code: Optional[pulumi.Input[int]] = None,
-                 details: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]] = None,
+                 details: Optional[pulumi.Input[str]] = None,
                  message: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[int] code: The status code, which should be an enum value of `google.rpc.Code`
-        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]] details: A list of messages that carry the error details.
+        :param pulumi.Input[str] details: A list of messages that carry the error details.
         :param pulumi.Input[str] message: Error message
         """
         if code is not None:
             pulumi.set(__self__, "code", code)
         if details is not None:
             pulumi.set(__self__, "details", details)
         if message is not None:
@@ -926,22 +926,22 @@
 
     @code.setter
     def code(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "code", value)
 
     @property
     @pulumi.getter
-    def details(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]]:
+    def details(self) -> Optional[pulumi.Input[str]]:
         """
         A list of messages that carry the error details.
         """
         return pulumi.get(self, "details")
 
     @details.setter
-    def details(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, Any]]]]]):
+    def details(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "details", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
         """
         Error message
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/android_app.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/android_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/apple_app.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/apple_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/database_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/database_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/extensions_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/extensions_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_android_app.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_android_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_android_app_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_android_app_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_apple_app.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_apple_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_apple_app_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_apple_app_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_hosting_channel.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_hosting_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_web_app.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_web_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/get_web_app_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/get_web_app_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_channel.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_custom_domain.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_release.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_release.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_site.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_site.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/hosting_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/hosting_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -921,19 +921,19 @@
         return pulumi.get(self, "path")
 
 
 @pulumi.output_type
 class HostingCustomDomainIssue(dict):
     def __init__(__self__, *,
                  code: Optional[int] = None,
-                 details: Optional[Sequence[Mapping[str, Any]]] = None,
+                 details: Optional[str] = None,
                  message: Optional[str] = None):
         """
         :param int code: The status code, which should be an enum value of `google.rpc.Code`
-        :param Sequence[Mapping[str, Any]] details: A list of messages that carry the error details.
+        :param str details: A list of messages that carry the error details.
         :param str message: Error message
         """
         if code is not None:
             pulumi.set(__self__, "code", code)
         if details is not None:
             pulumi.set(__self__, "details", details)
         if message is not None:
@@ -945,15 +945,15 @@
         """
         The status code, which should be an enum value of `google.rpc.Code`
         """
         return pulumi.get(self, "code")
 
     @property
     @pulumi.getter
-    def details(self) -> Optional[Sequence[Mapping[str, Any]]]:
+    def details(self) -> Optional[str]:
         """
         A list of messages that carry the error details.
         """
         return pulumi.get(self, "details")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/project.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/storage_bucket.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebase/web_app.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebase/web_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/release.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/release.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firebaserules/ruleset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firebaserules/ruleset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/backup_schedule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/backup_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/database.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/document.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/document.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/field.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/field.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/index.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/index.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/firestore/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/firestore/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/access_approval_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/access_approval_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/get_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/get_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/get_organization_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/get_organization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_audit_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_audit_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/organization_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/organization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/folder/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/folder/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/backup_plan_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/backup_plan_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/get_backup_plan_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/get_backup_plan_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/get_restore_plan_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/get_restore_plan_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkebackup/restore_plan_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkebackup/restore_plan_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/feature_membership.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/feature_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/fleet.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/fleet.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/get_feature_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/get_feature_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/get_membership_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/get_membership_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/get_scope_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/get_scope_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/membership_rbac_role_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/membership_rbac_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/namespace.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkehub/scope_rbac_role_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkehub/scope_rbac_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/bare_metal_admin_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/bare_metal_admin_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/bare_metal_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/bare_metal_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/bare_metal_node_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/bare_metal_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/v_mware_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/v_mware_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/gkeonprem/v_mware_node_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/gkeonprem/v_mware_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/consent_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/consent_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dataset_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dataset_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/dicom_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/dicom_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/fhir_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/fhir_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_consent_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_consent_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_dataset_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_dataset_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_dicom_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_dicom_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_fhir_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_fhir_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/get_hl7_v2_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/get_hl7_v2_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/hl7_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/hl7_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/healthcare/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/healthcare/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/access_boundary_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/access_boundary_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/deny_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/deny_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_testable_permissions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_testable_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_workload_identity_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_workload_identity_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/get_workload_identity_pool_provider.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/get_workload_identity_pool_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workforce_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workforce_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workforce_pool_provider.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workforce_pool_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workload_identity_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workload_identity_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iam/workload_identity_pool_provider.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iam/workload_identity_pool_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_version_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_version_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_version_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_version_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/app_engine_version_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/app_engine_version_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/brand.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/client.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_app_engine_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_app_engine_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_app_engine_version_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_app_engine_version_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_client.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_tunnel_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_tunnel_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_tunnel_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_tunnel_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_region_backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_region_backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_type_app_engine_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_type_app_engine_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/get_web_type_compute_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/get_web_type_compute_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/tunnel_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/tunnel_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_backend_service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_backend_service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_backend_service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_backend_service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_region_backend_service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_region_backend_service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_region_backend_service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_region_backend_service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_region_backend_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_region_backend_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_app_enging_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_app_enging_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_app_enging_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_app_enging_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_app_enging_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_app_enging_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_compute_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_compute_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_compute_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_compute_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/iap/web_type_compute_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/iap/web_type_compute_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/default_supported_idp_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/default_supported_idp_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/inbound_saml_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/inbound_saml_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/oauth_idp_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/oauth_idp_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/project_default_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/project_default_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant_default_supported_idp_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant_default_supported_idp_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant_inbound_saml_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant_inbound_saml_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/identityplatform/tenant_oauth_idp_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/identityplatform/tenant_oauth_idp_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/endpoint_attachment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/endpoint_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/integrationconnectors/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/integrationconnectors/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/crypto_key_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/crypto_key_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_crypto_key_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_crypto_key_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_key_ring_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_key_ring_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_crypto_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_crypto_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_crypto_key_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_crypto_key_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_key_ring.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_key_ring.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_secret.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_secret_asymmetric.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_secret_asymmetric.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/get_kms_secret_ciphertext.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/get_kms_secret_ciphertext.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/key_ring_import_job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/key_ring_import_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/kms/secret_ciphertext.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/kms/secret_ciphertext.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/billing_account_bucket_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/billing_account_bucket_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/billing_account_exclusion.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/billing_account_exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/billing_account_sink.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/billing_account_sink.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_bucket_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_bucket_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_exclusion.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/folder_sink.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/folder_sink.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_folder_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_folder_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_organization_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_organization_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_project_cmek_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_project_cmek_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_project_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_project_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/get_sink.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/get_sink.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/linked_dataset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/linked_dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/log_view.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/log_view.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/metric.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_bucket_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_bucket_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_exclusion.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/organization_sink.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/organization_sink.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/project_bucket_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/project_bucket_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/project_exclusion.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/project_exclusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/logging/project_sink.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/logging/project_sink.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/looker/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/looker/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/memcache/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/memcache/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/migrationcenter/group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/migrationcenter/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/engine_model.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/engine_model.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/ml/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/ml/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/alert_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/alert_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/custom_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/custom_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/dashboard.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/dashboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/generic_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/generic_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_app_engine_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_app_engine_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_cluster_istio_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_cluster_istio_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_istio_canonical_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_istio_canonical_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_mesh_istio_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_mesh_istio_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_notification_channel.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_notification_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_secret_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_secret_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/get_uptime_check_i_ps.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/get_uptime_check_i_ps.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/metric_descriptor.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/metric_descriptor.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/monitored_project.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/monitored_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/notification_channel.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/notification_channel.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/slo.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/slo.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/monitoring/uptime_check_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/monitoring/uptime_check_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/active_directory.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/active_directory.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/backup_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/backup_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/backup_vault.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/backup_vault.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/kmsconfig.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/kmsconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/storage_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/storage_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/volume.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/netapp/volume_snapshot.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/netapp/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/hub.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/policy_based_route.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/policy_based_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/service_connection_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/service_connection_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkconnectivity/spoke.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkconnectivity/spoke.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/connectivity_test.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/connectivity_test.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkmanagement/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkmanagement/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/address_group_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/address_group_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/authorization_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/authorization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/client_tls_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/client_tls_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/gateway_security_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/gateway_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/gateway_security_policy_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/gateway_security_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/get_address_group_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/get_address_group_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/security_profile.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/security_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/server_tls_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/server_tls_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/tls_inspection_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/tls_inspection_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networksecurity/url_list.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networksecurity/url_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/edge_cache_keyset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/edge_cache_keyset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/edge_cache_origin.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/edge_cache_origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/edge_cache_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/edge_cache_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/endpoint_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/endpoint_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/gateway.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/gateway.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/grpc_route.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/grpc_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/http_route.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/http_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/mesh.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/mesh.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/service_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/service_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/tcp_route.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/tcp_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/networkservices/tls_route.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/networkservices/tls_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/environment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/get_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/get_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/get_runtime_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/get_runtime_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/location.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/location.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/notebooks/runtime_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/notebooks/runtime_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/access_approval_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/access_approval_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/folder.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_active_folder.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_active_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_billing_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_billing_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_client_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_client_open_id_user_info.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_client_open_id_user_info.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_folder.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_folders.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_folders.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_organization.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/get_project.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_audit_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_audit_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_custom_role.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/organizations/project.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/organizations/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/custom_constraint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/custom_constraint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/orgpolicy/policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/orgpolicy/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/guest_policies.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/guest_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/os_policy_assignment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/os_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/osconfig/patch_deployment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/osconfig/patch_deployment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/oslogin/ssh_public_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/oslogin/ssh_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/access_approval_settings.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/access_approval_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/api_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/default_service_accounts.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/default_service_accounts.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_organization_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_organization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_project.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/get_project_service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/get_project_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_audit_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_audit_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_custom_role.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_custom_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/organization_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/organization_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/service_identity.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/service_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/projects/usage_export_bucket.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/projects/usage_export_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/provider.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @pulumi.input_type
 class ProviderArgs:
     def __init__(__self__, *,
                  access_approval_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  access_context_manager_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  active_directory_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 add_terraform_attribution_label: Optional[pulumi.Input[bool]] = None,
                  alloydb_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  api_gateway_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  apigee_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  apikeys_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  app_engine_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  artifact_registry_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  assured_workloads_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -89,14 +90,15 @@
                  document_ai_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  document_ai_warehouse_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  edgecontainer_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  edgenetwork_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  essential_contacts_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  eventarc_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  filestore_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 firebase_app_check_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_database_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_extensions_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_hosting_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_storage_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebaserules_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firestore_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -161,14 +163,15 @@
                  spanner_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  sql_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_insights_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_transfer_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tags_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tags_location_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 terraform_attribution_label_addition_strategy: Optional[pulumi.Input[str]] = None,
                  tpu_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tpu_v2_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  universe_domain: Optional[pulumi.Input[str]] = None,
                  user_project_override: Optional[pulumi.Input[bool]] = None,
                  vertex_ai_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  vmwareengine_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  vpc_access_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -183,14 +186,16 @@
             pulumi.set(__self__, "access_approval_custom_endpoint", access_approval_custom_endpoint)
         if access_context_manager_custom_endpoint is not None:
             pulumi.set(__self__, "access_context_manager_custom_endpoint", access_context_manager_custom_endpoint)
         if access_token is not None:
             pulumi.set(__self__, "access_token", access_token)
         if active_directory_custom_endpoint is not None:
             pulumi.set(__self__, "active_directory_custom_endpoint", active_directory_custom_endpoint)
+        if add_terraform_attribution_label is not None:
+            pulumi.set(__self__, "add_terraform_attribution_label", add_terraform_attribution_label)
         if alloydb_custom_endpoint is not None:
             pulumi.set(__self__, "alloydb_custom_endpoint", alloydb_custom_endpoint)
         if api_gateway_custom_endpoint is not None:
             pulumi.set(__self__, "api_gateway_custom_endpoint", api_gateway_custom_endpoint)
         if apigee_custom_endpoint is not None:
             pulumi.set(__self__, "apigee_custom_endpoint", apigee_custom_endpoint)
         if apikeys_custom_endpoint is not None:
@@ -331,14 +336,16 @@
             pulumi.set(__self__, "edgenetwork_custom_endpoint", edgenetwork_custom_endpoint)
         if essential_contacts_custom_endpoint is not None:
             pulumi.set(__self__, "essential_contacts_custom_endpoint", essential_contacts_custom_endpoint)
         if eventarc_custom_endpoint is not None:
             pulumi.set(__self__, "eventarc_custom_endpoint", eventarc_custom_endpoint)
         if filestore_custom_endpoint is not None:
             pulumi.set(__self__, "filestore_custom_endpoint", filestore_custom_endpoint)
+        if firebase_app_check_custom_endpoint is not None:
+            pulumi.set(__self__, "firebase_app_check_custom_endpoint", firebase_app_check_custom_endpoint)
         if firebase_custom_endpoint is not None:
             pulumi.set(__self__, "firebase_custom_endpoint", firebase_custom_endpoint)
         if firebase_database_custom_endpoint is not None:
             pulumi.set(__self__, "firebase_database_custom_endpoint", firebase_database_custom_endpoint)
         if firebase_extensions_custom_endpoint is not None:
             pulumi.set(__self__, "firebase_extensions_custom_endpoint", firebase_extensions_custom_endpoint)
         if firebase_hosting_custom_endpoint is not None:
@@ -479,14 +486,16 @@
             pulumi.set(__self__, "storage_insights_custom_endpoint", storage_insights_custom_endpoint)
         if storage_transfer_custom_endpoint is not None:
             pulumi.set(__self__, "storage_transfer_custom_endpoint", storage_transfer_custom_endpoint)
         if tags_custom_endpoint is not None:
             pulumi.set(__self__, "tags_custom_endpoint", tags_custom_endpoint)
         if tags_location_custom_endpoint is not None:
             pulumi.set(__self__, "tags_location_custom_endpoint", tags_location_custom_endpoint)
+        if terraform_attribution_label_addition_strategy is not None:
+            pulumi.set(__self__, "terraform_attribution_label_addition_strategy", terraform_attribution_label_addition_strategy)
         if tpu_custom_endpoint is not None:
             pulumi.set(__self__, "tpu_custom_endpoint", tpu_custom_endpoint)
         if tpu_v2_custom_endpoint is not None:
             pulumi.set(__self__, "tpu_v2_custom_endpoint", tpu_v2_custom_endpoint)
         if universe_domain is not None:
             pulumi.set(__self__, "universe_domain", universe_domain)
         if user_project_override is not None:
@@ -541,14 +550,23 @@
         return pulumi.get(self, "active_directory_custom_endpoint")
 
     @active_directory_custom_endpoint.setter
     def active_directory_custom_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "active_directory_custom_endpoint", value)
 
     @property
+    @pulumi.getter(name="addTerraformAttributionLabel")
+    def add_terraform_attribution_label(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "add_terraform_attribution_label")
+
+    @add_terraform_attribution_label.setter
+    def add_terraform_attribution_label(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "add_terraform_attribution_label", value)
+
+    @property
     @pulumi.getter(name="alloydbCustomEndpoint")
     def alloydb_custom_endpoint(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "alloydb_custom_endpoint")
 
     @alloydb_custom_endpoint.setter
     def alloydb_custom_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alloydb_custom_endpoint", value)
@@ -1207,14 +1225,23 @@
         return pulumi.get(self, "filestore_custom_endpoint")
 
     @filestore_custom_endpoint.setter
     def filestore_custom_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "filestore_custom_endpoint", value)
 
     @property
+    @pulumi.getter(name="firebaseAppCheckCustomEndpoint")
+    def firebase_app_check_custom_endpoint(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "firebase_app_check_custom_endpoint")
+
+    @firebase_app_check_custom_endpoint.setter
+    def firebase_app_check_custom_endpoint(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "firebase_app_check_custom_endpoint", value)
+
+    @property
     @pulumi.getter(name="firebaseCustomEndpoint")
     def firebase_custom_endpoint(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "firebase_custom_endpoint")
 
     @firebase_custom_endpoint.setter
     def firebase_custom_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "firebase_custom_endpoint", value)
@@ -1855,14 +1882,23 @@
         return pulumi.get(self, "tags_location_custom_endpoint")
 
     @tags_location_custom_endpoint.setter
     def tags_location_custom_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tags_location_custom_endpoint", value)
 
     @property
+    @pulumi.getter(name="terraformAttributionLabelAdditionStrategy")
+    def terraform_attribution_label_addition_strategy(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "terraform_attribution_label_addition_strategy")
+
+    @terraform_attribution_label_addition_strategy.setter
+    def terraform_attribution_label_addition_strategy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "terraform_attribution_label_addition_strategy", value)
+
+    @property
     @pulumi.getter(name="tpuCustomEndpoint")
     def tpu_custom_endpoint(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "tpu_custom_endpoint")
 
     @tpu_custom_endpoint.setter
     def tpu_custom_endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tpu_custom_endpoint", value)
@@ -1963,14 +1999,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_approval_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  access_context_manager_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  active_directory_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 add_terraform_attribution_label: Optional[pulumi.Input[bool]] = None,
                  alloydb_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  api_gateway_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  apigee_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  apikeys_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  app_engine_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  artifact_registry_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  assured_workloads_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -2037,14 +2074,15 @@
                  document_ai_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  document_ai_warehouse_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  edgecontainer_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  edgenetwork_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  essential_contacts_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  eventarc_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  filestore_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 firebase_app_check_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_database_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_extensions_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_hosting_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_storage_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebaserules_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firestore_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -2109,14 +2147,15 @@
                  spanner_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  sql_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_insights_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_transfer_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tags_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tags_location_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 terraform_attribution_label_addition_strategy: Optional[pulumi.Input[str]] = None,
                  tpu_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tpu_v2_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  universe_domain: Optional[pulumi.Input[str]] = None,
                  user_project_override: Optional[pulumi.Input[bool]] = None,
                  vertex_ai_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  vmwareengine_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  vpc_access_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -2161,14 +2200,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_approval_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  access_context_manager_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  access_token: Optional[pulumi.Input[str]] = None,
                  active_directory_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 add_terraform_attribution_label: Optional[pulumi.Input[bool]] = None,
                  alloydb_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  api_gateway_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  apigee_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  apikeys_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  app_engine_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  artifact_registry_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  assured_workloads_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -2235,14 +2275,15 @@
                  document_ai_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  document_ai_warehouse_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  edgecontainer_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  edgenetwork_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  essential_contacts_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  eventarc_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  filestore_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 firebase_app_check_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_database_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_extensions_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_hosting_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebase_storage_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firebaserules_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  firestore_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -2307,14 +2348,15 @@
                  spanner_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  sql_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_insights_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  storage_transfer_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tags_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tags_location_custom_endpoint: Optional[pulumi.Input[str]] = None,
+                 terraform_attribution_label_addition_strategy: Optional[pulumi.Input[str]] = None,
                  tpu_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  tpu_v2_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  universe_domain: Optional[pulumi.Input[str]] = None,
                  user_project_override: Optional[pulumi.Input[bool]] = None,
                  vertex_ai_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  vmwareengine_custom_endpoint: Optional[pulumi.Input[str]] = None,
                  vpc_access_custom_endpoint: Optional[pulumi.Input[str]] = None,
@@ -2331,14 +2373,15 @@
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
             __props__.__dict__["access_approval_custom_endpoint"] = access_approval_custom_endpoint
             __props__.__dict__["access_context_manager_custom_endpoint"] = access_context_manager_custom_endpoint
             __props__.__dict__["access_token"] = access_token
             __props__.__dict__["active_directory_custom_endpoint"] = active_directory_custom_endpoint
+            __props__.__dict__["add_terraform_attribution_label"] = pulumi.Output.from_input(add_terraform_attribution_label).apply(pulumi.runtime.to_json) if add_terraform_attribution_label is not None else None
             __props__.__dict__["alloydb_custom_endpoint"] = alloydb_custom_endpoint
             __props__.__dict__["api_gateway_custom_endpoint"] = api_gateway_custom_endpoint
             __props__.__dict__["apigee_custom_endpoint"] = apigee_custom_endpoint
             __props__.__dict__["apikeys_custom_endpoint"] = apikeys_custom_endpoint
             __props__.__dict__["app_engine_custom_endpoint"] = app_engine_custom_endpoint
             __props__.__dict__["artifact_registry_custom_endpoint"] = artifact_registry_custom_endpoint
             __props__.__dict__["assured_workloads_custom_endpoint"] = assured_workloads_custom_endpoint
@@ -2405,14 +2448,15 @@
             __props__.__dict__["document_ai_custom_endpoint"] = document_ai_custom_endpoint
             __props__.__dict__["document_ai_warehouse_custom_endpoint"] = document_ai_warehouse_custom_endpoint
             __props__.__dict__["edgecontainer_custom_endpoint"] = edgecontainer_custom_endpoint
             __props__.__dict__["edgenetwork_custom_endpoint"] = edgenetwork_custom_endpoint
             __props__.__dict__["essential_contacts_custom_endpoint"] = essential_contacts_custom_endpoint
             __props__.__dict__["eventarc_custom_endpoint"] = eventarc_custom_endpoint
             __props__.__dict__["filestore_custom_endpoint"] = filestore_custom_endpoint
+            __props__.__dict__["firebase_app_check_custom_endpoint"] = firebase_app_check_custom_endpoint
             __props__.__dict__["firebase_custom_endpoint"] = firebase_custom_endpoint
             __props__.__dict__["firebase_database_custom_endpoint"] = firebase_database_custom_endpoint
             __props__.__dict__["firebase_extensions_custom_endpoint"] = firebase_extensions_custom_endpoint
             __props__.__dict__["firebase_hosting_custom_endpoint"] = firebase_hosting_custom_endpoint
             __props__.__dict__["firebase_storage_custom_endpoint"] = firebase_storage_custom_endpoint
             __props__.__dict__["firebaserules_custom_endpoint"] = firebaserules_custom_endpoint
             __props__.__dict__["firestore_custom_endpoint"] = firestore_custom_endpoint
@@ -2481,14 +2525,15 @@
             __props__.__dict__["spanner_custom_endpoint"] = spanner_custom_endpoint
             __props__.__dict__["sql_custom_endpoint"] = sql_custom_endpoint
             __props__.__dict__["storage_custom_endpoint"] = storage_custom_endpoint
             __props__.__dict__["storage_insights_custom_endpoint"] = storage_insights_custom_endpoint
             __props__.__dict__["storage_transfer_custom_endpoint"] = storage_transfer_custom_endpoint
             __props__.__dict__["tags_custom_endpoint"] = tags_custom_endpoint
             __props__.__dict__["tags_location_custom_endpoint"] = tags_location_custom_endpoint
+            __props__.__dict__["terraform_attribution_label_addition_strategy"] = terraform_attribution_label_addition_strategy
             __props__.__dict__["tpu_custom_endpoint"] = tpu_custom_endpoint
             __props__.__dict__["tpu_v2_custom_endpoint"] = tpu_v2_custom_endpoint
             __props__.__dict__["universe_domain"] = universe_domain
             __props__.__dict__["user_project_override"] = pulumi.Output.from_input(user_project_override).apply(pulumi.runtime.to_json) if user_project_override is not None else None
             __props__.__dict__["vertex_ai_custom_endpoint"] = vertex_ai_custom_endpoint
             __props__.__dict__["vmwareengine_custom_endpoint"] = vmwareengine_custom_endpoint
             __props__.__dict__["vpc_access_custom_endpoint"] = vpc_access_custom_endpoint
@@ -2876,14 +2921,19 @@
 
     @property
     @pulumi.getter(name="filestoreCustomEndpoint")
     def filestore_custom_endpoint(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "filestore_custom_endpoint")
 
     @property
+    @pulumi.getter(name="firebaseAppCheckCustomEndpoint")
+    def firebase_app_check_custom_endpoint(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "firebase_app_check_custom_endpoint")
+
+    @property
     @pulumi.getter(name="firebaseCustomEndpoint")
     def firebase_custom_endpoint(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "firebase_custom_endpoint")
 
     @property
     @pulumi.getter(name="firebaseDatabaseCustomEndpoint")
     def firebase_database_custom_endpoint(self) -> pulumi.Output[Optional[str]]:
@@ -3226,14 +3276,19 @@
 
     @property
     @pulumi.getter(name="tagsLocationCustomEndpoint")
     def tags_location_custom_endpoint(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "tags_location_custom_endpoint")
 
     @property
+    @pulumi.getter(name="terraformAttributionLabelAdditionStrategy")
+    def terraform_attribution_label_addition_strategy(self) -> pulumi.Output[Optional[str]]:
+        return pulumi.get(self, "terraform_attribution_label_addition_strategy")
+
+    @property
     @pulumi.getter(name="tpuCustomEndpoint")
     def tpu_custom_endpoint(self) -> pulumi.Output[Optional[str]]:
         return pulumi.get(self, "tpu_custom_endpoint")
 
     @property
     @pulumi.getter(name="tpuV2CustomEndpoint")
     def tpu_v2_custom_endpoint(self) -> pulumi.Output[Optional[str]]:
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_schema_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_schema_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_subscription.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_subscription_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_subscription_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_topic.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/get_topic_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/get_topic_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/lite_reservation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/lite_reservation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/lite_subscription.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/lite_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/lite_topic.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/lite_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/schema_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/schema_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/subscription_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/subscription_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/pubsub/topic_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/pubsub/topic_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/enterprise_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/enterprise_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/recaptcha/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/recaptcha/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/get_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/redis/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/redis/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/resourcemanager/lien.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/resourcemanager/lien.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/config_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/config_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/get_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/get_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/get_config_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/get_config_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/get_variable.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/get_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/runtimeconfig/variable.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/runtimeconfig/variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secret_version_access.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secret_version_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/get_secrets.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/get_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/secretmanager/secret_version.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/secretmanager/secret_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/get_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/get_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securesourcemanager/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securesourcemanager/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/event_threat_detection_custom_module.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/event_threat_detection_custom_module.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/folder_custom_module.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/folder_custom_module.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/get_source_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/get_source_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/mute_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/mute_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/notification_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/notification_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/organization_custom_module.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/organization_custom_module.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/project_custom_module.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/project_custom_module.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securitycenter/source_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securitycenter/source_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/posture.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/posture.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/securityposture/posture_deployment.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/securityposture/posture_deployment.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,20 +26,20 @@
         :param pulumi.Input[str] location: The location of the resource, eg. global`.
         :param pulumi.Input[str] parent: The parent of the resource, an organization. Format should be `organizations/{organization_id}`.
         :param pulumi.Input[str] posture_deployment_id: ID of the posture deployment.
                
                
                - - -
         :param pulumi.Input[str] posture_id: Relative name of the posture which needs to be deployed. It should be in the format:
-               organizations/<ORG_ID>/locations/<LOCATION>/postures/<postureID>
+               organizations/{organization_id}/locations/{location}/postures/{posture_id}
         :param pulumi.Input[str] posture_revision_id: Revision_id the posture which needs to be deployed.
         :param pulumi.Input[str] target_resource: The resource on which the posture should be deployed. This can be in one of the following formats:
-               projects/<project_number>
-               folders/<folder_number>
-               organizations/<organization_id>
+               projects/{project_number},
+               folders/{folder_number},
+               organizations/{organization_id}
         :param pulumi.Input[str] description: Description of the posture deployment.
         """
         pulumi.set(__self__, "location", location)
         pulumi.set(__self__, "parent", parent)
         pulumi.set(__self__, "posture_deployment_id", posture_deployment_id)
         pulumi.set(__self__, "posture_id", posture_id)
         pulumi.set(__self__, "posture_revision_id", posture_revision_id)
@@ -87,15 +87,15 @@
         pulumi.set(self, "posture_deployment_id", value)
 
     @property
     @pulumi.getter(name="postureId")
     def posture_id(self) -> pulumi.Input[str]:
         """
         Relative name of the posture which needs to be deployed. It should be in the format:
-        organizations/<ORG_ID>/locations/<LOCATION>/postures/<postureID>
+        organizations/{organization_id}/locations/{location}/postures/{posture_id}
         """
         return pulumi.get(self, "posture_id")
 
     @posture_id.setter
     def posture_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "posture_id", value)
 
@@ -112,17 +112,17 @@
         pulumi.set(self, "posture_revision_id", value)
 
     @property
     @pulumi.getter(name="targetResource")
     def target_resource(self) -> pulumi.Input[str]:
         """
         The resource on which the posture should be deployed. This can be in one of the following formats:
-        projects/<project_number>
-        folders/<folder_number>
-        organizations/<organization_id>
+        projects/{project_number},
+        folders/{folder_number},
+        organizations/{organization_id}
         """
         return pulumi.get(self, "target_resource")
 
     @target_resource.setter
     def target_resource(self, value: pulumi.Input[str]):
         pulumi.set(self, "target_resource", value)
 
@@ -160,39 +160,40 @@
                  update_time: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PostureDeployment resources.
         :param pulumi.Input[str] create_time: Time the posture deployment was created in UTC.
         :param pulumi.Input[str] description: Description of the posture deployment.
         :param pulumi.Input[str] desired_posture_id: This is an output only optional field which will be filled in case when
                PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-               It denotes the desired Posture to be deployed.
+               It denotes the desired posture to be deployed.
         :param pulumi.Input[str] desired_posture_revision_id: This is an output only optional field which will be filled in case when
                PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-               It denotes the desired Posture revision_id to be deployed.
+               It denotes the desired posture revision_id to be deployed.
         :param pulumi.Input[str] etag: For Resource freshness validation (https://google.aip.dev/154)
         :param pulumi.Input[str] failure_message: This is a output only optional field which will be filled in case where
                PostureDeployment enters a failure state like UPDATE_FAILED or
                CREATE_FAILED or DELETE_FAILED. It will have the failure message for posture deployment's
                CREATE/UPDATE/DELETE methods.
         :param pulumi.Input[str] location: The location of the resource, eg. global`.
         :param pulumi.Input[str] name: Name of the posture deployment instance.
         :param pulumi.Input[str] parent: The parent of the resource, an organization. Format should be `organizations/{organization_id}`.
         :param pulumi.Input[str] posture_deployment_id: ID of the posture deployment.
                
                
                - - -
         :param pulumi.Input[str] posture_id: Relative name of the posture which needs to be deployed. It should be in the format:
-               organizations/<ORG_ID>/locations/<LOCATION>/postures/<postureID>
+               organizations/{organization_id}/locations/{location}/postures/{posture_id}
         :param pulumi.Input[str] posture_revision_id: Revision_id the posture which needs to be deployed.
         :param pulumi.Input[bool] reconciling: If set, there are currently changes in flight to the posture deployment.
-        :param pulumi.Input[str] state: State of the posture deployment.
+        :param pulumi.Input[str] state: State of the posture deployment. A posture deployment can be in the following terminal states:
+               ACTIVE, CREATE_FAILED, UPDATE_FAILED, DELETE_FAILED.
         :param pulumi.Input[str] target_resource: The resource on which the posture should be deployed. This can be in one of the following formats:
-               projects/<project_number>
-               folders/<folder_number>
-               organizations/<organization_id>
+               projects/{project_number},
+               folders/{folder_number},
+               organizations/{organization_id}
         :param pulumi.Input[str] update_time: Time the posture deployment was updated in UTC.
         """
         if create_time is not None:
             pulumi.set(__self__, "create_time", create_time)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if desired_posture_id is not None:
@@ -250,29 +251,29 @@
 
     @property
     @pulumi.getter(name="desiredPostureId")
     def desired_posture_id(self) -> Optional[pulumi.Input[str]]:
         """
         This is an output only optional field which will be filled in case when
         PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-        It denotes the desired Posture to be deployed.
+        It denotes the desired posture to be deployed.
         """
         return pulumi.get(self, "desired_posture_id")
 
     @desired_posture_id.setter
     def desired_posture_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desired_posture_id", value)
 
     @property
     @pulumi.getter(name="desiredPostureRevisionId")
     def desired_posture_revision_id(self) -> Optional[pulumi.Input[str]]:
         """
         This is an output only optional field which will be filled in case when
         PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-        It denotes the desired Posture revision_id to be deployed.
+        It denotes the desired posture revision_id to be deployed.
         """
         return pulumi.get(self, "desired_posture_revision_id")
 
     @desired_posture_revision_id.setter
     def desired_posture_revision_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desired_posture_revision_id", value)
 
@@ -355,15 +356,15 @@
         pulumi.set(self, "posture_deployment_id", value)
 
     @property
     @pulumi.getter(name="postureId")
     def posture_id(self) -> Optional[pulumi.Input[str]]:
         """
         Relative name of the posture which needs to be deployed. It should be in the format:
-        organizations/<ORG_ID>/locations/<LOCATION>/postures/<postureID>
+        organizations/{organization_id}/locations/{location}/postures/{posture_id}
         """
         return pulumi.get(self, "posture_id")
 
     @posture_id.setter
     def posture_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "posture_id", value)
 
@@ -391,30 +392,31 @@
     def reconciling(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "reconciling", value)
 
     @property
     @pulumi.getter
     def state(self) -> Optional[pulumi.Input[str]]:
         """
-        State of the posture deployment.
+        State of the posture deployment. A posture deployment can be in the following terminal states:
+        ACTIVE, CREATE_FAILED, UPDATE_FAILED, DELETE_FAILED.
         """
         return pulumi.get(self, "state")
 
     @state.setter
     def state(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "state", value)
 
     @property
     @pulumi.getter(name="targetResource")
     def target_resource(self) -> Optional[pulumi.Input[str]]:
         """
         The resource on which the posture should be deployed. This can be in one of the following formats:
-        projects/<project_number>
-        folders/<folder_number>
-        organizations/<organization_id>
+        projects/{project_number},
+        folders/{folder_number},
+        organizations/{organization_id}
         """
         return pulumi.get(self, "target_resource")
 
     @target_resource.setter
     def target_resource(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "target_resource", value)
 
@@ -512,20 +514,20 @@
         :param pulumi.Input[str] location: The location of the resource, eg. global`.
         :param pulumi.Input[str] parent: The parent of the resource, an organization. Format should be `organizations/{organization_id}`.
         :param pulumi.Input[str] posture_deployment_id: ID of the posture deployment.
                
                
                - - -
         :param pulumi.Input[str] posture_id: Relative name of the posture which needs to be deployed. It should be in the format:
-               organizations/<ORG_ID>/locations/<LOCATION>/postures/<postureID>
+               organizations/{organization_id}/locations/{location}/postures/{posture_id}
         :param pulumi.Input[str] posture_revision_id: Revision_id the posture which needs to be deployed.
         :param pulumi.Input[str] target_resource: The resource on which the posture should be deployed. This can be in one of the following formats:
-               projects/<project_number>
-               folders/<folder_number>
-               organizations/<organization_id>
+               projects/{project_number},
+               folders/{folder_number},
+               organizations/{organization_id}
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: PostureDeploymentArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -683,39 +685,40 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] create_time: Time the posture deployment was created in UTC.
         :param pulumi.Input[str] description: Description of the posture deployment.
         :param pulumi.Input[str] desired_posture_id: This is an output only optional field which will be filled in case when
                PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-               It denotes the desired Posture to be deployed.
+               It denotes the desired posture to be deployed.
         :param pulumi.Input[str] desired_posture_revision_id: This is an output only optional field which will be filled in case when
                PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-               It denotes the desired Posture revision_id to be deployed.
+               It denotes the desired posture revision_id to be deployed.
         :param pulumi.Input[str] etag: For Resource freshness validation (https://google.aip.dev/154)
         :param pulumi.Input[str] failure_message: This is a output only optional field which will be filled in case where
                PostureDeployment enters a failure state like UPDATE_FAILED or
                CREATE_FAILED or DELETE_FAILED. It will have the failure message for posture deployment's
                CREATE/UPDATE/DELETE methods.
         :param pulumi.Input[str] location: The location of the resource, eg. global`.
         :param pulumi.Input[str] name: Name of the posture deployment instance.
         :param pulumi.Input[str] parent: The parent of the resource, an organization. Format should be `organizations/{organization_id}`.
         :param pulumi.Input[str] posture_deployment_id: ID of the posture deployment.
                
                
                - - -
         :param pulumi.Input[str] posture_id: Relative name of the posture which needs to be deployed. It should be in the format:
-               organizations/<ORG_ID>/locations/<LOCATION>/postures/<postureID>
+               organizations/{organization_id}/locations/{location}/postures/{posture_id}
         :param pulumi.Input[str] posture_revision_id: Revision_id the posture which needs to be deployed.
         :param pulumi.Input[bool] reconciling: If set, there are currently changes in flight to the posture deployment.
-        :param pulumi.Input[str] state: State of the posture deployment.
+        :param pulumi.Input[str] state: State of the posture deployment. A posture deployment can be in the following terminal states:
+               ACTIVE, CREATE_FAILED, UPDATE_FAILED, DELETE_FAILED.
         :param pulumi.Input[str] target_resource: The resource on which the posture should be deployed. This can be in one of the following formats:
-               projects/<project_number>
-               folders/<folder_number>
-               organizations/<organization_id>
+               projects/{project_number},
+               folders/{folder_number},
+               organizations/{organization_id}
         :param pulumi.Input[str] update_time: Time the posture deployment was updated in UTC.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PostureDeploymentState.__new__(_PostureDeploymentState)
 
         __props__.__dict__["create_time"] = create_time
@@ -754,25 +757,25 @@
 
     @property
     @pulumi.getter(name="desiredPostureId")
     def desired_posture_id(self) -> pulumi.Output[str]:
         """
         This is an output only optional field which will be filled in case when
         PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-        It denotes the desired Posture to be deployed.
+        It denotes the desired posture to be deployed.
         """
         return pulumi.get(self, "desired_posture_id")
 
     @property
     @pulumi.getter(name="desiredPostureRevisionId")
     def desired_posture_revision_id(self) -> pulumi.Output[str]:
         """
         This is an output only optional field which will be filled in case when
         PostureDeployment state is UPDATE_FAILED or CREATE_FAILED or DELETE_FAILED.
-        It denotes the desired Posture revision_id to be deployed.
+        It denotes the desired posture revision_id to be deployed.
         """
         return pulumi.get(self, "desired_posture_revision_id")
 
     @property
     @pulumi.getter
     def etag(self) -> pulumi.Output[str]:
         """
@@ -827,15 +830,15 @@
         return pulumi.get(self, "posture_deployment_id")
 
     @property
     @pulumi.getter(name="postureId")
     def posture_id(self) -> pulumi.Output[str]:
         """
         Relative name of the posture which needs to be deployed. It should be in the format:
-        organizations/<ORG_ID>/locations/<LOCATION>/postures/<postureID>
+        organizations/{organization_id}/locations/{location}/postures/{posture_id}
         """
         return pulumi.get(self, "posture_id")
 
     @property
     @pulumi.getter(name="postureRevisionId")
     def posture_revision_id(self) -> pulumi.Output[str]:
         """
@@ -851,26 +854,27 @@
         """
         return pulumi.get(self, "reconciling")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[str]:
         """
-        State of the posture deployment.
+        State of the posture deployment. A posture deployment can be in the following terminal states:
+        ACTIVE, CREATE_FAILED, UPDATE_FAILED, DELETE_FAILED.
         """
         return pulumi.get(self, "state")
 
     @property
     @pulumi.getter(name="targetResource")
     def target_resource(self) -> pulumi.Output[str]:
         """
         The resource on which the posture should be deployed. This can be in one of the following formats:
-        projects/<project_number>
-        folders/<folder_number>
-        organizations/<organization_id>
+        projects/{project_number},
+        folders/{folder_number},
+        organizations/{organization_id}
         """
         return pulumi.get(self, "target_resource")
 
     @property
     @pulumi.getter(name="updateTime")
     def update_time(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_access_token.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_id_token.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_id_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_jwt.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_jwt.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_account_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_account_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/get_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/get_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceaccount/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceaccount/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/endpoint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/get_namespace_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/get_namespace_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/get_service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/get_service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/namespace_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/namespace_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicedirectory/service_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicedirectory/service_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/connection.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/get_peered_dns_domain.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/get_peered_dns_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/servicenetworking/peered_dns_domain.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/servicenetworking/peered_dns_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/serviceusage/consumer_quota_override.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/serviceusage/consumer_quota_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/get_repository.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/get_repository_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/get_repository_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sourcerepo/repository_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sourcerepo/repository_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/database_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/database_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/get_database_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/get_database_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/get_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/get_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/get_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/spanner/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/spanner/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/database.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/database_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/database_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_backup_run.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_backup_run.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_ca_certs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_ca_certs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database_instance_latest_recovery_time.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database_instance_latest_recovery_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_database_instances.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_database_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_databases.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/get_tiers.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/get_tiers.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/source_representation_instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/source_representation_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/ssl_cert.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/ssl_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/sql/user.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/sql/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_access_control.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_access_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_acl.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/bucket_object.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/bucket_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/default_object_access_control.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/default_object_access_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/default_object_acl.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/default_object_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket_object.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_bucket_object_content.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_bucket_object_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_object_signed_url.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_object_signed_url.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_project_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_project_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_transfer_project_service_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_transfer_project_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/get_transfer_project_servie_account.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/get_transfer_project_servie_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/hmac_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/hmac_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/insights_report_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/insights_report_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/notification.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/object_access_control.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/object_access_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/object_acl.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/object_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/transfer_agent_pool.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/transfer_agent_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/storage/transfer_job.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/storage/transfer_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_key_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_key_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_value.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/get_tag_value_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/get_tag_value_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/location_tag_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/location_tag_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_key_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_key_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tags/tag_value_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tags/tag_value_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/get_tensorflow_versions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/get_tensorflow_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/get_v2_accelerator_types.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/get_v2_accelerator_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/get_v2_runtime_versions.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/get_v2_runtime_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/node.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/node.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/tpu/v2_vm.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/tpu/v2_vm.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_dataset.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_endpoint_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_endpoint_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_group.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_group_feature.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_group_feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_online_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_online_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_online_store_featureview.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_online_store_featureview.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_feature.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_feature.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_entity_type_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_feature_store_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_feature_store_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_index.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_index.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_index_endpoint.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_index_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_metadata_store.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_metadata_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/ai_tensorboard.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/ai_tensorboard.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_endpoint_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_endpoint_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_featurestore_entitytype_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_featurestore_entitytype_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_featurestore_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_featurestore_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/get_ai_index.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/get_ai_index.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vertex/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vertex/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/external_access_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/external_access_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/external_address.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/external_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_external_access_rule.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_external_access_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_external_address.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_external_address.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_network.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_network_peering.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_network_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_network_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_network_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_nsx_credentials.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_nsx_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_private_cloud.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_private_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_subnet.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/get_vcenter_credentials.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/get_vcenter_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/network.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/network_peering.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/network_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/network_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/network_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/private_cloud.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/private_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vmwareengine/subnet.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vmwareengine/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/connector.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/get_connector.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/get_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/vpcaccess/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/vpcaccess/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/get_instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/get_instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,16 +577,14 @@
         import pulumi_gcp as gcp
 
         my_network = gcp.compute.Network("myNetwork", auto_create_subnetworks=False)
         my_subnetwork = gcp.compute.Subnetwork("mySubnetwork",
             network=my_network.id,
             region="us-central1",
             ip_cidr_range="10.0.1.0/24")
-        keyring = gcp.kms.KeyRing("keyring", location="global")
-        crypto_key = gcp.kms.CryptoKey("crypto-key", key_ring=keyring.id)
         instance = gcp.workbench.Instance("instance",
             location="us-central1-a",
             gce_setup=gcp.workbench.InstanceGceSetupArgs(
                 machine_type="n1-standard-4",
                 accelerator_configs=[gcp.workbench.InstanceGceSetupAcceleratorConfigArgs(
                     type="NVIDIA_TESLA_T4",
                     core_count="1",
@@ -595,21 +593,21 @@
                 service_accounts=[gcp.workbench.InstanceGceSetupServiceAccountArgs(
                     email="my@service-account.com",
                 )],
                 boot_disk=gcp.workbench.InstanceGceSetupBootDiskArgs(
                     disk_size_gb="310",
                     disk_type="PD_SSD",
                     disk_encryption="GMEK",
-                    kms_key=crypto_key.id,
+                    kms_key="my-crypto-key",
                 ),
                 data_disks=gcp.workbench.InstanceGceSetupDataDisksArgs(
                     disk_size_gb="330",
                     disk_type="PD_SSD",
                     disk_encryption="GMEK",
-                    kms_key=crypto_key.id,
+                    kms_key="my-crypto-key",
                 ),
                 network_interfaces=[gcp.workbench.InstanceGceSetupNetworkInterfaceArgs(
                     network=my_network.id,
                     subnet=my_subnetwork.id,
                     nic_type="GVNIC",
                 )],
                 metadata={
@@ -741,16 +739,14 @@
         import pulumi_gcp as gcp
 
         my_network = gcp.compute.Network("myNetwork", auto_create_subnetworks=False)
         my_subnetwork = gcp.compute.Subnetwork("mySubnetwork",
             network=my_network.id,
             region="us-central1",
             ip_cidr_range="10.0.1.0/24")
-        keyring = gcp.kms.KeyRing("keyring", location="global")
-        crypto_key = gcp.kms.CryptoKey("crypto-key", key_ring=keyring.id)
         instance = gcp.workbench.Instance("instance",
             location="us-central1-a",
             gce_setup=gcp.workbench.InstanceGceSetupArgs(
                 machine_type="n1-standard-4",
                 accelerator_configs=[gcp.workbench.InstanceGceSetupAcceleratorConfigArgs(
                     type="NVIDIA_TESLA_T4",
                     core_count="1",
@@ -759,21 +755,21 @@
                 service_accounts=[gcp.workbench.InstanceGceSetupServiceAccountArgs(
                     email="my@service-account.com",
                 )],
                 boot_disk=gcp.workbench.InstanceGceSetupBootDiskArgs(
                     disk_size_gb="310",
                     disk_type="PD_SSD",
                     disk_encryption="GMEK",
-                    kms_key=crypto_key.id,
+                    kms_key="my-crypto-key",
                 ),
                 data_disks=gcp.workbench.InstanceGceSetupDataDisksArgs(
                     disk_size_gb="330",
                     disk_type="PD_SSD",
                     disk_encryption="GMEK",
-                    kms_key=crypto_key.id,
+                    kms_key="my-crypto-key",
                 ),
                 network_interfaces=[gcp.workbench.InstanceGceSetupNetworkInterfaceArgs(
                     network=my_network.id,
                     subnet=my_subnetwork.id,
                     nic_type="GVNIC",
                 )],
                 metadata={
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/instance_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/instance_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workbench/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workbench/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workflows/workflow.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/__init__.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/_inputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/get_workstation_config_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/get_workstation_config_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/get_workstation_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/get_workstation_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/outputs.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_cluster.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_config_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_config_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_iam_binding.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_iam_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_iam_member.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_iam_member.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp/workstations/workstation_iam_policy.py` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp/workstations/workstation_iam_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/PKG-INFO` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gcp
-Version: 7.9.0a1707891532
+Version: 7.9.0a1707934510
 Summary: A Pulumi package for creating and managing Google Cloud Platform resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-gcp
 Keywords: pulumi,gcp
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_gcp Version: 7.9.0a1707891532 Summary: A
+Metadata-Version: 2.1 Name: pulumi_gcp Version: 7.9.0a1707934510 Summary: A
 Pulumi package for creating and managing Google Cloud Platform resources.
 License: Apache-2.0 Project-URL: Homepage, https://pulumi.io Project-URL:
 Repository, https://github.com/pulumi/pulumi-gcp Keywords: pulumi,gcp Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Requires-Dist:
 parver>=0.2.1 Requires-Dist: pulumi<4.0.0,>=3.0.0 Requires-Dist: semver>=2.8.1
 [![Actions Status](https://github.com/pulumi/pulumi-gcp/workflows/master/
 badge.svg)](https://github.com/pulumi/pulumi-gcp/actions) [![Slack](http://
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pulumi_gcp.egg-info/SOURCES.txt` & `pulumi_gcp-7.9.0a1707934510/pulumi_gcp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -274,14 +274,18 @@
 pulumi_gcp/cloudbuildv2/get_connection_iam_policy.py
 pulumi_gcp/cloudbuildv2/outputs.py
 pulumi_gcp/cloudbuildv2/repository.py
 pulumi_gcp/clouddeploy/__init__.py
 pulumi_gcp/clouddeploy/_inputs.py
 pulumi_gcp/clouddeploy/automation.py
 pulumi_gcp/clouddeploy/delivery_pipeline.py
+pulumi_gcp/clouddeploy/delivery_pipeline_iam_binding.py
+pulumi_gcp/clouddeploy/delivery_pipeline_iam_member.py
+pulumi_gcp/clouddeploy/delivery_pipeline_iam_policy.py
+pulumi_gcp/clouddeploy/get_delivery_pipeline_iam_policy.py
 pulumi_gcp/clouddeploy/outputs.py
 pulumi_gcp/clouddeploy/target.py
 pulumi_gcp/clouddomains/__init__.py
 pulumi_gcp/clouddomains/_inputs.py
 pulumi_gcp/clouddomains/outputs.py
 pulumi_gcp/clouddomains/registration.py
 pulumi_gcp/cloudfunctions/__init__.py
@@ -449,14 +453,15 @@
 pulumi_gcp/compute/image_iam_member.py
 pulumi_gcp/compute/image_iam_policy.py
 pulumi_gcp/compute/instance.py
 pulumi_gcp/compute/instance_from_machine_image.py
 pulumi_gcp/compute/instance_from_template.py
 pulumi_gcp/compute/instance_group.py
 pulumi_gcp/compute/instance_group_manager.py
+pulumi_gcp/compute/instance_group_membership.py
 pulumi_gcp/compute/instance_group_named_port.py
 pulumi_gcp/compute/instance_iam_binding.py
 pulumi_gcp/compute/instance_iam_member.py
 pulumi_gcp/compute/instance_iam_policy.py
 pulumi_gcp/compute/instance_settings.py
 pulumi_gcp/compute/instance_template.py
 pulumi_gcp/compute/interconnect_attachment.py
@@ -794,14 +799,15 @@
 pulumi_gcp/filestore/get_instance.py
 pulumi_gcp/filestore/instance.py
 pulumi_gcp/filestore/outputs.py
 pulumi_gcp/filestore/snapshot.py
 pulumi_gcp/firebase/__init__.py
 pulumi_gcp/firebase/_inputs.py
 pulumi_gcp/firebase/android_app.py
+pulumi_gcp/firebase/app_check_service_config.py
 pulumi_gcp/firebase/apple_app.py
 pulumi_gcp/firebase/database_instance.py
 pulumi_gcp/firebase/extensions_instance.py
 pulumi_gcp/firebase/get_android_app.py
 pulumi_gcp/firebase/get_android_app_config.py
 pulumi_gcp/firebase/get_apple_app.py
 pulumi_gcp/firebase/get_apple_app_config.py
```

### Comparing `pulumi_gcp-7.9.0a1707891532/pyproject.toml` & `pulumi_gcp-7.9.0a1707934510/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_gcp"
   description = "A Pulumi package for creating and managing Google Cloud Platform resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "gcp"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "7.9.0a1707891532"
+  version = "7.9.0a1707934510"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-gcp"
 
 [build-system]
```

