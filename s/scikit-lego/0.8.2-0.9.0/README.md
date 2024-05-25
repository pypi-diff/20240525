# Comparing `tmp/scikit-lego-0.8.2.tar.gz` & `tmp/scikit-lego-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-lego-0.8.2.tar", last modified: Tue Apr 16 12:17:58 2024, max compression
+gzip compressed data, was "scikit-lego-0.9.0.tar", last modified: Sat May 25 11:01:24 2024, max compression
```

## Comparing `scikit-lego-0.8.2.tar` & `scikit-lego-0.9.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.786196 scikit-lego-0.8.2/
--rw-r--r--   0 vincent    (501) staff       (20)     1077 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)    10406 2024-04-16 12:17:58.786012 scikit-lego-0.8.2/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)     2450 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/pyproject.toml
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.772588 scikit-lego-0.8.2/scikit_lego.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)    10406 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)     1984 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)      631 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)        7 2024-04-16 12:17:58.000000 scikit-lego-0.8.2/scikit_lego.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)       38 2024-04-16 12:17:58.786234 scikit-lego-0.8.2/setup.cfg
--rw-r--r--   0 vincent    (501) staff       (20)      182 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/setup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.777341 scikit-lego-0.8.2/sklego/
--rw-r--r--   0 vincent    (501) staff       (20)      194 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3175 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/base.py
--rw-r--r--   0 vincent    (501) staff       (20)    10255 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/common.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.779340 scikit-lego-0.8.2/sklego/data/
--rw-r--r--   0 vincent    (501) staff       (20)    59235 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/abalone.zip
--rw-r--r--   0 vincent    (501) staff       (20)    18826 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/arrests.zip
--rw-r--r--   0 vincent    (501) staff       (20)     2108 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/chickweight.zip
--rw-r--r--   0 vincent    (501) staff       (20)     3620 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/hearts.zip
--rw-r--r--   0 vincent    (501) staff       (20)     1340 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/heroes.zip
--rw-r--r--   0 vincent    (501) staff       (20)     2974 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/data/penguins.zip
--rw-r--r--   0 vincent    (501) staff       (20)    18044 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/datasets.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.779917 scikit-lego-0.8.2/sklego/decomposition/
--rw-r--r--   0 vincent    (501) staff       (20)      205 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/decomposition/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     5335 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/decomposition/pca_reconstruction.py
--rw-r--r--   0 vincent    (501) staff       (20)     5152 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/decomposition/umap_reconstruction.py
--rw-r--r--   0 vincent    (501) staff       (20)     4265 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/dummy.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.780556 scikit-lego-0.8.2/sklego/feature_selection/
--rw-r--r--   0 vincent    (501) staff       (20)      132 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/feature_selection/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     9598 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/feature_selection/mrmr.py
--rw-r--r--   0 vincent    (501) staff       (20)    46591 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/linear_model.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.783581 scikit-lego-0.8.2/sklego/meta/
--rw-r--r--   0 vincent    (501) staff       (20)     1282 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     7590 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/_decay_utils.py
--rw-r--r--   0 vincent    (501) staff       (20)     2241 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/_grouped_utils.py
--rw-r--r--   0 vincent    (501) staff       (20)     8373 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/_shrinkage_utils.py
--rw-r--r--   0 vincent    (501) staff       (20)     4104 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/confusion_balancer.py
--rw-r--r--   0 vincent    (501) staff       (20)     6146 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/decay_estimator.py
--rw-r--r--   0 vincent    (501) staff       (20)     2945 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/estimator_transformer.py
--rw-r--r--   0 vincent    (501) staff       (20)    18461 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/grouped_predictor.py
--rw-r--r--   0 vincent    (501) staff       (20)     7598 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/grouped_transformer.py
--rw-r--r--   0 vincent    (501) staff       (20)    25493 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/hierarchical_predictor.py
--rw-r--r--   0 vincent    (501) staff       (20)     9056 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/ordinal_classification.py
--rw-r--r--   0 vincent    (501) staff       (20)     4376 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/meta/outlier_classifier.py
--rw-r--r--   0 vincent    (501) staff       (20)     6705 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/regression_outlier_detector.py
--rw-r--r--   0 vincent    (501) staff       (20)     7619 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/subjective_classifier.py
--rw-r--r--   0 vincent    (501) staff       (20)     4038 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/thresholder.py
--rw-r--r--   0 vincent    (501) staff       (20)     6177 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/meta/zero_inflated_regressor.py
--rw-r--r--   0 vincent    (501) staff       (20)     8652 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/metrics.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.784210 scikit-lego-0.8.2/sklego/mixture/
--rw-r--r--   0 vincent    (501) staff       (20)      378 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/mixture/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     5365 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_classifier.py
--rw-r--r--   0 vincent    (501) staff       (20)     7678 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_detector.py
--rw-r--r--   0 vincent    (501) staff       (20)     4726 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/mixture/gmm_classifier.py
--rw-r--r--   0 vincent    (501) staff       (20)     6989 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/mixture/gmm_outlier_detector.py
--rw-r--r--   0 vincent    (501) staff       (20)    26016 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/model_selection.py
--rw-r--r--   0 vincent    (501) staff       (20)    12490 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/naive_bayes.py
--rw-r--r--   0 vincent    (501) staff       (20)     4702 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/neighbors.py
--rw-r--r--   0 vincent    (501) staff       (20)     1711 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/notinstalled.py
--rw-r--r--   0 vincent    (501) staff       (20)    10311 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/pandas_utils.py
--rw-r--r--   0 vincent    (501) staff       (20)    13636 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/pipeline.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-04-16 12:17:58.785785 scikit-lego-0.8.2/sklego/preprocessing/
--rw-r--r--   0 vincent    (501) staff       (20)     1032 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     8999 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/preprocessing/columncapper.py
--rw-r--r--   0 vincent    (501) staff       (20)     3518 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/dictmapper.py
--rw-r--r--   0 vincent    (501) staff       (20)     4348 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/formulaictransformer.py
--rw-r--r--   0 vincent    (501) staff       (20)     3347 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/identitytransformer.py
--rw-r--r--   0 vincent    (501) staff       (20)     8980 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/preprocessing/intervalencoder.py
--rw-r--r--   0 vincent    (501) staff       (20)     2779 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/outlier_remover.py
--rw-r--r--   0 vincent    (501) staff       (20)    13377 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/pandastransformers.py
--rw-r--r--   0 vincent    (501) staff       (20)     9605 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/projections.py
--rw-r--r--   0 vincent    (501) staff       (20)     3209 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/preprocessing/randomadder.py
--rw-r--r--   0 vincent    (501) staff       (20)    10461 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/preprocessing/repeatingbasis.py
--rw-r--r--   0 vincent    (501) staff       (20)     1388 2024-04-16 12:06:00.000000 scikit-lego-0.8.2/sklego/testing.py
--rw-r--r--   0 vincent    (501) staff       (20)     1513 2024-04-16 12:05:47.000000 scikit-lego-0.8.2/sklego/this.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.907998 scikit-lego-0.9.0/
+-rw-r--r--   0 vincent    (501) staff       (20)     1077 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)    10418 2024-05-25 11:01:24.907817 scikit-lego-0.9.0/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)     2717 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/pyproject.toml
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.899052 scikit-lego-0.9.0/scikit_lego.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)    10418 2024-05-25 11:01:24.000000 scikit-lego-0.9.0/scikit_lego.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)     1984 2024-05-25 11:01:24.000000 scikit-lego-0.9.0/scikit_lego.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2024-05-25 11:01:24.000000 scikit-lego-0.9.0/scikit_lego.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      710 2024-05-25 11:01:24.000000 scikit-lego-0.9.0/scikit_lego.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        7 2024-05-25 11:01:24.000000 scikit-lego-0.9.0/scikit_lego.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2024-05-25 11:01:24.908034 scikit-lego-0.9.0/setup.cfg
+-rw-r--r--   0 vincent    (501) staff       (20)      182 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.901983 scikit-lego-0.9.0/sklego/
+-rw-r--r--   0 vincent    (501) staff       (20)      194 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3175 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/base.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10259 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/common.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.903524 scikit-lego-0.9.0/sklego/data/
+-rw-r--r--   0 vincent    (501) staff       (20)    59235 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/data/abalone.zip
+-rw-r--r--   0 vincent    (501) staff       (20)    18826 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/data/arrests.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     2108 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/data/chickweight.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     3620 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/data/hearts.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     1340 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/data/heroes.zip
+-rw-r--r--   0 vincent    (501) staff       (20)     2974 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/data/penguins.zip
+-rw-r--r--   0 vincent    (501) staff       (20)    18092 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/datasets.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.903941 scikit-lego-0.9.0/sklego/decomposition/
+-rw-r--r--   0 vincent    (501) staff       (20)      205 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/decomposition/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5130 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/decomposition/pca_reconstruction.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5404 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/decomposition/umap_reconstruction.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4355 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/dummy.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.904174 scikit-lego-0.9.0/sklego/feature_selection/
+-rw-r--r--   0 vincent    (501) staff       (20)      132 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/feature_selection/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9665 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/feature_selection/mrmr.py
+-rw-r--r--   0 vincent    (501) staff       (20)    47794 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/linear_model.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.905902 scikit-lego-0.9.0/sklego/meta/
+-rw-r--r--   0 vincent    (501) staff       (20)     1282 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/meta/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7590 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/meta/_decay_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1903 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/_grouped_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8707 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/_shrinkage_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4288 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/confusion_balancer.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6266 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/decay_estimator.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2986 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/estimator_transformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19460 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/grouped_predictor.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8093 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/grouped_transformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    26757 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/hierarchical_predictor.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9082 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/ordinal_classification.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4504 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/outlier_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7798 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/regression_outlier_detector.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7762 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/subjective_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5102 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/thresholder.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6332 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/meta/zero_inflated_regressor.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8652 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/metrics.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.906402 scikit-lego-0.9.0/sklego/mixture/
+-rw-r--r--   0 vincent    (501) staff       (20)      378 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/mixture/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5487 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/mixture/bayesian_gmm_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7725 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/mixture/bayesian_gmm_detector.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4848 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/mixture/gmm_classifier.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7032 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/mixture/gmm_outlier_detector.py
+-rw-r--r--   0 vincent    (501) staff       (20)    27090 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/model_selection.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12666 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/naive_bayes.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4743 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/neighbors.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1711 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/notinstalled.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10650 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/pandas_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13636 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/pipeline.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2024-05-25 11:01:24.907531 scikit-lego-0.9.0/sklego/preprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)     1066 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9061 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/columncapper.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3680 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/dictmapper.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4388 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/formulaictransformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3347 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/preprocessing/identitytransformer.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8980 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/preprocessing/intervalencoder.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2797 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/outlier_remover.py
+-rw-r--r--   0 vincent    (501) staff       (20)    17691 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/pandastransformers.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9797 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/projections.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3279 2024-05-25 11:00:16.000000 scikit-lego-0.9.0/sklego/preprocessing/randomadder.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10461 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/preprocessing/repeatingbasis.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1388 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/testing.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1513 2024-05-25 11:00:11.000000 scikit-lego-0.9.0/sklego/this.py
```

### Comparing `scikit-lego-0.8.2/LICENSE` & `scikit-lego-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/PKG-INFO` & `scikit-lego-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-lego
-Version: 0.8.2
+Version: 0.9.0
 Summary: A collection of lego bricks for scikit-learn pipelines
 Author: Vincent D. Warmerdam, Matthijs Brouns
 Maintainer: Francesco Bruzzesi
 License: MIT License
         
         Copyright (c) 2019 vincent d warmerdam 
         
