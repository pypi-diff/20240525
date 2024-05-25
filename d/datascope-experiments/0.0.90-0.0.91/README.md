# Comparing `tmp/datascope-experiments-0.0.90.tar.gz` & `tmp/datascope-experiments-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascope-experiments-0.0.90.tar", last modified: Wed May 22 23:51:22 2024, max compression
+gzip compressed data, was "datascope-experiments-0.0.91.tar", last modified: Sat May 25 01:04:51 2024, max compression
```

## Comparing `datascope-experiments-0.0.90.tar` & `datascope-experiments-0.0.91.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.696550 datascope-experiments-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 23:51:22.696550 datascope-experiments-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.688550 datascope-experiments-0.0.90/datascope/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.688550 datascope-experiments-0.0.90/datascope/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.688550 datascope-experiments-0.0.90/datascope/experiments/baselines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.688550 datascope-experiments-0.0.90/datascope/experiments/baselines/influence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/influence/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    33529 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/influence/genericNeuralNet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/influence/hessians.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/influence/importance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/influence/logisticRegressionWithLBFGS.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.688550 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/default_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/few_shot_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/matchingnet_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/predesigned_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.692550 datascope-experiments-0.0.90/datascope/experiments/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64198 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/bench/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/bench/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/bench/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.692550 datascope-experiments-0.0.90/datascope/experiments/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79148 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/datasets/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.692550 datascope-experiments-0.0.90/datascope/experiments/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/pipelines/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    23200 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/pipelines/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/pipelines/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/pipelines/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.692550 datascope-experiments-0.0.90/datascope/experiments/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48488 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/reports/aggregate_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.692550 datascope-experiments-0.0.90/datascope/experiments/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/scenarios/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5252 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/scenarios/compute_time.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17082 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/scenarios/data_discard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18245 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/scenarios/data_repair_scenario.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18480 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/scenarios/label_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/scenarios/marginal_contribution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.692550 datascope-experiments-0.0.90/datascope/experiments/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/utility/files.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/datascope/experiments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 23:51:22.696550 datascope-experiments-0.0.90/datascope_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 23:51:22.000000 datascope-experiments-0.0.90/datascope_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-22 23:51:22.000000 datascope-experiments-0.0.90/datascope_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 23:51:22.000000 datascope-experiments-0.0.90/datascope_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 23:51:22.000000 datascope-experiments-0.0.90/datascope_experiments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 23:51:22.000000 datascope-experiments-0.0.90/datascope_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 23:51:22.000000 datascope-experiments-0.0.90/datascope_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 23:51:22.696550 datascope-experiments-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-22 23:50:29.000000 datascope-experiments-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.498496 datascope-experiments-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-25 01:04:51.498496 datascope-experiments-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.490496 datascope-experiments-0.0.91/datascope/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.490496 datascope-experiments-0.0.91/datascope/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.490496 datascope-experiments-0.0.91/datascope/experiments/baselines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.490496 datascope-experiments-0.0.91/datascope/experiments/baselines/influence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/influence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/influence/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33529 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/influence/genericNeuralNet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/influence/hessians.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/influence/importance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/influence/logisticRegressionWithLBFGS.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.494496 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/default_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/few_shot_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/matchingnet_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/predesigned_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.494496 datascope-experiments-0.0.91/datascope/experiments/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66494 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/bench/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/bench/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9493 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/bench/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.494496 datascope-experiments-0.0.91/datascope/experiments/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79148 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/datasets/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.494496 datascope-experiments-0.0.91/datascope/experiments/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/pipelines/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23200 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/pipelines/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/pipelines/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/pipelines/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.494496 datascope-experiments-0.0.91/datascope/experiments/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48488 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/reports/aggregate_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.498496 datascope-experiments-0.0.91/datascope/experiments/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/scenarios/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5252 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/scenarios/compute_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17206 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/scenarios/data_discard.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18263 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/scenarios/data_repair_scenario.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18480 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/scenarios/label_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8088 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/scenarios/marginal_contribution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.498496 datascope-experiments-0.0.91/datascope/experiments/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/utility/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/datascope/experiments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 01:04:51.498496 datascope-experiments-0.0.91/datascope_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-25 01:04:51.000000 datascope-experiments-0.0.91/datascope_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-25 01:04:51.000000 datascope-experiments-0.0.91/datascope_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 01:04:51.000000 datascope-experiments-0.0.91/datascope_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 01:04:51.000000 datascope-experiments-0.0.91/datascope_experiments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-25 01:04:51.000000 datascope-experiments-0.0.91/datascope_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 01:04:51.000000 datascope-experiments-0.0.91/datascope_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 01:04:51.498496 datascope-experiments-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-25 01:03:59.000000 datascope-experiments-0.0.91/setup.py
```

### Comparing `datascope-experiments-0.0.90/PKG-INFO` & `datascope-experiments-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.90
+Version: 0.0.91
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/influence/dataset.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/influence/dataset.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/influence/genericNeuralNet.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/influence/genericNeuralNet.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/influence/hessians.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/influence/hessians.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/influence/importance.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/influence/importance.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/influence/logisticRegressionWithLBFGS.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/influence/logisticRegressionWithLBFGS.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/default_configs.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/default_configs.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/few_shot_classifier.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/few_shot_classifier.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/matchingnet_networks.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/matchingnet_networks.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/predesigned_modules.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/predesigned_modules.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/resnet.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/resnet.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/baselines/matchingnet/utils.py` & `datascope-experiments-0.0.91/datascope/experiments/baselines/matchingnet/utils.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/bench/__init__.py` & `datascope-experiments-0.0.91/datascope/experiments/bench/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     Scenario,
     Study,
     Report,
     Backend,
     Queue as QueueProtocol,
     attribute,
     result,
