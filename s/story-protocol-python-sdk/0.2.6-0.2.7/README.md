# Comparing `tmp/story_protocol_python_sdk-0.2.6.tar.gz` & `tmp/story_protocol_python_sdk-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "story_protocol_python_sdk-0.2.6.tar", last modified: Fri May 24 19:12:04 2024, max compression
+gzip compressed data, was "story_protocol_python_sdk-0.2.7.tar", last modified: Fri May 24 21:33:40 2024, max compression
```

## Comparing `story_protocol_python_sdk-0.2.6.tar` & `story_protocol_python_sdk-0.2.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-24 19:12:03.000000 story_protocol_python_sdk-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.362907 story_protocol_python_sdk-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.362907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
--rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseRegistry/
--rw-r--r--   0 runner    (1001) docker     (127)    25612 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseToken/
--rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicensingModule/
--rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/
--rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.366907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyModule/
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
--rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/IPAsset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/License.py
--rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/Royalty.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/config_impl.json
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/generate_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/generate_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/story_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/utils/license_terms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 19:11:59.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/utils/transaction_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 19:12:04.370907 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-24 19:12:04.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-24 19:12:04.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 19:12:04.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 19:12:04.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 19:12:04.000000 story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-24 21:33:39.000000 story_protocol_python_sdk-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.759725 story_protocol_python_sdk-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.759725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.763725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.763725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.763725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/
+-rw-r--r--   0 runner    (1001) docker     (127)    15302 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.763725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseRegistry/
+-rw-r--r--   0 runner    (1001) docker     (127)    25612 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseRegistry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.763725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseToken/
+-rw-r--r--   0 runner    (1001) docker     (127)    21851 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseToken/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.763725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicensingModule/
+-rw-r--r--   0 runner    (1001) docker     (127)    18746 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicensingModule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.763725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/
+-rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyModule/
+-rw-r--r--   0 runner    (1001) docker     (127)    15228 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyModule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/
+-rw-r--r--   0 runner    (1001) docker     (127)    13327 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/IPAsset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/License.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8282 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/Royalty.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/config_impl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/generate_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/generate_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/story_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/utils/license_terms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-24 21:33:35.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/utils/transaction_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 21:33:40.767725 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-24 21:33:40.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-24 21:33:40.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 21:33:40.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 21:33:40.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 21:33:40.000000 story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/top_level.txt
```

### Comparing `story_protocol_python_sdk-0.2.6/LICENSE` & `story_protocol_python_sdk-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/PKG-INFO` & `story_protocol_python_sdk-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.2.6/README.md` & `story_protocol_python_sdk-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/setup.py` & `story_protocol_python_sdk-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='story_protocol_python_sdk',
-    version='0.2.6',
+    version='0.2.7',
     packages=find_packages(where='src', exclude=["tests"]),
     package_dir={'': 'src'},
     install_requires=[
         'web3>=5.0.0',
         'pytest',
         'python-dotenv'
     ],
```

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IPAssetRegistry/IPAssetRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/IpRoyaltyVaultImpl/IpRoyaltyVaultImpl_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseRegistry/LicenseRegistry_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicenseToken/LicenseToken_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/LicensingModule/LicensingModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/PILicenseTemplate/PILicenseTemplate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyModule/RoyaltyModule_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/abi/RoyaltyPolicyLAP/RoyaltyPolicyLAP_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/IPAsset.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/IPAsset.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/License.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/License.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/resources/Royalty.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/resources/Royalty.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/config.json` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/config.json`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/generate_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/generate_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/scripts/generate_client_impl.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/scripts/generate_client_impl.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/story_client.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/story_client.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/utils/license_terms.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/utils/license_terms.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk/utils/transaction_utils.py` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/PKG-INFO` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: story_protocol_python_sdk
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python SDK for interacting with the Story Protocol.
 Home-page: https://github.com/storyprotocol/python-sdk
 Author: Andrew Chung
 Author-email: andrew@storyprotocol.xyz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `story_protocol_python_sdk-0.2.6/src/story_protocol_python_sdk.egg-info/SOURCES.txt` & `story_protocol_python_sdk-0.2.7/src/story_protocol_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

