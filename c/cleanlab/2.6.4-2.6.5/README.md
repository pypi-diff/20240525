# Comparing `tmp/cleanlab-2.6.4.tar.gz` & `tmp/cleanlab-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-2.6.4.tar", last modified: Tue May  7 18:24:11 2024, max compression
+gzip compressed data, was "cleanlab-2.6.5.tar", last modified: Fri May 24 23:39:20 2024, max compression
```

## Comparing `cleanlab-2.6.4.tar` & `cleanlab-2.6.5.tar`

### file list

```diff
@@ -1,121 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.791739 cleanlab-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-05-07 18:24:04.000000 cleanlab-2.6.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-07 18:24:04.000000 cleanlab-2.6.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    21688 2024-05-07 18:24:04.000000 cleanlab-2.6.4/DEVELOPMENT.md
--rw-r--r--   0 runner    (1001) docker     (127)    34524 2024-05-07 18:24:04.000000 cleanlab-2.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-07 18:24:04.000000 cleanlab-2.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    63287 2024-05-07 18:24:11.791739 cleanlab-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21200 2024-05-07 18:24:04.000000 cleanlab-2.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.771739 cleanlab-2.6.4/cleanlab/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.771739 cleanlab-2.6.4/cleanlab/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/benchmarking/noise_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    53475 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    69517 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/data_valuation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.775739 cleanlab-2.6.4/cleanlab/datalab/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/datalab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.775739 cleanlab-2.6.4/cleanlab/datalab/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.775739 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/adapter/imagelab.py
--rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/data_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/helper_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/data_valuation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/imbalance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/issue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/label.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    20403 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/noniid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/null.py
--rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/outlier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/label.py
--rw-r--r--   0 runner    (1001) docker     (127)    15788 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/underperforming_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/model_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/datalab/internal/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    24156 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/cifar_cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/coteaching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.779739 cleanlab-2.6.4/cleanlab/experimental/datalab/
--rw-r--r--   0 runner    (1001) docker     (127)    18095 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/datalab/data_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    35575 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/label_issues_batched.py
--rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/mnist_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/experimental/span_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    43279 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.783738 cleanlab-2.6.4/cleanlab/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/label_quality_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/latent_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/multiannotator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23533 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/multilabel_scorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/multilabel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/numerics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/object_detection_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/outlier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/regression_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/segmentation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/token_classification_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    29055 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/internal/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.783738 cleanlab-2.6.4/cleanlab/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/models/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/models/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    90505 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multiannotator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.783738 cleanlab-2.6.4/cleanlab/multilabel_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/multilabel_classification/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/object_detection/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    49070 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    34427 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/object_detection/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    30679 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/outlier.py
--rw-r--r--   0 runner    (1001) docker     (127)    25824 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/regression/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39296 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/regression/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/regression/rank.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    14450 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/segmentation/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/token_classification/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-05-07 18:24:04.000000 cleanlab-2.6.4/cleanlab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 18:24:11.787739 cleanlab-2.6.4/cleanlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    63287 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 18:24:11.000000 cleanlab-2.6.4/cleanlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-07 18:24:04.000000 cleanlab-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-07 18:24:11.791739 cleanlab-2.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-07 18:24:04.000000 cleanlab-2.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.740982 cleanlab-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-05-24 23:39:12.000000 cleanlab-2.6.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-24 23:39:12.000000 cleanlab-2.6.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21688 2024-05-24 23:39:12.000000 cleanlab-2.6.5/DEVELOPMENT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34524 2024-05-24 23:39:12.000000 cleanlab-2.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 23:39:12.000000 cleanlab-2.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    63319 2024-05-24 23:39:20.740982 cleanlab-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21232 2024-05-24 23:39:12.000000 cleanlab-2.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.728982 cleanlab-2.6.5/cleanlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.728982 cleanlab-2.6.5/cleanlab/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/benchmarking/noise_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53455 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69437 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/data_valuation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.728982 cleanlab-2.6.5/cleanlab/datalab/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29414 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/datalab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.728982 cleanlab-2.6.5/cleanlab/datalab/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.728982 cleanlab-2.6.5/cleanlab/datalab/internal/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/adapter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/adapter/imagelab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/data_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/helper_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20877 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.732982 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/data_valuation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10157 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/imbalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/issue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.732982 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/multilabel/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/multilabel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/multilabel/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17660 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/noniid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/outlier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.732982 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9304 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/regression/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/underperforming_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11198 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/model_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/datalab/internal/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24156 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.732982 cleanlab-2.6.5/cleanlab/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/experimental/cifar_cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/experimental/coteaching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.732982 cleanlab-2.6.5/cleanlab/experimental/datalab/
+-rw-r--r--   0 runner    (1001) docker     (127)    18095 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/experimental/datalab/data_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35575 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/experimental/label_issues_batched.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/experimental/mnist_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/experimental/span_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43279 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.736982 cleanlab-2.6.5/cleanlab/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/label_quality_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14645 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/latent_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16160 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/multiannotator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23533 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/multilabel_scorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/multilabel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.736982 cleanlab-2.6.5/cleanlab/internal/neighbor/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/neighbor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24264 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/neighbor/knn_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/neighbor/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/neighbor/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/numerics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/object_detection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/outlier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/regression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/segmentation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8945 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/token_classification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29430 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/internal/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.736982 cleanlab-2.6.5/cleanlab/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12093 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/models/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12449 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/models/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91265 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/multiannotator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.736982 cleanlab-2.6.5/cleanlab/multilabel_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/multilabel_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/multilabel_classification/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17287 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/multilabel_classification/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/multilabel_classification/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.740982 cleanlab-2.6.5/cleanlab/object_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/object_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19629 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/object_detection/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49070 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/object_detection/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34427 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/object_detection/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30438 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/outlier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25824 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.740982 cleanlab-2.6.5/cleanlab/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39296 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/regression/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/regression/rank.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.740982 cleanlab-2.6.5/cleanlab/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/segmentation/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/segmentation/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14450 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/segmentation/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.740982 cleanlab-2.6.5/cleanlab/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/token_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/token_classification/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12231 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/token_classification/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13905 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/token_classification/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9447 2024-05-24 23:39:12.000000 cleanlab-2.6.5/cleanlab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 23:39:20.740982 cleanlab-2.6.5/cleanlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    63319 2024-05-24 23:39:20.000000 cleanlab-2.6.5/cleanlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-05-24 23:39:20.000000 cleanlab-2.6.5/cleanlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 23:39:20.000000 cleanlab-2.6.5/cleanlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-24 23:39:20.000000 cleanlab-2.6.5/cleanlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 23:39:20.000000 cleanlab-2.6.5/cleanlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-24 23:39:13.000000 cleanlab-2.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-24 23:39:20.740982 cleanlab-2.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-24 23:39:13.000000 cleanlab-2.6.5/setup.py
```

### Comparing `cleanlab-2.6.4/CODE_OF_CONDUCT.md` & `cleanlab-2.6.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/CONTRIBUTING.md` & `cleanlab-2.6.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/DEVELOPMENT.md` & `cleanlab-2.6.5/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/LICENSE` & `cleanlab-2.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/PKG-INFO` & `cleanlab-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab
-Version: 2.6.4
+Version: 2.6.5
 Summary: The standard package for data-centric AI, machine learning with label errors, and automatically finding and fixing dataset issues in Python.
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -701,16 +701,16 @@
 Provides-Extra: datalab
 Requires-Dist: datasets>=2.7.0; extra == "datalab"
 Provides-Extra: image
 Requires-Dist: datasets>=2.7.0; extra == "image"
 Requires-Dist: cleanvision>=0.3.6; extra == "image"
 Provides-Extra: all
 Requires-Dist: cleanvision>=0.3.6; extra == "all"
-Requires-Dist: datasets>=2.7.0; extra == "all"
 Requires-Dist: matplotlib>=3.5.1; extra == "all"
+Requires-Dist: datasets>=2.7.0; extra == "all"
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanlab_logo_open_source.png" width=60% height=60%>
 </p>
 
 
 cleanlab helps you **clean** data and **lab**els by automatically detecting issues in a ML dataset. To facilitate **machine learning with messy, real-world data**, this data-centric AI package uses your *existing* models to estimate dataset problems that can be fixed to train even *better* models.