+    LazyLoader,
     get_scenario_runner,
     add_dynamic_arguments,
     DEFAULT_RESULTS_PATH,
     DEFAULT_RESULTS_SCENARIOS_PATH,
     DEFAULT_REPORTS_PATH,
     DEFAULT_STUDY_PATH,
     DEFAULT_BACKEND,
@@ -25,14 +26,15 @@
     "Scenario",
     "Study",
     "Report",
     "Backend",
     "QueueProtocol",
     "attribute",
     "result",
+    "LazyLoader",
     "get_scenario_runner",
     "add_dynamic_arguments",
     "DEFAULT_RESULTS_PATH",
     "DEFAULT_RESULTS_SCENARIOS_PATH",
     "DEFAULT_REPORTS_PATH",
     "DEFAULT_STUDY_PATH",
     "DEFAULT_BACKEND",
```

### Comparing `datascope-experiments-0.0.90/datascope/experiments/bench/base.py` & `datascope-experiments-0.0.91/datascope/experiments/bench/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import logging.handlers
 import numpy as np
 import os
 import pandas as pd
 import pickle
 import random
 import re
+import shutil
 import signal
 import socket
 import string
 import subprocess
 import sys
 import threading
 import time
@@ -410,17 +411,17 @@
         name = base[len(basename) + 1 :]  # noqa: E203
 
         if name == "":
             continue
 
         if ext == ".npy":
             if name in lazy:
-                res[name] = LazyLoader(lambda: np.load(path))
+                res[name] = LazyLoader(lambda: np.load(path, allow_pickle=True))
             else:
-                res[name] = np.load(path)
+                res[name] = np.load(path, allow_pickle=True)
         elif ext == ".csv":
             if name in lazy:
                 res[name] = LazyLoader(lambda: pd.read_csv(path, index_col=0))
             else:
                 res[name] = pd.read_csv(path, index_col=0)
         elif ext == ".yaml":
             with open(path) as f:
@@ -640,14 +641,18 @@
     @cached_property
     def attributes(self) -> Dict[str, Any]:
         props = attribute.get_properties(type(self))
         attributes = dict((name, get_property_value(self, name)) for name in props.keys())
         attributes[self._class_argname] = self.get_class_identifier()
         return attributes
 
+    @cached_property
+    def flattened_attributes(self) -> Dict[str, Any]:
+        return self._flatten_attributes(self.attributes)
+
     def __repr__(self) -> str:
         full_class_id = "%s.%s" % (type(self).__module__, type(self).__name__)
         class_id = self.get_class_identifier()
         result = str(self)
         if result.startswith(class_id) and class_id != full_class_id:
             result = result.replace(class_id, full_class_id, 1)
         return result
@@ -661,21 +666,27 @@
         if len(attribute_string) > 0:
             result += "(%s)" % attribute_string
         return result
 
     @classmethod
     def _compose_attributes(cls: Type["Configurable"], attributes: Dict[str, Any]) -> Dict[str, Any]:
         attribute_descriptors: Dict[str, AttributeDescriptor] = cls._get_attribute_descriptors()
