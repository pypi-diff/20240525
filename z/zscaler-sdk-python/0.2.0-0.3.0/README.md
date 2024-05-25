# Comparing `tmp/zscaler_sdk_python-0.2.0.tar.gz` & `tmp/zscaler_sdk_python-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler_sdk_python-0.2.0.tar", max compression
+gzip compressed data, was "zscaler_sdk_python-0.3.0.tar", max compression
```

## Comparing `zscaler_sdk_python-0.2.0.tar` & `zscaler_sdk_python-0.3.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     1113 2024-05-14 20:28:06.217430 zscaler_sdk_python-0.2.0/LICENSE.md
--rw-r--r--   0        0        0    15746 2024-05-14 20:28:06.217430 zscaler_sdk_python-0.2.0/README.md
--rw-r--r--   0        0        0     2314 2024-05-14 20:28:50.857702 zscaler_sdk_python-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1277 2024-05-14 20:28:50.861702 zscaler_sdk_python-0.2.0/zscaler/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/__init__.py
--rw-r--r--   0        0        0     3195 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/cache.py
--rw-r--r--   0        0        0     1479 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/no_op_cache.py
--rw-r--r--   0        0        0     4967 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/cache/zscaler_cache.py
--rw-r--r--   0        0        0      738 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/constants.py
--rw-r--r--   0        0        0        0 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/__init__.py
--rw-r--r--   0        0        0      172 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/error.py
--rw-r--r--   0        0        0      638 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/http_error.py
--rw-r--r--   0        0        0      628 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/errors/zscaler_api_error.py
--rw-r--r--   0        0        0       63 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/exceptions/__init__.py
--rw-r--r--   0        0        0     2025 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/exceptions/exceptions.py
--rw-r--r--   0        0        0     2099 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/logger.py
--rw-r--r--   0        0        0        0 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/ratelimiter/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0        0        0      639 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/user_agent.py
--rw-r--r--   0        0        0    19073 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/utils.py
--rw-r--r--   0        0        0    21568 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/__init__.py
--rw-r--r--   0        0        0     1534 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/activate.py
--rw-r--r--   0        0        0    14194 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0        0        0     2372 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/apptotal.py
--rw-r--r--   0        0        0     2992 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/audit_logs.py
--rw-r--r--   0        0        0     3140 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/authentication_settings.py
--rw-r--r--   0        0        0     2754 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/client.py
--rw-r--r--   0        0        0    18513 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/cloud_apps.py
--rw-r--r--   0        0        0     2872 2024-05-14 20:28:06.237430 zscaler_sdk_python-0.2.0/zscaler/zia/device_management.py
--rw-r--r--   0        0        0    27473 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/dlp.py
--rw-r--r--   0        0        0      794 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/errors.py
--rw-r--r--   0        0        0    39908 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/firewall.py
--rw-r--r--   0        0        0    11686 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/forwarding_control.py
--rw-r--r--   0        0        0     2909 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/isolation_profile.py
--rw-r--r--   0        0        0     5835 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/labels.py
--rw-r--r--   0        0        0    30762 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/locations.py
--rw-r--r--   0        0        0     6724 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/sandbox.py
--rw-r--r--   0        0        0     6792 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/security.py
--rw-r--r--   0        0        0     5298 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/ssl_inspection.py
--rw-r--r--   0        0        0    30729 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/traffic.py
--rw-r--r--   0        0        0    14484 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/url_categories.py
--rw-r--r--   0        0        0    14319 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/url_filtering.py
--rw-r--r--   0        0        0    13735 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/users.py
--rw-r--r--   0        0        0    12376 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/web_dlp.py
--rw-r--r--   0        0        0     1897 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/workload_groups.py
--rw-r--r--   0        0        0     6842 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zia/zpa_gateway.py
--rw-r--r--   0        0        0     2709 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/README.md
--rw-r--r--   0        0        0    24498 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/__init__.py
--rw-r--r--   0        0        0    13187 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments.py
--rw-r--r--   0        0        0    12445 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0        0        0    12019 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0        0        0     8054 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/certificates.py
--rw-r--r--   0        0        0     3844 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/client.py
--rw-r--r--   0        0        0     2667 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0        0        0    20849 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/connectors.py
--rw-r--r--   0        0        0     6189 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/emergency_access.py
--rw-r--r--   0        0        0      844 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/errors.py
--rw-r--r--   0        0        0     2764 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/idp.py
--rw-r--r--   0        0        0    33962 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/inspection.py
--rw-r--r--   0        0        0    27713 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/isolation.py
--rw-r--r--   0        0        0    21546 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/lss.py
--rw-r--r--   0        0        0     2734 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/machine_groups.py
--rw-r--r--   0        0        0    31713 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/policies.py
--rw-r--r--   0        0        0     5640 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/posture_profiles.py
--rw-r--r--   0        0        0    31880 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0        0        0     9887 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/provisioning.py
--rw-r--r--   0        0        0     3632 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/saml_attributes.py
--rw-r--r--   0        0        0     4172 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/scim_attributes.py
--rw-r--r--   0        0        0     3691 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/scim_groups.py
--rw-r--r--   0        0        0     6103 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/segment_groups.py
--rw-r--r--   0        0        0     7775 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/server_groups.py
--rw-r--r--   0        0        0     6477 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/servers.py
--rw-r--r--   0        0        0    15428 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/service_edges.py
--rw-r--r--   0        0        0     3684 2024-05-14 20:28:06.241430 zscaler_sdk_python-0.2.0/zscaler/zpa/trusted_networks.py
--rw-r--r--   0        0        0    17559 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1113 2024-05-25 00:09:19.060317 zscaler_sdk_python-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0    15746 2024-05-25 00:09:19.060317 zscaler_sdk_python-0.3.0/README.md
+-rw-r--r--   0        0        0     2325 2024-05-25 00:09:57.476060 zscaler_sdk_python-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1277 2024-05-25 00:09:57.480060 zscaler_sdk_python-0.3.0/zscaler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/__init__.py
+-rw-r--r--   0        0        0     3195 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/cache.py
+-rw-r--r--   0        0        0     1479 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/no_op_cache.py
+-rw-r--r--   0        0        0     4967 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0        0        0      853 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/constants.py
+-rw-r--r--   0        0        0        0 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/__init__.py
+-rw-r--r--   0        0        0      172 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/error.py
+-rw-r--r--   0        0        0      638 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/http_error.py
+-rw-r--r--   0        0        0      628 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/errors/zscaler_api_error.py
+-rw-r--r--   0        0        0       63 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/exceptions/__init__.py
+-rw-r--r--   0        0        0     2025 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2099 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/logger.py
+-rw-r--r--   0        0        0        0 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0        0        0      639 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/user_agent.py
+-rw-r--r--   0        0        0    19073 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/utils.py
+-rw-r--r--   0        0        0    21568 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/__init__.py
+-rw-r--r--   0        0        0     1534 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/activate.py
+-rw-r--r--   0        0        0    14194 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0        0        0     2372 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/apptotal.py
+-rw-r--r--   0        0        0     2992 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/audit_logs.py
+-rw-r--r--   0        0        0     3140 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/authentication_settings.py
+-rw-r--r--   0        0        0     2754 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/client.py
+-rw-r--r--   0        0        0    18513 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/cloud_apps.py
+-rw-r--r--   0        0        0     2872 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/device_management.py
+-rw-r--r--   0        0        0    27473 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/dlp.py
+-rw-r--r--   0        0        0      794 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/errors.py
+-rw-r--r--   0        0        0    39908 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/firewall.py
+-rw-r--r--   0        0        0    11686 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/forwarding_control.py
+-rw-r--r--   0        0        0     2909 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/isolation_profile.py
+-rw-r--r--   0        0        0     5835 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/labels.py
+-rw-r--r--   0        0        0    30762 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/locations.py
+-rw-r--r--   0        0        0     6724 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/sandbox.py
+-rw-r--r--   0        0        0     6792 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/security.py
+-rw-r--r--   0        0        0     5298 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0        0        0    30729 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/traffic.py
+-rw-r--r--   0        0        0    14484 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/url_categories.py
+-rw-r--r--   0        0        0    14319 2024-05-25 00:09:19.084317 zscaler_sdk_python-0.3.0/zscaler/zia/url_filtering.py
+-rw-r--r--   0        0        0    13735 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/users.py
+-rw-r--r--   0        0        0    12376 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/web_dlp.py
+-rw-r--r--   0        0        0     1897 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/workload_groups.py
+-rw-r--r--   0        0        0     6842 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zia/zpa_gateway.py
+-rw-r--r--   0        0        0     2709 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/README.md
+-rw-r--r--   0        0        0    24891 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/__init__.py
+-rw-r--r--   0        0        0    15006 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments.py
+-rw-r--r--   0        0        0    12445 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0        0        0    12019 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0        0        0     8054 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/certificates.py
+-rw-r--r--   0        0        0     3844 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/client.py
+-rw-r--r--   0        0        0     2667 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0        0        0    20849 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/connectors.py
+-rw-r--r--   0        0        0     6189 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/emergency_access.py
+-rw-r--r--   0        0        0      844 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/errors.py
+-rw-r--r--   0        0        0     2764 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/idp.py
+-rw-r--r--   0        0        0    33962 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/inspection.py
+-rw-r--r--   0        0        0    27713 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/isolation.py
+-rw-r--r--   0        0        0    21546 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/lss.py
+-rw-r--r--   0        0        0     2734 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/machine_groups.py
+-rw-r--r--   0        0        0    31713 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/policies.py
+-rw-r--r--   0        0        0    70610 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/policiesv2.py
+-rw-r--r--   0        0        0     5640 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0        0        0    31880 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0        0        0     9887 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/provisioning.py
+-rw-r--r--   0        0        0     3632 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0        0        0     4172 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0        0        0     3691 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/scim_groups.py
+-rw-r--r--   0        0        0     6103 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/segment_groups.py
+-rw-r--r--   0        0        0     7775 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/server_groups.py
+-rw-r--r--   0        0        0     6477 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/servers.py
+-rw-r--r--   0        0        0    15428 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/service_edges.py
+-rw-r--r--   0        0        0     3684 2024-05-25 00:09:19.088317 zscaler_sdk_python-0.3.0/zscaler/zpa/trusted_networks.py
+-rw-r--r--   0        0        0    17529 1970-01-01 00:00:00.000000 zscaler_sdk_python-0.3.0/PKG-INFO
```

### Comparing `zscaler_sdk_python-0.2.0/LICENSE.md` & `zscaler_sdk_python-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/README.md` & `zscaler_sdk_python-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/pyproject.toml` & `zscaler_sdk_python-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zscaler-sdk-python"
-version = "0.2.0"
+version = "0.3.0"
 description = "Official Python SDK for the Zscaler Products (Beta)"
 authors = ["Zscaler, Inc. <devrel@zscaler.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/zscaler/zscaler-sdk-python"
 repository = "https://github.com/zscaler/zscaler-sdk-python"
 documentation = "https://zscaler-sdk-python.readthedocs.io"
@@ -31,35 +31,34 @@
 python = ">=3.8,<4.0"
 arrow = "*"
 certifi = "*"
 charset-normalizer = "*"
 idna = "*"
 python-box = "^7.1.1"
 python-dateutil = "*"
-requests = "*"
+requests = ">=2.32.0"
 responses = "*"
 restfly = "*"
 six = "*"
-urllib3 = "*"
 flatdict = "*"
 pyyaml = "*"
 xmltodict = "*"
 yarl = "*"
 pycryptodomex = "*"
 aenum = "*"
 pydash = "*"
 flake8 = "*"
 pytz = "*"
-black = "^24.4.1"
-cryptography = "^3.4"
+black = "*"
+cryptography = ">=3.4,<43.0"
 
 [tool.poetry.dev-dependencies]
-black = "*"
-pytest = "*"
-pytest-asyncio = "*"
+black = "24.3.0"
+pytest = "^8.2.1"
+pytest-asyncio = ">=0.23.7"
 pytest-mock = "*"
 pytest-recording = "*"
 pytest-cov = "*"
 pyfakefs = "*"
 isort = "*"
 wheel = "*"
 sphinx = "*"
```

### Comparing `zscaler_sdk_python-0.2.0/zscaler/__init__.py` & `zscaler_sdk_python-0.3.0/zscaler/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler_sdk_python-0.2.0/zscaler/cache/cache.py` & `zscaler_sdk_python-0.3.0/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/cache/no_op_cache.py` & `zscaler_sdk_python-0.3.0/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/cache/zscaler_cache.py` & `zscaler_sdk_python-0.3.0/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/constants.py` & `zscaler_sdk_python-0.3.0/zscaler/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,19 @@
     "ZPATWO": "https://config.zpatwo.net",
     "BETA": "https://config.zpabeta.net",
     "GOV": "https://config.zpagov.net",
     "GOVUS": "https://config.zpagov.us",
     "PREVIEW": "https://config.zpapreview.net",
     "QA": "https://config.qa.zpath.net",
     "QA2": "https://pdx2-zpa-config.qa2.zpath.net",
+    "DEV": "https://public-api.dev.zpath.net",
 }
 
