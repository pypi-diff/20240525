# Comparing `tmp/webull_python_sdk_core-0.1.6.tar.gz` & `tmp/webull_python_sdk_core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull_python_sdk_core-0.1.6.tar", last modified: Sat May 11 03:35:46 2024, max compression
+gzip compressed data, was "webull_python_sdk_core-0.1.7.tar", last modified: Sat May 25 02:17:35 2024, max compression
```

## Comparing `webull_python_sdk_core-0.1.6.tar` & `webull_python_sdk_core-0.1.7.tar`

### file list

```diff
@@ -1,191 +1,191 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.720464 webull_python_sdk_core-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-11 03:35:46.720464 webull_python_sdk_core-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:35:46.724464 webull_python_sdk_core-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.720464 webull_python_sdk_core-0.1.6/webull_python_sdk_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-11 03:35:46.000000 webull_python_sdk_core-0.1.6/webull_python_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-11 03:35:46.000000 webull_python_sdk_core-0.1.6/webull_python_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:35:46.000000 webull_python_sdk_core-0.1.6/webull_python_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-11 03:35:46.000000 webull_python_sdk_core-0.1.6/webull_python_sdk_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-11 03:35:46.000000 webull_python_sdk_core-0.1.6/webull_python_sdk_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.692463 webull_python_sdk_core-0.1.6/webullsdkcore/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.692463 webull_python_sdk_core-0.1.6/webullsdkcore/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.696464 webull_python_sdk_core-0.1.6/webullsdkcore/auth/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/algorithm/sha_hmac1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/algorithm/sha_hmac256.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.696464 webull_python_sdk_core-0.1.6/webullsdkcore/auth/composer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/composer/default_signature_composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.696464 webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/app_key_signer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/signer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/signer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.696464 webull_python_sdk_core-0.1.6/webullsdkcore/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.696464 webull_python_sdk_core-0.1.6/webullsdkcore/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/common/api_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/common/easy_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/common/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.696464 webull_python_sdk_core-0.1.6/webullsdkcore/data/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/data/endpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/data/retry_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.696464 webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/chained_endpoint_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/default_endpoint_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/local_config_regional_endpoint_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/resolver_endpoint_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/user_customized_endpoint_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.700464 webull_python_sdk_core-0.1.6/webullsdkcore/exception/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/exception/error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/exception/error_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/exception/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.700464 webull_python_sdk_core-0.1.6/webullsdkcore/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/http/method_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/http/protocol_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.700464 webull_python_sdk_core-0.1.6/webullsdkcore/retry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/retry/backoff_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/retry/retry_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/retry/retry_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/retry/retry_policy_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.700464 webull_python_sdk_core-0.1.6/webullsdkcore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/utils/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.700464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.704464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/_internal_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/help.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    34579 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.704464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.704464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   271088 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.712464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31822 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/big5freq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/big5prober.py
--rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/chardistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/charsetgroupprober.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/charsetprober.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.712464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/cli/chardetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/codingstatemachine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/cp949prober.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/escprober.py
--rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/escsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/eucjpprober.py
--rw-r--r--   0 runner    (1001) docker     (127)    14114 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euckrfreq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euckrprober.py
--rw-r--r--   0 runner    (1001) docker     (127)    32189 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euctwfreq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euctwprober.py
--rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/gb2312freq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/gb2312prober.py
--rw-r--r--   0 runner    (1001) docker     (127)    14406 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/hebrewprober.py
--rw-r--r--   0 runner    (1001) docker     (127)    26345 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/jisfreq.py
--rw-r--r--   0 runner    (1001) docker     (127)    20211 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/jpcntx.py
--rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langbulgarianmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langcyrillicmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langgreekmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langhebrewmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langhungarianmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langthaimodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langturkishmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/latin1prober.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/mbcharsetprober.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/mbcsgroupprober.py
--rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/mbcssm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/sbcharsetprober.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/sbcsgroupprober.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/sjisprober.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/universaldetector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/utf8prober.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.716464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    35660 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/connectionpool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.716464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_appengine_environ.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.716464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18128 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/appengine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/ntlmpool.py
--rw-r--r--   0 runner    (1001) docker     (127)    16405 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/pyopenssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    30853 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/securetransport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/filepost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.720464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.720464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/ordered_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/six.py
--rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/socks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.720464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/poolmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:35:46.720464 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/ssl_.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    28091 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/status_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/structures.py
--rw-r--r--   0 runner    (1001) docker     (127)    28182 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31456 2024-05-11 03:35:43.000000 webull_python_sdk_core-0.1.6/webullsdkcore/vendored/six.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.770145 webull_python_sdk_core-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-25 02:17:35.770145 webull_python_sdk_core-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:17:35.770145 webull_python_sdk_core-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.770145 webull_python_sdk_core-0.1.7/webull_python_sdk_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-25 02:17:35.000000 webull_python_sdk_core-0.1.7/webull_python_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-25 02:17:35.000000 webull_python_sdk_core-0.1.7/webull_python_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:17:35.000000 webull_python_sdk_core-0.1.7/webull_python_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-25 02:17:35.000000 webull_python_sdk_core-0.1.7/webull_python_sdk_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-25 02:17:35.000000 webull_python_sdk_core-0.1.7/webull_python_sdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.746144 webull_python_sdk_core-0.1.7/webullsdkcore/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.746144 webull_python_sdk_core-0.1.7/webullsdkcore/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.746144 webull_python_sdk_core-0.1.7/webullsdkcore/auth/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/algorithm/sha_hmac1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/algorithm/sha_hmac256.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.746144 webull_python_sdk_core-0.1.7/webullsdkcore/auth/composer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/composer/default_signature_composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.746144 webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/app_key_signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/signer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.746144 webull_python_sdk_core-0.1.7/webullsdkcore/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.750144 webull_python_sdk_core-0.1.7/webullsdkcore/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/common/api_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/common/easy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/common/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.750144 webull_python_sdk_core-0.1.7/webullsdkcore/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/data/endpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/data/retry_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.750144 webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/chained_endpoint_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/default_endpoint_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/local_config_regional_endpoint_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/resolver_endpoint_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/user_customized_endpoint_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.750144 webull_python_sdk_core-0.1.7/webullsdkcore/exception/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/exception/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/exception/error_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/exception/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.750144 webull_python_sdk_core-0.1.7/webullsdkcore/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/http/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/http/protocol_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.750144 webull_python_sdk_core-0.1.7/webullsdkcore/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/retry/backoff_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/retry/retry_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/retry/retry_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/retry/retry_policy_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.754145 webull_python_sdk_core-0.1.7/webullsdkcore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/utils/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.754145 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.754145 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/_internal_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21554 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6805 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18761 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34579 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.754145 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.758144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   271088 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.762144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31822 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/big5freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/big5prober.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/chardistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/charsetgroupprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/charsetprober.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.762144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/cli/chardetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/codingstatemachine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/cp949prober.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/escprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11078 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/escsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/eucjpprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14114 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euckrfreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euckrprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32189 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euctwfreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euctwprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/gb2312freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/gb2312prober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14406 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/hebrewprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26345 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/jisfreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20211 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/jpcntx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13407 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langbulgarianmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18516 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langcyrillicmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13256 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langgreekmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langhebrewmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langhungarianmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langthaimodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langturkishmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/latin1prober.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/mbcharsetprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/mbcsgroupprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/mbcssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/sbcharsetprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/sbcsgroupprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/sjisprober.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/universaldetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/utf8prober.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.766144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35660 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/connectionpool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.766144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_appengine_environ.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.766144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18128 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/appengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16405 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30853 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/filepost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.766144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.766144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/ordered_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30666 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/six.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/socks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.766144 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17555 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/poolmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26218 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:17:35.770145 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13809 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/ssl_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28091 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/status_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28182 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31456 2024-05-25 02:16:47.000000 webull_python_sdk_core-0.1.7/webullsdkcore/vendored/six.py
```

### Comparing `webull_python_sdk_core-0.1.6/setup.py` & `webull_python_sdk_core-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webull_python_sdk_core.egg-info/SOURCES.txt` & `webull_python_sdk_core-0.1.7/webull_python_sdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/auth/algorithm/sha_hmac1.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/auth/algorithm/sha_hmac1.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/auth/algorithm/sha_hmac256.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/auth/algorithm/sha_hmac256.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/auth/composer/default_signature_composer.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/auth/composer/default_signature_composer.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/auth/credentials.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/app_key_signer.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/app_key_signer.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/signer.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/signer.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/auth/signers/signer_factory.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/auth/signers/signer_factory.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/cache/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/client.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/client.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/common/api_type.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/common/api_type.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/common/easy_enum.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/common/easy_enum.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/compat.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/compat.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/chained_endpoint_resolver.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/chained_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/default_endpoint_resolver.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/default_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/local_config_regional_endpoint_resolver.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/local_config_regional_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/resolver_endpoint_request.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/resolver_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/endpoint/user_customized_endpoint_resolver.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/endpoint/user_customized_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/exception/error_code.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/exception/error_code.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/exception/error_msg.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/exception/error_msg.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/exception/exceptions.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/headers.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/headers.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/http/method_type.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/http/method_type.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/http/protocol_type.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/http/protocol_type.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/http/request.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/http/request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/http/response.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/http/response.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/request.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/retry/backoff_strategy.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/retry/backoff_strategy.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/retry/retry_condition.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/retry/retry_condition.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/retry/retry_policy.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/retry/retry_policy.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/retry/retry_policy_context.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/retry/retry_policy_context.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/utils/common.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/utils/common.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/utils/data.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/utils/data.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/utils/validation.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/utils/validation.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/__version__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/__version__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/_internal_utils.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/adapters.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/api.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/api.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/auth.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/auth.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/certs.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/certs.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/compat.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/compat.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/cookies.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/exceptions.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/help.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/help.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/hooks.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/models.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/models.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/__main__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/__main__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/cacert.pem` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/certifi/core.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/big5freq.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/big5prober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/chardistribution.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/charsetgroupprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/charsetprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/cli/chardetect.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/codingstatemachine.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/compat.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/cp949prober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/enums.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/escprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/escsm.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/eucjpprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euckrfreq.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euckrprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euctwfreq.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/euctwprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/gb2312freq.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/gb2312prober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/hebrewprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/jisfreq.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/jpcntx.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langbulgarianmodel.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langcyrillicmodel.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langcyrillicmodel.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langgreekmodel.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langhebrewmodel.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langhungarianmodel.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langthaimodel.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/langturkishmodel.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/latin1prober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/mbcharsetprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/mbcsgroupprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/mbcssm.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/sbcharsetprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/sbcsgroupprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/sjisprober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/universaldetector.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/utf8prober.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/chardet/version.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/chardet/version.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/_collections.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/connection.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/connectionpool.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_appengine_environ.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/bindings.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/low_level.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/appengine.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/ntlmpool.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/pyopenssl.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/securetransport.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/contrib/socks.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/exceptions.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/fields.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/filepost.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/makefile.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/ordered_dict.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/ordered_dict.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/six.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/socks.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/socks.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/poolmanager.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/request.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/response.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/__init__.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/connection.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/queue.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/queue.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/request.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/response.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/retry.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/selectors.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/selectors.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/ssl_.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/timeout.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/url.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages/urllib3/util/wait.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/packages.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/packages.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/sessions.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/status_codes.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/structures.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/structures.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/requests/utils.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/requests/utils.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_core-0.1.6/webullsdkcore/vendored/six.py` & `webull_python_sdk_core-0.1.7/webullsdkcore/vendored/six.py`

 * *Files identical despite different names*