-        result: Dict[str, Any] = {}
+        result_properties = result.get_properties(cls)
+
+        composed_result: Dict[str, Any] = {}
         skip_prefixes: Set[str] = set()
         for k in sorted(attributes.keys()):
-            if any(k.startswith(prefix) for prefix in skip_prefixes):
+            if (
+                any(k.startswith(prefix) for prefix in skip_prefixes)
+                and k not in attribute_descriptors
+                and k not in result_properties
+            ):
                 continue
             v = attributes[k]
-            result[k] = v
+            composed_result[k] = v
             if isinstance(v, str) or isinstance(v, dict):
                 target_base_descriptor = attribute_descriptors.get(k, None)
                 if target_base_descriptor is not None:
                     target_base_cls = target_base_descriptor.attr_type
                     if target_base_cls is not None and issubclass(target_base_cls, Configurable):
                         target_cls_id = v if isinstance(v, str) else v.get(target_base_cls._class_argname, None)
                         if target_cls_id is None:
@@ -717,19 +728,19 @@
                             if isinstance(v, dict):
                                 target_attributes.update(
                                     {kk: vv for kk, vv in v.items() if kk != target_base_cls._class_argname}
                                 )
 
                             # Recursively compose target attributes and instantiate the configurable object.
                             target_attributes = target_cls._compose_attributes(target_attributes)
-                            result[k] = target_cls(**target_attributes)
+                            composed_result[k] = target_cls(**target_attributes)
 
                             # Ensure that the nested attributes are not passed to the parent object constructor.
                             skip_prefixes.add(k + cls.NESTING_SEPARATOR)
-        return result
+        return composed_result
 
     @classmethod
     def _flatten_attributes(cls: Type["Configurable"], attributes: Dict[str, Any]) -> Dict[str, Any]:
         result: Dict[str, Any] = {}
         for k, v in attributes.items():
             if isinstance(v, Configurable):
                 result[k] = v.get_class_identifier()
@@ -900,64 +911,88 @@
                     # assert isinstance(scenario, Scenario)
                     yield scenario
 
     @classmethod
     def is_valid_config(cls, **attributes: Any) -> bool:
         return True
 
-    def save(self, path: str) -> None:
+    def save(self, path: str, include_results: bool = True) -> None:
         if os.path.splitext(path)[1] != "":
             raise ValueError("The provided path '%s' is not a valid directory path." % path)
         os.makedirs(path, exist_ok=True)
 
         # Write a log file.
         logpath = os.path.join(path, "scenario.log")
         with open(logpath, "w") as f:
             self._logstream.seek(0)
             copyfileobj(self._logstream, f)
             self._logstream.seek(0, SEEK_END)
 
         # Save attributes as a single yaml file.
-        attributes = self._flatten_attributes(self.attributes)
+        attributes = self.flattened_attributes
         save_dict(attributes, path, "attributes")
 
         # Save results as separate files.
-        props: Dict[str, result] = result.get_properties(type(self))
-        results = dict((name, prop.fget(self) if prop.fget is not None else None) for (name, prop) in props.items())
-        save_dict(results, path, "results")
+        if include_results:
+            props: Dict[str, result] = result.get_properties(type(self))
+            results = dict((name, prop.fget(self) if prop.fget is not None else None) for (name, prop) in props.items())
+            save_dict(results, path, "results")
 
     @classmethod
     def load(cls, path: str) -> "Scenario":
         if not os.path.isdir(path):
             raise ValueError("The provided path '%s' does not point to a directory." % path)
 
         # Load the log file.
         logpath = os.path.join(path, "scenario.log")
         logstream: Optional[TextIOBase] = None
         if os.path.isfile(logpath):
             with open(logpath, "r") as f:
                 logstream = StringIO(f.read())
 
+        # Load config attributes and determine scenario type.
         attributes = load_dict(path, "attributes")