+DEV_AUTH_URL = "https://authn1.dev.zpath.net/authn/v1/oauth/token"
+
 RETRYABLE_STATUS_CODES = {429, 500, 502, 503, 504}
 MAX_RETRIES = 5
 BACKOFF_FACTOR = 1
 BACKOFF_BASE_DURATION = 2
 
 DATETIME_FORMAT = "%a, %d %b %Y %H:%M:%S %Z"
```

### Comparing `zscaler_sdk_python-0.2.0/zscaler/errors/http_error.py` & `zscaler_sdk_python-0.3.0/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/errors/zscaler_api_error.py` & `zscaler_sdk_python-0.3.0/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/exceptions/exceptions.py` & `zscaler_sdk_python-0.3.0/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/logger.py` & `zscaler_sdk_python-0.3.0/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/ratelimiter/ratelimiter.py` & `zscaler_sdk_python-0.3.0/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/user_agent.py` & `zscaler_sdk_python-0.3.0/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/utils.py` & `zscaler_sdk_python-0.3.0/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/__init__.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/activate.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/admin_and_role_management.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/apptotal.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/audit_logs.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/authentication_settings.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/client.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/cloud_apps.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/device_management.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/dlp.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/errors.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/firewall.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/forwarding_control.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/isolation_profile.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/labels.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/locations.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/sandbox.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/security.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/ssl_inspection.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/traffic.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/traffic.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/url_categories.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/url_filtering.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/users.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/web_dlp.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/workload_groups.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zia/zpa_gateway.py` & `zscaler_sdk_python-0.3.0/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/README.md` & `zscaler_sdk_python-0.3.0/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/__init__.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import requests
 from box import BoxList
 
 from zscaler import __version__
 from zscaler.cache.no_op_cache import NoOpCache
 from zscaler.cache.zscaler_cache import ZscalerCache