@@ -729,17 +729,17 @@
 # cleanlab estimates the predictions you would have gotten if you had trained with *no* label issues.
 cl.predict(test_data)
 
 # A universal data-centric AI tool, cleanlab quantifies class-level issues and overall data quality, for any dataset.
 cleanlab.dataset.health_summary(labels, confident_joint=cl.confident_joint)
 ```
 
-Get started with: [tutorials](https://docs.cleanlab.ai/stable/tutorials/image.html), [documentation](https://docs.cleanlab.ai/), [examples](https://github.com/cleanlab/examples), and [blogs](https://cleanlab.ai/blog/).
+Get started with: [tutorials](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html), [documentation](https://docs.cleanlab.ai/), [examples](https://github.com/cleanlab/examples), and [blogs](https://cleanlab.ai/blog/).
 
- - Learn to run cleanlab on your data in 5 minutes for: [image](https://docs.cleanlab.ai/stable/tutorials/image.html), [text](https://docs.cleanlab.ai/stable/tutorials/datalab/text.html), [audio](https://docs.cleanlab.ai/stable/tutorials/audio.html), or [tabular](https://docs.cleanlab.ai/stable/tutorials/datalab/tabular.html) data.
+ - Learn to run cleanlab on your data in 5 minutes for: [image](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html), [text](https://docs.cleanlab.ai/stable/tutorials/datalab/text.html), [audio](https://docs.cleanlab.ai/stable/tutorials/datalab/audio.html), or [tabular](https://docs.cleanlab.ai/stable/tutorials/datalab/tabular.html) data.
 - Use cleanlab to automatically: [detect data issues (outliers, duplicates, label errors, etc)](https://docs.cleanlab.ai/stable/tutorials/datalab/datalab_quickstart.html), [train robust models](https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html), [infer consensus + annotator-quality for multi-annotator data](https://docs.cleanlab.ai/stable/tutorials/multiannotator.html), [suggest data to (re)label next (active learning)](https://github.com/cleanlab/examples/blob/master/active_learning_multiannotator/active_learning.ipynb). 
 
 
 [![pypi](https://img.shields.io/pypi/v/cleanlab.svg)](https://pypi.org/pypi/cleanlab/)
 [![os](https://img.shields.io/badge/platform-noarch-lightgrey)](https://pypi.org/pypi/cleanlab/)
 [![py\_versions](https://img.shields.io/badge/python-3.8%2B-blue)](https://pypi.org/pypi/cleanlab/)
 [![build\_status](https://github.com/cleanlab/cleanlab/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab/actions?query=workflow%3ACI)
@@ -843,15 +843,15 @@
 cl.predict(test_data)
 ```
 
 #### Want to see a working example? [Here’s a compliant PyTorch MNIST CNN class](https://github.com/cleanlab/cleanlab/blob/master/cleanlab/experimental/mnist_pytorch.py)
 
 More details are provided in documentation of [cleanlab.classification.CleanLearning](https://docs.cleanlab.ai/stable/cleanlab/classification.html).
 
-Note, some libraries exist to give you sklearn-compatibility for free. For PyTorch, check out the [skorch](https://skorch.readthedocs.io/) Python library which will wrap your PyTorch model into a sklearn-compatible model ([example](https://docs.cleanlab.ai/stable/tutorials/image.html)). For TensorFlow/Keras, check out our [Keras wrapper](https://docs.cleanlab.ai/stable/cleanlab/models/keras.html). Many libraries also already offer a special scikit-learn API, for example: [XGBoost](https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn) or [LightGBM](https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html).
+Note, some libraries exist to give you sklearn-compatibility for free. For PyTorch, check out the [skorch](https://skorch.readthedocs.io/) Python library which will wrap your PyTorch model into a sklearn-compatible model ([example](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html)). For TensorFlow/Keras, check out our [Keras wrapper](https://docs.cleanlab.ai/stable/cleanlab/models/keras.html). Many libraries also already offer a special scikit-learn API, for example: [XGBoost](https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn) or [LightGBM](https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html).
 
 <br/>
 </details>
 
 cleanlab is useful across a wide variety of Machine Learning tasks. Specific tasks this data-centric AI solution offers dedicated functionality for include:
 1. [Binary and multi-class classification](https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html)
 2. [Multi-label classification](https://docs.cleanlab.ai/stable/tutorials/multilabel_classification.html) (e.g. image/document tagging)
```

### Comparing `cleanlab-2.6.4/README.md` & `cleanlab-2.6.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 # cleanlab estimates the predictions you would have gotten if you had trained with *no* label issues.
 cl.predict(test_data)
 
 # A universal data-centric AI tool, cleanlab quantifies class-level issues and overall data quality, for any dataset.
 cleanlab.dataset.health_summary(labels, confident_joint=cl.confident_joint)
 ```
 
-Get started with: [tutorials](https://docs.cleanlab.ai/stable/tutorials/image.html), [documentation](https://docs.cleanlab.ai/), [examples](https://github.com/cleanlab/examples), and [blogs](https://cleanlab.ai/blog/).
+Get started with: [tutorials](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html), [documentation](https://docs.cleanlab.ai/), [examples](https://github.com/cleanlab/examples), and [blogs](https://cleanlab.ai/blog/).
 
- - Learn to run cleanlab on your data in 5 minutes for: [image](https://docs.cleanlab.ai/stable/tutorials/image.html), [text](https://docs.cleanlab.ai/stable/tutorials/datalab/text.html), [audio](https://docs.cleanlab.ai/stable/tutorials/audio.html), or [tabular](https://docs.cleanlab.ai/stable/tutorials/datalab/tabular.html) data.
+ - Learn to run cleanlab on your data in 5 minutes for: [image](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html), [text](https://docs.cleanlab.ai/stable/tutorials/datalab/text.html), [audio](https://docs.cleanlab.ai/stable/tutorials/datalab/audio.html), or [tabular](https://docs.cleanlab.ai/stable/tutorials/datalab/tabular.html) data.
 - Use cleanlab to automatically: [detect data issues (outliers, duplicates, label errors, etc)](https://docs.cleanlab.ai/stable/tutorials/datalab/datalab_quickstart.html), [train robust models](https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html), [infer consensus + annotator-quality for multi-annotator data](https://docs.cleanlab.ai/stable/tutorials/multiannotator.html), [suggest data to (re)label next (active learning)](https://github.com/cleanlab/examples/blob/master/active_learning_multiannotator/active_learning.ipynb). 
 
 
 [![pypi](https://img.shields.io/pypi/v/cleanlab.svg)](https://pypi.org/pypi/cleanlab/)
 [![os](https://img.shields.io/badge/platform-noarch-lightgrey)](https://pypi.org/pypi/cleanlab/)
 [![py\_versions](https://img.shields.io/badge/python-3.8%2B-blue)](https://pypi.org/pypi/cleanlab/)
 [![build\_status](https://github.com/cleanlab/cleanlab/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab/actions?query=workflow%3ACI)
@@ -133,15 +133,15 @@
 cl.predict(test_data)
 ```
 
 #### Want to see a working example? [Here’s a compliant PyTorch MNIST CNN class](https://github.com/cleanlab/cleanlab/blob/master/cleanlab/experimental/mnist_pytorch.py)
 
 More details are provided in documentation of [cleanlab.classification.CleanLearning](https://docs.cleanlab.ai/stable/cleanlab/classification.html).
 
-Note, some libraries exist to give you sklearn-compatibility for free. For PyTorch, check out the [skorch](https://skorch.readthedocs.io/) Python library which will wrap your PyTorch model into a sklearn-compatible model ([example](https://docs.cleanlab.ai/stable/tutorials/image.html)). For TensorFlow/Keras, check out our [Keras wrapper](https://docs.cleanlab.ai/stable/cleanlab/models/keras.html). Many libraries also already offer a special scikit-learn API, for example: [XGBoost](https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn) or [LightGBM](https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html).
+Note, some libraries exist to give you sklearn-compatibility for free. For PyTorch, check out the [skorch](https://skorch.readthedocs.io/) Python library which will wrap your PyTorch model into a sklearn-compatible model ([example](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html)). For TensorFlow/Keras, check out our [Keras wrapper](https://docs.cleanlab.ai/stable/cleanlab/models/keras.html). Many libraries also already offer a special scikit-learn API, for example: [XGBoost](https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn) or [LightGBM](https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html).
 
 <br/>
 </details>
 
 cleanlab is useful across a wide variety of Machine Learning tasks. Specific tasks this data-centric AI solution offers dedicated functionality for include:
 1. [Binary and multi-class classification](https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html)
 2. [Multi-label classification](https://docs.cleanlab.ai/stable/tutorials/multilabel_classification.html) (e.g. image/document tagging)
```

### Comparing `cleanlab-2.6.4/cleanlab/__init__.py` & `cleanlab-2.6.5/cleanlab/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/benchmarking/noise_generation.py` & `cleanlab-2.6.5/cleanlab/benchmarking/noise_generation.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/classification.py` & `cleanlab-2.6.5/cleanlab/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
         label_quality_scores_kwargs={},
         verbose=False,
         low_memory=False,
     ):
         self._default_clf = False
         if clf is None:
             # Use logistic regression if no classifier is provided.
-            clf = LogReg(multi_class="auto", solver="lbfgs")
+            clf = LogReg(solver="lbfgs")
             self._default_clf = True
 
         # Make sure the given classifier has the appropriate methods defined.
         if not hasattr(clf, "fit"):
             raise ValueError("The classifier (clf) must define a .fit() method.")
         if not hasattr(clf, "predict_proba"):
             raise ValueError("The classifier (clf) must define a .predict_proba() method.")
```

### Comparing `cleanlab-2.6.4/cleanlab/count.py` & `cleanlab-2.6.5/cleanlab/count.py`

 * *Files 1% similar despite different names*

```diff
@@ -892,15 +892,15 @@
 
     return py, noise_matrix, inv_noise_matrix, confident_joint
 
 
 def estimate_confident_joint_and_cv_pred_proba(
     X,
     labels,
-    clf=LogReg(multi_class="auto", solver="lbfgs"),
+    clf=LogReg(solver="lbfgs"),
     *,
     cv_n_folds=5,
     thresholds=None,
     seed=None,
     calibrate=True,
     clf_kwargs={},
     validation_func=None,
@@ -1074,15 +1074,15 @@
 
     return confident_joint, pred_probs
 
 
 def estimate_py_noise_matrices_and_cv_pred_proba(
     X,
     labels,
-    clf=LogReg(multi_class="auto", solver="lbfgs"),
+    clf=LogReg(solver="lbfgs"),
     *,
     cv_n_folds=5,
     thresholds=None,
     converge_latent_estimates=False,
     py_method="cnt",
     seed=None,
     clf_kwargs={},
@@ -1185,15 +1185,15 @@
 
     return py, noise_matrix, inv_noise_matrix, confident_joint, pred_probs
 
 
 def estimate_cv_predicted_probabilities(
     X,
     labels,
-    clf=LogReg(multi_class="auto", solver="lbfgs"),
+    clf=LogReg(solver="lbfgs"),
     *,
     cv_n_folds=5,
     seed=None,
     clf_kwargs={},
     validation_func=None,
 ) -> np.ndarray:
     """This function computes the out-of-sample predicted
@@ -1251,15 +1251,15 @@
         validation_func=validation_func,
     )[-1]
 
 
 def estimate_noise_matrices(
     X,
     labels,
-    clf=LogReg(multi_class="auto", solver="lbfgs"),
+    clf=LogReg(solver="lbfgs"),
     *,
     cv_n_folds=5,
     thresholds=None,
     converge_latent_estimates=True,
     seed=None,
     clf_kwargs={},
     validation_func=None,
```

### Comparing `cleanlab-2.6.4/cleanlab/data_valuation.py` & `cleanlab-2.6.5/cleanlab/data_valuation.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,20 @@
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 """
 Methods for quantifying the value of each data point in a Machine Learning dataset.
 Data Valuation helps us assess individual training data points' contributions to a ML model's predictive performance.
 """
 
 
-from typing import Callable, Optional, Union, cast
+from typing import Callable, Optional, Union
 
 import numpy as np
 from scipy.sparse import csr_matrix
-from scipy.spatial.distance import euclidean
-from sklearn.neighbors import NearestNeighbors
-from sklearn.exceptions import NotFittedError
-from sklearn.utils.validation import check_is_fitted
+
+from cleanlab.internal.neighbor.knn_graph import create_knn_graph_and_index
 
 
 def _knn_shapley_score(knn_graph: csr_matrix, labels: np.ndarray, k: int) -> np.ndarray:
     """Compute the Shapley values of data points based on a knn graph."""
     N = labels.shape[0]
     scores = np.zeros((N, N))
     dist = knn_graph.indices.reshape(N, -1)
@@ -41,37 +39,14 @@
         s[idx[k - 1]] = float(ans[k - 1] == y)
         ans_matches = (ans == y).flatten()
         for j in range(k - 2, -1, -1):
             s[idx[j]] = s[idx[j + 1]] + float(int(ans_matches[j]) - int(ans_matches[j + 1]))
     return 0.5 * (np.mean(scores / k, axis=0) + 1)
 
 
-def _process_knn_graph_from_features(
-    features: np.ndarray, metric: Optional[Union[str, Callable]], k: int = 10
-) -> csr_matrix:
-    """Calculate the knn graph from the features if it is not provided in the kwargs."""
-    if k > len(features):  # Ensure number of neighbors less than number of examples
-        raise ValueError(
-            f"Number of nearest neighbors k={k} cannot exceed the number of examples N={len(features)} passed into the estimator (knn)."
-        )
-    if metric == None:
-        metric = (
-            "cosine"
-            if features.shape[1] > 3
-            else "euclidean" if features.shape[0] > 100 else euclidean
-        )
-    knn = NearestNeighbors(n_neighbors=k, metric=metric).fit(features)
-    knn_graph = knn.kneighbors_graph(mode="distance")
-    try:
-        check_is_fitted(knn)
-    except NotFittedError:
-        knn.fit(features)
-    return knn_graph
-
-
 def data_shapley_knn(
     labels: np.ndarray,
     *,
     features: Optional[np.ndarray] = None,
     knn_graph: Optional[csr_matrix] = None,
     metric: Optional[Union[str, Callable]] = None,
     k: int = 10,
@@ -131,10 +106,11 @@
     >>> features = np.array([[0, 1, 2, 3, 4]]).T
     >>> data_shapley_knn(labels=labels, features=features, k=4)
     array([0.55 , 0.525, 0.55 , 0.525, 0.55 ])
     """
     if knn_graph is None and features is None:
         raise ValueError("Either knn_graph or features must be provided.")
 
+    # Use provided knn_graph or compute it from features
     if knn_graph is None:
-        knn_graph = _process_knn_graph_from_features(cast(np.ndarray, features), metric, k)
+        knn_graph, _ = create_knn_graph_and_index(features, n_neighbors=k, metric=metric)
     return _knn_shapley_score(knn_graph, labels, k)
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/datalab.py` & `cleanlab-2.6.5/cleanlab/datalab/datalab.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/adapter/imagelab.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/adapter/imagelab.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/data.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/data.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/data_issues.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/data_issues.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/display.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/display.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/helper_factory.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/helper_factory.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_finder.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,31 +37,33 @@
 
 from cleanlab.datalab.internal.issue_manager_factory import (
     _IssueManagerFactory,
     list_default_issue_types,
 )
 from cleanlab.datalab.internal.model_outputs import (
     MultiClassPredProbs,
-    RegressionPredictions,
     MultiLabelPredProbs,
+    RegressionPredictions,
 )
 from cleanlab.datalab.internal.task import Task
 
 if TYPE_CHECKING:  # pragma: no cover
-    import numpy.typing as npt
     from typing import Callable
 
+    import numpy.typing as npt
+
     from cleanlab.datalab.datalab import Datalab
 
 
 _CLASSIFICATION_ARGS_DICT = {
     "label": ["pred_probs", "features"],
     "outlier": ["pred_probs", "features", "knn_graph"],
     "near_duplicate": ["features", "knn_graph"],
     "non_iid": ["pred_probs", "features", "knn_graph"],
+    # The underperforming_group issue type requires a pair of inputs: (pred_probs, <any_of_the_other_three>)
     "underperforming_group": ["pred_probs", "features", "knn_graph", "cluster_ids"],
     "data_valuation": ["features", "knn_graph"],
     "class_imbalance": [],
     "null": ["features"],
 }
 _REGRESSION_ARGS_DICT = {
     "label": ["features", "predictions"],
@@ -478,8 +480,20 @@
             "class_imbalance" in issue_types_copy
             and not self.datalab.has_labels
             and self.task == Task.CLASSIFICATION
         )
         if drop_class_imbalance_check:
             issue_types_copy.pop("class_imbalance")
 
+        required_pairs_for_underperforming_group = [
+            ("pred_probs", "features"),
+            ("pred_probs", "knn_graph"),
+            ("pred_probs", "cluster_ids"),
+        ]
+        drop_underperforming_group_check = "underperforming_group" in issue_types_copy and not any(
+            all(key in kwargs and kwargs.get(key) is not None for key in pair)
+            for pair in required_pairs_for_underperforming_group
+        )
+        if drop_underperforming_group_check:
+            issue_types_copy.pop("underperforming_group")
+
         return issue_types_copy
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/data_valuation.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/data_valuation.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,27 +21,23 @@
     Callable,
     ClassVar,
     Dict,
     List,
     Optional,
     Union,
 )
-import warnings
 
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
-from scipy.spatial.distance import euclidean
-from sklearn.exceptions import NotFittedError
-from sklearn.neighbors import NearestNeighbors
-from sklearn.utils.validation import check_is_fitted
 
 from cleanlab.data_valuation import data_shapley_knn
 from cleanlab.datalab.internal.issue_manager import IssueManager
+from cleanlab.internal.neighbor.knn_graph import create_knn_graph_and_index
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
     import pandas as pd
     from cleanlab.datalab.datalab import Datalab
 
 
@@ -135,41 +131,19 @@
         if not isinstance(labels, np.ndarray):
             error_msg = (
                 f"Expected labels to be a numpy array of shape (n_samples,) to use with DataValuationIssueManager, "
                 f"but got {type(labels)} instead."
             )
             raise TypeError(error_msg)
         if knn_graph is None or metric_changes:
-            if features is None:
-                raise ValueError(
-                    "If a knn_graph is not provided, features must be provided to fit a new knn."
-                )
-            if self.metric is None:
-                self.metric = (
-                    "cosine"
-                    if features.shape[1] > 3
-                    else "euclidean" if features.shape[0] > 100 else euclidean
-                )
-            knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric).fit(features)
-
-            if self.metric and self.metric != knn.metric:
-                warnings.warn(
-                    f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
-                    "Most likely an existing NearestNeighbors object was passed in, but a different "
-                    "metric was specified."
-                )
+            knn_graph, knn = create_knn_graph_and_index(
+                features, n_neighbors=self.k, metric=self.metric
+            )
             self.metric = knn.metric
 
-            try:
-                check_is_fitted(knn)
-            except NotFittedError:
-                knn.fit(features)
-
-            knn_graph = knn.kneighbors_graph(mode="distance")
-
         scores = data_shapley_knn(labels, knn_graph=knn_graph, k=self.k)
 
         self.issues = pd.DataFrame(
             {
                 f"is_{self.issue_name}_issue": scores < self.threshold,
                 self.issue_score_key: scores,
             },
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/duplicate.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/duplicate.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, List, Optional, Union
 import warnings
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
-from scipy.spatial.distance import euclidean
-from sklearn.neighbors import NearestNeighbors
-from sklearn.exceptions import NotFittedError
-from sklearn.utils.validation import check_is_fitted
+
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
+from cleanlab.internal.neighbor.knn_graph import create_knn_graph_and_index
 from cleanlab.internal.constants import EPSILON
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
     from cleanlab.datalab.datalab import Datalab
 
 
@@ -72,40 +70,18 @@
         **kwargs,
     ) -> None:
         knn_graph = self._process_knn_graph_from_inputs(kwargs)
         old_knn_metric = self.datalab.get_info("statistics").get("knn_metric")
         metric_changes = self.metric and self.metric != old_knn_metric
 
         if knn_graph is None or metric_changes:
-            if features is None:
-                raise ValueError(
-                    "If a knn_graph is not provided, features must be provided to fit a new knn."
-                )
-            if self.metric is None:
-                self.metric = (
-                    "cosine"
-                    if features.shape[1] > 3
-                    else "euclidean" if features.shape[0] > 100 else euclidean
-                )
-            knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric)
-
-            if self.metric and self.metric != knn.metric:
-                warnings.warn(
-                    f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
-                    "Most likely an existing NearestNeighbors object was passed in, but a different "
-                    "metric was specified."
-                )
+            knn_graph, knn = create_knn_graph_and_index(
+                features, n_neighbors=self.k, metric=self.metric
+            )
             self.metric = knn.metric
-
-            try:
-                check_is_fitted(knn)
-            except NotFittedError:
-                knn.fit(features)
-
-            knn_graph = knn.kneighbors_graph(mode="distance")
         N = knn_graph.shape[0]
         nn_distances = knn_graph.data.reshape(N, -1)[:, 0]
         median_nn_distance = max(np.median(nn_distances), EPSILON)  # avoid threshold = 0
         self.near_duplicate_sets = self._neighbors_within_radius(
             knn_graph, self.threshold, median_nn_distance
         )
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/imbalance.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/imbalance.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/issue_manager.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/issue_manager.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/label.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/label.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/multilabel/label.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/multilabel/label.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/noniid.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/noniid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, Optional, Union, cast
-import warnings
 import itertools
 
 from scipy.stats import gaussian_kde
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
-from scipy.spatial.distance import euclidean
-from sklearn.neighbors import NearestNeighbors
-from sklearn.exceptions import NotFittedError
-from sklearn.utils.validation import check_is_fitted
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
+from cleanlab.internal.neighbor.knn_graph import create_knn_graph_and_index
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
     from cleanlab.datalab.datalab import Datalab
 
 
 def simplified_kolmogorov_smirnov_test(
@@ -162,91 +158,35 @@
         if pred_probs is not None:
             return pred_probs
 
         raise ValueError(
             "If a knn_graph is not provided, either 'features' or 'pred_probs' must be provided to fit a new knn."
         )
 
-    def _setup_knn(
-        self,
-        features: Optional[npt.NDArray],
-        pred_probs: Optional[np.ndarray],
-        knn_graph: Optional[csr_matrix],
-        metric_changes: bool,
-    ) -> Optional[NearestNeighbors]:
-        """
-        Selects features (or pred_probs if features are None) and sets up a NearestNeighbors object if needed.
-
-        Parameters
-        ----------
-        features :
-            Original feature array or None.
-
-        pred_probs :
-            Predicted probabilities array or None.
-
-        knn_graph :
-            A precomputed KNN-graph stored in a csr_matrix or None. If None, a new NearestNeighbors object will be created.
-
-        metric_changes :
-            Whether the metric used to compute the KNN-graph has changed.
-            This is a result of comparing the metric of a pre-existing KNN-graph and the metric specified by the user.
-
-        Returns
-        -------
-        knn :
-            A NearestNeighbors object or None.
-        """
-        if features is None and pred_probs is not None:
-            self._skip_storing_knn_graph_for_pred_probs = True
-
-        if knn_graph is not None and not metric_changes:
-            return None
-        features_to_use = self._determine_features(features, pred_probs)
-
-        if self.metric is None:
-            self.metric = (
-                "cosine"
-                if features_to_use.shape[1] > 3
-                else "euclidean" if features_to_use.shape[0] > 100 else euclidean
-            )
-
-        knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric)
-
-        if self.metric != knn.metric:
-            warnings.warn(
-                f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
-                "Most likely an existing NearestNeighbors object was passed in, but a different "
-                "metric was specified."
-            )
-        self.metric = knn.metric
-
-        try:
-            check_is_fitted(knn)
-        except NotFittedError:
-            knn.fit(features_to_use)
-
-        return knn
-
     def find_issues(
         self,
         features: Optional[npt.NDArray] = None,
         pred_probs: Optional[np.ndarray] = None,
         **kwargs,
     ) -> None:
         knn_graph = self._process_knn_graph_from_inputs(kwargs)
         old_knn_metric = self.datalab.get_info("statistics").get("knn_metric")
         metric_changes = bool(self.metric and self.metric != old_knn_metric)
-        knn = self._setup_knn(features, pred_probs, knn_graph, metric_changes)
 
         if knn_graph is None or metric_changes:
-            self.neighbor_index_choices = self._get_neighbors(knn=knn)
-        else:
-            self._skip_storing_knn_graph_for_pred_probs = False
-            self.neighbor_index_choices = self._get_neighbors(knn_graph=knn_graph)
+            if features is None and pred_probs is not None:
+                self._skip_storing_knn_graph_for_pred_probs = True
+
+            features_to_use = self._determine_features(features, pred_probs)
+            knn_graph, knn = create_knn_graph_and_index(
+                features=features_to_use, n_neighbors=self.k, metric=self.metric
+            )
+            self.metric = knn.metric  # Update the metric to the one used in the KNN object.
+
+        self.neighbor_index_choices = self._get_neighbors(knn_graph=knn_graph)
 
         self.num_neighbors = self.k
 
         indices = np.arange(self.N)
         self.neighbor_index_distances = np.abs(indices.reshape(-1, 1) - self.neighbor_index_choices)
 
         self.statistics = self._get_statistics(self.neighbor_index_distances)
@@ -262,17 +202,15 @@
                 f"is_{self.issue_name}_issue": issue_mask,
                 self.issue_score_key: scores,
             },
         )
 
         self.summary = self.make_summary(score=self.p_value)
 
-        if knn_graph is None:
-            self.info = self.collect_info(knn=knn)
-        self.info = self.collect_info(knn_graph=knn_graph, knn=knn)
+        self.info = self.collect_info(knn_graph=knn_graph)
 
     def _process_knn_graph_from_inputs(self, kwargs: Dict[str, Any]) -> Union[csr_matrix, None]:
         """Determine if a knn_graph is provided in the kwargs or if one is already stored in the associated Datalab instance."""
         knn_graph_kwargs: Optional[csr_matrix] = kwargs.get("knn_graph", None)
         knn_graph_stats = self.datalab.get_info("statistics").get("weighted_knn_graph", None)
 
         knn_graph: Optional[csr_matrix] = None
@@ -288,30 +226,24 @@
 
         if need_to_recompute_knn:
             # If the provided knn graph is insufficient, then we need to recompute the knn graph
             # with the provided features
             knn_graph = None
         return knn_graph
 
-    def collect_info(
-        self, knn_graph: Optional[csr_matrix] = None, knn: Optional[NearestNeighbors] = None
-    ) -> dict:
+    def collect_info(self, knn_graph: csr_matrix) -> dict:
         issues_dict = {
             "p-value": self.p_value,
         }
 
         params_dict = {
             "metric": self.metric,
             "k": self.k,
         }
-        if knn_graph is None:
-            assert knn is not None, "If knn_graph is None, knn must be provided."
-            knn_graph = knn.kneighbors_graph(mode="distance")  # type: ignore[union-attr]
 
-        assert knn_graph is not None, "knn_graph must be provided or computed."
         statistics_dict = self._build_statistics_dictionary(knn_graph=knn_graph)
 
         info_dict = {
             **issues_dict,
             **params_dict,  # type: ignore[arg-type]
             **statistics_dict,  # type: ignore[arg-type]
         }
@@ -484,30 +416,21 @@
         reverse = N - indices
         normalizer = np.where(indices > reverse, indices, reverse)
 
         scores = stats / normalizer
         scores = np.tanh(-1 * scores) + 1
         return scores
 
-    def _get_neighbors(
-        self, knn: Optional[NearestNeighbors] = None, knn_graph: Optional[csr_matrix] = None
-    ) -> np.ndarray:
+    def _get_neighbors(self, knn_graph: csr_matrix) -> np.ndarray:
         """
-        Given a fitted knn object or a knn graph, returns an (N, k) array in
+        Given a knn graph, returns an (N, k) array in
         which j is in A[i] if item i and j are nearest neighbors.
         """
-        if knn_graph is not None:
-            N = knn_graph.shape[0]
-            kneighbors = knn_graph.indices.reshape(N, -1)
-        elif knn is not None:
-            _, kneighbors = knn.kneighbors()
-            N = kneighbors.shape[0]
-        else:
-            raise ValueError("Must provide either knn or knn_graph")
-        self.N = N
+        self.N = knn_graph.shape[0]
+        kneighbors = knn_graph.indices.reshape(self.N, -1)
         return kneighbors
 
     def _get_statistics(
         self,
         neighbor_index_distances,
     ) -> dict[str, float]:
         neighbor_index_distances = neighbor_index_distances.flatten()
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/null.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/null.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from collections import Counter
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, List
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, List, Optional
 
 import numpy as np
 import pandas as pd
-from numpy import ndarray
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
 
 
@@ -30,20 +29,22 @@
     verbosity_levels = {
         0: [],
         1: [],
         2: ["most_common_issue"],
     }
 
     @staticmethod
-    def _calculate_null_issues(features: npt.NDArray) -> tuple[ndarray, ndarray, Any]:
+    def _calculate_null_issues(
+        features: npt.NDArray[Any],
+    ) -> tuple[npt.NDArray[np.bool_], npt.NDArray[np.float64], npt.NDArray[np.bool_]]:
         """Tracks the number of null values in each row of a feature array,
         computes quality scores based on the fraction of null values in each row,
         and returns a boolean array indicating whether each row only has null values."""
         cols = features.shape[1]
-        null_tracker = np.isnan(features)
+        null_tracker = pd.isna(features)
         non_null_count = cols - null_tracker.sum(axis=1)
         scores = non_null_count / cols
         is_null_issue = non_null_count == 0
         return is_null_issue, scores, null_tracker
 
     def find_issues(
         self,
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/outlier.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/outlier.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from scipy.sparse import csr_matrix
 from scipy.stats import iqr
 import numpy as np
 import pandas as pd
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
+from cleanlab.internal.neighbor.knn_graph import construct_knn_graph_from_index
 from cleanlab.outlier import OutOfDistribution, transform_distances_to_scores
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
     from sklearn.neighbors import NearestNeighbors
     from cleanlab.datalab.datalab import Datalab
 
@@ -128,15 +129,16 @@
             raise ValueError(f"Either features pred_probs must be provided.")
 
         if features is not None or knn_graph is not None:
             if knn_graph is None:
                 assert (
                     features is not None
                 ), "features must be provided so that we can compute the knn graph."
-                knn_graph = self._process_knn_graph_from_features(kwargs)
+                knn_graph = self._process_knn_graph_from_features(features, kwargs)
+
             distances = knn_graph.data.reshape(knn_graph.shape[0], -1)
 
             assert isinstance(distances, np.ndarray)
             (
                 self.threshold,
                 issue_threshold,  # Useful info for detecting issues in test data
                 is_issue_column,
@@ -201,29 +203,29 @@
             iqr_scale = 1 / threshold - 1 if threshold != 0 else np.inf
             issue_threshold = q3_distance + iqr_scale * iqr(avg_distances)
             return float(issue_threshold)
 
         issue_threshold = compute_issue_threshold(avg_distances, threshold)
         return threshold, issue_threshold, avg_distances > issue_threshold
 
-    def _process_knn_graph_from_features(self, kwargs: Dict) -> csr_matrix:
+    def _process_knn_graph_from_features(self, features: np.ndarray, kwargs: Dict) -> csr_matrix:
         # Check if the weighted knn graph exists in info
         knn_graph = self.datalab.get_info("statistics").get("weighted_knn_graph", None)
 
         # Used to check if the knn graph needs to be recomputed, already set in the knn object
         k: int = 0
         if knn_graph is not None:
             k = knn_graph.nnz // knn_graph.shape[0]
 
         knn: NearestNeighbors = self.ood.params["knn"]  # type: ignore
         if kwargs.get("knn", None) is not None or knn.n_neighbors > k:  # type: ignore[union-attr]
             # If the pre-existing knn graph has fewer neighbors than the knn object,
             # then we need to recompute the knn graph
             assert knn == self.ood.params["knn"]  # type: ignore[union-attr]
-            knn_graph = knn.kneighbors_graph(mode="distance")  # type: ignore[union-attr]
+            knn_graph = construct_knn_graph_from_index(knn, correction_features=features)
             self._metric = knn.metric  # type: ignore[union-attr]
 
         return knn_graph
 
     def collect_info(
         self,
         *,
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/regression/label.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/regression/label.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager/underperforming_group.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager/underperforming_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,18 @@
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, Optional, Union, Tuple
 import warnings
 import inspect
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
-from scipy.spatial.distance import euclidean
-from sklearn.neighbors import NearestNeighbors
-from sklearn.exceptions import NotFittedError
-from sklearn.utils.validation import check_is_fitted
 from sklearn.cluster import DBSCAN
 
 from cleanlab.datalab.internal.issue_manager import IssueManager
+from cleanlab.internal.neighbor.knn_graph import create_knn_graph_and_index
 from cleanlab.rank import get_self_confidence_for_each_label
 
 if TYPE_CHECKING:  # pragma: no cover
     import numpy.typing as npt
     from cleanlab.datalab.datalab import Datalab
 
 
@@ -149,39 +146,18 @@
         self, features: Optional[npt.NDArray], find_issues_kwargs: Dict[str, Any]
     ) -> csr_matrix:
         knn_graph = self._process_knn_graph_from_inputs(find_issues_kwargs)
         old_knn_metric = self.datalab.get_info("statistics").get("knn_metric")
         metric_changes = self.metric and self.metric != old_knn_metric
 
         if knn_graph is None or metric_changes:
-            if features is None:
-                raise ValueError(
-                    "If a knn_graph is not provided, features must be provided to fit a new knn."
-                )
-            if self.metric is None:
-                self.metric = (
-                    "cosine"
-                    if features.shape[1] > 3
-                    else "euclidean" if features.shape[0] > 100 else euclidean
-                )
-            knn = NearestNeighbors(n_neighbors=self.k, metric=self.metric)
-
-            if self.metric and self.metric != knn.metric:
-                warnings.warn(
-                    f"Metric {self.metric} does not match metric {knn.metric} used to fit knn. "
-                    "Most likely an existing NearestNeighbors object was passed in, but a different "
-                    "metric was specified."
-                )
+            knn_graph, knn = create_knn_graph_and_index(
+                features, n_neighbors=self.k, metric=self.metric
+            )
             self.metric = knn.metric
-
-            try:
-                check_is_fitted(knn)
-            except NotFittedError:
-                knn.fit(features)
-            knn_graph = knn.kneighbors_graph(mode="distance")
         return knn_graph
 
     def perform_clustering(self, knn_graph: csr_matrix) -> npt.NDArray[np.int_]:
         """Perform clustering of datapoints using a knn graph as distance matrix.
 
         Args:
             knn_graph (csr_matrix): Sparse Distance Matrix.
```

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/issue_manager_factory.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/issue_manager_factory.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/model_outputs.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/model_outputs.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/report.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/report.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/serialize.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/serialize.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/datalab/internal/task.py` & `cleanlab-2.6.5/cleanlab/datalab/internal/task.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/dataset.py` & `cleanlab-2.6.5/cleanlab/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/experimental/cifar_cnn.py` & `cleanlab-2.6.5/cleanlab/experimental/cifar_cnn.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/experimental/coteaching.py` & `cleanlab-2.6.5/cleanlab/experimental/coteaching.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/experimental/datalab/data_monitor.py` & `cleanlab-2.6.5/cleanlab/experimental/datalab/data_monitor.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/experimental/label_issues_batched.py` & `cleanlab-2.6.5/cleanlab/experimental/label_issues_batched.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/experimental/mnist_pytorch.py` & `cleanlab-2.6.5/cleanlab/experimental/mnist_pytorch.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/experimental/span_classification.py` & `cleanlab-2.6.5/cleanlab/experimental/span_classification.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/filter.py` & `cleanlab-2.6.5/cleanlab/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/constants.py` & `cleanlab-2.6.5/cleanlab/internal/constants.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/label_quality_utils.py` & `cleanlab-2.6.5/cleanlab/internal/label_quality_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/latent_algebra.py` & `cleanlab-2.6.5/cleanlab/internal/latent_algebra.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/multiannotator_utils.py` & `cleanlab-2.6.5/cleanlab/internal/multiannotator_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Helper methods used internally in cleanlab.multiannotator
 """
 
-from cleanlab.typing import LabelLike
-from typing import Optional, Tuple
 import warnings
+from typing import Optional, Tuple
+
 import numpy as np
 import pandas as pd
-from cleanlab.internal.validation import assert_valid_class_labels
+
 from cleanlab.internal.numerics import softmax
 from cleanlab.internal.util import get_num_classes, value_counts
+from cleanlab.internal.validation import assert_valid_class_labels
+from cleanlab.typing import LabelLike
 
 SMALL_CONST = 1e-30
 
 
 def assert_valid_inputs_multiannotator(
     labels_multiannotator: np.ndarray,
     pred_probs: Optional[np.ndarray] = None,
@@ -85,19 +87,18 @@
             raise ValueError(
                 "Each example only has one label, collapse the labels into a 1-D array and use "
                 "cleanlab.rank.get_label_quality_scores instead"
             )
 
         # Raise warning if no examples with 2 or more annotators agree
         # TODO: might shift this later in the code to avoid extra compute
-        if np.apply_along_axis(
-            lambda s: np.array_equal(np.unique(s[~np.isnan(s)]), s[~np.isnan(s)]),
-            axis=1,
-            arr=labels_multiannotator,
-        ).all():
+        has_agreement = np.zeros(labels_multiannotator.shape[0], dtype=bool)
+        for i in np.unique(labels_multiannotator):
+            has_agreement |= (labels_multiannotator == i).sum(axis=1) > 1
+        if not has_agreement.any():
             warnings.warn("Annotators do not agree on any example. Check input data.")
 
     # Check labels
     all_labels_flatten = labels_multiannotator.ravel()
     all_labels_flatten = all_labels_flatten[~np.isnan(all_labels_flatten)]
     assert_valid_class_labels(all_labels_flatten, allow_one_class=True)
```

### Comparing `cleanlab-2.6.4/cleanlab/internal/multilabel_scorer.py` & `cleanlab-2.6.5/cleanlab/internal/multilabel_scorer.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/multilabel_utils.py` & `cleanlab-2.6.5/cleanlab/internal/multilabel_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/numerics.py` & `cleanlab-2.6.5/cleanlab/internal/numerics.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/object_detection_utils.py` & `cleanlab-2.6.5/cleanlab/internal/object_detection_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/outlier.py` & `cleanlab-2.6.5/cleanlab/internal/outlier.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/regression_utils.py` & `cleanlab-2.6.5/cleanlab/internal/regression_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/segmentation_utils.py` & `cleanlab-2.6.5/cleanlab/internal/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/token_classification_utils.py` & `cleanlab-2.6.5/cleanlab/internal/token_classification_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/internal/util.py` & `cleanlab-2.6.5/cleanlab/internal/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 """
 Ancillary helper methods used internally throughout this package; mostly related to Confident Learning algorithms.
 """
 
 import warnings
+from typing import Optional, Tuple, Union
+
 import numpy as np
 import pandas as pd
-from typing import Union, Tuple
 
-from cleanlab.typing import DatasetLike, LabelLike
-from cleanlab.internal.validation import labels_to_array
 from cleanlab.internal.constants import FLOATING_POINT_COMPARISON, TINY_VALUE
+from cleanlab.internal.validation import labels_to_array
+from cleanlab.typing import DatasetLike, LabelLike
 
 
 def remove_noise_from_class(noise_matrix, class_without_noise) -> np.ndarray:
     """A helper function in the setting of PU learning.
     Sets all P(label=class_without_noise|true_label=any_other_class) = 0
     in noise_matrix for pulearning setting, where we have
     generalized the positive class in PU learning to be any
@@ -134,15 +135,15 @@
     x = vectorized_clip(x)  # Clip all values (efficiently)
     x = (
         x * prev_sum / np.clip(float(sum(x)), a_min=TINY_VALUE, a_max=None)
     )  # Re-normalized values to sum to previous sum
     return x
 
 
-def value_counts(x, *, num_classes=None, multi_label=False) -> np.ndarray:
+def value_counts(x, *, num_classes: Optional[int] = None, multi_label=False) -> np.ndarray:
     """Returns an np.ndarray of shape (K, 1), with the
     value counts for every unique item in the labels list/array,
     where K is the number of unique entries in labels.
 
     Works for both single-labeled and multi-labeled data.
 
     Parameters
@@ -169,25 +170,35 @@
       not the number of examples. So, the calibrated `confident_joint` will sum
       to the number of total labels."""
 
     # Efficient method if x is pd.Series, np.ndarray, or list
     if multi_label:
         x = [z for lst in x for z in lst]  # Flatten
     unique_classes, counts = np.unique(x, return_counts=True)
+
+    # Early exit if num_classes is not provided or redundant
     if num_classes is None or num_classes == len(unique_classes):
         return counts
+
     # Else, there are missing classes
-    if num_classes <= max(unique_classes):
-        raise ValueError(f"Required: num_classes > max(x), but {num_classes} <= {max(x)}.")
+    labels_are_integers = np.issubdtype(np.array(x).dtype, np.integer)
+    if labels_are_integers and num_classes <= np.max(unique_classes):
+        raise ValueError(f"Required: num_classes > max(x), but {num_classes} <= {np.max(x)}.")
+
     # Add zero counts for all missing classes in [0, 1,..., num_classes-1]
-    # multi_label=False regardless because x was flattened.
-    missing_classes = get_missing_classes(x, num_classes=num_classes, multi_label=False)
-    missing_counts = [(z, 0) for z in missing_classes]
+    total_counts = np.zeros(num_classes, dtype=int)
+    # Fill in counts for classes that are present.
+    # If labels are integers, unique_classes can be used directly as indices to place counts
+    # into the correct positions in total_counts array.
+    # If labels are strings, use a slice to fill counts sequentially since strings do not map to indices.
+    count_ids = unique_classes if labels_are_integers else slice(len(unique_classes))
+    total_counts[count_ids] = counts
+
     # Return counts with zeros for all missing classes.
-    return np.array(list(zip(*sorted(list(zip(unique_classes, counts)) + missing_counts)))[1])
+    return total_counts
 
 
 def value_counts_fill_missing_classes(x, num_classes, *, multi_label=False) -> np.ndarray:
     """Same as ``internal.util.value_counts`` but requires that num_classes is provided and
     always fills missing classes with zero counts.
 
     See ``internal.util.value_counts`` for parameter docstrings."""
@@ -576,17 +587,15 @@
     -------
     Tuple (pre_X, buffer_size) where:
       pre_X : Dataset that was previously transformed to get ShuffleDataset (or None),
       buffer_size : int `buffer_size` previously used in ShuffleDataset,
         or ``len(pre_X)`` if buffer_size cannot be determined, or None if no ShuffleDataset found.
     """
     try:
-        from tensorflow.python.data.ops.dataset_ops import (
-            ShuffleDataset,
-        )
+        from tensorflow.python.data.ops.dataset_ops import ShuffleDataset
 
         X_inputs = [X]
         while len(X_inputs) == 1:
             pre_X = X_inputs[0]
             if isinstance(pre_X, ShuffleDataset):
                 buffer_size = len(pre_X)
                 if hasattr(pre_X, "_buffer_size"):
```

### Comparing `cleanlab-2.6.4/cleanlab/internal/validation.py` & `cleanlab-2.6.5/cleanlab/internal/validation.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/models/fasttext.py` & `cleanlab-2.6.5/cleanlab/models/fasttext.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/models/keras.py` & `cleanlab-2.6.5/cleanlab/models/keras.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/multiannotator.py` & `cleanlab-2.6.5/cleanlab/multiannotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,30 +38,29 @@
 The algorithms to compute these active learning scores are described in `the ActiveLab paper <https://arxiv.org/abs/2301.11856>`_.
 
 Each of the main functions in this module utilizes any trained classifier model.
 Variants of these functions are provided for settings where you have trained an ensemble of multiple models.
 """
 
 import warnings
+from typing import Any, Dict, List, Optional, Tuple, Union
+
 import numpy as np
 import pandas as pd
 
-from typing import List, Dict, Any, Union, Tuple, Optional
-
-from cleanlab.rank import get_label_quality_scores
-from cleanlab.internal.util import get_num_classes, value_counts
 from cleanlab.internal.constants import CLIPPING_LOWER_BOUND
-
 from cleanlab.internal.multiannotator_utils import (
     assert_valid_inputs_multiannotator,
     assert_valid_pred_probs,
     check_consensus_label_classes,
     find_best_temp_scaler,
     temp_scale_pred_probs,
 )
+from cleanlab.internal.util import get_num_classes, value_counts
+from cleanlab.rank import get_label_quality_scores
 
 
 def get_label_quality_multiannotator(
     labels_multiannotator: Union[pd.DataFrame, np.ndarray],
     pred_probs: np.ndarray,
     *,
     consensus_method: Union[str, List[str]] = "best_quality",
@@ -957,41 +956,46 @@
         )
 
     if pred_probs is not None:
         num_classes = pred_probs.shape[1]
     else:
         num_classes = int(np.nanmax(labels_multiannotator) + 1)
 
-    def get_labels_mode(label_count, num_classes):
-        max_count_idx = np.where(label_count == np.nanmax(label_count))[0].astype(float)
-        return np.pad(
-            max_count_idx, (0, num_classes - len(max_count_idx)), "constant", constant_values=np.NaN
-        )
+    array_idx = np.arange(labels_multiannotator.shape[0])
+    label_count = np.zeros((labels_multiannotator.shape[0], num_classes))
+    for i in range(labels_multiannotator.shape[1]):
+        not_nan_mask = ~np.isnan(labels_multiannotator[:, i])
+        # Get the indexes where the label is not missing for the annotator i as int.
+        label_index = labels_multiannotator[not_nan_mask, i].astype(int)
+        # Increase the counts of those labels by 1.
+        label_count[array_idx[not_nan_mask], label_index] += 1
+
+    mode_labels_multiannotator = np.full(label_count.shape, np.nan)
+    modes_mask = label_count == np.max(label_count, axis=1).reshape(-1, 1)
+    insert_index = np.zeros(modes_mask.shape[0], dtype=int)
+    for i in range(modes_mask.shape[1]):
+        mode_index = np.where(modes_mask[:, i])[0]
+        mode_labels_multiannotator[mode_index, insert_index[mode_index]] = i
+        insert_index[mode_index] += 1
 
     majority_vote_label = np.full(len(labels_multiannotator), np.nan)
-    label_count = np.apply_along_axis(
-        lambda s: np.bincount(s[~np.isnan(s)].astype(int), minlength=num_classes),
-        axis=1,
-        arr=labels_multiannotator,
-    )
-    mode_labels_multiannotator = np.apply_along_axis(
-        get_labels_mode, axis=1, arr=label_count, num_classes=num_classes
-    )
-
-    nontied_idx = []
-    tied_idx = dict()
+    label_mode_count = (~np.isnan(mode_labels_multiannotator)).sum(axis=1)
 
     # obtaining consensus using annotator majority vote
-    for idx, label_mode in enumerate(mode_labels_multiannotator):
-        label_mode = label_mode[~np.isnan(label_mode)].astype(int)
-        if len(label_mode) == 1:
-            majority_vote_label[idx] = label_mode[0]
-            nontied_idx.append(idx)
-        else:
-            tied_idx[idx] = label_mode
+    mode_count_one_mask = label_mode_count == 1
+    majority_vote_label[mode_count_one_mask] = mode_labels_multiannotator[mode_count_one_mask, 0]
+    nontied_idx = array_idx[mode_count_one_mask]
+    tied_idx = {
+        i: label_mode[:count].astype(int)
+        for i, label_mode, count in zip(
+            array_idx[~mode_count_one_mask],
+            mode_labels_multiannotator[~mode_count_one_mask, :],
+            label_mode_count[~mode_count_one_mask],
+        )
+    }
 
     # tiebreak 1: using pred_probs (if provided)
     if pred_probs is not None and len(tied_idx) > 0:
         for idx, label_mode in tied_idx.copy().items():
             max_pred_probs = np.where(
                 pred_probs[idx, label_mode] == np.max(pred_probs[idx, label_mode])
             )[0]
@@ -1303,17 +1307,17 @@
 
     Returns
     -------
     annotator_agreement : np.ndarray
         An array of shape ``(N,)`` with the fraction of annotators that agree with each consensus label.
     """
     annotator_agreement = np.zeros(len(labels_multiannotator))
-    for i, labels in enumerate(labels_multiannotator):
-        annotator_agreement[i] = np.mean(labels[~np.isnan(labels)] == consensus_label[i])
-
+    for i in range(labels_multiannotator.shape[1]):
+        annotator_agreement += labels_multiannotator[:, i] == consensus_label
+    annotator_agreement /= (~np.isnan(labels_multiannotator)).sum(axis=1)
     return annotator_agreement
 
 
 def _get_annotator_agreement_with_annotators(
     labels_multiannotator: np.ndarray,
     num_annotations: np.ndarray,
     verbose: bool = True,
@@ -1380,32 +1384,30 @@
         The index of the annotator we want to compute the annotator agreement for.
 
     Returns
     -------
     annotator_agreement : float
         An float repesenting the agreement of each annotator with other annotators that labeled the same examples.
     """
-    annotator_agreement_per_example = np.zeros(len(labels_multiannotator))
-
-    for i, labels in enumerate(labels_multiannotator):
-        labels_subset = labels[~np.isnan(labels)]
-        examples_num_annotators = len(labels_subset)
-        if examples_num_annotators > 1:
-            annotator_agreement_per_example[i] = (
-                np.sum(labels_subset == labels[annotator_idx]) - 1
-            ) / (examples_num_annotators - 1)
-
     adjusted_num_annotations = num_annotations - 1
     if np.sum(adjusted_num_annotations) == 0:
-        annotator_agreement = np.NaN
-    else:
-        annotator_agreement = np.average(
-            annotator_agreement_per_example, weights=num_annotations - 1
-        )
+        return np.NaN
 
+    multi_annotations_mask = num_annotations > 1
+    annotator_agreement_per_example = np.zeros(len(labels_multiannotator))
+    for i in range(labels_multiannotator.shape[1]):
+        annotator_agreement_per_example[multi_annotations_mask] += (
+            labels_multiannotator[multi_annotations_mask, annotator_idx]
+            == labels_multiannotator[multi_annotations_mask, i]
+        )
+    annotator_agreement_per_example[multi_annotations_mask] = (
+        annotator_agreement_per_example[multi_annotations_mask] - 1
+    ) / adjusted_num_annotations[multi_annotations_mask]
+
+    annotator_agreement = np.average(annotator_agreement_per_example, weights=num_annotations - 1)
     return annotator_agreement
 
 
 def _get_post_pred_probs_and_weights(
     labels_multiannotator: np.ndarray,
     consensus_label: np.ndarray,
     prior_pred_probs: np.ndarray,
@@ -1487,43 +1489,38 @@
         annotator_agreement_with_annotators = _get_annotator_agreement_with_annotators(
             labels_multiannotator, num_annotations, verbose
         )
         annotator_error = 1 - annotator_agreement_with_annotators
         adjusted_annotator_agreement = np.clip(
             1 - (annotator_error / most_likely_class_error), a_min=CLIPPING_LOWER_BOUND, a_max=None
         )
-
         # compute model weight
         model_error = np.mean(np.argmax(prior_pred_probs_subset, axis=1) != consensus_label_subset)
         model_weight = np.max(
             [(1 - (model_error / most_likely_class_error)), CLIPPING_LOWER_BOUND]
         ) * np.sqrt(np.mean(num_annotations))
 
+        non_nan_mask = ~np.isnan(labels_multiannotator)
+        annotation_weight = np.zeros(labels_multiannotator.shape[0])
+        for i in range(labels_multiannotator.shape[1]):
+            annotation_weight[non_nan_mask[:, i]] += adjusted_annotator_agreement[i]
+        total_weight = annotation_weight + model_weight
+
         # compute weighted average
         post_pred_probs = np.full(prior_pred_probs.shape, np.nan)
-        for i, labels in enumerate(labels_multiannotator):
-            labels_mask = ~np.isnan(labels)
-            labels_subset = labels[labels_mask]
-            post_pred_probs[i] = [
-                np.average(
-                    [prior_pred_probs[i, true_label]]
-                    + [
-                        (
-                            consensus_likelihood
-                            if annotator_label == true_label
-                            else non_consensus_likelihood
-                        )
-                        for annotator_label in labels_subset
-                    ],
-                    weights=np.concatenate(
-                        ([model_weight], adjusted_annotator_agreement[labels_mask])
-                    ),
+        for i in range(prior_pred_probs.shape[1]):
+            post_pred_probs[:, i] = prior_pred_probs[:, i] * model_weight
+            for k in range(labels_multiannotator.shape[1]):
+                mask = ~np.isnan(labels_multiannotator[:, k])
+                post_pred_probs[mask, i] += np.where(
+                    labels_multiannotator[mask, k] == i,
+                    adjusted_annotator_agreement[k] * consensus_likelihood,
+                    adjusted_annotator_agreement[k] * non_consensus_likelihood,
                 )
-                for true_label in range(num_classes)
-            ]
+            post_pred_probs[:, i] /= total_weight
 
         return_model_weight = model_weight
         return_annotator_weight = adjusted_annotator_agreement
 
     elif quality_method == "agreement":
         num_classes = get_num_classes(pred_probs=prior_pred_probs)
         label_counts = np.full((len(labels_multiannotator), num_classes), np.NaN)
```

### Comparing `cleanlab-2.6.4/cleanlab/multilabel_classification/dataset.py` & `cleanlab-2.6.5/cleanlab/multilabel_classification/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/multilabel_classification/filter.py` & `cleanlab-2.6.5/cleanlab/multilabel_classification/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/multilabel_classification/rank.py` & `cleanlab-2.6.5/cleanlab/multilabel_classification/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/object_detection/filter.py` & `cleanlab-2.6.5/cleanlab/object_detection/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/object_detection/rank.py` & `cleanlab-2.6.5/cleanlab/object_detection/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/object_detection/summary.py` & `cleanlab-2.6.5/cleanlab/object_detection/summary.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/outlier.py` & `cleanlab-2.6.5/cleanlab/outlier.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 """
 Methods for finding out-of-distribution examples in a dataset via scores that quantify how atypical each example is compared to the others.
 
 The underlying algorithms are described in `this paper <https://arxiv.org/abs/2207.03061>`_.
 """
 
 import warnings
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Dict, Optional, Tuple, Union
 
 import numpy as np
-from scipy.spatial.distance import euclidean
 from sklearn.exceptions import NotFittedError
 from sklearn.neighbors import NearestNeighbors
 
 from cleanlab.count import get_confident_thresholds
 from cleanlab.internal.label_quality_utils import (
     _subtract_confident_thresholds,
     get_normalized_entropy,
 )
+from cleanlab.internal.neighbor.knn_graph import correct_knn_distances_and_indices, features_to_knn
 from cleanlab.internal.numerics import softmax
 from cleanlab.internal.outlier import correct_precision_errors, transform_distances_to_scores
 from cleanlab.internal.validation import assert_valid_inputs, labels_to_array
 from cleanlab.typing import LabelLike
 
 
 class OutOfDistribution:
@@ -418,40 +418,25 @@
         -------
         ood_features_scores : Tuple[np.ndarray, Optional[NearestNeighbors]]
         Return a tuple whose first element is array of `ood_features_scores` and second is a `knn` Estimator object.
         """
         DEFAULT_K = 10
         # fit skip over (if knn is not None) then skipping fit and suggest score else fit.
         distance_metric = None
+        correct_knn = False
         if knn is None:  # setup default KNN estimator
             # Make sure both knn and features are not None
-            if features is None:
-                raise ValueError(
-                    "Both knn and features arguments cannot be None at the same time. Not enough information to compute outlier scores."
-                )
-            if k is None:
-                k = DEFAULT_K  # use default when knn and k are both None
-            N, M = features.shape
-            if k > N:  # Ensure number of neighbors less than number of examples
-                raise ValueError(
-                    f"Number of nearest neighbors k={k} cannot exceed the number of examples N={len(features)} passed into the estimator (knn)."
-                )
-
-            # strings are used for sklearn metrics, callables are scipy pairwise distance functions
-            metric: Union[str, Callable]
-            if M > 3:  # use euclidean distance for lower dimensional spaces
-                metric = "cosine"
-            elif N > 100:  # Use efficient implementation (numerically unstable in edge cases)
-                metric = "euclidean"
-            else:  # Use scipy implementation for precise results
-                metric = euclidean
-
-            knn = NearestNeighbors(n_neighbors=k, metric=metric).fit(features)
+            knn = features_to_knn(features, n_neighbors=k)
+            correct_knn = True
             features = None  # features should be None in knn.kneighbors(features) to avoid counting duplicate data points
-            distance_metric = metric if isinstance(metric, str) else str(metric.__name__)
+            # Log knn metric as string to ensure compatibility for score correction
+            distance_metric = (
+                metric if isinstance((metric := knn.metric), str) else str(metric.__name__)
+            )
+            k = knn.n_neighbors
 
         elif k is None:
             k = knn.n_neighbors
 
         max_k = knn.n_neighbors  # number of neighbors previously used in NearestNeighbors object
         if k > max_k:  # if k provided is too high, use max possible number of nearest neighbors
             warnings.warn(
@@ -466,15 +451,26 @@
             knn.kneighbors(features)
         except NotFittedError:
             knn.fit(features)
 
         # Get distances to k-nearest neighbors Note that the knn object contains the specification of distance metric
         # and n_neighbors (k value) If our query set of features matches the training set used to fit knn, the nearest
         # neighbor of each point is the point itself, at a distance of zero.
-        distances, _ = knn.kneighbors(features)
+        distances, indices = knn.kneighbors(features)
+        if (
+            correct_knn
+        ):  # This should only happen if knn is None at the start of this function. Will NEVER happen for approximate KNN provided by user.
+            _features_for_correction = (
+                knn._fit_X if features is None else features
+            )  # Hacky way to get features (training or test). Storing np.unique results is a hassle. ONLY WORKS WITH sklearn NearestNeighbors object
+            distances, _ = correct_knn_distances_and_indices(
+                features=_features_for_correction,
+                distances=distances,
+                indices=indices,
+            )
 
         # Calculate average distance to k-nearest neighbors
         avg_knn_distances = distances[:, :k].mean(axis=1)
 
         if self.params["scaling_factor"] is None:
             self.params["scaling_factor"] = float(
                 max(np.median(avg_knn_distances), 100 * np.finfo(np.float_).eps)
```

### Comparing `cleanlab-2.6.4/cleanlab/rank.py` & `cleanlab-2.6.5/cleanlab/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/regression/learn.py` & `cleanlab-2.6.5/cleanlab/regression/learn.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/regression/rank.py` & `cleanlab-2.6.5/cleanlab/regression/rank.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 If you have a sklearn-compatible regression model, consider using `cleanlab.regression.learn.CleanLearning` instead, which can more accurately identify noisy label values.
 """
 
 from typing import Dict, Callable, Optional, Union
 import numpy as np
 from numpy.typing import ArrayLike
-from scipy.spatial.distance import euclidean
-from sklearn.neighbors import NearestNeighbors
 
+from cleanlab.internal.neighbor.metric import decide_euclidean_metric
+from cleanlab.internal.neighbor.knn_graph import features_to_knn
 from cleanlab.outlier import OutOfDistribution
 from cleanlab.internal.regression_utils import assert_valid_prediction_inputs
 
 from cleanlab.internal.constants import TINY_VALUE
 
 
 def get_label_quality_scores(
@@ -138,15 +138,15 @@
 
 def _get_outre_score_for_each_label(
     labels: np.ndarray,
     predictions: np.ndarray,
     *,
     residual_scale: float = 5,
     frac_neighbors: float = 0.5,
-    neighbor_metric: Optional[Union[str, Callable]] = "euclidean",
+    neighbor_metric: Optional[Union[str, Callable]] = None,
 ) -> np.ndarray:
     """Returns OUTRE based label-quality scores.
 
     This function computes label-quality scores for regression datasets,
     where a lower score indicates labels that are less likely to be correct.
 
     Parameters
@@ -177,17 +177,14 @@
     labels = (labels - labels.mean()) / (labels.std() + TINY_VALUE)
     residual = residual_scale * ((residual - residual.mean()) / (residual.std() + TINY_VALUE))
 
     # 2D features by combining labels and residual
     features = np.array([labels, residual]).T
 
     neighbors = int(np.ceil(frac_neighbors * labels.shape[0]))
-    if neighbor_metric is None:
-        if features.shape[0] > 100:
-            neighbor_metric = "euclidean"
-        else:
-            neighbor_metric = euclidean
-    knn = NearestNeighbors(n_neighbors=neighbors, metric=neighbor_metric).fit(features)
+    # Use provided metric or select a decent implementation of the euclidean metric for knn search
+    neighbor_metric = neighbor_metric or decide_euclidean_metric(features)
+    knn = features_to_knn(features, n_neighbors=neighbors, metric=neighbor_metric)
     ood = OutOfDistribution(params={"knn": knn})
 
     label_quality_scores = ood.score(features=features)
     return label_quality_scores
```

### Comparing `cleanlab-2.6.4/cleanlab/segmentation/filter.py` & `cleanlab-2.6.5/cleanlab/segmentation/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/segmentation/rank.py` & `cleanlab-2.6.5/cleanlab/segmentation/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/segmentation/summary.py` & `cleanlab-2.6.5/cleanlab/segmentation/summary.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/token_classification/filter.py` & `cleanlab-2.6.5/cleanlab/token_classification/filter.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/token_classification/rank.py` & `cleanlab-2.6.5/cleanlab/token_classification/rank.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/token_classification/summary.py` & `cleanlab-2.6.5/cleanlab/token_classification/summary.py`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/cleanlab/version.py` & `cleanlab-2.6.5/cleanlab/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with cleanlab.  If not, see <https://www.gnu.org/licenses/>.
 
 
-__version__ = "2.6.4"
+__version__ = "2.6.5"
 
-# 2.6.4 - Not yet released, you are using bleeding-edge developer version. See its documentation at: https://docs.cleanlab.ai/master/
+# 2.6.6 - Not yet released, you are using bleeding-edge developer version. See its documentation at: https://docs.cleanlab.ai/master/
 
 # ------------------------------------------------
 # | PREVIOUS MAJOR VERSION RELEASE NOTES SUMMARY |
 # ------------------------------------------------
 
 # 2.6.0 - Elevating Data Insights: Comprehensive Issue Checks & Expanded ML Task Compatibility
 #
```

### Comparing `cleanlab-2.6.4/cleanlab.egg-info/PKG-INFO` & `cleanlab-2.6.5/cleanlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab
-Version: 2.6.4
+Version: 2.6.5
 Summary: The standard package for data-centric AI, machine learning with label errors, and automatically finding and fixing dataset issues in Python.
 Author-email: "Cleanlab Inc." <team@cleanlab.ai>
 License: 
                             GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -701,16 +701,16 @@
 Provides-Extra: datalab
 Requires-Dist: datasets>=2.7.0; extra == "datalab"
 Provides-Extra: image
 Requires-Dist: datasets>=2.7.0; extra == "image"
 Requires-Dist: cleanvision>=0.3.6; extra == "image"
 Provides-Extra: all
 Requires-Dist: cleanvision>=0.3.6; extra == "all"
-Requires-Dist: datasets>=2.7.0; extra == "all"
 Requires-Dist: matplotlib>=3.5.1; extra == "all"
+Requires-Dist: datasets>=2.7.0; extra == "all"
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/cleanlab/assets/master/cleanlab/cleanlab_logo_open_source.png" width=60% height=60%>
 </p>
 
 
 cleanlab helps you **clean** data and **lab**els by automatically detecting issues in a ML dataset. To facilitate **machine learning with messy, real-world data**, this data-centric AI package uses your *existing* models to estimate dataset problems that can be fixed to train even *better* models.
@@ -729,17 +729,17 @@
 # cleanlab estimates the predictions you would have gotten if you had trained with *no* label issues.
 cl.predict(test_data)
 
 # A universal data-centric AI tool, cleanlab quantifies class-level issues and overall data quality, for any dataset.
 cleanlab.dataset.health_summary(labels, confident_joint=cl.confident_joint)
 ```
 
-Get started with: [tutorials](https://docs.cleanlab.ai/stable/tutorials/image.html), [documentation](https://docs.cleanlab.ai/), [examples](https://github.com/cleanlab/examples), and [blogs](https://cleanlab.ai/blog/).
+Get started with: [tutorials](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html), [documentation](https://docs.cleanlab.ai/), [examples](https://github.com/cleanlab/examples), and [blogs](https://cleanlab.ai/blog/).
 
- - Learn to run cleanlab on your data in 5 minutes for: [image](https://docs.cleanlab.ai/stable/tutorials/image.html), [text](https://docs.cleanlab.ai/stable/tutorials/datalab/text.html), [audio](https://docs.cleanlab.ai/stable/tutorials/audio.html), or [tabular](https://docs.cleanlab.ai/stable/tutorials/datalab/tabular.html) data.
+ - Learn to run cleanlab on your data in 5 minutes for: [image](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html), [text](https://docs.cleanlab.ai/stable/tutorials/datalab/text.html), [audio](https://docs.cleanlab.ai/stable/tutorials/datalab/audio.html), or [tabular](https://docs.cleanlab.ai/stable/tutorials/datalab/tabular.html) data.
 - Use cleanlab to automatically: [detect data issues (outliers, duplicates, label errors, etc)](https://docs.cleanlab.ai/stable/tutorials/datalab/datalab_quickstart.html), [train robust models](https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html), [infer consensus + annotator-quality for multi-annotator data](https://docs.cleanlab.ai/stable/tutorials/multiannotator.html), [suggest data to (re)label next (active learning)](https://github.com/cleanlab/examples/blob/master/active_learning_multiannotator/active_learning.ipynb). 
 
 
 [![pypi](https://img.shields.io/pypi/v/cleanlab.svg)](https://pypi.org/pypi/cleanlab/)
 [![os](https://img.shields.io/badge/platform-noarch-lightgrey)](https://pypi.org/pypi/cleanlab/)
 [![py\_versions](https://img.shields.io/badge/python-3.8%2B-blue)](https://pypi.org/pypi/cleanlab/)
 [![build\_status](https://github.com/cleanlab/cleanlab/workflows/CI/badge.svg)](https://github.com/cleanlab/cleanlab/actions?query=workflow%3ACI)
@@ -843,15 +843,15 @@
 cl.predict(test_data)
 ```
 
 #### Want to see a working example? [Here’s a compliant PyTorch MNIST CNN class](https://github.com/cleanlab/cleanlab/blob/master/cleanlab/experimental/mnist_pytorch.py)
 
 More details are provided in documentation of [cleanlab.classification.CleanLearning](https://docs.cleanlab.ai/stable/cleanlab/classification.html).
 
-Note, some libraries exist to give you sklearn-compatibility for free. For PyTorch, check out the [skorch](https://skorch.readthedocs.io/) Python library which will wrap your PyTorch model into a sklearn-compatible model ([example](https://docs.cleanlab.ai/stable/tutorials/image.html)). For TensorFlow/Keras, check out our [Keras wrapper](https://docs.cleanlab.ai/stable/cleanlab/models/keras.html). Many libraries also already offer a special scikit-learn API, for example: [XGBoost](https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn) or [LightGBM](https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html).
+Note, some libraries exist to give you sklearn-compatibility for free. For PyTorch, check out the [skorch](https://skorch.readthedocs.io/) Python library which will wrap your PyTorch model into a sklearn-compatible model ([example](https://docs.cleanlab.ai/stable/tutorials/datalab/image.html)). For TensorFlow/Keras, check out our [Keras wrapper](https://docs.cleanlab.ai/stable/cleanlab/models/keras.html). Many libraries also already offer a special scikit-learn API, for example: [XGBoost](https://xgboost.readthedocs.io/en/stable/python/python_api.html#module-xgboost.sklearn) or [LightGBM](https://lightgbm.readthedocs.io/en/latest/pythonapi/lightgbm.LGBMClassifier.html).
 
 <br/>
 </details>
 
 cleanlab is useful across a wide variety of Machine Learning tasks. Specific tasks this data-centric AI solution offers dedicated functionality for include:
 1. [Binary and multi-class classification](https://docs.cleanlab.ai/stable/tutorials/indepth_overview.html)
 2. [Multi-label classification](https://docs.cleanlab.ai/stable/tutorials/multilabel_classification.html) (e.g. image/document tagging)
```

### Comparing `cleanlab-2.6.4/cleanlab.egg-info/SOURCES.txt` & `cleanlab-2.6.5/cleanlab.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,18 @@
 cleanlab/internal/object_detection_utils.py
 cleanlab/internal/outlier.py
 cleanlab/internal/regression_utils.py
 cleanlab/internal/segmentation_utils.py
 cleanlab/internal/token_classification_utils.py
 cleanlab/internal/util.py
 cleanlab/internal/validation.py
+cleanlab/internal/neighbor/__init__.py
+cleanlab/internal/neighbor/knn_graph.py
+cleanlab/internal/neighbor/metric.py
+cleanlab/internal/neighbor/search.py
 cleanlab/models/__init__.py
 cleanlab/models/fasttext.py
 cleanlab/models/keras.py
 cleanlab/multilabel_classification/__init__.py
 cleanlab/multilabel_classification/dataset.py
 cleanlab/multilabel_classification/filter.py
 cleanlab/multilabel_classification/rank.py
```

### Comparing `cleanlab-2.6.4/pyproject.toml` & `cleanlab-2.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cleanlab-2.6.4/setup.py` & `cleanlab-2.6.5/setup.py`

 * *Files identical despite different names*

