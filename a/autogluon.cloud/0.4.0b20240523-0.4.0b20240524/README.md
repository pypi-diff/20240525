# Comparing `tmp/autogluon.cloud-0.4.0b20240523.tar.gz` & `tmp/autogluon.cloud-0.4.0b20240524.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autogluon.cloud-0.4.0b20240523.tar", last modified: Thu May 23 09:05:24 2024, max compression
+gzip compressed data, was "dist/autogluon.cloud-0.4.0b20240524.tar", last modified: Fri May 24 09:05:22 2024, max compression
```

## Comparing `autogluon.cloud-0.4.0b20240523.tar` & `autogluon.cloud-0.4.0b20240524.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/backend_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/ray_aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    22735 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    59108 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/tabular_sagemaker_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/cluster_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/ray_cluster_config_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/ray_cluster_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/data/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/data/format_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/default_cluster_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/default_cluster_configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/endpoint/sagemaker_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/ray_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/remote_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/sagemaker_job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38576 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/tabular_cloud_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/ray_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/ray_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/ray_scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/script_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/ag_sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/aws_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/deserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/dlc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/ray_aws_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/sagemaker_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-23 09:05:14.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-23 09:05:23.000000 autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:05:24.000000 autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/backend_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/ray_aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22735 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59108 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/tabular_sagemaker_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/cluster_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/ray_cluster_config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/ray_cluster_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/data/format_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/default_cluster_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/default_cluster_configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/endpoint/sagemaker_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/ray_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9790 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/sagemaker_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38576 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/tabular_cloud_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13310 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/ray_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/ray_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/ray_scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/script_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/ag_sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/aws_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/dlc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/ray_aws_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/sagemaker_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-05-24 09:05:12.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 09:05:21.000000 autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:05:22.000000 autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/zip-safe
```

### Comparing `autogluon.cloud-0.4.0b20240523/LICENSE` & `autogluon.cloud-0.4.0b20240524/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/PKG-INFO` & `autogluon.cloud-0.4.0b20240524/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.cloud
-Version: 0.4.0b20240523
+Version: 0.4.0b20240524
 Summary: Train and deploy AutoGluon backed models on the cloud
 Home-page: https://github.com/autogluon/autogluon-cloud
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-cloud/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-cloud/
```

### Comparing `autogluon.cloud-0.4.0b20240523/README.md` & `autogluon.cloud-0.4.0b20240524/README.md`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/setup.cfg` & `autogluon.cloud-0.4.0b20240524/setup.cfg`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/setup.py` & `autogluon.cloud-0.4.0b20240524/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/backend.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/backend_factory.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/backend_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/multimodal_sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/ray_aws_backend.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/ray_aws_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/ray_backend.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/ray_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/sagemaker_backend.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/backend/timeseries_sagemaker_backend.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/cluster_config_generator.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/cluster_config_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/cluster_manager.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/constants.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/ray_aws_cluster_config_generator.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/ray_aws_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/cluster/ray_cluster_manager.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/cluster/ray_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/data/format_converter.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/data/format_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/endpoint/endpoint.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/endpoint/sagemaker_endpoint.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/endpoint/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/ray_job.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/ray_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/remote_job.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/remote_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/job/sagemaker_job.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/job/sagemaker_job.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/cloud_predictor.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/multimodal_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/tabular_cloud_predictor.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/tabular_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/predictor/timeseries_cloud_predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/ray_scripts/train.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/ray_scripts/train.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/multimodal_serve.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/tabular_serve.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/timeseries_serve.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/sagemaker_scripts/train.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/sagemaker_scripts/train.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/scripts/script_manager.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/scripts/script_manager.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/ag_sagemaker.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/ag_sagemaker.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/aws_utils.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/deserializers.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/deserializers.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/dlc_utils.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/dlc_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/ec2.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/ec2.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/iam.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/ray_aws_iam.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/ray_aws_iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/s3_utils.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/sagemaker_iam.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/sagemaker_iam.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/serializers.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon/cloud/utils/utils.py` & `autogluon.cloud-0.4.0b20240524/src/autogluon/cloud/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/PKG-INFO` & `autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.cloud
-Version: 0.4.0b20240523
+Version: 0.4.0b20240524
 Summary: Train and deploy AutoGluon backed models on the cloud
 Home-page: https://github.com/autogluon/autogluon-cloud
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-cloud/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-cloud/
```

### Comparing `autogluon.cloud-0.4.0b20240523/src/autogluon.cloud.egg-info/SOURCES.txt` & `autogluon.cloud-0.4.0b20240524/src/autogluon.cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

