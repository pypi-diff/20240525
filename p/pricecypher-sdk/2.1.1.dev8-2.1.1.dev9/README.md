# Comparing `tmp/pricecypher_sdk-2.1.1.dev8.tar.gz` & `tmp/pricecypher_sdk-2.1.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pricecypher_sdk-2.1.1.dev8.tar", last modified: Thu May 23 12:56:08 2024, max compression
+gzip compressed data, was "pricecypher_sdk-2.1.1.dev9.tar", last modified: Thu May 23 21:05:48 2024, max compression
```

## Comparing `pricecypher_sdk-2.1.1.dev8.tar` & `pricecypher_sdk-2.1.1.dev9.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.772449 pricecypher_sdk-2.1.1.dev8/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.705824 pricecypher_sdk-2.1.1.dev8/.github/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.711556 pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      968 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      595 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1129 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/.github/pull_request_template.md
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.717175 pricecypher_sdk-2.1.1.dev8/.idea/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      372 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/.idea/.gitignore
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.720323 pricecypher_sdk-2.1.1.dev8/.idea/inspectionProfiles/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      174 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      181 2024-05-23 12:45:46.000000 pricecypher_sdk-2.1.1.dev8/.idea/vcs.xml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1756 2024-05-23 12:56:07.000000 pricecypher_sdk-2.1.1.dev8/ChangeLog
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1080 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev8/LICENSE
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1805 2024-05-23 12:56:08.772073 pricecypher_sdk-2.1.1.dev8/PKG-INFO
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      385 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/Pipfile
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    68635 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/Pipfile.lock
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3241 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.1.dev8/README.md
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      110 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/pyproject.toml
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      781 2024-05-23 12:56:08.775492 pricecypher_sdk-2.1.1.dev8/setup.cfg
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      104 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/setup.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.688001 pricecypher_sdk-2.1.1.dev8/src/
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.723861 pricecypher_sdk-2.1.1.dev8/src/pricecypher/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      484 2024-05-23 12:35:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.725973 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      666 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/base_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1179 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1131 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_value_collection.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2337 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/config_sections.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.730771 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1639 2024-05-23 12:48:40.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/BaseHandler.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      760 2024-05-23 12:53:16.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/InferenceHandler.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1240 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/QualityTestScript.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1824 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/ScopeScript.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1664 2024-05-23 12:54:10.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/Script.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      245 2024-05-23 12:54:46.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.733413 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3349 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/PredictResult.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3054 2022-11-02 15:42:11.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/TestResult.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       54 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.735691 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      109 2024-05-23 12:01:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/Accuracy.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      119 2022-10-07 14:52:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/TestStatus.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       66 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/enums/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    17732 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/datasets.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.737162 pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      572 2022-10-20 11:57:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/JsonEncoder.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       48 2022-10-20 11:55:13.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/__init__.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.740864 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      107 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      808 2022-09-30 14:31:36.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/base_endpoint.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2150 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/config.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     5245 2024-04-25 08:28:14.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/datasets.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1517 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/users.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     4068 2024-05-23 12:45:00.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/exceptions.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.744545 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      238 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1355 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/config.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     3493 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/datasets.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      843 2022-07-29 09:08:07.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/namespaced_schema.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      667 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/users.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.745919 pricecypher_sdk-2.1.1.dev8/src/pricecypher/oidc/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       61 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/oidc/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     2657 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/oidc/auth.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    12259 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher/rest.py
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.770678 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1805 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/PKG-INFO
--rw-r--r--   0 marvanderhorst   (502) staff       (20)     1991 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       50 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/entry_points.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/not-zip-safe
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       47 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/pbr.json
--rw-r--r--   0 marvanderhorst   (502) staff       (20)      645 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/requires.txt
--rw-r--r--   0 marvanderhorst   (502) staff       (20)       12 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 12:56:08.768997 pricecypher_sdk-2.1.1.dev8/tests/
--rw-r--r--   0 marvanderhorst   (502) staff       (20)        0 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev8/tests/__init__.py
--rw-r--r--   0 marvanderhorst   (502) staff       (20)    25578 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev8/tests/test_rest.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.337314 pricecypher_sdk-2.1.1.dev9/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.170283 pricecypher_sdk-2.1.1.dev9/.github/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.176525 pricecypher_sdk-2.1.1.dev9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      968 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      595 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1129 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev9/.github/pull_request_template.md
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.178233 pricecypher_sdk-2.1.1.dev9/.idea/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      372 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev9/.idea/.gitignore
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.182366 pricecypher_sdk-2.1.1.dev9/.idea/inspectionProfiles/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      174 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      181 2024-05-23 12:45:46.000000 pricecypher_sdk-2.1.1.dev9/.idea/vcs.xml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1816 2024-05-23 21:05:47.000000 pricecypher_sdk-2.1.1.dev9/ChangeLog
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1080 2022-03-25 10:57:36.000000 pricecypher_sdk-2.1.1.dev9/LICENSE
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1805 2024-05-23 21:05:48.337092 pricecypher_sdk-2.1.1.dev9/PKG-INFO
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      385 2024-05-23 21:02:16.000000 pricecypher_sdk-2.1.1.dev9/Pipfile
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    68635 2024-05-23 21:03:44.000000 pricecypher_sdk-2.1.1.dev9/Pipfile.lock
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3241 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.1.dev9/README.md
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      110 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev9/pyproject.toml
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      781 2024-05-23 21:05:48.340172 pricecypher_sdk-2.1.1.dev9/setup.cfg
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      104 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev9/setup.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.153774 pricecypher_sdk-2.1.1.dev9/src/
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.207347 pricecypher_sdk-2.1.1.dev9/src/pricecypher/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      484 2024-05-23 12:35:35.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.220441 pricecypher_sdk-2.1.1.dev9/src/pricecypher/collections/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      666 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/collections/base_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1179 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/collections/scope_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1131 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/collections/scope_value_collection.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2337 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/config_sections.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.243311 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1639 2024-05-23 12:48:40.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/BaseHandler.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      760 2024-05-23 12:53:16.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/InferenceHandler.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1240 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/QualityTestScript.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1824 2023-09-29 14:57:00.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/ScopeScript.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1664 2024-05-23 12:54:10.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/Script.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      245 2024-05-23 12:54:46.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.257177 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/dataclasses/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3349 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/dataclasses/PredictResult.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3054 2022-11-02 15:42:11.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/dataclasses/TestResult.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       54 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/dataclasses/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.267595 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/enums/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      109 2024-05-23 12:01:21.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/enums/Accuracy.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      119 2022-10-07 14:52:35.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/enums/TestStatus.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       66 2024-05-23 12:46:35.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/enums/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    17732 2024-05-23 11:12:21.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/datasets.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.272674 pricecypher_sdk-2.1.1.dev9/src/pricecypher/encoders/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      572 2022-10-20 11:57:22.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/encoders/JsonEncoder.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       48 2022-10-20 11:55:13.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/encoders/__init__.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.290992 pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      107 2023-08-22 09:53:07.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      808 2022-09-30 14:31:36.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/base_endpoint.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2150 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/config.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     5245 2024-04-25 08:28:14.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/datasets.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1517 2023-09-28 11:29:21.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/users.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     4068 2024-05-23 12:45:00.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/exceptions.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.308443 pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      238 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1355 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/config.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     3493 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/datasets.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      843 2022-07-29 09:08:07.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/namespaced_schema.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      667 2023-08-22 09:53:08.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/users.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.314717 pricecypher_sdk-2.1.1.dev9/src/pricecypher/oidc/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       61 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/oidc/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     2657 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/oidc/auth.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    12259 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher/rest.py
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.335858 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1805 2024-05-23 21:05:47.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)     1991 2024-05-23 21:05:48.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-05-23 21:05:47.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       50 2024-05-23 21:05:47.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        1 2024-05-23 12:56:08.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       47 2024-05-23 21:05:47.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/pbr.json
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)      645 2024-05-23 21:05:47.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/requires.txt
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)       12 2024-05-23 21:05:47.000000 pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 marvanderhorst   (502) staff       (20)        0 2024-05-23 21:05:48.335028 pricecypher_sdk-2.1.1.dev9/tests/
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)        0 2022-05-17 11:22:56.000000 pricecypher_sdk-2.1.1.dev9/tests/__init__.py
+-rw-r--r--   0 marvanderhorst   (502) staff       (20)    25578 2024-05-23 11:12:22.000000 pricecypher_sdk-2.1.1.dev9/tests/test_rest.py
```

### Comparing `pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/bug_report.md` & `pricecypher_sdk-2.1.1.dev9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/.github/ISSUE_TEMPLATE/feature_request.md` & `pricecypher_sdk-2.1.1.dev9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/.github/pull_request_template.md` & `pricecypher_sdk-2.1.1.dev9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/ChangeLog` & `pricecypher_sdk-2.1.1.dev9/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGES
 =======
 