-        attributes = cls._compose_attributes(attributes)
-        lazy = [k for k, v in result.get_properties(cls).items() if v.lazy]
+        class_id = attributes.get(cls._class_argname, None)
+        if class_id is None:
+            raise ValueError("The file '%s' does not contain a valid scenario class identifier." % path)
+        target_class: Type[Scenario] = cls.get_subclasses().get(class_id, None)
+        if target_class is None:
+            raise ValueError("The provided class ID '%s' does not correspond to any valid scenario class." % class_id)
+
+        # Load results.
+        attributes = target_class._compose_attributes(attributes)
+        lazy = [k for k, v in result.get_properties(target_class).items() if v.lazy]
         results = load_dict(path, "results", lazy=lazy)
         kwargs = {"logstream": logstream}
-        scenario = cls.from_dict({**attributes, **results, **kwargs})
+        scenario = target_class.from_dict({**attributes, **results, **kwargs})
         assert isinstance(scenario, Scenario)
         return scenario
 
     @classmethod
     def isscenario(cls, path: str) -> bool:
         attributes_filename = os.path.join(path, ".".join(["attributes", "yaml"]))
         return os.path.isdir(path) and os.path.isfile(attributes_filename)  # TODO: Refine this check.
 
-    def is_match(self, other: "Scenario") -> bool:
-        other_attributes = other.attributes
-        return all(other_attributes.get(k, None) == v for (k, v) in self.attributes.items() if k != "id")
+    def is_match(self, other: Union["Scenario", Dict[str, Any]], ignore_id: bool = True) -> bool:
+        self_attributes = self.flattened_attributes
+        other_attributes = other.flattened_attributes if isinstance(other, Scenario) else other
+        for key, self_value in self_attributes.items():
+            if key == "id" and ignore_id:
+                continue
+            other_value = other_attributes.get(key, None)
+            if other_value is not None:
+                if isinstance(other_value, Iterable) and not isinstance(other_value, str):
+                    if isinstance(self_value, Iterable) and not isinstance(self_value, str):
+                        raise ValueError("Both values are iterable. This is not supported.")
+                    if self_value not in other_value:
+                        return False
+                else:
+                    if self_value != other_value:
+                        return False
+        return True
 
 
 class ScenarioEvent:
     class Type(Enum):
         STARTED = "started"
         COMPLETED = "completed"
 
@@ -996,19 +1031,15 @@
 
     def __len__(self) -> int:
         return self._data.__len__()
 
     @property
     def df(self):
         data = [
-            (
-                x._flatten_attributes(x.attributes)
-                if isinstance(x, Configurable)
-                else {a: get_value(x, a) for a in self._attributes}
-            )
+            (x.flattened_attributes if isinstance(x, Configurable) else {a: get_value(x, a) for a in self._attributes})
             for x in self._data
         ]
         df = pd.DataFrame.from_dict({a: [x.get(a, None) for x in data] for a in self._attributes})
         if self._key is not None:
             df.set_index(self._key, inplace=True)
         return df.dropna(axis=1, how="all")
 
@@ -1312,15 +1343,15 @@
                     scenarios_running = 0
                     for scenario in self.scenarios:
                         scenarios_pending -= 1
                         if scenario.completed:
                             if pbar is not None:
                                 pbar.update(1)
                         else:
-                            path = self.save_scenario(scenario)
+                            path = self.save_scenario(scenario, include_results=False)
                             logpath = os.path.join(path, "slurm.log")
                             run_command = "python -m datascope.experiments run-scenario -o %s -e %s -m %s" % (
                                 path,
                                 address,
                                 slurm_jobmemory,
                             )
                             slurm_command = "sbatch --job-name=%s" % self.id
@@ -1389,25 +1420,34 @@
             exppath = scenario_path_format.format_map(replacements)
             if exppath in scenario_paths:
                 raise ValueError(
                     "Provided scenario_path does not produce unique paths. The path '%s' caused a conflict." % exppath
                 )
             scenario_paths.add(exppath)
 
-    def save_scenario(self, scenario: Scenario) -> str:
+    def save_scenario(self, scenario: Scenario, include_results: bool = True) -> str:
         if self.path is None:
             raise ValueError("This study has no output path.")
         attributes = re.findall(r"\{(.*?)\}", self._scenario_path_format)
         replacements = dict((name, get_property_value(scenario, name)) for name in attributes)
         exppath = self._scenario_path_format.format_map(replacements)
         full_exppath = os.path.join(self.path, "scenarios", exppath)
-        scenario.save(full_exppath)
+        scenario.save(full_exppath, include_results=include_results)
         return full_exppath
 