-from zscaler.constants import ZPA_BASE_URLS
+from zscaler.constants import ZPA_BASE_URLS, DEV_AUTH_URL
 from zscaler.errors.http_error import HTTPError, ZscalerAPIError
 from zscaler.exceptions.exceptions import HTTPException, ZscalerAPIException
 from zscaler.logger import setup_logging
 from zscaler.ratelimiter.ratelimiter import RateLimiter
 from zscaler.user_agent import UserAgent
 from zscaler.utils import (
     convert_keys_to_snake,
@@ -36,14 +36,15 @@
 from zscaler.zpa.emergency_access import EmergencyAccessAPI
 from zscaler.zpa.idp import IDPControllerAPI
 from zscaler.zpa.inspection import InspectionControllerAPI
 from zscaler.zpa.isolation import IsolationAPI
 from zscaler.zpa.lss import LSSConfigControllerAPI
 from zscaler.zpa.machine_groups import MachineGroupsAPI
 from zscaler.zpa.policies import PolicySetsAPI
+from zscaler.zpa.policiesv2 import PolicySetsV2API
 from zscaler.zpa.posture_profiles import PostureProfilesAPI
 from zscaler.zpa.privileged_remote_access import PrivilegedRemoteAccessAPI
 from zscaler.zpa.provisioning import ProvisioningKeyAPI
 from zscaler.zpa.saml_attributes import SAMLAttributesAPI
 from zscaler.zpa.scim_attributes import ScimAttributeHeaderAPI
 from zscaler.zpa.scim_groups import SCIMGroupsAPI
 from zscaler.zpa.segment_groups import SegmentGroupsAPI
@@ -147,22 +148,25 @@
             "Authorization": f"Bearer {self.access_token}",
             "User-Agent": self.user_agent,
         }
 
     @retry_with_backoff(retries=5)
     def login(self):
         """Log in to the ZPA API and set the access token for subsequent requests."""