+* Install \`pbr\` as regular package instead of dev-package
 * Refactor contracts
 * Update contracts and exceptions
 * Update gitignore
 * Add access token generator
 * Update dependencies
 * Update exceptions
 * Restructure location of collections module
```

### Comparing `pricecypher_sdk-2.1.1.dev8/LICENSE` & `pricecypher_sdk-2.1.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/PKG-INFO` & `pricecypher_sdk-2.1.1.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pricecypher-sdk
-Version: 2.1.1.dev8
+Version: 2.1.1.dev9
 Summary: Python wrapper around the different PriceCypher APIs
 Home-page: https://github.com/marketredesign/pricecypher_python_sdk
 Author: Deloitte Consulting B.V.
 Project-URL: Bug Tracker, https://github.com/marketredesign/pricecypher_python_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pricecypher_sdk-2.1.1.dev8/Pipfile.lock` & `pricecypher_sdk-2.1.1.dev9/Pipfile.lock`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9797709235209235%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'f39e9314c4807280a9801065740cda11b3f61c3f864122b6abc58a5da37e33f8'}}",*

 * * "'default'": "{'pbr': OrderedDict([('hashes', "*

 * *              "['sha256:4a7317d5e3b17a3dccb6a8cfe67dab65b20551404c52c8ed41279fa4f0cb4cda', "*

 * *              "'sha256:d1377122a5a00e2f940ee482999518efe16d745d423a670c27773dfbc3c9a7d9']), "*

 * *              '(\'index\', \'pypi\'), (\'markers\', "python_version >= \'2.6\'"), (\'version\', '*

 * *              "'==6.0.0')])}",*

 * * "'develop'": "{delete: ['pb […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "97b01c470a6588d020d982ea6f833b590e3e96fa95336c76040df497d9fa4c2c"