-    def save(self, save_scenarios: bool = True) -> None:
+    def delete_scenario(self, scenario: Scenario) -> None:
+        if self.path is None:
+            raise ValueError("This study has no output path.")
+        attributes = re.findall(r"\{(.*?)\}", self._scenario_path_format)
+        replacements = dict((name, get_property_value(scenario, name)) for name in attributes)
+        exppath = self._scenario_path_format.format_map(replacements)
+        full_exppath = os.path.join(self.path, "scenarios", exppath)
+        shutil.rmtree(full_exppath)
+
+    def save(self, save_scenarios: bool = True, include_results: bool = True) -> None:
         # Make directory that will contain the study.
         os.makedirs(self.path, exist_ok=True)
 
         # Write a marker file.
         markerpath = os.path.join(self.path, "study.yml")
         with open(markerpath, "w") as f:
             yaml.safe_dump({"id": self.id, "scenario_path_format": self.scenario_path_format}, f)
@@ -1418,15 +1458,15 @@
             self._logstream.seek(0)
             copyfileobj(self._logstream, f)
             self._logstream.seek(0, SEEK_END)
 
         # Save all scenarios.
         if save_scenarios:
             for scenario in self.scenarios:
-                self.save_scenario(scenario)
+                self.save_scenario(scenario, include_results=include_results)
 
     @classmethod
     def load_scenarios(cls, path: str) -> List[Scenario]:
         # Load all scenarios.
         scenarios: List[Scenario] = []
         for attpath in glob(os.path.join(path, "**/attributes.yaml"), recursive=True):
             exppath = os.path.dirname(attpath)
@@ -1525,19 +1565,19 @@
         df = pd.concat(
             [s.dataframe.assign(scenario=s.get_class_identifier(), id=s.id) for s in self.scenarios], ignore_index=True
         )
         df.sort_index(inplace=True)
         return df
 
     def get_scenarios(self, **attributes: Dict[str, Any]) -> Sequence[Scenario]:
-        res: List[Scenario] = []
-        for exp in self.scenarios:
-            if all(has_attribute_value(exp, name, value) for (name, value) in attributes.items() if hasattr(exp, name)):
-                res.append(exp)
-        return res
+        result: List[Scenario] = []
+        for scenario in self.scenarios:
+            if scenario.is_match(attributes, ignore_id=False):
+                result.append(scenario)
+        return result
 
     @classmethod
     def union(
         cls: Type["Study"],
         *studies: "Study",
         id: Optional[str] = None,
         outpath: str = DEFAULT_RESULTS_PATH,
```

### Comparing `datascope-experiments-0.0.90/datascope/experiments/bench/commands.py` & `datascope-experiments-0.0.91/datascope/experiments/bench/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             logstream=study._logstream,
         )
     else:
         study = Study(scenarios=scenarios, outpath=output_path)
 
     # Eagerly save the study with all unfinished scenarios.
     if not no_save:
-        study.save()
+        study.save(include_results=False)
 
     # Run the study.
     study.run(
         backend=backend,
         ray_address=ray_address,
         ray_numprocs=ray_numprocs,
         slurm_jobtime=slurm_jobtime,
@@ -131,17 +131,17 @@
         if len(scenarios) == 0:
             raise ValueError("The provided attributes do not correspond to any valid scenario.")
         elif len(scenarios) > 1:
             raise ValueError("The provided attributes correspond to more than one valid scenario.")
         scenario = scenarios[0]
         path = os.path.join(output_path, scenario.id)
 
-        # Eagerly save the scenario.
+        # Eagerly save the scenario (config attributes only).
         if not no_save:
-            scenario.save(path)
+            scenario.save(path, include_results=False)
     queue: Optional[QueueProtocol] = None
     pickled_queue = False
     if event_server is not None:
         client = zerorpc.Client()
         client.connect(event_server)
         queue = client
         pickled_queue = True
```

### Comparing `datascope-experiments-0.0.90/datascope/experiments/bench/main.py` & `datascope-experiments-0.0.91/datascope/experiments/bench/main.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/datasets/__init__.py` & `datascope-experiments-0.0.91/datascope/experiments/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/datasets/base.py` & `datascope-experiments-0.0.91/datascope/experiments/datasets/base.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/datasets/cache.py` & `datascope-experiments-0.0.91/datascope/experiments/datasets/cache.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/pipelines/__init__.py` & `datascope-experiments-0.0.91/datascope/experiments/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/pipelines/models.py` & `datascope-experiments-0.0.91/datascope/experiments/pipelines/models.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/pipelines/pipelines.py` & `datascope-experiments-0.0.91/datascope/experiments/pipelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/pipelines/postprocessors.py` & `datascope-experiments-0.0.91/datascope/experiments/pipelines/postprocessors.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/pipelines/utility.py` & `datascope-experiments-0.0.91/datascope/experiments/pipelines/utility.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/reports/aggregate_plot.py` & `datascope-experiments-0.0.91/datascope/experiments/reports/aggregate_plot.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/scenarios/compute_time.py` & `datascope-experiments-0.0.91/datascope/experiments/scenarios/compute_time.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/scenarios/data_discard.py` & `datascope-experiments-0.0.91/datascope/experiments/scenarios/data_discard.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
         # Compute importance scores and time it.
         random = np.random.RandomState(seed=self.seed)
         importance_time_start = process_time_ns()
         importance: Optional[Importance] = None
         importances: Optional[NDArray] = None
         if self.method == RepairMethod.RANDOM:
-            importances = np.array(random.rand(dataset.trainsize))
+            importances = np.array(random.rand(dataset.provenance.num_units))
         elif self.method == RepairMethod.INFLUENCE:
             from ..baselines.influence.importance import InfluenceImportance
 
             dataset_f = dataset.apply(pipeline)
             importance = InfluenceImportance()
             importances = np.array(
                 importance.fit(dataset_f.X_train, dataset_f.y_train, provenance=dataset_f.provenance).score(
@@ -316,15 +316,19 @@
             discarded_units[target_units] = True
             present_units = np.invert(discarded_units).astype(int)
             present_idx = dataset.provenance.query(present_units)
             dataset_current = dataset.select_train(present_idx)  # type: ignore
             discarded_rel += rel_units_per_checkpoint
 
             # Compute quality metrics.
-            dataset_current_f = dataset_current.apply(pipeline, cache_dir=self.pipeline_cache_dir)
+            dataset_current_f = (
+                dataset_current
+                if self.eager_preprocessing
+                else dataset_current.apply(pipeline, cache_dir=self.pipeline_cache_dir)
+            )
             scores = self.compute_model_quality_scores(
                 model=model,
                 dataset=dataset_current_f,
                 postprocessor=postprocessor,
                 compute_eqodds=compute_eqodds,
                 groupings_val=groupings_val,
                 groupings_test=groupings_test,
```

### Comparing `datascope-experiments-0.0.90/datascope/experiments/scenarios/data_repair_scenario.py` & `datascope-experiments-0.0.91/datascope/experiments/scenarios/data_repair_scenario.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,19 +202,19 @@
 
 
 def get_relative_score(scores: Series, lower_is_better: bool = False) -> Series:
     start_score = scores.iloc[0]
     if lower_is_better:
         min_score = min(scores)
         delta_score = abs(start_score - min_score)
-        return scores.apply(lambda x: (x - min_score) / delta_score)
+        return scores.apply(lambda x: (x - min_score) / (delta_score + 1e-9))
     else:
         max_score = max(scores)
         delta_score = abs(start_score - max_score)
-        return scores.apply(lambda x: (x - start_score) / delta_score)
+        return scores.apply(lambda x: (x - start_score) / (delta_score + 1e-9))
 
 
 class DataRepairScenario(Scenario, abstract=True):
     def __init__(
         self,
         dataset: Dataset,
         pipeline: Pipeline,
```

### Comparing `datascope-experiments-0.0.90/datascope/experiments/scenarios/label_repair.py` & `datascope-experiments-0.0.91/datascope/experiments/scenarios/label_repair.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/scenarios/marginal_contribution.py` & `datascope-experiments-0.0.91/datascope/experiments/scenarios/marginal_contribution.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope/experiments/utility/files.py` & `datascope-experiments-0.0.91/datascope/experiments/utility/files.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/datascope_experiments.egg-info/PKG-INFO` & `datascope-experiments-0.0.91/datascope_experiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.90
+Version: 0.0.91
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.90/datascope_experiments.egg-info/SOURCES.txt` & `datascope-experiments-0.0.91/datascope_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.90/setup.py` & `datascope-experiments-0.0.91/setup.py`

 * *Files identical despite different names*