@@ -43,14 +43,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: cvxpy
 Provides-Extra: formulaic
 Provides-Extra: umap
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: test-all
 Provides-Extra: utils
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Downloads](https://static.pepy.tech/badge/scikit-lego/month)](https://www.pepy.tech/projects/scikit-lego)
 [![Version](https://img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/scikit-lego.svg)](https://anaconda.org/conda-forge/scikit-lego)
@@ -169,15 +170,15 @@
 - `sklego.meta.ZeroInflatedRegressor` predicts zero or applies a regression based on a classifier
 - `sklego.preprocessing.ColumnCapper` limits extreme values of the model features
 - `sklego.preprocessing.ColumnDropper` drops a column from pandas
 - `sklego.preprocessing.ColumnSelector` selects columns based on column name
 - `sklego.preprocessing.InformationFilter` transformer that can de-correlate features
 - `sklego.preprocessing.IdentityTransformer` returns the same data, allows for concatenating pipelines
 - `sklego.preprocessing.OrthogonalTransformer` makes all features linearly independent
-- `sklego.preprocessing.PandasTypeSelector` selects columns based on pandas type
+- `sklego.preprocessing.TypeSelector` selects columns based on type
 - `sklego.preprocessing.RandomAdder` adds randomness in training
 - `sklego.preprocessing.RepeatingBasisFunction` repeating feature engineering, useful for timeseries
 - `sklego.preprocessing.DictMapper` assign numeric values on categorical columns
 - `sklego.preprocessing.OutlierRemover` experimental method to remove outliers during training
 - `sklego.model_selection.GroupTimeSeriesSplit` timeseries Kfold for groups with different amount of observations per group
 - `sklego.model_selection.KlusterFoldValidation` experimental feature that does K folds based on clustering
 - `sklego.model_selection.TimeGapSplit` timeseries Kfold with a gap between train/test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-lego Version: 0.8.2 Summary: A collection of
+Metadata-Version: 2.1 Name: scikit-lego Version: 0.9.0 Summary: A collection of
 lego bricks for scikit-learn pipelines Author: Vincent D. Warmerdam, Matthijs
 Brouns Maintainer: Francesco Bruzzesi License: MIT License Copyright (c) 2019
 vincent d warmerdam Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -23,47 +23,48 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: cvxpy Provides-Extra: formulaic
 Provides-Extra: umap Provides-Extra: all Provides-Extra: docs Provides-Extra:
-test Provides-Extra: utils Provides-Extra: dev License-File: LICENSE [!
-[Downloads](https://static.pepy.tech/badge/scikit-lego/month)](https://
-www.pepy.tech/projects/scikit-lego) [![Version](https://img.shields.io/pypi/v/
-scikit-lego)](https://pypi.org/project/scikit-lego/) [![Conda Version](https://
-img.shields.io/conda/vn/conda-forge/scikit-lego.svg)](https://anaconda.org/
-conda-forge/scikit-lego) ![](https://img.shields.io/github/license/koaning/
-scikit-lego) ![](https://img.shields.io/pypi/pyversions/scikit-lego) ![](https:
-//img.shields.io/github/contributors/koaning/scikit-lego) [![Ruff](https://
-img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/
-main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![DOI](https://
-zenodo.org/badge/166836939.svg)](https://zenodo.org/badge/latestdoi/166836939)
-# scikit-lego _[_i_m_a_g_e_s_/_l_o_g_o_._p_n_g_]We love scikit learn but very often we find
-ourselves writing custom transformers, metrics and models. The goal of this
-project is to attempt to consolidate these into a package that offers code
-quality/testing. This project started as a collaboration between multiple
-companies in the Netherlands but has since received contributions from around
-the globe. It was initiated by [Matthijs Brouns](https://www.mbrouns.com/) and
-[Vincent D. Warmerdam](https://koaning.io) as a tool to teach people how to
-contribute to open source. Note that we're not formally affiliated with the
-scikit-learn project at all, but we aim to strictly adhere to their standards.
-The same holds with lego. LEGOÂ® is a trademark of the LEGO Group of companies
-which does not sponsor, authorize or endorse this project. ## Installation
-Install `scikit-lego` via pip with ```bash python -m pip install scikit-lego
-``` Via [conda](https://conda.io/projects/conda/en/latest/) with ```bash conda
-install -c conda-forge scikit-lego ``` Alternatively, to edit and contribute
-you can fork/clone and run: ```bash python -m pip install -e ".[dev]" python
-setup.py develop ``` ## Documentation The documentation can be found [here]
-(https://koaning.github.io/scikit-lego/). ## Usage We offer custom metrics,
-models and transformers. You can import them just like you would in scikit-
-learn. ```python # the scikit learn stuff we love from sklearn.preprocessing
-import StandardScaler from sklearn.pipeline import Pipeline # from scikit lego
-stuff we add from sklego.preprocessing import RandomAdder from sklego.mixture
-import GMMClassifier ... mod = Pipeline([ ("scale", StandardScaler()),
+test Provides-Extra: test-all Provides-Extra: utils Provides-Extra: dev
+License-File: LICENSE [![Downloads](https://static.pepy.tech/badge/scikit-lego/
+month)](https://www.pepy.tech/projects/scikit-lego) [![Version](https://
+img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/) [!
+[Conda Version](https://img.shields.io/conda/vn/conda-forge/scikit-lego.svg)]
+(https://anaconda.org/conda-forge/scikit-lego) ![](https://img.shields.io/
+github/license/koaning/scikit-lego) ![](https://img.shields.io/pypi/pyversions/
+scikit-lego) ![](https://img.shields.io/github/contributors/koaning/scikit-
+lego) [![Ruff](https://img.shields.io/endpoint?url=https://
+raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://
+github.com/astral-sh/ruff) [![DOI](https://zenodo.org/badge/166836939.svg)]
+(https://zenodo.org/badge/latestdoi/166836939) # scikit-lego _[_i_m_a_g_e_s_/
+_l_o_g_o_._p_n_g_]We love scikit learn but very often we find ourselves writing custom
+transformers, metrics and models. The goal of this project is to attempt to
+consolidate these into a package that offers code quality/testing. This project
+started as a collaboration between multiple companies in the Netherlands but
+has since received contributions from around the globe. It was initiated by
+[Matthijs Brouns](https://www.mbrouns.com/) and [Vincent D. Warmerdam](https://
+koaning.io) as a tool to teach people how to contribute to open source. Note
+that we're not formally affiliated with the scikit-learn project at all, but we
+aim to strictly adhere to their standards. The same holds with lego. LEGOÂ® is
+a trademark of the LEGO Group of companies which does not sponsor, authorize or
+endorse this project. ## Installation Install `scikit-lego` via pip with
+```bash python -m pip install scikit-lego ``` Via [conda](https://conda.io/
+projects/conda/en/latest/) with ```bash conda install -c conda-forge scikit-
+lego ``` Alternatively, to edit and contribute you can fork/clone and run:
+```bash python -m pip install -e ".[dev]" python setup.py develop ``` ##
+Documentation The documentation can be found [here](https://koaning.github.io/
+scikit-lego/). ## Usage We offer custom metrics, models and transformers. You
+can import them just like you would in scikit-learn. ```python # the scikit
+learn stuff we love from sklearn.preprocessing import StandardScaler from
+sklearn.pipeline import Pipeline # from scikit lego stuff we add from
+sklego.preprocessing import RandomAdder from sklego.mixture import
+GMMClassifier ... mod = Pipeline([ ("scale", StandardScaler()),
 ("random_noise", RandomAdder()), ("model", GMMClassifier()) ]) ... ``` ##
 Features Here's a list of features that this library currently offers: -
 `sklego.datasets.load_abalone` loads in the abalone dataset -
 `sklego.datasets.load_arrests` loads in a dataset with fairness concerns -
 `sklego.datasets.load_chicken` loads in the joyful chickweight dataset -
 `sklego.datasets.load_heroes` loads a heroes of the storm dataset -
 `sklego.datasets.load_hearts` loads a dataset about hearts -
@@ -108,17 +109,17 @@
 `sklego.preprocessing.ColumnCapper` limits extreme values of the model features
 - `sklego.preprocessing.ColumnDropper` drops a column from pandas -
 `sklego.preprocessing.ColumnSelector` selects columns based on column name -
 `sklego.preprocessing.InformationFilter` transformer that can de-correlate
 features - `sklego.preprocessing.IdentityTransformer` returns the same data,
 allows for concatenating pipelines -
 `sklego.preprocessing.OrthogonalTransformer` makes all features linearly
-independent - `sklego.preprocessing.PandasTypeSelector` selects columns based
-on pandas type - `sklego.preprocessing.RandomAdder` adds randomness in training
-- `sklego.preprocessing.RepeatingBasisFunction` repeating feature engineering,
+independent - `sklego.preprocessing.TypeSelector` selects columns based on type
+- `sklego.preprocessing.RandomAdder` adds randomness in training -
+`sklego.preprocessing.RepeatingBasisFunction` repeating feature engineering,
 useful for timeseries - `sklego.preprocessing.DictMapper` assign numeric values
 on categorical columns - `sklego.preprocessing.OutlierRemover` experimental
 method to remove outliers during training -
 `sklego.model_selection.GroupTimeSeriesSplit` timeseries Kfold for groups with
 different amount of observations per group -
 `sklego.model_selection.KlusterFoldValidation` experimental feature that does K
 folds based on clustering - `sklego.model_selection.TimeGapSplit` timeseries
```

### Comparing `scikit-lego-0.8.2/pyproject.toml` & `scikit-lego-0.9.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scikit-lego"
-version = "0.8.2"
+version = "0.9.0"
 description="A collection of lego bricks for scikit-learn pipelines"
 
 license = {file = "LICENSE"}
 readme = "readme.md"
 requires-python = ">=3.6"
 authors = [
     {name = "Vincent D. Warmerdam"},
@@ -16,14 +16,15 @@
 ]
 
 maintainers = [
     {name = "Francesco Bruzzesi"}
 ]
 
 dependencies = [
+    "narwhals>=0.8.13",
     "pandas>=1.1.5",
     "scikit-learn>=1.0",
     "importlib-metadata >= 1.0; python_version < '3.8'",
     "importlib-resources; python_version < '3.9'",
 ]
 
 classifiers = [
@@ -41,37 +42,42 @@
 
 [project.urls]
 repository = "https://github.com/koaning/scikit-lego"
 issue-tracker = "https://github.com/koaning/scikit-lego/issues"
 documentation = "https://koaning.github.io/scikit-lego/"
 
 [project.optional-dependencies]
-cvxpy = ["cmake", "osqp", "cvxpy>=1.1.8"]
+cvxpy = ["cmake", "osqp", "cvxpy>=1.1.8", "numpy<2.0"]
 formulaic = ["formulaic>=0.6.0"]
-umap = ["umap-learn>=0.4.6"]
+umap = ["umap-learn>=0.4.6", "numpy<2.0"]
 
 all = ["scikit-lego[cvxpy,formulaic,umap]"]
 
 docs = [
     "mkdocs>=1.5.3",
     "mkdocs-autorefs>=0.5.0",
     "mkdocs-material>=9.4.5",
     "mkdocs-material-extensions>=1.2",
     "mkdocstrings>=0.23.0",
     "mkdocstrings-python>=1.7.3",
 ]
 
 test = [
-    "scikit-lego[all]",
+    "narwhals[polars]",
+    "pyarrow",
     "pytest>=6.2.5",
     "pytest-xdist>=1.34.0",
     "pytest-cov>=2.6.1",
     "pytest-mock>=1.6.3",
 ]
 
+test-all = [
+    "scikit-lego[all,test]",
+]
+
 utils = [
     "matplotlib>=3.0.2",
     "jupyter>=1.0.0",
     "jupyterlab>=0.35.4",
 ]
 
 dev = [
@@ -100,9 +106,11 @@
 extend-select = ["I"]
 ignore = [
     "E731",  # do not assign a `lambda` expression, use a `def`
     ]
 
 [tool.pytest.ini_options]
 markers = [
-    "cvxpy: tests that require cvxpy (deselect with '-m \"not cvxpy\"')"
+    "cvxpy: tests that require cvxpy (deselect with '-m \"not cvxpy\"')",
+    "formulaic: tests that require formulaic (deselect with '-m \"not formulaic\"')",
+    "umap: tests that require umap (deselect with '-m \"not umap\"')"
 ]
```

### Comparing `scikit-lego-0.8.2/scikit_lego.egg-info/PKG-INFO` & `scikit-lego-0.9.0/scikit_lego.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-lego
-Version: 0.8.2
+Version: 0.9.0
 Summary: A collection of lego bricks for scikit-learn pipelines
 Author: Vincent D. Warmerdam, Matthijs Brouns
 Maintainer: Francesco Bruzzesi
 License: MIT License
         
         Copyright (c) 2019 vincent d warmerdam 
         
@@ -43,14 +43,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: cvxpy
 Provides-Extra: formulaic
 Provides-Extra: umap
 Provides-Extra: all
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: test-all
 Provides-Extra: utils
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Downloads](https://static.pepy.tech/badge/scikit-lego/month)](https://www.pepy.tech/projects/scikit-lego)
 [![Version](https://img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/scikit-lego.svg)](https://anaconda.org/conda-forge/scikit-lego)
@@ -169,15 +170,15 @@
 - `sklego.meta.ZeroInflatedRegressor` predicts zero or applies a regression based on a classifier
 - `sklego.preprocessing.ColumnCapper` limits extreme values of the model features
 - `sklego.preprocessing.ColumnDropper` drops a column from pandas
 - `sklego.preprocessing.ColumnSelector` selects columns based on column name
 - `sklego.preprocessing.InformationFilter` transformer that can de-correlate features
 - `sklego.preprocessing.IdentityTransformer` returns the same data, allows for concatenating pipelines
 - `sklego.preprocessing.OrthogonalTransformer` makes all features linearly independent
-- `sklego.preprocessing.PandasTypeSelector` selects columns based on pandas type
+- `sklego.preprocessing.TypeSelector` selects columns based on type
 - `sklego.preprocessing.RandomAdder` adds randomness in training
 - `sklego.preprocessing.RepeatingBasisFunction` repeating feature engineering, useful for timeseries
 - `sklego.preprocessing.DictMapper` assign numeric values on categorical columns
 - `sklego.preprocessing.OutlierRemover` experimental method to remove outliers during training
 - `sklego.model_selection.GroupTimeSeriesSplit` timeseries Kfold for groups with different amount of observations per group
 - `sklego.model_selection.KlusterFoldValidation` experimental feature that does K folds based on clustering
 - `sklego.model_selection.TimeGapSplit` timeseries Kfold with a gap between train/test
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scikit-lego Version: 0.8.2 Summary: A collection of
+Metadata-Version: 2.1 Name: scikit-lego Version: 0.9.0 Summary: A collection of
 lego bricks for scikit-learn pipelines Author: Vincent D. Warmerdam, Matthijs
 Brouns Maintainer: Francesco Bruzzesi License: MIT License Copyright (c) 2019
 vincent d warmerdam Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
@@ -23,47 +23,48 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Python: >=3.6 Description-
 Content-Type: text/markdown Provides-Extra: cvxpy Provides-Extra: formulaic
 Provides-Extra: umap Provides-Extra: all Provides-Extra: docs Provides-Extra:
-test Provides-Extra: utils Provides-Extra: dev License-File: LICENSE [!
-[Downloads](https://static.pepy.tech/badge/scikit-lego/month)](https://
-www.pepy.tech/projects/scikit-lego) [![Version](https://img.shields.io/pypi/v/
-scikit-lego)](https://pypi.org/project/scikit-lego/) [![Conda Version](https://
-img.shields.io/conda/vn/conda-forge/scikit-lego.svg)](https://anaconda.org/
-conda-forge/scikit-lego) ![](https://img.shields.io/github/license/koaning/
-scikit-lego) ![](https://img.shields.io/pypi/pyversions/scikit-lego) ![](https:
-//img.shields.io/github/contributors/koaning/scikit-lego) [![Ruff](https://
-img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/
-main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) [![DOI](https://
-zenodo.org/badge/166836939.svg)](https://zenodo.org/badge/latestdoi/166836939)
-# scikit-lego _[_i_m_a_g_e_s_/_l_o_g_o_._p_n_g_]We love scikit learn but very often we find
-ourselves writing custom transformers, metrics and models. The goal of this
-project is to attempt to consolidate these into a package that offers code
-quality/testing. This project started as a collaboration between multiple
-companies in the Netherlands but has since received contributions from around
-the globe. It was initiated by [Matthijs Brouns](https://www.mbrouns.com/) and
-[Vincent D. Warmerdam](https://koaning.io) as a tool to teach people how to
-contribute to open source. Note that we're not formally affiliated with the
-scikit-learn project at all, but we aim to strictly adhere to their standards.
-The same holds with lego. LEGOÂ® is a trademark of the LEGO Group of companies
-which does not sponsor, authorize or endorse this project. ## Installation
-Install `scikit-lego` via pip with ```bash python -m pip install scikit-lego
-``` Via [conda](https://conda.io/projects/conda/en/latest/) with ```bash conda
-install -c conda-forge scikit-lego ``` Alternatively, to edit and contribute
-you can fork/clone and run: ```bash python -m pip install -e ".[dev]" python
-setup.py develop ``` ## Documentation The documentation can be found [here]
-(https://koaning.github.io/scikit-lego/). ## Usage We offer custom metrics,
-models and transformers. You can import them just like you would in scikit-
-learn. ```python # the scikit learn stuff we love from sklearn.preprocessing
-import StandardScaler from sklearn.pipeline import Pipeline # from scikit lego
-stuff we add from sklego.preprocessing import RandomAdder from sklego.mixture
-import GMMClassifier ... mod = Pipeline([ ("scale", StandardScaler()),
+test Provides-Extra: test-all Provides-Extra: utils Provides-Extra: dev
+License-File: LICENSE [![Downloads](https://static.pepy.tech/badge/scikit-lego/
+month)](https://www.pepy.tech/projects/scikit-lego) [![Version](https://
+img.shields.io/pypi/v/scikit-lego)](https://pypi.org/project/scikit-lego/) [!
+[Conda Version](https://img.shields.io/conda/vn/conda-forge/scikit-lego.svg)]
+(https://anaconda.org/conda-forge/scikit-lego) ![](https://img.shields.io/
+github/license/koaning/scikit-lego) ![](https://img.shields.io/pypi/pyversions/
+scikit-lego) ![](https://img.shields.io/github/contributors/koaning/scikit-
+lego) [![Ruff](https://img.shields.io/endpoint?url=https://
+raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://
+github.com/astral-sh/ruff) [![DOI](https://zenodo.org/badge/166836939.svg)]
+(https://zenodo.org/badge/latestdoi/166836939) # scikit-lego _[_i_m_a_g_e_s_/
+_l_o_g_o_._p_n_g_]We love scikit learn but very often we find ourselves writing custom
+transformers, metrics and models. The goal of this project is to attempt to
+consolidate these into a package that offers code quality/testing. This project
+started as a collaboration between multiple companies in the Netherlands but
+has since received contributions from around the globe. It was initiated by
+[Matthijs Brouns](https://www.mbrouns.com/) and [Vincent D. Warmerdam](https://
+koaning.io) as a tool to teach people how to contribute to open source. Note
+that we're not formally affiliated with the scikit-learn project at all, but we
+aim to strictly adhere to their standards. The same holds with lego. LEGOÂ® is
+a trademark of the LEGO Group of companies which does not sponsor, authorize or
+endorse this project. ## Installation Install `scikit-lego` via pip with
+```bash python -m pip install scikit-lego ``` Via [conda](https://conda.io/
+projects/conda/en/latest/) with ```bash conda install -c conda-forge scikit-
+lego ``` Alternatively, to edit and contribute you can fork/clone and run:
+```bash python -m pip install -e ".[dev]" python setup.py develop ``` ##
+Documentation The documentation can be found [here](https://koaning.github.io/
+scikit-lego/). ## Usage We offer custom metrics, models and transformers. You
+can import them just like you would in scikit-learn. ```python # the scikit
+learn stuff we love from sklearn.preprocessing import StandardScaler from
+sklearn.pipeline import Pipeline # from scikit lego stuff we add from
+sklego.preprocessing import RandomAdder from sklego.mixture import
+GMMClassifier ... mod = Pipeline([ ("scale", StandardScaler()),
 ("random_noise", RandomAdder()), ("model", GMMClassifier()) ]) ... ``` ##
 Features Here's a list of features that this library currently offers: -
 `sklego.datasets.load_abalone` loads in the abalone dataset -
 `sklego.datasets.load_arrests` loads in a dataset with fairness concerns -
 `sklego.datasets.load_chicken` loads in the joyful chickweight dataset -
 `sklego.datasets.load_heroes` loads a heroes of the storm dataset -
 `sklego.datasets.load_hearts` loads a dataset about hearts -
@@ -108,17 +109,17 @@
 `sklego.preprocessing.ColumnCapper` limits extreme values of the model features
 - `sklego.preprocessing.ColumnDropper` drops a column from pandas -
 `sklego.preprocessing.ColumnSelector` selects columns based on column name -
 `sklego.preprocessing.InformationFilter` transformer that can de-correlate
 features - `sklego.preprocessing.IdentityTransformer` returns the same data,
 allows for concatenating pipelines -
 `sklego.preprocessing.OrthogonalTransformer` makes all features linearly
-independent - `sklego.preprocessing.PandasTypeSelector` selects columns based
-on pandas type - `sklego.preprocessing.RandomAdder` adds randomness in training
-- `sklego.preprocessing.RepeatingBasisFunction` repeating feature engineering,
+independent - `sklego.preprocessing.TypeSelector` selects columns based on type
+- `sklego.preprocessing.RandomAdder` adds randomness in training -
+`sklego.preprocessing.RepeatingBasisFunction` repeating feature engineering,
 useful for timeseries - `sklego.preprocessing.DictMapper` assign numeric values
 on categorical columns - `sklego.preprocessing.OutlierRemover` experimental
 method to remove outliers during training -
 `sklego.model_selection.GroupTimeSeriesSplit` timeseries Kfold for groups with
 different amount of observations per group -
 `sklego.model_selection.KlusterFoldValidation` experimental feature that does K
 folds based on clustering - `sklego.model_selection.TimeGapSplit` timeseries
```

### Comparing `scikit-lego-0.8.2/scikit_lego.egg-info/SOURCES.txt` & `scikit-lego-0.9.0/scikit_lego.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/scikit_lego.egg-info/requires.txt` & `scikit-lego-0.9.0/scikit_lego.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+narwhals>=0.8.13
 pandas>=1.1.5
 scikit-learn>=1.0
 
 [:python_version < "3.8"]
 importlib-metadata>=1.0
 
 [:python_version < "3.9"]
@@ -10,14 +11,15 @@
 [all]
 scikit-lego[cvxpy,formulaic,umap]
 
 [cvxpy]
 cmake
 osqp
 cvxpy>=1.1.8
+numpy<2.0
 
 [dev]
 scikit-lego[all,docs,test]
 pre-commit>=1.18.3
 ruff>=0.1.6
 
 [docs]
@@ -28,20 +30,25 @@
 mkdocstrings>=0.23.0
 mkdocstrings-python>=1.7.3
 
 [formulaic]
 formulaic>=0.6.0
 
 [test]
-scikit-lego[all]
+narwhals[polars]
+pyarrow
 pytest>=6.2.5
 pytest-xdist>=1.34.0
 pytest-cov>=2.6.1
 pytest-mock>=1.6.3
 
+[test-all]
+scikit-lego[all,test]
+
 [umap]
 umap-learn>=0.4.6
+numpy<2.0
 
 [utils]
 matplotlib>=3.0.2
 jupyter>=1.0.0
 jupyterlab>=0.35.4
```

### Comparing `scikit-lego-0.8.2/sklego/base.py` & `scikit-lego-0.9.0/sklego/base.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/common.py` & `scikit-lego-0.9.0/sklego/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     assert np.all(trf.transform(X_train) != X_train)
     assert np.all(trf.transform(X_test) == X_test)
     ```
     """
 
     _HASHERS = {
-        pd.DataFrame: lambda X: hashlib.sha256(pd.util.hash_pandas_object(X, index=True).values).hexdigest(),
+        pd.DataFrame: lambda X: hashlib.sha256(pd.util.hash_pandas_object(X, index=True).to_numpy()).hexdigest(),
         np.ndarray: lambda X: hash(X.data.tobytes()),
         np.memmap: lambda X: hash(X.data.tobytes()),
     }
 
     def fit(self, X, y=None):
         """Fit the mixin by calculating the hash of `X` and stores it in `self.X_hash_`.
```

### Comparing `scikit-lego-0.8.2/sklego/data/abalone.zip` & `scikit-lego-0.9.0/sklego/data/abalone.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/data/arrests.zip` & `scikit-lego-0.9.0/sklego/data/arrests.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/data/chickweight.zip` & `scikit-lego-0.9.0/sklego/data/chickweight.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/data/hearts.zip` & `scikit-lego-0.9.0/sklego/data/hearts.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/data/heroes.zip` & `scikit-lego-0.9.0/sklego/data/heroes.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/data/penguins.zip` & `scikit-lego-0.9.0/sklego/data/penguins.zip`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/datasets.py` & `scikit-lego-0.9.0/sklego/datasets.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,16 +108,16 @@
                 "island",
                 "bill_length_mm",
                 "bill_depth_mm",
                 "flipper_length_mm",
                 "body_mass_g",
                 "sex",
             ]
-        ].values,
-        df["species"].values,
+        ].to_numpy(),
+        df["species"].to_numpy(),
     )
     if return_X_y:
         return X, y
     return {"data": X, "target": y}
 
 
 def load_arrests(return_X_y=False, as_frame=False):
@@ -158,16 +158,16 @@
     - Personal communication from Michael Friendly, York University.
     """
     filepath = importlib_resources.files("sklego") / "data" / "arrests.zip"
     df = pd.read_csv(filepath)
     if as_frame:
         return df
     X, y = (
-        df[["colour", "year", "age", "sex", "employed", "citizen", "checks"]].values,
-        df["released"].values,
+        df[["colour", "year", "age", "sex", "employed", "citizen", "checks"]].to_numpy(),
+        df["released"].to_numpy(),
     )
     if return_X_y:
         return X, y
     return {"data": X, "target": y}
 
 
 def load_chicken(return_X_y=False, as_frame=False):
@@ -204,15 +204,15 @@
     - Crowder, M. and Hand, D. (1990), Analysis of Repeated Measures, Chapman and Hall (example 5.3)
     - Hand, D. and Crowder, M. (1996), Practical Longitudinal Data Analysis, Chapman and Hall (table A.2)
     """
     filepath = importlib_resources.files("sklego") / "data" / "chickweight.zip"
     df = pd.read_csv(filepath)
     if as_frame:
         return df
-    X, y = df[["time", "diet", "chick"]].values, df["weight"].values
+    X, y = df[["time", "diet", "chick"]].to_numpy(), df["weight"].to_numpy()
     if return_X_y:
         return X, y
     return {"data": X, "target": y}
 
 
 def load_abalone(return_X_y=False, as_frame=False):
     """
@@ -261,16 +261,16 @@
             "height",
             "whole_weight",
             "shucked_weight",
             "viscera_weight",
             "shell_weight",
             "rings",
         ]
-    ].values
-    y = df["sex"].values
+    ].to_numpy()
+    y = df["sex"].to_numpy()
     if return_X_y:
         return X, y
     return {"data": X, "target": y}
 
 
 def load_heroes(return_X_y=False, as_frame=False):
     """A dataset from the video game [Heroes of the storm](https://heroesofthestorm.blizzard.com/en-us/).
@@ -300,16 +300,16 @@
     # Index(['name', 'attack_type', 'role', 'health', 'attack', 'attack_spd'], dtype='object')
     ```
     """
     filepath = importlib_resources.files("sklego") / "data" / "heroes.zip"
     df = pd.read_csv(filepath)
     if as_frame:
         return df
-    X = df[["health", "attack"]].values
-    y = df["attack_type"].values
+    X = df[["health", "attack"]].to_numpy()
+    y = df["attack_type"].to_numpy()
     if return_X_y:
         return X, y
     return {"data": X, "target": y}
 
 
 def load_hearts(return_X_y=False, as_frame=False):
     """Loads the Cleveland Heart Diseases dataset.
@@ -373,16 +373,16 @@
             "thalach",
             "exang",
             "oldpeak",
             "slope",
             "ca",
             "thal",
         ]
-    ].values
-    y = df["target"].values
+    ].to_numpy()
+    y = df["target"].to_numpy()
     if return_X_y:
         return X, y
     return {"data": X, "target": y}
 
 
 def make_simpleseries(
     n_samples=365 * 5,
```

### Comparing `scikit-lego-0.8.2/sklego/decomposition/pca_reconstruction.py` & `scikit-lego-0.9.0/sklego/decomposition/pca_reconstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,21 +89,17 @@
             svd_solver=self.svd_solver,
             tol=self.tol,
             iterated_power=self.iterated_power,
             random_state=self.random_state,
         )
         self.pca_.fit(X, y)
         self.offset_ = -self.threshold
-        return self
 
-    def transform(self, X):
-        """Transform the data using the underlying PCA method."""
-        X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
-        check_is_fitted(self, ["pca_", "offset_"])
-        return self.pca_.transform(X)
+        self.n_features_in_ = X.shape[1]
+        return self
 
     def difference(self, X):
         """Return the calculated difference between original and reconstructed data. Row by row.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features )
```

### Comparing `scikit-lego-0.8.2/sklego/decomposition/umap_reconstruction.py` & `scikit-lego-0.9.0/sklego/decomposition/umap_reconstruction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 try:
     import umap
 except ImportError:
     from sklego.notinstalled import NotInstalledPackage
 
     umap = NotInstalledPackage("umap-learn")
 
+
 import numpy as np
 from sklearn.base import BaseEstimator, OutlierMixin
 from sklearn.utils.validation import FLOAT_DTYPES, check_array, check_is_fitted
 
 
 class UMAPOutlierDetection(BaseEstimator, OutlierMixin):
     """`UMAPOutlierDetection` is an outlier detector based on the reconstruction error from UMAP.
@@ -81,36 +82,32 @@
         Raises
         ------
         ValueError
             - If `n_components` is less than 2.
             - If `threshold` is `None`.
         """
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
-        if self.n_components < 2:
-            raise ValueError("Number of components must be at least two.")
+        if y is not None:
+            y = check_array(y, estimator=self, ensure_2d=False)
+
         if not self.threshold:
             raise ValueError("The `threshold` value cannot be `None`.")
 
         self.umap_ = umap.UMAP(
             n_components=self.n_components,
             n_neighbors=self.n_neighbors,
             min_dist=self.min_dist,
             metric=self.metric,
             random_state=self.random_state,
         )
         self.umap_.fit(X, y)
         self.offset_ = -self.threshold
+        self.n_features_in_ = X.shape[1]
         return self
 
-    def transform(self, X):
-        """Transform the data using the underlying UMAP method."""
-        X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
-        check_is_fitted(self, ["umap_", "offset_"])
-        return self.umap_.transform(X)
-
     def difference(self, X):
         """Return the calculated difference between original and reconstructed data. Row by row.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features )
             Data to calculate the difference for.
@@ -144,7 +141,19 @@
             The predicted data. 1 for inliers, -1 for outliers.
         """
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
         check_is_fitted(self, ["umap_", "offset_"])
         result = np.ones(X.shape[0])
         result[self.difference(X) > self.threshold] = -1
         return result.astype(int)
+
+    def decision_function(self, X):
+        """Calculate the decision function for the data as the difference between `threshold` and the `.difference(X)`
+        (which is the difference between original data and reconstructed data)."""
+        return self.threshold - self.difference(X)
+
+    def score_samples(self, X):
+        """Calculate the score for the samples"""
+        return -self.difference(X)
+
+    def _more_tags(self):
+        return {"non_deterministic": True}
```

### Comparing `scikit-lego-0.8.2/sklego/dummy.py` & `scikit-lego-0.9.0/sklego/dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,7 +120,10 @@
     def allowed_strategies(self):
         warn(
             "Please use `_ALLOWED_STRATEGIES` instead of `allowed_strategies`,"
             "`allowed_strategies` will be deprecated in future versions",
             DeprecationWarning,
         )
         return self._ALLOWED_STRATEGIES
+
+    def _more_tags(self):
+        return {"poor_score": True, "non_deterministic": True}
```

### Comparing `scikit-lego-0.8.2/sklego/feature_selection/mrmr.py` & `scikit-lego-0.9.0/sklego/feature_selection/mrmr.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,14 +126,16 @@
     selected_features = mrmr.selected_features_
 
     # Get the scores of the selected features
     feature_scores = mrmr.scores_
     ```
     """
 
+    _required_parameters = ["k"]
+
     def __init__(self, k, *, relevance_func="f", redundancy_func="p", kind="auto"):
         self.k = k
         self.relevance_func = relevance_func
         self.redundancy_func = redundancy_func
         self.kind = kind
 
     def _get_support_mask(self):
@@ -195,15 +197,15 @@
         Raises
         ------
         ValueError
             if:
 
                 k parameter is not integer type or is < n_features_in (X.shape[1]) or < 1
         """
-        X, y = check_X_y(X, y)
+        X, y = check_X_y(X, y, dtype="numeric", y_numeric=True)
         self._y_dtype = y.dtype
 
         relevance = self._get_relevance
         redundancy = self._get_redundancy
 
         self.n_features_in_ = X.shape[1]
         left_features = list(range(self.n_features_in_))
```

### Comparing `scikit-lego-0.8.2/sklego/linear_model.py` & `scikit-lego-0.9.0/sklego/linear_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 try:
     import cvxpy as cp
 except ImportError:
     from sklego.notinstalled import NotInstalledPackage
 
     cp = NotInstalledPackage("cvxpy")
-
+import logging
 from abc import ABC, abstractmethod
+from inspect import signature
 from warnings import warn
 
+import narwhals as nw
 import numpy as np
-import pandas as pd
 from scipy.optimize import minimize
 from scipy.special._ufuncs import expit
 from sklearn.base import BaseEstimator, RegressorMixin
 from sklearn.linear_model._base import LinearClassifierMixin
 from sklearn.multiclass import OneVsOneClassifier, OneVsRestClassifier
 from sklearn.preprocessing import LabelEncoder
 from sklearn.utils import check_X_y
@@ -80,14 +81,15 @@
         if self.span is not None:
             if not 0 <= self.span <= 1:
                 raise ValueError(f"Param `span` must be 0 <= span <= 1, got: {self.span}")
         if self.sigma < 0:
             raise ValueError(f"Param `sigma` must be >= 0, got: {self.sigma}")
         self.X_ = X
         self.y_ = y
+        self.n_features_in_ = X.shape[1]
         return self
 
     def _calc_wts(self, x_i):
         """Calculate the weights for a single point `x_i` using the training data `self.X_` and the parameters
         `self.sigma` and `self.span`. The weights are calculated as `np.exp(-(distances**2) / self.sigma)`,
         where distances are the distances between `x_i` and all the training samples.
 
@@ -487,23 +489,23 @@
         ValueError
             If `penalty` is not one of "l1" or "none".
         """
         if self.penalty not in ["l1", "none"]:
             raise ValueError(f"penalty should be either 'l1' or 'none', got {self.penalty}")
 
         self.sensitive_col_idx_ = self.sensitive_cols
-        if isinstance(X, pd.DataFrame):
+        X = nw.from_native(X, eager_only=True, strict=False)
+        if isinstance(X, nw.DataFrame):
             self.sensitive_col_idx_ = [i for i, name in enumerate(X.columns) if name in self.sensitive_cols]
         X, y = check_X_y(X, y, accept_large_sparse=False)
-
         sensitive = X[:, self.sensitive_col_idx_]
         if not self.train_sensitive_cols:
             X = np.delete(X, self.sensitive_col_idx_, axis=1)
-        X = self._add_intercept(X)
 
+        X = self._add_intercept(X)
         column_or_1d(y)
         label_encoder = LabelEncoder().fit(y)
         y = label_encoder.transform(y)
         self.classes_ = label_encoder.classes_
 
         if len(self.classes_) > 2:
             raise ValueError(
@@ -529,20 +531,28 @@
         )
         if self.penalty == "l1":
             log_likelihood -= cp.sum((1 / self.C) * cp.norm(theta[1:]))
 
         constraints = self.constraints(y_hat, y, sensitive, n_obs)
 
         problem = cp.Problem(cp.Maximize(log_likelihood), constraints)
-        problem.solve(max_iters=self.max_iter)
+
+        if "max_iters" in signature(problem.solve).parameters:
+            kwargs = {"max_iters": self.max_iter}
+        else:
+            if self.max_iter:
+                logging.warning("solver does not support `max_iters` and it `self.max_iter` will be ignored")
+            kwargs = {}
+
+        problem.solve(**kwargs)
 
         if problem.status in ["infeasible", "unbounded"]:
             raise ValueError(f"problem was found to be {problem.status}")
 
-        self.n_iter_ = problem.solver_stats.num_iters
+        self.n_iter_ = getattr(problem.solver_stats, "num_iters", 0)
 
         if self.fit_intercept:
             self.coef_ = theta.value[np.newaxis, 1:]
             self.intercept_ = theta.value[0:1]
         else:
             self.coef_ = theta.value[np.newaxis, :]
             self.intercept_ = np.array([0.0])
@@ -573,14 +583,17 @@
             X = np.delete(X, self.sensitive_col_idx_, axis=1)
         return super().decision_function(X)
 
     def _add_intercept(self, X):
         if self.fit_intercept:
             return np.c_[np.ones(len(X)), X]
 
+    def _more_tags(self):
+        return {"poor_score": True}
+
 
 class DemographicParityClassifier(BaseEstimator, LinearClassifierMixin):
     r"""`DemographicParityClassifier` is a logistic regression classifier which can be constrained on demographic
     parity (p% score).
 
     It minimizes the log loss while constraining the correlation between the specified `sensitive_cols` and the
     distance to the decision boundary of the classifier.
@@ -1013,25 +1026,24 @@
         overestimation_punishment_factor=1.0,
     ):
         super().__init__(alpha, l1_ratio, fit_intercept, copy_X, positive, method)
         self.overestimation_punishment_factor = overestimation_punishment_factor
 
     def _get_objective(self, X, y, sample_weight):
         def imbalanced_loss(params):
-            return 0.5 * np.mean(
-                sample_weight
-                * np.where(X @ params > y, self.overestimation_punishment_factor, 1)
-                * np.square(y - X @ params)
+            return 0.5 * np.average(
+                np.where(X @ params > y, self.overestimation_punishment_factor, 1) * np.square(y - X @ params),
+                weights=sample_weight,
             ) + self._regularized_loss(params)
 
         def grad_imbalanced_loss(params):
             return (
                 -(sample_weight * np.where(X @ params > y, self.overestimation_punishment_factor, 1) * (y - X @ params))
                 @ X
-                / X.shape[0]
+                / sample_weight.sum()
             ) + self._regularized_grad_loss(params)
 
         return imbalanced_loss, grad_imbalanced_loss
 
 
 class QuantileRegression(BaseScipyMinimizeRegressor):
     r"""Compute quantile regression. This can be used for computing confidence intervals of linear regressions.
@@ -1053,14 +1065,19 @@
 
     Compared to linear regression, this approach is robust to outliers.
 
     !!! info
         This implementation uses
         [scipy.optimize.minimize](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html).
 
+    !!! warning
+        If, while fitting the model, `sample_weight` contains any zero values, some solvers may not converge properly.
+        We would expect that a sample weight of zero is equivalent to removing the sample, however unittests tell us
+        that this is always the case only for `method='SLSQP'` (our default)
+
     Parameters
     ----------
     alpha : float, default=0.0
         Constant that multiplies the penalty terms.
     l1_ratio : float, default=0.0
         The ElasticNet mixing parameter, with `0 <= l1_ratio <= 1`:
 
@@ -1124,23 +1141,24 @@
         quantile=0.5,
     ):
         super().__init__(alpha, l1_ratio, fit_intercept, copy_X, positive, method)
         self.quantile = quantile
 
     def _get_objective(self, X, y, sample_weight):
         def quantile_loss(params):
-            return np.mean(
-                sample_weight * np.where(X @ params < y, self.quantile, 1 - self.quantile) * np.abs(y - X @ params)
+            return np.average(
+                np.where(X @ params < y, self.quantile, 1 - self.quantile) * np.abs(y - X @ params),
+                weights=sample_weight,
             ) + self._regularized_loss(params)
 
         def grad_quantile_loss(params):
             return (
                 -(sample_weight * np.where(X @ params < y, self.quantile, 1 - self.quantile) * np.sign(y - X @ params))
                 @ X
-                / X.shape[0]
+                / sample_weight.sum()
             ) + self._regularized_grad_loss(params)
 
         return quantile_loss, grad_quantile_loss
 
     def fit(self, X, y, sample_weight=None):
         """Fit the estimator on training data `X` and `y` by minimizing the quantile loss function.
 
@@ -1182,14 +1200,19 @@
     Compared to linear regression, this approach is robust to outliers. You can even optimize for the lowest MAPE
     (Mean Average Percentage Error), by providing `sample_weight=np.abs(1/y_train)` when fitting the regressor.
 
     !!! info
         This implementation uses
         [scipy.optimize.minimize](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html).
 
+    !!! warning
+        If, while fitting the model, `sample_weight` contains any zero values, some solvers may not converge properly.
+        We would expect that a sample weight of zero is equivalent to removing the sample, however unittests tell us
+        that this is always the case only for `method='SLSQP'` (our default)
+
     Parameters
     ----------
     alpha : float, default=0.0
         Constant that multiplies the penalty terms.
     l1_ratio : float, default=0.0
         The ElasticNet mixing parameter, with `0 <= l1_ratio <= 1`:
```

### Comparing `scikit-lego-0.8.2/sklego/meta/__init__.py` & `scikit-lego-0.9.0/sklego/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/meta/_decay_utils.py` & `scikit-lego-0.9.0/sklego/meta/_decay_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/meta/_shrinkage_utils.py` & `scikit-lego-0.9.0/sklego/meta/_shrinkage_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from functools import partial
+
+import narwhals as nw
 import numpy as np
 from sklearn.utils.validation import check_is_fitted
 
-from sklego.common import expanding_list
+from sklego.common import as_list, expanding_list
 
 
 def constant_shrinkage(group_sizes, alpha: float) -> np.ndarray:
     r"""The augmented prediction for each level is the weighted average between its prediction and the augmented
     prediction for its parent.
 
     Let $\hat{y}_i$ be the prediction at level $i$, with $i=0$ being the root, than the augmented prediction
@@ -43,14 +46,19 @@
     -------
     np.ndarray
         The weights for each group.
     """
     return np.asarray(group_sizes)
 
 
+def no_shrinkage_function(x, n):
+    # n = len(self.fitted_levels_[-1])
+    return np.pad([1], (len(x) - 1, n - len(x)), "constant", constant_values=(0))
+
+
 def min_n_obs_shrinkage(group_sizes, min_n_obs: int) -> np.ndarray:
     """Use only the smallest group with a certain amount of observations.
 
     Parameters
     ----------
     group_sizes : array-like
         The number of observations in each group.
@@ -113,15 +121,15 @@
 
         elif callable(self.shrinkage):
             self.__check_shrinkage_func()
             shrinkage_function_ = self.shrinkage
 
         elif self.shrinkage is None:
             """Instead of keeping two different behaviors for shrinkage and non-shrinkage cases, this conditional block
-            maps no shrinkage to a constant shrinkage function, wit  all the weight on the grouped passed,
+            maps no shrinkage to a constant shrinkage function, with all the weight on the grouped passed,
             independently from the level sizes, as expected from the other shrinkage functions (*).
             This allows the rest of the code to be agnostic to the shrinkage function, and the shrinkage factors.
 
             (*) Consider the following example:
 
             - groups = ["a", "b"] with values (0, 0), (0, 1) and (1, 0) of respective sizes 6, 5, 9.
             - Considering these sizes, in `__fit_shrinkage_factors` the hierarchical_counts will be:
@@ -146,19 +154,15 @@
                     (1, 1): array([0., 1., 0.]),
                     (1, 0, 0): array([0., 0., 1.]),
                     (1, 0, 1): array([0., 0., 1.]),
                     (1, 1, 0): array([0., 0., 1.])
                 }
             """
 
-            def no_shrinkage_function(x):
-                n = len(self.fitted_levels_[-1])
-                return np.lib.pad([1], (len(x) - 1, n - len(x)), "constant", constant_values=(0))
-
-            shrinkage_function_ = no_shrinkage_function
+            shrinkage_function_ = partial(no_shrinkage_function, n=self.n_fitted_levels_)
 
         else:
             raise ValueError(
                 f"`shrinkage` should be either `None`, {self._ALLOWED_SHRINKAGE.keys()}, or a callable. "
                 f"Found {self.shrinkage} of type {type(self.shrinkage)}"
             )
         return shrinkage_function_
@@ -186,25 +190,31 @@
             The DataFrame to group by.
         groups : list[str | int]
             The columns to group by.
         most_granular_only : bool
             Whether to return only the shrinkage factors for the most granular group values.
         """
         check_is_fitted(self, ["estimators_", "shrinkage_function_"])
-        counts = frame.groupby(groups).size().rename("counts")
+        counts = frame.group_by(groups).agg(nw.len().alias("counts"))
         all_grp_values = list(self.estimators_.keys())
 
         if most_granular_only:
-            all_grp_values = [grp_value for grp_value in all_grp_values if len(grp_value) == len(groups)]
+            all_grp_values = [grp_value for grp_value in all_grp_values if len(as_list(grp_value)) == len(groups)]
 
         hierarchical_counts = {
-            grp_value: [counts.loc[subgroup].sum() for subgroup in expanding_list(grp_value, tuple)]
+            grp_value: [
+                # As zip is "zip shortest" and filter works with comma separate conditions:
+                counts.filter(*[nw.col(c) == v for c, v in zip(groups, subgroup)])
+                .select(nw.sum("counts"))
+                .to_numpy()[0][0]
+                for subgroup in expanding_list(grp_value, tuple)
+            ]
             for grp_value in all_grp_values
         }
 
         shrinkage_factors = {
-            grp_value: self.shrinkage_function_(counts, **self.shrinkage_kwargs)
-            for grp_value, counts in hierarchical_counts.items()
+            grp_value: self.shrinkage_function_(counts_, **self.shrinkage_kwargs)
+            for grp_value, counts_ in hierarchical_counts.items()
         }
 
         # Normalize and pad
         return {grp_value: shrink_array / shrink_array.sum() for grp_value, shrink_array in shrinkage_factors.items()}
```

### Comparing `scikit-lego-0.8.2/sklego/meta/confusion_balancer.py` & `scikit-lego-0.9.0/sklego/meta/confusion_balancer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from sklearn import clone
 from sklearn.base import BaseEstimator, ClassifierMixin, MetaEstimatorMixin
 from sklearn.metrics import confusion_matrix
 from sklearn.utils.multiclass import unique_labels
 from sklearn.utils.validation import FLOAT_DTYPES, check_array, check_is_fitted, check_X_y
 
 from sklego.base import ProbabilisticClassifier
 
 
-class ConfusionBalancer(BaseEstimator, ClassifierMixin, MetaEstimatorMixin):
+class ConfusionBalancer(BaseEstimator, MetaEstimatorMixin, ClassifierMixin):
     r"""The `ConfusionBalancer` estimator attempts to give it's child estimator a more balanced output by learning from
     the confusion matrix during training.
 
     The idea is that the confusion matrix calculates $P(C_i | M_i)$ where $C_i$ is the actual class and $M_i$ is the
     class that the underlying model gives. We use these probabilities to attempt a more balanced prediction by averaging
     the correction from the confusion matrix with the original probabilities.
 
@@ -29,14 +30,16 @@
     ----------
     classes_ : array-like of shape (n_classes,)
         The target class labels.
     cfm_ : array-like of shape (n_classes, n_classes)
         The confusion matrix used for the correction.
     """
 
+    _required_parameters = ["estimator"]
+
     def __init__(self, estimator, alpha: float = 0.5, cfm_smooth=0):
         self.estimator = estimator
         self.alpha = alpha
         self.cfm_smooth = cfm_smooth
 
     def fit(self, X, y):
         """Fit the underlying estimator on the training data `X` and `y`, it calculates the confusion matrix,
@@ -61,18 +64,19 @@
         """
 
         X, y = check_X_y(X, y, estimator=self.estimator, dtype=FLOAT_DTYPES)
         if not isinstance(self.estimator, ProbabilisticClassifier):
             raise ValueError(
                 "The ConfusionBalancer meta model only works on classification models with .predict_proba."
             )
-        self.estimator.fit(X, y)
+        self.estimator_ = clone(self.estimator).fit(X, y)
         self.classes_ = unique_labels(y)
-        cfm = confusion_matrix(y, self.estimator.predict(X)).T + self.cfm_smooth
+        cfm = confusion_matrix(y, self.estimator_.predict(X)).T + self.cfm_smooth
         self.cfm_ = cfm / cfm.sum(axis=1).reshape(-1, 1)
+        self.n_features_in_ = X.shape[1]
         return self
 
     def predict_proba(self, X):
         """Predict probabilities for new data `X` using the underlying estimator and then applying the confusion matrix
         correction.
 
         Parameters
@@ -81,16 +85,17 @@
             The data to predict.
 
         Returns
         -------
         array-like of shape (n_samples, n_classes)
             The predicted values.
         """
-        X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
-        preds = self.estimator.predict_proba(X)
+        check_is_fitted(self, ["cfm_", "classes_", "estimator_"])
+        X = check_array(X, dtype=FLOAT_DTYPES)
+        preds = self.estimator_.predict_proba(X)
         return (1 - self.alpha) * preds + self.alpha * preds @ self.cfm_
 
     def predict(self, X):
         """Predict most likely class for new data `X` using the underlying estimator.
 
         Parameters
         ----------
@@ -98,10 +103,10 @@
             The data to predict.
 
         Returns
         -------
         array-like of shape (n_samples,)
             The predicted values.
         """
-        check_is_fitted(self, ["cfm_", "classes_"])
-        X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
+        check_is_fitted(self, ["cfm_", "classes_", "estimator_"])
+        X = check_array(X, dtype=FLOAT_DTYPES)
         return self.classes_[self.predict_proba(X).argmax(axis=1)]
```

### Comparing `scikit-lego-0.8.2/sklego/meta/decay_estimator.py` & `scikit-lego-0.9.0/sklego/meta/decay_estimator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sklearn import clone
-from sklearn.base import BaseEstimator
+from sklearn.base import BaseEstimator, MetaEstimatorMixin
 from sklearn.utils.validation import FLOAT_DTYPES, check_is_fitted, check_X_y
 
 from sklego.meta._decay_utils import exponential_decay, linear_decay, sigmoid_decay, stepwise_decay
 
 
-class DecayEstimator(BaseEstimator):
+class DecayEstimator(BaseEstimator, MetaEstimatorMixin):
     """Morphs an estimator such that the training weights can be adapted to ensure that points that are far away have
     less weight.
 
     This meta estimator will only work for estimators that allow a `sample_weights` argument in their `.fit()` method.
     The meta estimator `.fit()` method computes the weights to pass to the estimator's `.fit()` method.
 
     !!! warning
@@ -81,14 +81,16 @@
     _ALLOWED_DECAYS = {
         "linear": linear_decay,
         "exponential": exponential_decay,
         "stepwise": stepwise_decay,
         "sigmoid": sigmoid_decay,
     }
 
+    _required_parameters = ["model"]
+
     def __init__(self, model, decay_func="exponential", check_input=False, **decay_kwargs):
         self.model = model
         self.decay_func = decay_func
         self.check_input = check_input
         self.decay_kwargs = decay_kwargs
 
     def _is_classifier(self):
@@ -133,14 +135,16 @@
             self.estimator_.fit(X, y, sample_weight=self.weights_)
         except TypeError as e:
             if "sample_weight" in str(e):
                 raise TypeError(f"Model {type(self.model).__name__}.fit() does not have 'sample_weight'")
 
         if self._is_classifier():
             self.classes_ = self.estimator_.classes_
+
+        self.n_features_in_ = X.shape[1]
         return self
 
     def predict(self, X):
         """Predict target values for `X` using trained underlying estimator.
 
         Parameters
         ----------
```

### Comparing `scikit-lego-0.8.2/sklego/meta/estimator_transformer.py` & `scikit-lego-0.9.0/sklego/meta/estimator_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
         if self.check_input:
             X, y = check_X_y(X, y, estimator=self, dtype=FLOAT_DTYPES, multi_output=True)
 
         self.multi_output_ = len(y.shape) > 1
         self.estimator_ = clone(self.estimator)
         self.estimator_.fit(X, y, **kwargs)
+        self.n_features_in_ = X.shape[1]
         return self
 
     def transform(self, X):
         """Transform the data by applying the `predict_func` of the fitted estimator.
 
         Parameters
         ----------
```

### Comparing `scikit-lego-0.8.2/sklego/meta/grouped_predictor.py` & `scikit-lego-0.9.0/sklego/meta/grouped_predictor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+from copy import deepcopy
+from typing import List, Union
+
+import narwhals as nw
 import numpy as np
 import pandas as pd
 from sklearn import clone
 from sklearn.base import BaseEstimator, ClassifierMixin, MetaEstimatorMixin, RegressorMixin, is_classifier, is_regressor
 from sklearn.utils.metaestimators import available_if
-from sklearn.utils.validation import check_array, check_is_fitted
+from sklearn.utils.validation import check_is_fitted
 
 from sklego.common import as_list, expanding_list
-from sklego.meta._grouped_utils import _split_groups_and_values
+from sklego.meta._grouped_utils import parse_X_y
 from sklego.meta._shrinkage_utils import (
     ShrinkageMixin,
     constant_shrinkage,
     equal_shrinkage,
     min_n_obs_shrinkage,
     relative_shrinkage,
 )
@@ -82,14 +86,16 @@
     _ALLOWED_SHRINKAGE = {
         "constant": constant_shrinkage,
         "relative": relative_shrinkage,
         "min_n_obs": min_n_obs_shrinkage,
         "equal": equal_shrinkage,
     }
 
+    _required_parameters = ["estimator", "groups"]
+
     def __init__(
         self,
         estimator,
         groups,
         shrinkage=None,
         use_global_model=True,
         check_X=True,
@@ -105,68 +111,59 @@
     def __fit_single_group(self, group, X, y=None):
         """Fit estimator to the given group."""
         try:
             return clone(self.estimator).fit(X, y)
         except Exception as e:
             raise type(e)(f"Exception for group {group}: {e}")
 
-    def __fit_grouped_estimator(self, X_group, X_value, y=None, columns=None):
+    def __fit_grouped_estimator(
+        self, frame: nw.DataFrame, y: Union[np.ndarray, None] = None, columns: Union[List[int], List[str], None] = None
+    ):
         """Fit an estimator to each group"""
-        # Reset indices such that they are the same in X and y
-        if not columns:
-            columns = X_group.columns.tolist()
 
-        # Make the groups based on the groups dataframe, use the indices on the values array
-        try:
-            group_indices = X_group.groupby(columns).indices
-        except TypeError:
-            # This one is needed because of line #918 of sklearn/utils/estimator_checks
-            raise TypeError("argument must be a string, date or number")
-
-        if y is not None:
-            if isinstance(y, pd.Series):
-                y.index = X_group.index
-
-            grouped_estimators = {
-                # Fit a clone of the transformer to each group
-                group: self.__fit_single_group(group, X_value[indices, :], y[indices])
-                for group, indices in group_indices.items()
-            }
-        else:
-            grouped_estimators = {
-                group: self.__fit_single_group(group, X_value[indices, :]) for group, indices in group_indices.items()
-            }
+        if columns is None:
+            columns = self._groups
+
+        grouped_estimators = {
+            # Fit a clone of the estimators to each group
+            (group_name[0] if len(group_name) == 1 else group_name): self.__fit_single_group(
+                group=(group_name[0] if len(group_name) == 1 else group_name),
+                X=nw.to_native(X_grp.drop(["__sklego_target__", *columns, *as_list(self.groups)])),
+                y=(nw.to_native(X_grp.select("__sklego_target__")).to_numpy().reshape(-1) if y is not None else None),
+            )
+            for group_name, X_grp in frame.group_by(columns)
+        }
 
         return grouped_estimators
 
-    def __fit_shrinkage_groups(self, X_group, X_value, y):
+    def __fit_shrinkage_groups(self, frame, y):
         estimators = {}
 
         for grouping_colnames in self.group_colnames_hierarchical_:
             # Fit a grouped estimator to each (sub)group hierarchically
-            estimators.update(self.__fit_grouped_estimator(X_group, X_value, y, columns=grouping_colnames))
+            estimators.update(self.__fit_grouped_estimator(frame, y, columns=grouping_colnames))
 
         return estimators
 
-    def __add_shrinkage_column(self, X_group):
+    def __add_shrinkage_column(self, frame, groups=None):
         """Add global group as first column if needed for shrinkage"""
 
         if self.shrinkage is not None and self.use_global_model:
-            return pd.concat(
-                [
-                    pd.Series(
-                        [self._global_col_value] * len(X_group),
-                        name=self._global_col_name,
-                    ),
-                    X_group,
-                ],
-                axis=1,
+            n_samples = frame.shape[0]
+            native_space = nw.get_native_namespace(frame)
+
+            frame = frame.select(
+                nw.from_native(native_space.Series([self._global_col_value] * n_samples), allow_series=True).alias(
+                    self._global_col_name
+                ),
+                nw.all(),
             )
+            groups = [self._global_col_name] if groups is None else [self._global_col_name, *groups]
 
-        return X_group
+        return frame, groups
 
     def fit(self, X, y=None):
         """Fit one estimator for each group of training data `X` and `y`.
 
         Will also learn the groups that exist within the dataset.
 
         If `use_global_model=True` a fallback estimator will be fitted on the entire dataset in case a group is not
@@ -183,71 +180,86 @@
         -------
         self : GroupedPredictor
             The fitted estimator.
         """
         if self.shrinkage is not None and not is_regressor(self.estimator):
             raise ValueError("Shrinkage is only available for regression models")
 
-        X_group, X_value = _split_groups_and_values(
-            X, self.groups, min_value_cols=0, check_X=self.check_X, **self._check_kwargs
-        )
-
-        X_group = self.__add_shrinkage_column(X_group)
+        _group_cols = as_list(deepcopy(self.groups)) if self.groups is not None else None
 
-        if y is not None:
-            y = check_array(y, ensure_2d=False)
+        if (
+            self.shrinkage is not None
+            and _group_cols is not None
+            and len(_group_cols) == 1
+            and not self.use_global_model
+        ):
+            raise ValueError("Shrinkage is not null, but found a total of 1 groups")
+
+        X = nw.from_native(X, strict=False, eager_only=True)
+
+        frame = parse_X_y(X, y, _group_cols, check_X=self.check_X, **self._check_kwargs)
+        frame, _group_cols = self.__add_shrinkage_column(frame, _group_cols)
+        self.n_features_in_ = frame.shape[1] - 1
+        self.n_fitted_levels_ = 1 + self.use_global_model
 
         self.shrinkage_function_ = self._set_shrinkage_function()
 
         # List of all hierarchical subsets of columns
-        self.group_colnames_hierarchical_ = expanding_list(X_group.columns, list)
-
+        self.group_colnames_hierarchical_ = expanding_list(_group_cols, list)
         self.fallback_ = None
 
         if self.shrinkage is None and self.use_global_model:
-            self.fallback_ = clone(self.estimator).fit(X_value, y)
+            X_ = nw.to_native(frame.drop([*_group_cols, "__sklego_target__"]))
+            y_ = nw.to_native(frame["__sklego_target__"])
+
+            self.fallback_ = clone(self.estimator).fit(X_, y_)
 
         if self.shrinkage is not None:
-            self.estimators_ = self.__fit_shrinkage_groups(X_group, X_value, y)
+            self.estimators_ = self.__fit_shrinkage_groups(frame, y)
         else:
-            self.estimators_ = self.__fit_grouped_estimator(X_group, X_value, y)
+            self.estimators_ = self.__fit_grouped_estimator(frame, y, columns=_group_cols)
 
         self.groups_ = as_list(self.estimators_.keys())
 
         if self.shrinkage is not None:
-            _groups = [self._global_col_name] + as_list(self.groups) if self.use_global_model else as_list(self.groups)
-            self.shrinkage_factors_ = self._fit_shrinkage_factors(X_group, groups=_groups, most_granular_only=True)
+            _groups = (
+                [self._global_col_name, *as_list(deepcopy(self.groups))]
+                if self.use_global_model
+                else as_list(deepcopy(self.groups))
+            )
+
+            self.shrinkage_factors_ = self._fit_shrinkage_factors(frame, groups=_groups, most_granular_only=True)
+            self.shrinkage_factors_ = {(k[0] if len(k) == 1 else k): v for k, v in self.shrinkage_factors_.items()}
 
         return self
 
-    def __predict_shrinkage_groups(self, X_group, X_value, method="predict"):
+    def __predict_shrinkage_groups(self, frame, method="predict", groups=None):
         """Make predictions for all shrinkage groups"""
         # DataFrame with predictions for each hierarchy level, per row. Missing groups errors are thrown here.
         hierarchical_predictions = pd.concat(
             [
-                pd.Series(self.__predict_groups(X_group, X_value, level_columns, method=method))
+                pd.Series(self.__predict_groups(frame, method=method, groups=level_columns))
                 for level_columns in self.group_colnames_hierarchical_
             ],
             axis=1,
         )
 
         # This is a Series with values the tuples of hierarchical grouping
-        prediction_groups = pd.Series([tuple(_) for _ in X_group.itertuples(index=False)])
+        prediction_groups = pd.Series([tuple(_) for _ in frame.select(groups).to_pandas().itertuples(index=False)])
 
         # This is a Series of arrays
         shrinkage_factors = prediction_groups.map(self.shrinkage_factors_)
 
         # Convert the Series of arrays it to a DataFrame
         shrinkage_factors = pd.DataFrame.from_dict(shrinkage_factors.to_dict()).T
+
         return (hierarchical_predictions * shrinkage_factors).sum(axis=1)
 
     def __predict_single_group(self, group, X, method="predict"):
         """Predict a single group by getting its estimator from the fitted dict"""
-        # Keep track of the original index such that we can sort in __predict_groups
-        index = X.index
 
         try:
             group_predictor = self.estimators_[group]
         except KeyError:
             if self.fallback_:
                 group_predictor = self.fallback_
             else:
@@ -255,46 +267,37 @@
 
         is_predict_proba = is_classifier(group_predictor) and method == "predict_proba"
         # Ensure to provide pd.DataFrame with the correct label name
         extra_kwargs = {"columns": group_predictor.classes_} if is_predict_proba else {}
 
         # getattr(group_predictor, method) returns the predict method of the fitted model
         # if the method argument is "predict" and the predict_proba method if method argument is "predict_proba"
-        return pd.DataFrame(getattr(group_predictor, method)(X), **extra_kwargs).set_index(index)
+        return pd.DataFrame(getattr(group_predictor, method)(X), **extra_kwargs)
 
-    def __predict_groups(
-        self,
-        X_group: pd.DataFrame,
-        X_value: np.array,
-        group_cols=None,
-        method="predict",
-    ):
+    def __predict_groups(self, frame: nw.DataFrame, method="predict", groups=None):
         """Predict for all groups"""
-        # Reset indices such that they are the same in X_group (reset in __check_grouping_columns),
-        # this way we can track the order of the result
-        X_value = pd.DataFrame(X_value).reset_index(drop=True)
-
-        if group_cols is None:
-            group_cols = X_group.columns.tolist()
-
-        # Make the groups based on the groups dataframe, use the indices on the values array
-        group_indices = X_group.groupby(group_cols).indices
 
+        n_samples = frame.shape[0]
+        frame = frame.with_columns(__sklego_index__=np.arange(n_samples))
         return (
             pd.concat(
                 [
-                    self.__predict_single_group(group, X_value.loc[indices, :], method=method)
-                    for group, indices in group_indices.items()
+                    self.__predict_single_group(
+                        (group_value[0] if len(group_value) == 1 else group_value),
+                        nw.to_native(X_grp.drop(["__sklego_index__", *groups, *as_list(self.groups)])),
+                        method=method,
+                    ).set_index(nw.to_native(X_grp["__sklego_index__"]).to_numpy().reshape(-1).astype(int))
+                    for group_value, X_grp in frame.group_by(groups)
                 ],
                 axis=0,
             )
-            # Fill with prob = 0 for impossible labels in predict_proba
             .fillna(0)
             .sort_index()
-            .values.squeeze()
+            .to_numpy()
+            .squeeze()
         )
 
     def predict(self, X):
         """Predict target values on new data `X` by predicting on each group. If a group is not found during
         `.predict()` and `use_global_model=True` the fallback estimator will be used. If `use_global_model=False` a
         `ValueError` will be raised.
 
@@ -306,24 +309,25 @@
         Returns
         -------
         array-like of shape (n_samples,)
             Predicted target values.
         """
         check_is_fitted(self, ["estimators_", "groups_", "fallback_"])
 
-        X_group, X_value = _split_groups_and_values(
-            X, self.groups, min_value_cols=0, check_X=self.check_X, **self._check_kwargs
+        _group_cols = as_list(deepcopy(self.groups)) if self.groups is not None else None
+        X = nw.from_native(X, strict=False, eager_only=True)
+        frame = parse_X_y(X, y=None, groups=_group_cols, check_X=self.check_X, **self._check_kwargs).drop(
+            "__sklego_target__"
         )
-
-        X_group = self.__add_shrinkage_column(X_group)
+        frame, _group_cols = self.__add_shrinkage_column(frame, _group_cols)
 
         if self.shrinkage is None:
-            return self.__predict_groups(X_group, X_value, method="predict")
+            return self.__predict_groups(frame, method="predict", groups=_group_cols)
         else:
-            return self.__predict_shrinkage_groups(X_group, X_value, method="predict")
+            return self.__predict_shrinkage_groups(frame, method="predict", groups=_group_cols)
 
     # This ensures that the meta-estimator only has the predict_proba method if the estimator has it
     @available_if(lambda self: hasattr(self.estimator, "predict_proba"))
     def predict_proba(self, X):
         """Predict probabilities on new data `X`.
 
         !!! warning
@@ -337,24 +341,25 @@
         Returns
         -------
         array-like of shape (n_samples, n_classes)
             Predicted probabilities per class.
         """
         check_is_fitted(self, ["estimators_", "groups_", "fallback_"])
 
-        X_group, X_value = _split_groups_and_values(
-            X, self.groups, min_value_cols=0, check_X=self.check_X, **self._check_kwargs
+        _group_cols = as_list(deepcopy(self.groups)) if self.groups is not None else None
+        X = nw.from_native(X, strict=False, eager_only=True)
+        frame = parse_X_y(X, y=None, groups=_group_cols, check_X=self.check_X, **self._check_kwargs).drop(
+            "__sklego_target__"
         )
-
-        X_group = self.__add_shrinkage_column(X_group)
+        frame, _group_cols = self.__add_shrinkage_column(frame, _group_cols)
 
         if self.shrinkage is None:
-            return self.__predict_groups(X_group, X_value, method="predict_proba")
+            return self.__predict_groups(frame, method="predict_proba", groups=_group_cols)
         else:
-            return self.__predict_shrinkage_groups(X_group, X_value, method="predict_proba")
+            return self.__predict_shrinkage_groups(frame, method="predict_proba", groups=_group_cols)
 
     # This ensures that the meta-estimator only has the predict_proba method if the estimator has it
     @available_if(lambda self: hasattr(self.estimator, "decision_function"))
     def decision_function(self, X):
         """Predict confidence scores for samples in `X`.
 
         !!! warning
@@ -370,30 +375,35 @@
         array-like of shape (n_samples,) or (n_samples, n_classes)
             Confidence scores per (n_samples, n_classes) combination.
             In the binary case, confidence score for self.classes_[1] where > 0 means this class would be
             predicted.
         """
         check_is_fitted(self, ["estimators_", "groups_", "fallback_"])
 
-        X_group, X_value = _split_groups_and_values(
-            X, self.groups, min_value_cols=0, check_X=self.check_X, **self._check_kwargs
-        )
+        _group_cols = as_list(deepcopy(self.groups)) if self.groups is not None else None
+        X = nw.from_native(X, strict=False, eager_only=True)
 
-        X_group = self.__add_shrinkage_column(X_group)
+        frame = parse_X_y(X, y=None, groups=_group_cols, check_X=self.check_X, **self._check_kwargs).drop(
+            "__sklego_target__"
+        )
+        frame, _group_cols = self.__add_shrinkage_column(frame, _group_cols)
 
         if self.shrinkage is None:
-            return self.__predict_groups(X_group, X_value, method="decision_function")
+            return self.__predict_groups(frame, method="decision_function", groups=_group_cols)
         else:
-            return self.__predict_shrinkage_groups(X_group, X_value, method="decision_function")
+            return self.__predict_shrinkage_groups(frame, method="decision_function", groups=_group_cols)
 
     @property
     def _estimator_type(self):
         """Computes `_estimator_type` dynamically from the wrapped model."""
         return self.estimator._estimator_type
 
+    def _more_tags(self):
+        return {"allow_nan": True}
+
 
 class GroupedRegressor(GroupedPredictor, RegressorMixin):
     """`GroupedRegressor` is a meta-estimator that fits a separate regressor for each group in the input data.
 
     Its spec is the same as [`GroupedPredictor`][sklego.meta.grouped_predictor.GroupedPredictor] but it is available
     only for regression models.
```

### Comparing `scikit-lego-0.8.2/sklego/meta/grouped_transformer.py` & `scikit-lego-0.9.0/sklego/meta/grouped_transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from typing import Union
+
+import narwhals as nw
 import numpy as np
-import pandas as pd
-from sklearn.base import BaseEstimator, TransformerMixin, clone
+from sklearn.base import BaseEstimator, MetaEstimatorMixin, TransformerMixin, clone
 from sklearn.utils.validation import check_is_fitted
 
-from sklego.meta._grouped_utils import _split_groups_and_values
+from sklego.common import as_list
+from sklego.meta._grouped_utils import parse_X_y
 
 
-class GroupedTransformer(BaseEstimator, TransformerMixin):
+class GroupedTransformer(TransformerMixin, MetaEstimatorMixin, BaseEstimator):
     """Construct a transformer per data group. Splits data by groups from single or multiple columns and transforms
     remaining columns using the transformers corresponding to the groups.
 
     Parameters
     ----------
     transformer : scikit-learn compatible transformer
         The transformer to be applied per group.
@@ -28,14 +31,15 @@
         The fitted transformers per group or a single fitted transformer if `groups` is `None`.
     fallback_ : scikit-learn compatible transformer | None
         The fitted transformer to fall back to in case a group is not found during `.transform()`. Only present if
         `use_global_model` is `True`.
     """
 
     _check_kwargs = {"accept_large_sparse": False}
+    _required_parameters = ["transformer", "groups"]
 
     def __init__(self, transformer, groups, use_global_model=True, check_X=True):
         self.transformer = transformer
         self.groups = groups
         self.use_global_model = use_global_model
         self.check_X = check_X
 
@@ -57,36 +61,26 @@
             The fitted transformer for the group.
         """
         try:
             return clone(self.transformer).fit(X, y)
         except Exception as e:
             raise type(e)(f"Exception for group {group}: {e}")
 
-    def __fit_grouped_transformer(self, X_group: pd.DataFrame, X_value: np.ndarray, y=None):
+    def __fit_grouped_transformer(self, frame: nw.DataFrame, y: Union[np.ndarray, None]):
         """Fit a transformer to each group"""
-        # Make the groups based on the groups dataframe, use the indices on the values array
-        try:
-            group_indices = X_group.groupby(X_group.columns.tolist()).indices
-        except TypeError:
-            # This one is needed because of line #918 of sklearn/utils/estimator_checks
-            raise TypeError("argument must be a string, date or number")
-
-        if y is not None:
-            if isinstance(y, pd.Series):
-                y.index = X_group.index
-
-            grouped_transformers = {
-                # Fit a clone of the transformer to each group
-                group: self.__fit_single_group(group, X_value[indices, :], y[indices])
-                for group, indices in group_indices.items()
-            }
-        else:
-            grouped_transformers = {
-                group: self.__fit_single_group(group, X_value[indices, :]) for group, indices in group_indices.items()
-            }
+
+        grouped_transformers = {
+            # Fit a clone of the transformer to each group
+            group_name: self.__fit_single_group(
+                group_name,
+                X=nw.to_native(X_grp.drop(["__sklego_target__", *self.groups_])),
+                y=(nw.to_native(X_grp["__sklego_target__"]) if y is not None else None),
+            )
+            for group_name, X_grp in frame.group_by(self.groups_)
+        }
 
         return grouped_transformers
 
     def __check_transformer(self):
         """Check if the supplied transformer has a `transform` method and raise a `ValueError` if not."""
         if not hasattr(self.transformer, "transform"):
             raise ValueError("The supplied transformer should have a 'transform' method")
@@ -109,63 +103,79 @@
 
         Returns
         -------
         self : GroupedTransformer
             The fitted transformer.
         """
         self.__check_transformer()
-
         self.fallback_ = None
+        self.groups_ = as_list(self.groups) if self.groups is not None else None
+
+        X = nw.from_native(X, strict=False, eager_only=True)
+        if not isinstance(X, nw.DataFrame) and self.groups_ is not None:
+            # Accounts for negative indices if X is an array
+            self.groups_ = [
+                X.shape[1] + group if isinstance(group, int) and group < 0 else group for group in self.groups_
+            ]
+
+        frame = parse_X_y(X, y, self.groups_, check_X=self.check_X, **self._check_kwargs)
 
         if self.groups is None:
-            self.transformers_ = clone(self.transformer).fit(X, y)
+            X_, y_ = (
+                nw.to_native(frame.drop("__sklego_target__")),
+                nw.to_native(frame["__sklego_target__"]) if y is not None else None,
+            )
+            self.transformers_ = clone(self.transformer).fit(X_, y=y_)
             return self
 
-        X_group, X_value = _split_groups_and_values(X, self.groups, check_X=self.check_X, **self._check_kwargs)
-        self.transformers_ = self.__fit_grouped_transformer(X_group, X_value, y)
+        self.transformers_ = self.__fit_grouped_transformer(frame, y)
 
         if self.use_global_model:
-            self.fallback_ = clone(self.transformer).fit(X_value, y)
+            X_, y_ = (
+                nw.to_native(frame.drop(["__sklego_target__", *self.groups_])),
+                nw.to_native(frame["__sklego_target__"]) if y is not None else None,
+            )
+            self.fallback_ = clone(self.transformer).fit(X_, y_)
 
+        self.n_features_in_ = X.shape[1]
         return self
 
     def __transform_single_group(self, group, X):
         """Transform a single group by getting its transformer from the fitted dict"""
-        # Keep track of the original index such that we can sort in __transform_groups
-        index = X.index
         try:
             group_transformer = self.transformers_[group]
         except KeyError:
             if self.fallback_:
                 group_transformer = self.fallback_
             else:
                 raise ValueError(f"Found new group {group} during transform with use_global_model = False")
 
-        return pd.DataFrame(group_transformer.transform(X)).set_index(index)
+        return np.asarray(group_transformer.transform(X))
 
-    def __transform_groups(self, X_group: pd.DataFrame, X_value: np.ndarray):
+    def __transform_groups(self, frame: nw.DataFrame):
         """Transform all groups"""
-        # Reset indices such that they are the same in X_group (reset in __check_grouping_columns),
-        # this way we can track the order of the result
-        X_value = pd.DataFrame(X_value).reset_index(drop=True)
-
-        # Make the groups based on the groups dataframe, use the indices on the values array
-        group_indices = X_group.groupby(X_group.columns.tolist()).indices
-
-        return (
-            pd.concat(
-                [
-                    self.__transform_single_group(group, X_value.loc[indices, :])
-                    for group, indices in group_indices.items()
-                ],
-                axis=0,
+
+        n_samples = frame.shape[0]
+        frame = frame.with_columns(__sklego_index__=np.arange(n_samples))
+
+        results = [
+            (
+                nw.to_native(X_grp.select("__sklego_index__")).to_numpy().squeeze().astype(int),
+                self.__transform_single_group(
+                    group_name, nw.to_native(X_grp.drop(["__sklego_index__", *self.groups_]))
+                ),
             )
-            .sort_index()
-            .to_numpy()
-        )
+            for group_name, X_grp in frame.group_by(self.groups_)
+        ]
+
+        output = np.zeros(shape=(n_samples, results[0][1].shape[1]))
+        for grp_index, grp_result in results:
+            output[grp_index, :] = grp_result
+
+        return output
 
     def transform(self, X):
         """Transform new data `X` by transforming on each group. If a group is not found during `.transform()` and
         `use_global_model=True` the fallback transformer will be used. If `use_global_model=False` a `ValueError` will
         be raised.
 
         Parameters
@@ -176,13 +186,20 @@
         Returns
         -------
         array-like of shape (n_samples, n_features)
             Data transformed per group.
         """
         check_is_fitted(self, ["fallback_", "transformers_"])
 
+        X = nw.from_native(X, strict=False, eager_only=True)
+        frame = parse_X_y(X, y=None, groups=self.groups_, check_X=self.check_X, **self._check_kwargs).drop(
+            "__sklego_target__"
+        )
+
         if self.groups is None:
-            return self.transformers_.transform(X)
+            X_ = nw.to_native(frame)
+            return self.transformers_.transform(X_)
 
-        X_group, X_value = _split_groups_and_values(X, self.groups, **self._check_kwargs)
+        return self.__transform_groups(frame)
 
-        return self.__transform_groups(X_group, X_value)
+    def _more_tags(self):
+        return {"allow_nan": True}
```

### Comparing `scikit-lego-0.8.2/sklego/meta/hierarchical_predictor.py` & `scikit-lego-0.9.0/sklego/meta/hierarchical_predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from warnings import warn
 
+import narwhals as nw
 import numpy as np
 import pandas as pd
 from joblib import Parallel, delayed
 from sklearn import clone
 from sklearn.base import (
     BaseEstimator,
     ClassifierMixin,
@@ -12,14 +13,15 @@
     is_classifier,
     is_regressor,
 )
 from sklearn.utils.metaestimators import available_if
 from sklearn.utils.validation import check_array, check_is_fitted
 
 from sklego.common import as_list, expanding_list
+from sklego.meta._grouped_utils import _data_format_checks, _validate_groups_values
 from sklego.meta._shrinkage_utils import (
     ShrinkageMixin,
     constant_shrinkage,
     equal_shrinkage,
     min_n_obs_shrinkage,
     relative_shrinkage,
 )
@@ -191,14 +193,17 @@
         "min_n_obs": min_n_obs_shrinkage,
         "equal": equal_shrinkage,
     }
     _ALLOWED_FALLBACK = {"parent", "raise"}
 
     _GLOBAL_NAME = "__sklego_global_estimator__"
     _TARGET_NAME = "__sklego_target_value__"
+    _INDEX_NAME = "__sklego_index__"
+
+    _required_parameters = ["estimator", "groups"]
 
     def __init__(
         self,
         estimator,
         groups,
         *,
         shrinkage=None,
@@ -248,143 +253,174 @@
 
         if self.fallback_method not in self._ALLOWED_FALLBACK:
             raise ValueError(f"`fallback_method` should be either `parent` or `raise`. Found {self.fallback_method}")
 
         if not isinstance(self.check_X, bool):
             raise ValueError(f"`check_X` should be a boolean. Found {type(self.check_X)}")
 
-        self.groups_ = [self._GLOBAL_NAME] + as_list(self.groups)
+        self.groups_ = [self._GLOBAL_NAME, *as_list(self.groups)]
 
         # The only case in which we don't have to fit multiple levels is when shrinkage is None and fallback_method is 'raise'
         self.fitted_levels_ = expanding_list(self.groups_)
-        #     [self.groups_]
-        #     if (self.shrinkage is None and self.fallback_method == "raise")
-        #     else
-        # )
-
+        self.n_fitted_levels_ = len(self.fitted_levels_)
         # If invalid shrinkage, will raise ValueError (before fitting all the estimators!)
         self.shrinkage_function_ = self._set_shrinkage_function()
 
-        frame = (
-            pd.DataFrame(X)
-            .assign(**{self._TARGET_NAME: np.array(y), self._GLOBAL_NAME: 1})
-            .reset_index(drop=True)
-            .pipe(self.__validate_frame)
-        )
+        _data_format_checks(X)
 
-        self.estimators_ = self._fit_estimators(frame)
-        self.shrinkage_factors_ = self._fit_shrinkage_factors(frame, groups=self.groups_)
+        X = nw.from_native(X, strict=False, eager_only=True)
+        if not isinstance(X, nw.DataFrame):
+            X = nw.from_native(pd.DataFrame(X))
+
+        n_samples, self.n_features_in_ = X.shape
+
+        if n_samples < 2:
+            msg = f"Found {n_samples} sample or less, while a minimum of 2 is required."
+            raise ValueError(msg)
+
+        if self.n_features_in_ < 1:
+            msg = "Found 0 features, while a minimum of 1 if required."
+            raise ValueError(msg)
+
+        native_space = nw.get_native_namespace(X)
+
+        frame = X.with_columns(
+            **{
+                self._TARGET_NAME: nw.from_native(native_space.Series(y), allow_series=True),
+                self._GLOBAL_NAME: nw.from_native(native_space.Series([1] * n_samples), allow_series=True),
+            }
+        ).pipe(self.__validate_frame)
 
         self.n_groups_ = len(self.groups_)
         self.n_features_ = frame.shape[1] - self.n_groups_ - 1
-        self.n_features_in_ = frame.shape[1] - 2  # target and global columns
-        self.n_levels_ = len(self.fitted_levels_)
+
+        self.estimators_ = self._fit_estimators(frame)
+        self.shrinkage_factors_ = self._fit_shrinkage_factors(frame, groups=self.groups_)
 
         return self
 
     def predict(self, X):
         """Predict the target value for each sample in `X`."""
         raise NotImplementedError("This method should be implemented in the child class")
 
     def _predict_estimators(self, X, method_name):
         """Calls `method_name` on each level and apply shrinkage if necessary"""
 
         check_is_fitted(self, ["estimators_", "groups_"])
 
+        if len(X.shape) != 2:
+            raise ValueError(f"Reshape your data: X should be 2d, got {len(X.shape)}")
+
         if X.shape[1] != self.n_features_in_:
             raise ValueError(f"X should have {self.n_features_in_} features, got {X.shape[1]}")
 
-        frame = pd.DataFrame(X).reset_index(drop=True).assign(**{self._GLOBAL_NAME: 1})
+        X = nw.from_native(X, strict=False, eager_only=True)
+        if not isinstance(X, nw.DataFrame):
+            X = nw.from_native(pd.DataFrame(X))
+
+        n_samples = X.shape[0]
+        native_space = nw.get_native_namespace(X)
+
+        frame = X.with_columns(
+            **{
+                self._GLOBAL_NAME: nw.from_native(native_space.Series([1] * n_samples), allow_series=True),
+                self._INDEX_NAME: np.arange(n_samples),
+            }
+        ).pipe(self.__validate_frame)
 
         if not is_classifier(self.estimator):  # regressor or outlier detector
             n_out = 1
         else:
             if self.n_classes_ > 2 or method_name == "predict_proba":
                 n_out = self.n_classes_
             else:  # binary case with `method_name = "decision_function"`
                 n_out = 1
 
         preds = np.zeros((X.shape[0], self.n_levels_, n_out), dtype=float)
         shrinkage = np.zeros((X.shape[0], self.n_levels_), dtype=float)
 
         for level_idx, grp_names in enumerate(self.fitted_levels_):
-            for grp_values, grp_frame in frame.groupby(grp_names):
-                grp_idx = grp_frame.index
+            for grp_values, grp_frame in frame.group_by(grp_names):
+                grp_idx = nw.to_native(grp_frame.select(self._INDEX_NAME)).to_numpy().reshape(-1)
 
                 _estimator, _level = _get_estimator(
                     estimators=self.estimators_,
                     grp_values=grp_values,
                     grp_names=grp_names,
                     return_level=len(grp_names),
                     fallback_method=self.fallback_method,
                 )
                 _shrinkage_factor = self.shrinkage_factors_[grp_values[:_level]]
 
                 last_dim_ix = _estimator.classes_ if is_classifier(self.estimator) else [0]
-
-                raw_pred = getattr(_estimator, method_name)(grp_frame.drop(columns=self.groups_))
+                X_grp_ = nw.to_native(grp_frame.drop([*self.groups_, self._INDEX_NAME]))
+                raw_pred = getattr(_estimator, method_name)(X_grp_)
 
                 preds[np.ix_(grp_idx, [level_idx], last_dim_ix)] = np.atleast_3d(raw_pred[:, None])
-                shrinkage[np.ix_(grp_idx)] = np.lib.pad(
+                shrinkage[np.ix_(grp_idx)] = np.pad(
                     _shrinkage_factor, (0, self.n_levels_ - len(_shrinkage_factor)), "constant", constant_values=(0)
                 )
 
         return (preds * np.atleast_3d(shrinkage)).sum(axis=1).squeeze()
 
     def _fit_single_estimator(self, grp_frame):
         """Shortcut to fit an estimator on a single group"""
-        _X = grp_frame.drop(columns=self.groups_ + [self._TARGET_NAME])
-        _y = grp_frame[self._TARGET_NAME]
+        _X = nw.to_native(grp_frame.drop([*self.groups_, self._TARGET_NAME]))
+        _y = nw.to_native(grp_frame[self._TARGET_NAME])
+
         return clone(self.estimator).fit(_X, _y)
 
-    def _fit_estimators(self, frame):
+    def _fit_estimators(self, frame: nw.DataFrame):
         """Fits one estimator per level of the group column(s), and returns a dictionary of the fitted estimators.
 
         The keys of the dictionary are the group values, and the values are the fitted estimators.
         The if-else block is used to parallelize the fitting process if `n_jobs` is greater than 1.
         """
         # Question: Should the `estimators_` keys be named tuples instead of plain tuples?
         if self.n_jobs is None or self.n_jobs == 1:
             estimators_ = {
                 grp_values: self._fit_single_estimator(grp_frame)
                 for grp_names in self.fitted_levels_
-                for grp_values, grp_frame in frame.groupby(grp_names)
+                for grp_values, grp_frame in frame.group_by(grp_names)
             }
         else:
             fit_func = lambda grp_values, grp_frame: (grp_values, self._fit_single_estimator(grp_frame))
 
             estimators_ = dict(
                 Parallel(n_jobs=self.n_jobs)(
                     delayed(fit_func)(grp_values, grp_frame)
                     for grp_names in self.fitted_levels_
-                    for grp_values, grp_frame in frame.groupby(grp_names)
+                    for grp_values, grp_frame in frame.group_by(grp_names)
                 )
             )
 
         return estimators_
 
     def __validate_frame(self, frame):
         """Validate the input arrays"""
 
         if self.check_X:
-            X_values = frame.drop(columns=self.groups_ + [self._TARGET_NAME]).copy()
+            X_values = frame.drop([*self.groups_])
             check_array(X_values, **self._CHECK_KWARGS)
 
-        X_groups = frame.loc[:, self.groups_].copy()
-
-        X_group_num = X_groups.select_dtypes(include="number")
-        if X_group_num.shape[1]:
-            check_array(X_group_num, **self._CHECK_KWARGS)
-
-        # Only check missingness in object columns
-        if X_groups.select_dtypes(exclude="number").isnull().any(axis=None):
-            raise ValueError("Group columns contain NaN values")
+        _validate_groups_values(frame, self.groups_)
 
         return frame
 
+    @property
+    def n_levels_(self):
+        warn(
+            "Please use `n_fitted_levels_` instead of `n_levels_`, `n_levels_` will be deprecated in future versions",
+            DeprecationWarning,
+        )
+        return self.n_fitted_levels_
+
+    def _more_tags(self):
+        return {"allow_nan": True}
+
 
 class HierarchicalRegressor(HierarchicalPredictor, RegressorMixin):
     """A hierarchical regressor that predicts values using hierarchical grouping.
 
     This class extends [`HierarchicalPredictor`][sklego.meta.hierarchical_predictor.HierarchicalPredictor] and adds
     functionality specific to regression tasks.
```

### Comparing `scikit-lego-0.8.2/sklego/meta/ordinal_classification.py` & `scikit-lego-0.9.0/sklego/meta/ordinal_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,19 +89,21 @@
     Notes
     -----
     The implementation is based on the paper [A simple approach to ordinal classification](https://www.cs.waikato.ac.nz/~eibe/pubs/ordinal_tech_report.pdf)
     by Eibe Frank and Mark Hall.
 
     """
 
-    def __init__(self, estimator, *, n_jobs=None, use_calibration=False, **calibrarion_kwargs):
+    is_multiclass = True
+
+    def __init__(self, estimator, *, n_jobs=None, use_calibration=False, **calibration_kwargs):
         self.estimator = estimator
         self.n_jobs = n_jobs
         self.use_calibration = use_calibration
-        self.calibrarion_kwargs = calibrarion_kwargs
+        self.calibration_kwargs = calibration_kwargs
 
     def fit(self, X, y):
         """Fit the `OrdinalClassifier` model on training data `X` and `y` by fitting its underlying estimators on
         N-1 datasets `X` and `y` for each class `y_label` in `y` except `y.max()`.
 
         Parameters
         ----------
@@ -212,15 +214,15 @@
         Returns
         -------
         fitted_model : scikit-learn compatible classifier
             The fitted binary classifier.
         """
         y_bin = (y <= y_label).astype(int)
         if self.use_calibration:
-            return CalibratedClassifierCV(estimator=clone(self.estimator), **self.calibrarion_kwargs).fit(X, y_bin)
+            return CalibratedClassifierCV(estimator=clone(self.estimator), **self.calibration_kwargs).fit(X, y_bin)
         else:
             return clone(self.estimator).fit(X, y_bin)
 
     @property
     def n_classes_(self):
         """Number of classes."""
         return len(self.classes_)
```

### Comparing `scikit-lego-0.8.2/sklego/meta/outlier_classifier.py` & `scikit-lego-0.9.0/sklego/meta/outlier_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
-from sklearn.base import BaseEstimator, ClassifierMixin
+from sklearn import clone
+from sklearn.base import BaseEstimator, ClassifierMixin, MetaEstimatorMixin
 from sklearn.calibration import _SigmoidCalibration
 from sklearn.utils.validation import check_is_fitted, check_X_y
 
 from sklego.base import OutlierModel
 
 
-class OutlierClassifier(BaseEstimator, ClassifierMixin):
+class OutlierClassifier(BaseEstimator, ClassifierMixin, MetaEstimatorMixin):
     """Morphs an outlier detection model into a classifier.
 
-    When an outlier is detected it will output 1 and 0 otherwise. This way you can use familiar metrics again and
-    this allows you to consider outlier models as a fraud detector.
+    When an outlier is detected it will output 1 and 0 otherwise. This way you can use familiar metrics again and this
+    allows you to consider outlier models as a fraud detector.
 
     Parameters
     ----------
     model : scikit-learn compatible outlier detection model
         An outlier detection model that will be used for prediction.
 
     Attributes
@@ -45,14 +46,16 @@
     # [[0.34946567 0.65053433]
     #  [0.79707913 0.20292087]
     #  [0.80275406 0.19724594]
     #  [0.80275406 0.19724594]]
     ```
     """
 
+    _required_parameters = ["model"]
+
     def __init__(self, model):
         self.model = model
 
     def _is_outlier_model(self):
         """Check if the underlying model is an outlier detection model."""
         return isinstance(self.model, OutlierModel)
 
@@ -73,23 +76,24 @@
 
         Raises
         ------
         ValueError
             - If the underlying model is not an outlier detection model.
             - If the underlying model does not have a `decision_function` method.
         """
-        X, y = check_X_y(X, y, estimator=self)
         if not self._is_outlier_model():
             raise ValueError("Passed model does not detect outliers!")
         if not hasattr(self.model, "decision_function"):
             raise ValueError(
                 f"Passed model {self.model} does not have a `decision_function` "
                 f"method. This is required for `predict_proba` estimation."
             )
-        self.estimator_ = self.model.fit(X, y)
+        X, y = check_X_y(X, y)
+        self.estimator_ = clone(self.model).fit(X, y)
+        self.n_features_in_ = self.estimator_.n_features_in_
         self.classes_ = np.array([0, 1])
 
         # fit sigmoid function for `predict_proba`
         decision_function_scores = self.estimator_.decision_function(X)
         self._predict_proba_sigmoid = _SigmoidCalibration().fit(decision_function_scores, y)
 
         return self
@@ -105,16 +109,15 @@
         Returns
         -------
         np.ndarray of shape (n_samples,)
             The predicted values. 0 for inliers, 1 for outliers.
         """
         check_is_fitted(self, ["estimator_", "classes_"])
         preds = self.estimator_.predict(X)
-        result = np.zeros(preds.shape)
-        result[preds == -1] = 1
+        result = (preds == -1).astype(int)
         return result
 
     def predict_proba(self, X):
         """Predict probability estimates for new data.
 
         Parameters
         ----------
```

### Comparing `scikit-lego-0.8.2/sklego/meta/regression_outlier_detector.py` & `scikit-lego-0.9.0/sklego/meta/regression_outlier_detector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+import narwhals as nw
 import numpy as np
-import pandas as pd
+from sklearn import clone
 from sklearn.base import BaseEstimator, OutlierMixin
 from sklearn.utils.validation import check_array, check_is_fitted
 
 
 class RegressionOutlierDetector(BaseEstimator, OutlierMixin):
     """Morphs a regression estimator into one that can detect outliers. We will try to predict `column` in X.
 
     Parameters
     ----------
     model : scikit-learn compatible regression model
         A regression model that will be used for prediction.
-    column : int
-        The index of the target column to predict in the input data.
+    column : int | str
+        This should be:
+
+            - The index of the target column to predict in the input data, when the input is an array.
+            - The name of the target column to predict in the input data, when the input is a dataframe.
     lower : float, default=2.0
         Lower threshold for outlier detection. The method used for detection depends on the `method` parameter.
     upper : float, default=2.0
         Upper threshold for outlier detection. The method used for detection depends on the `method` parameter.
     method : Literal["sd", "relative", "absolute"], default="sd"
         The method to use for outlier detection.
 
@@ -28,16 +32,33 @@
     ----------
     estimator_ : scikit-learn compatible regression model
         The fitted underlying regression model.
     sd_ : float
         The standard deviation of the differences between true and predicted values.
     idx_ : int
         The index of the target column in the input data.
+
+    Notes
+    -----
+    Native cross-dataframe support is achieved using
+    [Narwhals](https://narwhals-dev.github.io/narwhals/){:target="_blank"}.
+    Supported dataframes are:
+
+    - pandas
+    - Polars (eager)
+    - Modin
+
+    See [Narwhals docs](https://narwhals-dev.github.io/narwhals/extending/){:target="_blank"} for an up-to-date list
+    (and to learn how you can add your dataframe library to it!), though note that only those
+    supported by [sklearn.utils.check_X_y](https://scikit-learn.org/stable/modules/generated/sklearn.utils.check_X_y.html)
+    will work with this class.
     """
 
+    _required_parameters = ["model", "column"]
+
     def __init__(self, model, column, lower=2, upper=2, method="sd"):
         self.model = model
         self.column = column
         self.lower = lower
         self.upper = upper
         self.method = method
 
@@ -108,21 +129,27 @@
             The fitted estimator.
 
         Raises
         ------
         ValueError
             If the `model` is not a regression estimator.
         """
-        self.idx_ = np.argmax([i == self.column for i in X.columns]) if isinstance(X, pd.DataFrame) else self.column
-        X = check_array(X, estimator=self)
+        X = nw.from_native(X, eager_only=True, strict=False)
+        self.idx_ = np.argmax([i == self.column for i in X.columns]) if isinstance(X, nw.DataFrame) else self.column
+        X = check_array(nw.to_native(X, strict=False), estimator=self)
+
+        self.n_features_in_ = X.shape[1]
+
         if not self._is_regression_model():
             raise ValueError("Passed model must be regression!")
         X, y = self.to_x_y(X)
-        self.estimator_ = self.model.fit(X, y)
+        self.estimator_ = clone(self.model).fit(X, y)
         self.sd_ = np.std(self.estimator_.predict(X) - y)
+        self.offset_ = 0
+
         return self
 
     def predict(self, X, y=None):
         """Predict which samples of `X` are outliers using the underlying estimator and given `method`.
 
         Parameters
         ----------
@@ -172,7 +199,10 @@
             ValueError(f"`method` must be in {allowed_methods} got: {self.method}")
         if self.method == "sd":
             return difference
         if self.method == "relative":
             return difference / y_true
         if self.method == "absolute":
             return difference
+
+    def decision_function(self, X):
+        return self.score_samples(X) - self.offset_
```

### Comparing `scikit-lego-0.8.2/sklego/meta/subjective_classifier.py` & `scikit-lego-0.9.0/sklego/meta/subjective_classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from sklearn import clone
 from sklearn.base import BaseEstimator, ClassifierMixin, MetaEstimatorMixin
 from sklearn.metrics import confusion_matrix
 from sklearn.preprocessing import normalize
 from sklearn.utils.validation import FLOAT_DTYPES, check_array, check_is_fitted, check_X_y
 
 
 class SubjectiveClassifier(BaseEstimator, ClassifierMixin, MetaEstimatorMixin):
@@ -42,14 +43,17 @@
         The fitted classifier.
     classes_ : array-like, shape=(n_classes,)
         The classes labels.
     posterior_matrix_ : array-like, shape=(n_classes, n_classes)
         The posterior probabilities for each class, given the prediction of the inner classifier.
     """
 
+    _ALLOWED_EVIDENCE = ("predict_proba", "confusion_matrix", "both")
+    _required_parameters = ["estimator", "prior"]
+
     def __init__(self, estimator, prior, evidence="both"):
         self.estimator = estimator
         self.prior = prior
         self.evidence = evidence
 
     def _likelihood(self, predicted_class, given_class, cfm):
         return cfm[given_class, predicted_class] / cfm[given_class, :].sum()
@@ -98,29 +102,29 @@
             raise ValueError(
                 "Invalid inner estimator: the SubjectiveClassifier meta model only works on classification models"
             )
 
         if not np.isclose(sum(self.prior.values()), 1):
             raise ValueError("Invalid prior: the prior probabilities of all classes should sum to 1")
 
-        valid_evidence_types = ["predict_proba", "confusion_matrix", "both"]
-        if self.evidence not in valid_evidence_types:
-            raise ValueError(f"Invalid evidence: the provided evidence should be one of {valid_evidence_types}")
+        if self.evidence not in self._ALLOWED_EVIDENCE:
+            raise ValueError(f"Invalid evidence: the provided evidence should be one of {self._ALLOWED_EVIDENCE}")
 
         X, y = check_X_y(X, y, estimator=self.estimator, dtype=FLOAT_DTYPES)
         if set(y) - set(self.prior.keys()):
             raise ValueError(
                 f"Training data is inconsistent with prior: no prior defined for classes "
                 f"{set(y) - set(self.prior.keys())}"
             )
-        self.estimator.fit(X, y)
-        cfm = confusion_matrix(y, self.estimator.predict(X))
+        self.estimator_ = clone(self.estimator).fit(X, y)
+        cfm = confusion_matrix(y, self.estimator_.predict(X))
         self.posterior_matrix_ = np.array(
             [[self._posterior(y, y_hat, cfm) for y_hat in range(cfm.shape[0])] for y in range(cfm.shape[0])]
         )
+        self.n_features_in_ = X.shape[1]
         return self
 
     @staticmethod
     def _weighted_proba(weights, y_hat_probas):
         return normalize(weights * y_hat_probas, norm="l1")
 
     @staticmethod
@@ -140,15 +144,15 @@
         Returns
         -------
         array-like of shape (n_samples, n_classes)
             The predicted probabilities.
         """
         check_is_fitted(self, ["posterior_matrix_"])
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
-        y_hats = self.estimator.predict_proba(X)  # these are ignorant of the prior
+        y_hats = self.estimator_.predict_proba(X)  # these are ignorant of the prior
 
         if self.evidence == "predict_proba":
             prior_weights = np.array([self.prior[klass] for klass in self.classes_])
             return self._weighted_proba(prior_weights, y_hats)
         else:
             posterior_probas = self._to_discrete(y_hats) @ self.posterior_matrix_.T
             return self._weighted_proba(posterior_probas, y_hats) if self.evidence == "both" else posterior_probas
@@ -169,8 +173,8 @@
         check_is_fitted(self, ["posterior_matrix_"])
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
         return self.classes_[self.predict_proba(X).argmax(axis=1)]
 
     @property
     def classes_(self):
         """Alias for `.classes_` attribute of the underlying estimator."""
-        return self.estimator.classes_
+        return self.estimator_.classes_
```

### Comparing `scikit-lego-0.8.2/sklego/meta/zero_inflated_regressor.py` & `scikit-lego-0.9.0/sklego/meta/zero_inflated_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from inspect import signature
 
 import numpy as np
-from sklearn.base import BaseEstimator, RegressorMixin, clone, is_classifier, is_regressor
+from sklearn.base import BaseEstimator, MetaEstimatorMixin, RegressorMixin, clone, is_classifier, is_regressor
 from sklearn.exceptions import NotFittedError
-from sklearn.utils.validation import check_array, check_is_fitted, check_X_y
+from sklearn.utils.validation import _check_sample_weight, check_array, check_is_fitted, check_X_y
 
 
-class ZeroInflatedRegressor(BaseEstimator, RegressorMixin):
+class ZeroInflatedRegressor(BaseEstimator, RegressorMixin, MetaEstimatorMixin):
     """A meta regressor for zero-inflated datasets, i.e. the targets contain a lot of zeroes.
 
     `ZeroInflatedRegressor` consists of a classifier and a regressor.
 
         - The classifier's task is to find of if the target is zero or not.
         - The regressor's task is to output a (usually positive) prediction whenever the classifier indicates that the
         there should be a non-zero prediction.
@@ -56,14 +56,16 @@
     #                       regressor=ExtraTreesRegressor(random_state=0))
 
     model.predict(X)[:5]
     # array([4.91483294, 0.        , 0.        , 0.04941909, 0.        ])
     ```
     """
 
+    _required_parameters = ["classifier", "regressor"]
+
     def __init__(self, classifier, regressor) -> None:
         self.classifier = classifier
         self.regressor = regressor
 
     def fit(self, X, y, sample_weight=None):
         """Fit the underlying classifier and regressor using `X` and `y` as training data. The regressor is only trained
         on examples where the target is non-zero.
@@ -92,27 +94,28 @@
         if not is_classifier(self.classifier):
             raise ValueError(
                 f"`classifier` has to be a classifier. Received instance of {type(self.classifier)} instead."
             )
         if not is_regressor(self.regressor):
             raise ValueError(f"`regressor` has to be a regressor. Received instance of {type(self.regressor)} instead.")
 
+        sample_weight = _check_sample_weight(sample_weight, X)
         try:
             check_is_fitted(self.classifier)
             self.classifier_ = self.classifier
         except NotFittedError:
             self.classifier_ = clone(self.classifier)
 
             if "sample_weight" in signature(self.classifier_.fit).parameters:
                 self.classifier_.fit(X, y != 0, sample_weight=sample_weight)
             else:
                 logging.warning("Classifier ignores sample_weight.")
                 self.classifier_.fit(X, y != 0)
 
-        non_zero_indices = np.where(self.classifier_.predict(X) == 1)[0]
+        non_zero_indices = np.where(y != 0)[0]
 
         if non_zero_indices.size > 0:
             try:
                 check_is_fitted(self.regressor)
                 self.regressor_ = self.regressor
             except NotFittedError:
                 self.regressor_ = clone(self.regressor)
```

### Comparing `scikit-lego-0.8.2/sklego/metrics.py` & `scikit-lego-0.9.0/sklego/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     M. Zafar et al. (2017), Fairness Constraints: Mechanisms for Fair Classification
     """
 
     def impl(estimator, X, y_true=None):
         """Remember: X is the thing going *in* to your pipeline."""
         sensitive_col = X[:, sensitive_column] if isinstance(X, np.ndarray) else X[sensitive_column]
 
-        if not np.all((sensitive_col == 0) | (sensitive_col == 1)):
+        if not ((sensitive_col == 0) | (sensitive_col == 1)).all():
             raise ValueError(
                 f"p_percent_score only supports binary indicator columns for `column`. "
                 f"Found values {np.unique(sensitive_col)}"
             )
 
         y_hat = estimator.predict(X)
         y_given_z1 = y_hat[sensitive_col == 1]
@@ -148,15 +148,15 @@
     M. Hardt, E. Price and N. Srebro (2016), Equality of Opportunity in Supervised Learning
     """
 
     def impl(estimator, X, y_true):
         """Remember: X is the thing going *in* to your pipeline."""
         sensitive_col = X[:, sensitive_column] if isinstance(X, np.ndarray) else X[sensitive_column]
 
-        if not np.all((sensitive_col == 0) | (sensitive_col == 1)):
+        if not ((sensitive_col == 0) | (sensitive_col == 1)).all():
             raise ValueError(
                 f"equal_opportunity_score only supports binary indicator columns for `column`. "
                 f"Found values {np.unique(sensitive_col)}"
             )
 
         y_hat = estimator.predict(X)
         y_given_z1_y1 = y_hat[(sensitive_col == 1) & (y_true == positive_target)]
```

### Comparing `scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_classifier.py` & `scikit-lego-0.9.0/sklego/mixture/bayesian_gmm_classifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,18 @@
                 covariance_prior=self.covariance_prior,
                 random_state=self.random_state,
                 warm_start=self.warm_start,
                 verbose=self.verbose,
                 verbose_interval=self.verbose_interval,
             )
             self.gmms_[c] = mixture.fit(subset_x, subset_y)
+
+        self.n_features_in_ = X.shape[1]
+        self.n_iter_ = sum(mixture.n_iter_ for mixture in self.gmms_.values())
+
         return self
 
     def predict(self, X):
         """Predict labels for `X` using fitted estimator.
 
         Parameters
         ----------
```

### Comparing `scikit-lego-0.8.2/sklego/mixture/bayesian_gmm_detector.py` & `scikit-lego-0.9.0/sklego/mixture/bayesian_gmm_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,46 +149,48 @@
             density = gaussian_kde(score_samples)
             max_x_value = minimize_scalar(lambda x: -density(x)).x
             mean_likelihood = score_samples.mean()
             new_likelihoods = score_samples[score_samples < max_x_value]
             new_likelihoods_std = np.std(new_likelihoods - mean_likelihood)
             self.likelihood_threshold_ = mean_likelihood - (self.threshold * new_likelihoods_std)
 
+        self.n_iter_ = self.gmm_.n_iter_
+        self.n_features_in_ = X.shape[1]
+        self.offset_ = self.likelihood_threshold_
         return self
 
     def score_samples(self, X):
         """Compute the log likelihood for each sample and return the negative value."""
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
         check_is_fitted(self, ["gmm_", "likelihood_threshold_"])
         if len(X.shape) == 1:
             X = np.expand_dims(X, 1)
 
-        return self.gmm_.score_samples(X) * -1
+        return self.gmm_.score_samples(X)
 
     def decision_function(self, X):
         # We subtract self.offset_ to make 0 be the threshold value for being an outlier:
-        return self.score_samples(X) + self.likelihood_threshold_
+        return self.score_samples(X) - self.offset_
 
     def predict(self, X):
         """Predict if a point is an outlier or not using the fitted estimator.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The data to predict.
 
         Returns
         -------
         array-like of shape (n_samples,)
             The predicted data. 1 for inliers, -1 for outliers.
         """
-        predictions = (self.decision_function(X) >= 0).astype(int)
-        predictions[predictions == 1] = -1
-        predictions[predictions == 0] = 1
-        return predictions
+        preds = (self.decision_function(X) >= 0).astype(int)
+        preds[preds == 0] = -1
+        return preds
 
     @property
     def allowed_methods(self):
         warn(
             "Please use `_ALLOWED_METHODS` instead of `allowed_methods`,"
             "`allowed_methods` will be deprecated in future versions",
             DeprecationWarning,
```

### Comparing `scikit-lego-0.8.2/sklego/mixture/gmm_classifier.py` & `scikit-lego-0.9.0/sklego/mixture/gmm_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,18 @@
                 precisions_init=self.precisions_init,
                 random_state=self.random_state,
                 warm_start=self.warm_start,
                 verbose=self.verbose,
                 verbose_interval=self.verbose_interval,
             )
             self.gmms_[c] = mixture.fit(subset_x, subset_y)
+
+        self.n_features_in_ = X.shape[1]
+        self.n_iter_ = sum(mixture.n_iter_ for mixture in self.gmms_.values())
+
         return self
 
     def predict(self, X):
         """Predict labels for `X` using fitted estimator.
 
         Parameters
         ----------
```

### Comparing `scikit-lego-0.8.2/sklego/mixture/gmm_outlier_detector.py` & `scikit-lego-0.9.0/sklego/mixture/gmm_outlier_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         self.precisions_init = precisions_init
         self.random_state = random_state
         self.warm_start = warm_start
         self.verbose = verbose
         self.verbose_interval = verbose_interval
 
     def fit(self, X: np.ndarray, y=None) -> "GMMOutlierDetector":
-        """Fit the `BayesianGMMOutlierDetector` model using `X`, `y` as training data.
+        """Fit the `GMMOutlierDetector` model using `X`, `y` as training data.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features )
             The training data.
         y : array-like of shape (n_samples,)
             Ignored, present for compatibility.
@@ -139,46 +139,48 @@
             density = gaussian_kde(score_samples)
             max_x_value = minimize_scalar(lambda x: -density(x)).x
             mean_likelihood = score_samples.mean()
             new_likelihoods = score_samples[score_samples < max_x_value]
             new_likelihoods_std = np.std(new_likelihoods - mean_likelihood)
             self.likelihood_threshold_ = mean_likelihood - (self.threshold * new_likelihoods_std)
 
+        self.n_iter_ = self.gmm_.n_iter_
+        self.n_features_in_ = X.shape[1]
+        self.offset_ = self.likelihood_threshold_
         return self
 
     def score_samples(self, X):
         """Compute the log likelihood for each sample and return the negative value."""
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
         check_is_fitted(self, ["gmm_", "likelihood_threshold_"])
         if len(X.shape) == 1:
             X = np.expand_dims(X, 1)
 
-        return -self.gmm_.score_samples(X)
+        return self.gmm_.score_samples(X)
 
     def decision_function(self, X):
         # We subtract self.offset_ to make 0 be the threshold value for being an outlier:
-        return self.score_samples(X) + self.likelihood_threshold_
+        return self.score_samples(X) - self.offset_
 
     def predict(self, X):
         """Predict if a point is an outlier or not using the fitted model.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
             The data to predict.
 
         Returns
         -------
         array-like of shape (n_samples,)
             The predicted data. 1 for inliers, -1 for outliers.
         """
-        predictions = (self.decision_function(X) >= 0).astype(int)
-        predictions[predictions == 1] = -1
-        predictions[predictions == 0] = 1
-        return predictions
+        preds = (self.decision_function(X) >= 0).astype(int)
+        preds[preds == 0] = -1
+        return preds
 
     @property
     def allowed_methods(self):
         warn(
             "Please use `_ALLOWED_METHODS` instead of `allowed_methods`,"
             "`allowed_methods` will be deprecated in future versions",
             DeprecationWarning,
```

### Comparing `scikit-lego-0.8.2/sklego/model_selection.py` & `scikit-lego-0.9.0/sklego/model_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numbers
 from datetime import timedelta
 from itertools import combinations
 from warnings import warn
 
+import narwhals as nw
 import numpy as np
 import pandas as pd
 from sklearn.exceptions import NotFittedError
 from sklearn.model_selection._split import _BaseKFold, check_array
 from sklearn.utils.validation import indexable
 
 from sklego.base import Clusterer
@@ -40,16 +41,18 @@
 
     `train_duration = total_length - (gap_duration + valid_duration * n_splits)`
 
     such that the shifting the entire window by one validation duration spans the whole training set.
 
     Parameters
     ----------
-    date_serie : pd.Series
+    date_serie : Series
         Series with the date, that should have all the indices of X used in the split() method.
+        If the Series is not pandas-like (for example, if it's a Polars Series, which does not have
+        an index) then it must the same same length as the `X` and `y` objects passed to `split`.
     valid_duration : datetime.timedelta
         Retraining period.
     train_duration : datetime.timedelta | None, default=None
         Historical training data.
     gap_duration : datetime.timedelta, default=timedelta(0)
         Forward looking window of the target. The period of the forward looking window necessary to create your target
         variable.
@@ -61,14 +64,29 @@
     n_splits : int | None, default=None
         Number of splits.
     window : Literal["rolling", "expanding"], default="rolling"
         Type of moving window to use.
 
         - `"rolling"` window has fixed size and is shifted entirely.
         - `"expanding"` left side of window is fixed, right border increases each fold.
+
+    Notes
+    -----
+    Native cross-dataframe support is achieved using
+    [Narwhals](https://narwhals-dev.github.io/narwhals/){:target="_blank"}.
+    Supported dataframes are:
+
+    - pandas
+    - Polars (eager)
+    - Modin
+    - cuDF
+
+    See [Narwhals docs](https://narwhals-dev.github.io/narwhals/extending/){:target="_blank"} for an up-to-date list
+    (and to learn how you can add your dataframe library to it!), though note that only those
+    convertible to `numpy` arrays will work with this class.
     """
 
     def __init__(
         self,
         date_serie,
         valid_duration,
         train_duration=None,
@@ -78,60 +96,59 @@
     ):
         if (train_duration is None) and (n_splits is None):
             raise ValueError("Either train_duration or n_splits have to be defined")
 
         if (train_duration is not None) and (train_duration <= gap_duration):
             raise ValueError("gap_duration is longer than train_duration, it should be shorter.")
 
-        if not date_serie.index.is_unique:
-            raise ValueError("date_serie doesn't have a unique index")
-
-        self.date_serie = date_serie.copy()
-        self.date_serie = self.date_serie.rename("__date__")
+        self.date_serie = nw.from_native(date_serie, series_only=True).alias("__date__")
         self.train_duration = train_duration
         self.valid_duration = valid_duration
         self.gap_duration = gap_duration
         self.n_splits = n_splits
         self.window = window
 
     def _join_date_and_x(self, X):
         """Creates a DataFrame indexed by the pandas index (the same as `date_serie`) with date column joined with that
         index and with the 'numpy index' column (i.e. just a range) that is required for the output and the rest of
         sklearn.
 
+        If the user is working with index-less dataframes (e.g. Polars), then `self.date_series` needs to be the same
+        length as `X`.
+
         Parameters
         ----------
-        X : pd.DataFrame
+        X : DataFrame
             Dataframe with the data to split
         """
-        X_index_df = pd.DataFrame(range(len(X)), columns=["np_index"], index=X.index)
-        X_index_df = X_index_df.join(self.date_serie)
+        X_index_df = nw.maybe_align_index(self.date_serie, X).to_frame().with_row_index("np_index")
 
         return X_index_df
 
     def split(self, X, y=None, groups=None):
         """Generate indices to split data into training and test set.
 
         Parameters
         ----------
-        X : pd.DataFrame
+        X : DataFrame
             Dataframe with the data to split.
         y : array-like | None, default=None
             Ignored, present for compatibility.
         groups : array-like | None, default=None
             Ignored, present for compatibility.
 
         Yields
         -------
         tuple[np.ndarray, np.ndarray]
             Train and test indices of the same fold.
         """
 
+        X = nw.from_native(X, eager_only=True)
         X_index_df = self._join_date_and_x(X)
-        X_index_df = X_index_df.sort_values("__date__", ascending=True)
+        X_index_df = X_index_df.sort("__date__", descending=False)
 
         if len(X) != len(X_index_df):
             raise AssertionError(
                 "X and X_index_df are not the same length, " "there must be some index missing in 'self.date_serie'"
             )
 
         date_min = X_index_df["__date__"].min()
@@ -163,39 +180,36 @@
             time_shift = self.valid_duration * n_split_max / self.n_splits
         else:
             time_shift = self.valid_duration
         while True:
             if current_date + self.train_duration + time_shift + self.gap_duration > date_max:
                 break
 
-            X_train_df = X_index_df[
-                (X_index_df["__date__"] >= start_date) & (X_index_df["__date__"] < current_date + self.train_duration)
-            ]
-            X_valid_df = X_index_df[
-                (X_index_df["__date__"] >= current_date + self.train_duration + self.gap_duration)
-                & (
-                    X_index_df["__date__"]
-                    < current_date + self.train_duration + self.valid_duration + self.gap_duration
-                )
-            ]
+            X_train_df = X_index_df.filter(
+                nw.col("__date__") >= start_date, nw.col("__date__") < current_date + self.train_duration
+            )
+            X_valid_df = X_index_df.filter(
+                nw.col("__date__") >= current_date + self.train_duration + self.gap_duration,
+                nw.col("__date__") < current_date + self.train_duration + self.valid_duration + self.gap_duration,
+            )
 
             current_date = current_date + time_shift
             if self.window == "rolling":
                 start_date = current_date
             yield (
-                X_train_df["np_index"].values,
-                X_valid_df["np_index"].values,
+                X_train_df["np_index"].to_numpy(),
+                X_valid_df["np_index"].to_numpy(),
             )
 
     def get_n_splits(self, X=None, y=None, groups=None):
         """Get the number of splits
 
         Parameters
         ----------
-        X : pd.DataFrame
+        X : DataFrame
             Dataframe with the data to split.
         y : array-like | None, default=None
             Ignored, present for compatibility.
         groups : array-like | None, default=None
             Ignored, present for compatibility.
 
         Returns
@@ -206,50 +220,60 @@
         return sum(1 for x in self.split(X, y, groups))
 
     def summary(self, X):
         """Describe all folds.
 
         Parameters
         ----------
-        X : pd.DataFrame
+        X : DataFrame
             Dataframe with the data to split.
 
         Returns
         -------
-        pd.DataFrame
+        DataFrame
             Summary of all folds.
         """
         summary = []
+        X = nw.from_native(X, eager_only=True)
         X_index_df = self._join_date_and_x(X)
 
-        def get_split_info(X, indices, j, part, summary):
-            dates = X_index_df.iloc[indices]["__date__"]
+        summary = {
+            "Start date": [],
+            "End date": [],
+            "Period": [],
+            "Unique days": [],
+            "nbr samples": [],
+            "part": [],
+            "fold": [],
+        }
+        native_namespace = nw.get_native_namespace(X)
+
+        def update_split_info(indices, j, part, summary):
+            dates = X_index_df["__date__"][indices]
             mindate = dates.min()
             maxdate = dates.max()
+            n_unique = dates.n_unique()
 
-            s = pd.Series(
-                {
-                    "Start date": mindate,
-                    "End date": maxdate,
-                    "Period": pd.to_datetime(maxdate, format="%Y%m%d") - pd.to_datetime(mindate, format="%Y%m%d"),
-                    "Unique days": len(dates.unique()),
-                    "nbr samples": len(indices),
-                },
-                name=(j, part),
-            )
-            summary.append(s)
-            return summary
+            summary["Start date"].append(mindate)
+            summary["End date"].append(maxdate)
+            summary["Period"].append(maxdate - mindate)
+            summary["Unique days"].append(n_unique)
+            summary["nbr samples"].append(len(indices))
+            summary["part"].append(part)
+            summary["fold"].append(j)
 
         j = 0
-        for i in self.split(X):
-            summary = get_split_info(X, i[0], j, "train", summary)
-            summary = get_split_info(X, i[1], j, "valid", summary)
+        for i in self.split(nw.to_native(X)):
+            update_split_info(native_namespace.Series(i[0]), j, "train", summary)
+            update_split_info(native_namespace.Series(i[1]), j, "valid", summary)
             j = j + 1
 
-        return pd.DataFrame(summary)
+        result = nw.from_native(native_namespace.DataFrame(summary))
+        result = nw.maybe_set_index(result, ["fold", "part"])
+        return nw.to_native(result)
 
 
 def KlusterFoldValidation(**kwargs):
     warn(
         "Please use `ClusterFoldValidation` instead of `KlusterFoldValidation`."
         "We will use correct spelling going forward and `KlusterFoldValidation` will be deprecated.",
         DeprecationWarning,
@@ -542,15 +566,15 @@
             .loc[lambda df: df["group_id"] != 0]
             .iloc[0]
             .name
         )
         # initialize the index of the last split point, to reduce the amount of possible index split options
         last_split_index = len(self._grouped_df) - (
             self._grouped_df.assign(
-                observations=lambda df: df["observations"].values[::-1],
+                observations=lambda df: df["observations"].to_numpy()[::-1],
                 cumsum_obs=lambda df: df["observations"].cumsum(),
             )
             .reset_index()
             .assign(group_id=lambda df: (df["cumsum_obs"] - 1) // init_ideal_group_size)
             .loc[lambda df: df["group_id"] != 0]
             .iloc[0]
             .name
```

### Comparing `scikit-lego-0.8.2/sklego/naive_bayes.py` & `scikit-lego-0.9.0/sklego/naive_bayes.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,15 @@
                     means_init=self.means_init,
                     precisions_init=self.precisions_init,
                     random_state=self.random_state,
                     warm_start=self.warm_start,
                 ).fit(subset_x[:, i].reshape(-1, 1), subset_y)
                 for i in range(X.shape[1])
             ]
+        self.n_iter_ = sum(sum(gmm.n_iter_ for gmm in gmm_c) for gmm_c in self.gmms_.values())
         return self
 
     def predict(self, X):
         """Predict labels for `X` using fitted estimator and `predict_proba` method, by picking the class with the
         highest probability.
 
         Parameters
@@ -136,15 +137,15 @@
         check_is_fitted(self, ["gmms_", "classes_", "n_features_in_"])
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
         if self.n_features_in_ != X.shape[1]:
             raise ValueError(f"number of columns {X.shape[1]} does not match fit size {self.n_features_in_}")
         check_is_fitted(self, ["gmms_", "classes_"])
         probs = np.zeros((X.shape[0], len(self.classes_)))
         for k, v in self.gmms_.items():
-            class_idx = int(np.argwhere(self.classes_ == k))
+            class_idx = np.argmax(self.classes_ == k)
             probs[:, class_idx] = np.array(
                 [m.score_samples(np.expand_dims(X[:, idx], 1)) for idx, m in enumerate(v)]
             ).sum(axis=0)
         likelihood = np.exp(probs)
         return likelihood / likelihood.sum(axis=1).reshape(-1, 1)
 
     @property
@@ -260,14 +261,15 @@
                     random_state=self.random_state,
                     warm_start=self.warm_start,
                     verbose=self.verbose,
                     verbose_interval=self.verbose_interval,
                 ).fit(subset_x[:, i].reshape(-1, 1), subset_y)
                 for i in range(X.shape[1])
             ]
+        self.n_iter_ = sum(sum(gmm.n_iter_ for gmm in gmm_c) for gmm_c in self.gmms_.values())
         return self
 
     def predict(self, X):
         """Predict labels for `X` using fitted estimator and `predict_proba` method, by picking the class with the
         highest probability.
 
         Parameters
@@ -301,15 +303,15 @@
         check_is_fitted(self, ["gmms_", "classes_", "n_features_in_"])
         X = check_array(X, estimator=self, dtype=FLOAT_DTYPES)
         if self.n_features_in_ != X.shape[1]:
             raise ValueError(f"number of columns {X.shape[1]} does not match fit size {self.n_features_in_}")
         check_is_fitted(self, ["gmms_", "classes_"])
         probs = np.zeros((X.shape[0], len(self.classes_)))
         for k, v in self.gmms_.items():
-            class_idx = int(np.argwhere(self.classes_ == k))
+            class_idx = np.argmax(self.classes_ == k)
             probs[:, class_idx] = np.array(
                 [m.score_samples(np.expand_dims(X[:, idx], 1)) for idx, m in enumerate(v)]
             ).sum(axis=0)
         likelihood = np.exp(probs)
         return likelihood / likelihood.sum(axis=1).reshape(-1, 1)
 
     @property
```

### Comparing `scikit-lego-0.8.2/sklego/neighbors.py` & `scikit-lego-0.9.0/sklego/neighbors.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
                 leaf_size=self.leaf_size,
                 metric_params=self.metric_params,
             ).fit(x_subset)
 
             # Computing target class prior
             self.priors_logp_[target_label] = np.log(len(x_subset) / len(X))
 
+        self.n_features_in_ = X.shape[1]
         return self
 
     def predict_proba(self, X):
         """Predict probabilities for `X` using fitted estimator and the joint distribution.
 
         The returned estimates for all classes are in the same order found in the `.classes_` attribute.
```

### Comparing `scikit-lego-0.8.2/sklego/notinstalled.py` & `scikit-lego-0.9.0/sklego/notinstalled.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/pandas_utils.py` & `scikit-lego-0.9.0/sklego/pandas_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime as dt
 import inspect
 from functools import partial, wraps
 
+import narwhals as nw
 import numpy as np
-import pandas as pd
 from scipy.ndimage import shift
 
 from sklego.common import as_list
 
 
 def _get_shape_delta(old_shape, new_shape):
     """Returns a string with the difference in shape between old and new."""
@@ -195,21 +195,35 @@
     lags : int | List[int]
         The amount of lag for each col.
     drop_na : bool, default=True
         Whether or not to remove rows that contain NA values.
 
     Returns
     -------
-    pd.DataFrame | np.ndarray
+    DataFrame | np.ndarray
         With only the selected cols.
 
     Raises
     ------
     ValueError
-        If the input is not a `pd.DataFrame` or `np.ndarray`.
+        If the input is not a supported DataFrame.
+
+    Notes
+    -----
+    Native cross-dataframe support is achieved using
+    [Narwhals](https://narwhals-dev.github.io/narwhals/){:target="_blank"}.
+    Supported dataframes are:
+
+    - pandas
+    - Polars (eager or lazy)
+    - Modin
+    - cuDF
+
+    See [Narwhals docs](https://narwhals-dev.github.io/narwhals/extending/){:target="_blank"} for an up-to-date list
+    (and to learn how you can add your dataframe library to it!).
 
     Examples
     --------
     ```py
     import pandas as pd
     df = pd.DataFrame([[1, 2, 3],
                        [4, 5, 6],
@@ -251,16 +265,17 @@
     # Now we can iterate over the list to determine
     # whether it is a list of integers
     if not all(isinstance(x, int) for x in lags):
         raise ValueError("lags must be a list of type: " + str(int))
 
     # The keys of the allowed_inputs dict contain the allowed
     # types, and the values contain the associated handlers
+    X = nw.from_native(X, strict=False)
     allowed_inputs = {
-        pd.core.frame.DataFrame: _add_lagged_pandas_columns,
+        nw.DataFrame: _add_lagged_dataframe_columns,
         np.ndarray: _add_lagged_numpy_columns,
     }
 
     # Choose the correct handler based on the input class
     for allowed_input, handler in allowed_inputs.items():
         if isinstance(X, allowed_input):
             return handler(X, cols, lags, drop_na)
@@ -294,15 +309,15 @@
 
     if not all([isinstance(col, int) for col in cols]):
         raise ValueError("Matrix columns are indexed by integers")
 
     if not all([col < X.shape[1] for col in cols]):
         raise KeyError("The column does not exist")
 
-    combos = (shift(X[:, col], -lag, cval=np.NaN) for col in cols for lag in lags)
+    combos = (shift(X[:, col], -lag, cval=np.nan) for col in cols for lag in lags)
 
     # In integer-based ndarrays, NaN values are represented as
     # -9223372036854775808, so we convert back and forth from
     # original to float and back to original dtype
     original_type = X.dtype
     X = np.asarray(X, dtype=float)
     answer = np.column_stack((X, *combos))
@@ -312,43 +327,39 @@
         answer = answer[~np.isnan(answer).any(axis=1)]
 
     # Change dtype back to its original
     answer = np.asarray(answer, dtype=original_type)
     return answer
 
 
-def _add_lagged_pandas_columns(df, cols, lags, drop_na):
+def _add_lagged_dataframe_columns(df, cols, lags, drop_na):
     """Append a lag columns.
 
     Parameters
     ----------
-    df : pd.DataFrame
+    df : narwhals.DataFrame | narwhals.LazyFrame
         Data to be lagged.
     cols : str | List[str]
         Column name / names.
     lags : int | List[int]
         The amount of lag for each col.
     drop_na : bool
         Whether or not to remove rows that contain NA values.
 
     Returns
     -------
-    pd.DataFrame
+    DataFrame
         Dataframe with concatenated lagged cols.
     """
 
     cols = as_list(cols)
 
-    # Indexes are not supported as pandas column names may be
-    # integers themselves, introducing unexpected behaviour
-    if not all([col in df.columns.values for col in cols]):
+    if not all([col in df.columns for col in cols]):
         raise KeyError("The column does not exist")
 
-    combos = (df[col].shift(-lag).rename(col + str(lag)) for col in cols for lag in lags)
-
-    answer = pd.concat([df, *combos], axis=1)
+    answer = df.with_columns(nw.col(col).shift(-lag).alias(col + str(lag)) for col in cols for lag in lags)
 
-    # Remove rows that contain NA values when drop_na is truthy
+    # Remove rows that contain null values when drop_na is truthy
     if drop_na:
-        answer = answer.dropna()
+        answer = answer.drop_nulls()
 
-    return answer
+    return nw.to_native(answer)
```

### Comparing `scikit-lego-0.8.2/sklego/pipeline.py` & `scikit-lego-0.9.0/sklego/pipeline.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/__init__.py` & `scikit-lego-0.9.0/sklego/preprocessing/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,21 +6,22 @@
     "FormulaicTransformer",
     "IdentityTransformer",
     "InformationFilter",
     "IntervalEncoder",
     "OrthogonalTransformer",
     "OutlierRemover",
     "PandasTypeSelector",
+    "TypeSelector",
     "RandomAdder",
     "RepeatingBasisFunction",
 ]
 
 from sklego.preprocessing.columncapper import ColumnCapper
 from sklego.preprocessing.dictmapper import DictMapper
 from sklego.preprocessing.formulaictransformer import FormulaicTransformer
 from sklego.preprocessing.identitytransformer import IdentityTransformer
 from sklego.preprocessing.intervalencoder import IntervalEncoder
 from sklego.preprocessing.outlier_remover import OutlierRemover
-from sklego.preprocessing.pandastransformers import ColumnDropper, ColumnSelector, PandasTypeSelector
+from sklego.preprocessing.pandastransformers import ColumnDropper, ColumnSelector, PandasTypeSelector, TypeSelector
 from sklego.preprocessing.projections import InformationFilter, OrthogonalTransformer
 from sklego.preprocessing.randomadder import RandomAdder
 from sklego.preprocessing.repeatingbasis import RepeatingBasisFunction
```

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/columncapper.py` & `scikit-lego-0.9.0/sklego/preprocessing/columncapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,7 +238,10 @@
     @property
     def n_columns_(self):
         warn(
             "Please use `n_features_in_` instead of `n_columns_`, `n_columns_` will be deprecated in future versions",
             DeprecationWarning,
         )
         return self.n_features_in_
+
+    def _more_tags(self):
+        return {"allow_nan": True}
```

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/dictmapper.py` & `scikit-lego-0.9.0/sklego/preprocessing/dictmapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     #        [ 130181],
     #        [ 367984],
     #        [      0],
     #        [ 165396]])
     ```
     """
 
+    _required_parameters = ["mapper", "default"]
+
     def __init__(self, mapper, default):
         self.mapper = mapper
         self.default = default
 
     def fit(self, X, y=None):
         """Checks the input data and records the number of features.
 
@@ -72,15 +74,15 @@
         self : DictMapper
             The fitted transformer.
         """
         X = check_array(
             X,
             copy=True,
             estimator=self,
-            force_all_finite=True,
+            force_all_finite=False,
             dtype=None,
             ensure_2d=True,
         )
         self.n_features_in_ = X.shape[1]
         return self
 
     def transform(self, X):
@@ -102,15 +104,15 @@
             If the number of columns from `X` differs from the number of columns when fitting.
         """
         check_is_fitted(self, ["n_features_in_"])
         X = check_array(
             X,
             copy=True,
             estimator=self,
-            force_all_finite=True,
+            force_all_finite=False,
             dtype=None,
             ensure_2d=True,
         )
 
         if X.shape[1] != self.n_features_in_:
             raise ValueError(f"number of columns {X.shape[1]} does not match fit size {self.n_features_in_}")
         return np.vectorize(self.mapper.get, otypes=[int])(X, self.default)
@@ -118,7 +120,10 @@
     @property
     def dim_(self):
         warn(
             "Please use `n_features_in_` instead of `dim_`, `dim_` will be deprecated in future versions",
             DeprecationWarning,
         )
         return self.n_features_in_
+
+    def _more_tags(self):
+        return {"preserves_dtype": None, "allow_nan": True, "no_validation": True}
```

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/formulaictransformer.py` & `scikit-lego-0.9.0/sklego/preprocessing/formulaictransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     #	Intercept	a[T.B]	a[T.C]	b	    a[T.B]:b	a[T.C]:b
     #0	1.0	        0	    0	    0.3	    0.0	        0.0
     #1	1.0	        1	    0	    0.1	    0.1	        0.0
     #2	1.0	        0	    1	    0.2	    0.0	        0.2
     ```
     """
 
+    _required_parameters = ["formula"]
+
     def __init__(self, formula, return_type="numpy"):
         self.formula = formula
         self.return_type = return_type
 
     def fit(self, X, y=None):
         """Fit the `FormulaicTransformer` to the data by compiling the formula specification into a model spec.
```

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/identitytransformer.py` & `scikit-lego-0.9.0/sklego/preprocessing/identitytransformer.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/intervalencoder.py` & `scikit-lego-0.9.0/sklego/preprocessing/intervalencoder.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/outlier_remover.py` & `scikit-lego-0.9.0/sklego/preprocessing/outlier_remover.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,18 +39,19 @@
     outlier_remover = OutlierRemover(isolation_forest, refit=True)
     outlier_remover.fit(X)
 
     X_trans = outlier_remover.transform_train(X)
     ```
     """
 
+    _required_parameters = ["outlier_detector"]
+
     def __init__(self, outlier_detector, refit=True):
         self.outlier_detector = outlier_detector
         self.refit = refit
-        self.estimator_ = None
 
     def fit(self, X, y=None):
         """Fit the estimator on training data `X` and `y` by fitting the underlying outlier detector if `refit` is True.
 
         Parameters
         ----------
         X : array-like of shape (n_samples, n_features)
```

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/projections.py` & `scikit-lego-0.9.0/sklego/preprocessing/projections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+import narwhals as nw
 import numpy as np
-import pandas as pd
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
 
 from sklego.common import as_list
 
 
@@ -75,15 +75,15 @@
         Q, R = np.linalg.qr(X)
         self.inv_R_ = np.linalg.inv(R)
 
         if self.normalize:
             self.normalization_vector_ = np.linalg.norm(Q, ord=2, axis=0)
         else:
             self.normalization_vector_ = np.ones((X.shape[1],))
-
+        self.n_features_in_ = X.shape[1]
         return self
 
     def transform(self, X):
         """Transforms `X` using the fitted inverse of R. Normalizes the result if required.
 
         Parameters
         ----------
@@ -171,30 +171,33 @@
     InformationFilter(columns=["length", "age"], alpha=0.5).fit_transform(df)
     # array([[50.10152483,  3.87905643],
     #        [50.26253897, 19.59684308],
     #        [52.66084873, 28.06719867]])
     ```
     """
 
+    _required_parameters = ["columns"]
+
     def __init__(self, columns, alpha=1):
         self.columns = columns
         self.alpha = alpha
 
     def _check_coltype(self, X):
         """Check if the `columns` type(s) are compatible with `X` type."""
+        X_ = nw.from_native(X, strict=False, eager_only=True)
         for col in as_list(self.columns):
             if isinstance(col, str):
-                if isinstance(X, np.ndarray):
+                if isinstance(X_, np.ndarray):
                     raise ValueError(f"column {col} is a string but datatype receive is numpy.")
-                if isinstance(X, pd.DataFrame):
-                    if col not in X.columns:
-                        raise ValueError(f"column {col} is not in {X.columns}")
+                if isinstance(X_, nw.DataFrame):
+                    if col not in X_.columns:
+                        raise ValueError(f"column {col} is not in {X_.columns}")
             if isinstance(col, int):
-                if col not in range(np.atleast_2d(np.array(X)).shape[1]):
-                    raise ValueError(f"column {col} is out of bounds for input shape {X.shape}")
+                if col not in range(np.atleast_2d(np.array(X_)).shape[1]):
+                    raise ValueError(f"column {col} is out of bounds for input shape {X_.shape}")
 
     def _col_idx(self, X, name):
         """Get the column index of a column name."""
         if isinstance(name, str):
             if isinstance(X, np.ndarray):
                 raise ValueError("You cannot have a column of type string on a numpy input matrix.")
             return {name: i for i, name in enumerate(X.columns)}[name]
@@ -238,14 +241,16 @@
         # gram smidt process but only on sensitive attributes
         for i, col in enumerate(X_fair.T):
             for v in v_vectors.T:
                 X_fair[:, i] = X_fair[:, i] - vector_projection(X_fair[:, i], v)
         # we want to learn matrix P: X P = X_fair
         # this means we first need to create X_fair in order to learn P
         self.projection_, resid, rank, s = np.linalg.lstsq(X, X_fair, rcond=None)
+        self.n_features_in_ = X.shape[1]
+
         return self
 
     def transform(self, X):
         """Transforms `X` by applying the information filter.
 
         Parameters
         ----------
```

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/randomadder.py` & `scikit-lego-0.9.0/sklego/preprocessing/randomadder.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,7 +97,10 @@
     @property
     def dim_(self):
         warn(
             "Please use `n_features_in_` instead of `dim_`, `dim_` will be deprecated in future versions",
             DeprecationWarning,
         )
         return self.n_features_in_
+
+    def _more_tags(self):
+        return {"non_deterministic": True}
```

### Comparing `scikit-lego-0.8.2/sklego/preprocessing/repeatingbasis.py` & `scikit-lego-0.9.0/sklego/preprocessing/repeatingbasis.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/testing.py` & `scikit-lego-0.9.0/sklego/testing.py`

 * *Files identical despite different names*

### Comparing `scikit-lego-0.8.2/sklego/this.py` & `scikit-lego-0.9.0/sklego/this.py`

 * *Files identical despite different names*