+            "sha256": "f39e9314c4807280a9801065740cda11b3f61c3f864122b6abc58a5da37e33f8"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.12"
         },
         "sources": [
             {
@@ -447,14 +447,23 @@
                 "sha256:e9b79011ff7a0f4b1d6da6a61aa1aa604fb312d6647de5bad20013682d1429ce",
                 "sha256:eee3a87076c0756de40b05c5e9a6069c035ba43e8dd71c379e68cab2c20f16ad"
             ],
             "index": "pypi",
             "markers": "python_version >= '3.9'",
             "version": "==2.2.2"
         },
+        "pbr": {
+            "hashes": [
+                "sha256:4a7317d5e3b17a3dccb6a8cfe67dab65b20551404c52c8ed41279fa4f0cb4cda",
+                "sha256:d1377122a5a00e2f940ee482999518efe16d745d423a670c27773dfbc3c9a7d9"
+            ],
+            "index": "pypi",
+            "markers": "python_version >= '2.6'",
+            "version": "==6.0.0"
+        },
         "pycparser": {
             "hashes": [
                 "sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6",
                 "sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc"
             ],
             "markers": "python_version >= '3.8'",
             "version": "==2.22"
@@ -930,23 +939,14 @@
             "hashes": [
                 "sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5",
                 "sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==24.0"
         },
-        "pbr": {
-            "hashes": [
-                "sha256:4a7317d5e3b17a3dccb6a8cfe67dab65b20551404c52c8ed41279fa4f0cb4cda",
-                "sha256:d1377122a5a00e2f940ee482999518efe16d745d423a670c27773dfbc3c9a7d9"
-            ],
-            "index": "pypi",
-            "markers": "python_version >= '2.6'",
-            "version": "==6.0.0"
-        },
         "pkginfo": {
             "hashes": [
                 "sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297",
                 "sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.10.0"
```

### Comparing `pricecypher_sdk-2.1.1.dev8/README.md` & `pricecypher_sdk-2.1.1.dev9/README.md`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/setup.cfg` & `pricecypher_sdk-2.1.1.dev9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/base_collection.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_collection.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/collections/scope_collection.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/collections/scope_value_collection.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/collections/scope_value_collection.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/config_sections.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/config_sections.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/BaseHandler.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/BaseHandler.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/InferenceHandler.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/InferenceHandler.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/QualityTestScript.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/QualityTestScript.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/ScopeScript.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/ScopeScript.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/Script.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/Script.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/PredictResult.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/dataclasses/PredictResult.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/contracts/dataclasses/TestResult.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/contracts/dataclasses/TestResult.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/datasets.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/datasets.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/encoders/JsonEncoder.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/encoders/JsonEncoder.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/base_endpoint.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/config.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/config.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/datasets.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/datasets.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/endpoints/users.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/exceptions.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/exceptions.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/config.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/config.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/datasets.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/datasets.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/namespaced_schema.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/namespaced_schema.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/models/users.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/models/users.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/oidc/auth.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/oidc/auth.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher/rest.py` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher/rest.py`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/PKG-INFO` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pricecypher-sdk
-Version: 2.1.1.dev8
+Version: 2.1.1.dev9
 Summary: Python wrapper around the different PriceCypher APIs
 Home-page: https://github.com/marketredesign/pricecypher_python_sdk
 Author: Deloitte Consulting B.V.
 Project-URL: Bug Tracker, https://github.com/marketredesign/pricecypher_python_sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/SOURCES.txt` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/src/pricecypher_sdk.egg-info/requires.txt` & `pricecypher_sdk-2.1.1.dev9/src/pricecypher_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pricecypher_sdk-2.1.1.dev8/tests/test_rest.py` & `pricecypher_sdk-2.1.1.dev9/tests/test_rest.py`

 * *Files identical despite different names*