-        data = urllib.parse.urlencode({"client_id": self.client_id, "client_secret": self.client_secret})
+        params = {"client_id": self.client_id, "client_secret": self.client_secret}
         headers = {
             "Content-Type": "application/x-www-form-urlencoded",
             "Accept": "application/json",
             "User-Agent": self.user_agent,
         }
         try:
             url = f"{self.baseurl}/signin"
+            if self.cloud == "DEV":
+                url = DEV_AUTH_URL + "?grant_type=CLIENT_CREDENTIALS"
+            data = urllib.parse.urlencode(params)
             resp = requests.post(url, data=data, headers=headers, timeout=self.timeout)
             # Avoid logging all data from the response, focus on the status and a summary instead
             logger.info("Login attempt with status: %d", resp.status_code)
             return resp
         except Exception as e:
             logger.error("Login failed due to an exception: %s", str(e))
             return None
@@ -568,14 +572,22 @@
         """
         The interface object for the :ref:`ZPA Policy Sets interface <zpa-policies>`.
 
         """
         return PolicySetsAPI(self)
 
     @property
+    def policiesv2(self):
+        """
+        The interface object for the :ref:`ZPA Policy Sets V2 interface <zpa-policiesv2>`.
+
+        """
+        return PolicySetsV2API(self)
+
+    @property
     def posture_profiles(self):
         """
         The interface object for the :ref:`ZPA Posture Profiles interface <zpa-posture_profiles>`.
 
         """
         return PostureProfilesAPI(self)
```

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments.py`

 * *Files 12% similar despite different names*

```diff
@@ -87,14 +87,48 @@
     def get_segment_by_name(self, name):
         apps = self.list_segments()
         for app in apps:
             if app.get("name") == name:
                 return app
         return None
 
+    def get_segments_by_type(self, application_type: str, expand_all: bool = False, **kwargs) -> Box:
+        """
+        Retrieve all configured application segments of a specified type, optionally expanding all related data.
+
+        Args:
+            application_type (str): Type of application segment to retrieve. Must be one of "BROWSER_ACCESS", "INSPECT", "SECURE_REMOTE_ACCESS".
+            expand_all (bool, optional): Whether to expand all related data. Defaults to False.
+
+        Keyword Args:
+            max_items (int, optional): The maximum number of items to request before stopping iteration.
+            max_pages (int, optional): The maximum number of pages to request before stopping iteration.
+            pagesize (int, optional): Specifies the page size. The default size is 20, but the maximum size is 500.
+            page (int, optional): Specifies the page number to begin fetching from.
+            search (str, optional): The search string used to match against features and fields.
+
+        Returns:
+            BoxList: List of application segments.
+
+        Examples:
+            >>> app_type = 'BROWSER_ACCESS'
+            >>> expand_all = True
+            >>> search = "ba_server01"
+            >>> app_segments = zpa.app_segments.get_segments_by_type(app_type, expand_all, search=search)
+        """
+        params = {"applicationType": application_type, "expandAll": "true" if expand_all else "false"}
+        # Include additional search parameters if specified
+        if "search" in kwargs:
+            params["search"] = kwargs["search"]
+
+        result, error = self.rest.get_paginated_data(path="/application/getAppsByType", params=params, **kwargs)
+        if error:
+            return BoxList([])  # Return an empty BoxList on failure due to the error
+        return result
+
     def delete_segment(self, segment_id: str, force_delete: bool = False) -> int:
         """
         Delete an application segment.
 
         Args:
             force_delete (bool):
                 Setting this field to true deletes the mapping between Application Segment and Segment Group.
```

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_inspection.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/app_segments_pra.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/certificates.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/client.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/cloud_connector_groups.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/connectors.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/emergency_access.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/errors.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/idp.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/inspection.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/isolation.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/isolation.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/lss.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/machine_groups.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/policies.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/policies.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/posture_profiles.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/privileged_remote_access.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/privileged_remote_access.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/provisioning.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/saml_attributes.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/scim_attributes.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/scim_groups.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/segment_groups.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/server_groups.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/servers.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/service_edges.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/zscaler/zpa/trusted_networks.py` & `zscaler_sdk_python-0.3.0/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler_sdk_python-0.2.0/PKG-INFO` & `zscaler_sdk_python-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.2.0
+Version: 0.3.0
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://github.com/zscaler/zscaler-sdk-python
 License: MIT
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Requires-Python: >=3.8,<4.0
@@ -19,32 +19,31 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Requires-Dist: aenum ; extra == "dev"
 Requires-Dist: arrow
-Requires-Dist: black (>=24.4.1,<25.0.0) ; extra == "dev"
+Requires-Dist: black ; extra == "dev"
 Requires-Dist: certifi
 Requires-Dist: charset-normalizer
-Requires-Dist: cryptography (>=3.4,<4.0)
+Requires-Dist: cryptography (>=3.4,<43.0)
 Requires-Dist: flake8
 Requires-Dist: flatdict
 Requires-Dist: idna
 Requires-Dist: pycryptodomex
 Requires-Dist: pydash ; extra == "dev"
 Requires-Dist: python-box (>=7.1.1,<8.0.0)
 Requires-Dist: python-dateutil
 Requires-Dist: pytz
 Requires-Dist: pyyaml
-Requires-Dist: requests
+Requires-Dist: requests (>=2.32.0)
 Requires-Dist: responses
 Requires-Dist: restfly
 Requires-Dist: six
-Requires-Dist: urllib3
 Requires-Dist: xmltodict
 Requires-Dist: yarl
 Project-URL: Bug Tracker, https://github.com/zscaler/zscaler-sdk-python/issues
 Project-URL: Documentation, https://zscaler-sdk-python.readthedocs.io
 Project-URL: Repository, https://github.com/zscaler/zscaler-sdk-python
 Description-Content-Type: text/markdown
```

