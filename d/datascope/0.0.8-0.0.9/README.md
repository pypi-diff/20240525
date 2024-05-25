# Comparing `tmp/datascope-0.0.8.tar.gz` & `tmp/datascope-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascope-0.0.8.tar", last modified: Tue Dec 27 00:55:40 2022, max compression
+gzip compressed data, was "datascope-0.0.9.tar", last modified: Sat Feb 11 00:35:44 2023, max compression
```

## Comparing `datascope-0.0.8.tar` & `datascope-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 00:55:40.739293 datascope-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-27 00:54:31.000000 datascope-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-27 00:54:31.000000 datascope-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2022-12-27 00:55:40.739293 datascope-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2022-12-27 00:54:31.000000 datascope-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 00:55:40.739293 datascope-0.0.8/datascope/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 00:55:40.739293 datascope-0.0.8/datascope/debugger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/debugger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/debugger/debugger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 00:55:40.739293 datascope-0.0.8/datascope/importance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/importance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17171 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/importance/add.py
--rw-r--r--   0 runner    (1001) docker     (123)    19976 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/importance/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/importance/importance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/importance/shapley.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/importance/shapley_cy.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-27 00:54:31.000000 datascope-0.0.8/datascope/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-27 00:55:40.739293 datascope-0.0.8/datascope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2022-12-27 00:55:40.000000 datascope-0.0.8/datascope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2022-12-27 00:55:40.000000 datascope-0.0.8/datascope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-27 00:55:40.000000 datascope-0.0.8/datascope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2022-12-27 00:55:40.000000 datascope-0.0.8/datascope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-27 00:55:40.000000 datascope-0.0.8/datascope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-27 00:54:31.000000 datascope-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2022-12-27 00:54:31.000000 datascope-0.0.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-27 00:54:31.000000 datascope-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-27 00:55:40.739293 datascope-0.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1978 2022-12-27 00:54:31.000000 datascope-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:35:44.383958 datascope-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-11 00:34:48.000000 datascope-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-11 00:34:48.000000 datascope-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-02-11 00:35:44.383958 datascope-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-02-11 00:34:48.000000 datascope-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:35:44.379958 datascope-0.0.9/datascope/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:35:44.383958 datascope-0.0.9/datascope/debugger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/debugger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/debugger/debugger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:35:44.383958 datascope-0.0.9/datascope/importance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/importance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/importance/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22762 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/importance/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/importance/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21620 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/importance/shapley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/importance/shapley_cy.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-11 00:34:48.000000 datascope-0.0.9/datascope/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 00:35:44.383958 datascope-0.0.9/datascope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-02-11 00:35:44.000000 datascope-0.0.9/datascope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-02-11 00:35:44.000000 datascope-0.0.9/datascope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 00:35:44.000000 datascope-0.0.9/datascope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-11 00:35:44.000000 datascope-0.0.9/datascope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-11 00:35:44.000000 datascope-0.0.9/datascope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-11 00:34:48.000000 datascope-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-02-11 00:34:48.000000 datascope-0.0.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-11 00:34:48.000000 datascope-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-11 00:35:44.383958 datascope-0.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1978 2023-02-11 00:34:48.000000 datascope-0.0.9/setup.py
```

### Comparing `datascope-0.0.8/LICENSE` & `datascope-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datascope-0.0.8/PKG-INFO` & `datascope-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope
-Version: 0.0.8
+Version: 0.0.9
 Summary: Measuring data importance over ML pipelines using the Shapley value.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Ease.ml/Datascope: Guiding your Data-centric Data Iterations, over End-to-end ML pipelines
         
         [![PyPI version](https://badge.fury.io/py/datascope.svg)](https://badge.fury.io/py/datascope)
```

### Comparing `datascope-0.0.8/README.md` & `datascope-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `datascope-0.0.8/datascope/debugger/debugger.py` & `datascope-0.0.9/datascope/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `datascope-0.0.8/datascope/importance/add.py` & `datascope-0.0.9/datascope/importance/add.py`

 * *Files identical despite different names*

### Comparing `datascope-0.0.8/datascope/importance/common.py` & `datascope-0.0.9/datascope/importance/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 import collections.abc
 import numpy as np
 import warnings
 
 from abc import ABC, abstractmethod
 from collections import defaultdict
+from functools import partial
 from numpy import ndarray
 from typing import Iterable, Optional, Callable, Sequence, Tuple, Union, List
 from typing_extensions import Protocol
 from sklearn.base import clone
-from sklearn.metrics import accuracy_score
+from sklearn.metrics import accuracy_score, roc_auc_score
 
 
 class SklearnModel(Protocol):
     def fit(self, X: ndarray, y: ndarray, sample_weight: Optional[ndarray] = None) -> None:
         pass
 
     def predict(self, X: ndarray) -> ndarray:
         pass
 
+    def predict_proba(self, X: ndarray) -> ndarray:
+        pass
+
 
 class SklearnTransformer(Protocol):
     def fit(self, X: ndarray, y: ndarray, sample_weight: Optional[ndarray] = None) -> None:
         pass
 
     def transform(self, X: ndarray) -> ndarray:
         pass
@@ -288,14 +292,85 @@
             if min_score > score:
                 min_score = score
                 result = elementwise_sore
 
         return result
 
 
+class SklearnModelRocAuc(SklearnModelUtility):
+    def __init__(self, model: SklearnModelOrPipeline) -> None:
+        metric = partial(roc_auc_score, multi_class="ovr")  # We multi-class mode to be one-vs-rest.
+        super().__init__(model, metric)
+
+    def _model_predict(self, model: SklearnModelOrPipeline, X_test: ndarray) -> ndarray:
+        y_test_pred_proba = model.predict_proba(X_test)
+        if y_test_pred_proba.shape[1] == 2:
+            y_test_pred_proba = y_test_pred_proba[:, 1]
+        return y_test_pred_proba
+
+    def null_score(
+        self,
+        X_train: ndarray,
+        y_train: ndarray,
+        X_test: ndarray,
+        y_test: ndarray,
+    ) -> float:
+        scores = []
+        classes = np.unique(y_train)
+        for x in classes:
+            y_spoof = np.full((y_test.shape[0], len(classes)), np.eye(len(classes))[x])
+            if y_spoof.shape[1] == 2:
+                y_spoof = y_spoof[:, 1]
+            scores.append(self._metric_score(self.metric, y_test, y_spoof, X_test=X_test))
+
+        return min(scores)
+
+    def elementwise_score(
+        self,
+        X_train: ndarray,
+        y_train: ndarray,
+        X_test: ndarray,
+        y_test: ndarray,
+    ) -> ndarray:
+        classes = np.unique(y_train)
+        result = np.zeros((len(y_train), len(y_test)))
+        for c in classes:
+            eq = np.equal.outer(y_train, y_test)
+            all_c = np.full_like(y_train, c, dtype=y_train.dtype)
+            tp = (eq * np.equal.outer(all_c, y_test)).astype(float)
+            tn = (eq * np.not_equal.outer(all_c, y_test)).astype(float)
+            p = np.equal(y_test, c).sum(dtype=float)
+            n = np.not_equal(y_test, c).sum(dtype=float)
+            result += (tp / p + tn / n) * 0.5
+        return result / float(len(classes))
+
+    def elementwise_null_score(
+        self,
+        X_train: ndarray,
+        y_train: ndarray,
+        X_test: ndarray,
+        y_test: ndarray,
+    ) -> ndarray:
+        result = np.zeros_like(y_test, dtype=float)
+        classes, counts = np.unique(y_test, return_counts=True)
+        least_frequent_class = classes[np.argmin(counts)]
+        y_spoof = np.full_like(y_test, least_frequent_class, dtype=y_test.dtype)
+
+        for c in classes:
+            eq = np.equal(y_spoof, y_test)
+            all_c = np.full_like(y_spoof, c, dtype=y_spoof.dtype)
+            tp = (eq * np.equal(all_c, y_test)).astype(float)
+            tn = (eq * np.not_equal(all_c, y_test)).astype(float)
+            p = np.equal(y_test, c).sum(dtype=float)
+            n = np.not_equal(y_test, c).sum(dtype=float)
+            result += (tp / p + tn / n) * 0.5
+
+        return result / float(len(classes))
+
+
 def compute_groupings(X: ndarray, sensitive_features: Union[int, Sequence[int]]) -> ndarray:
     if not isinstance(sensitive_features, collections.abc.Sequence):
         sensitive_features = [sensitive_features]
     X_sf = X[:, sensitive_features]
     unique_values = np.unique(X_sf, axis=0)
     groupings = np.zeros(X.shape[0], dtype=int)
     for i, unique in enumerate(unique_values):
```

### Comparing `datascope-0.0.8/datascope/importance/importance.py` & `datascope-0.0.9/datascope/importance/importance.py`

 * *Files identical despite different names*

### Comparing `datascope-0.0.8/datascope/importance/shapley.py` & `datascope-0.0.9/datascope/importance/shapley.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from scipy.special import comb
 
 # from numba import prange, jit
 from logging import Logger, getLogger
 from numpy import ndarray
 from scipy.sparse import csr_matrix, issparse, spmatrix
 from scipy.sparse.csgraph import connected_components
-from sklearn.metrics import DistanceMetric
+
+try:
+    from sklearn.metrics import DistanceMetric
+except ImportError:
+    from sklearn.neighbors import DistanceMetric
+
 from sklearn.pipeline import Pipeline
 
 from typing_extensions import Literal
 from typing import Dict, List, Optional, Iterable, Set, Tuple
 
 # from .add import ADD
 from .common import DEFAULT_SEED, DistanceCallable, Utility, binarize, get_indices, reshape
@@ -509,21 +514,29 @@
             provenance = binarize(provenance)
 
         # Apply the feature extraction pipeline if it was provided.
         if self.pipeline is not None:
             X = self.pipeline.fit_transform(X, y=y)
             X_test = self.pipeline.transform(X_test)
 
-        # Compute the distances between training and text data examples.
+        # Ensure X and X_test are not sparse.
         if issparse(X):
             assert isinstance(X, spmatrix)
             X = X.todense()
         if issparse(X_test):
             assert isinstance(X_test, spmatrix)
             X_test = X_test.todense()
+
+        # Convert matrices to instances of ndarray.
+        if isinstance(X, np.matrix):
+            X = np.asarray(X)
+        if isinstance(X_test, np.matrix):
+            X_test = np.asarray(X_test)
+
+        # Compute the distances between training and text data examples.
         distances = distance(X, X_test)
 
         # Compute the utilitiy values between training and test labels.
         utilities = self.utility.elementwise_score(X_train=X, y_train=y, X_test=X_test, y_test=y_test)
 
         # Compute null scores.
         null_scores = self.utility.elementwise_null_score(X, y, X_test, y_test)
```

### Comparing `datascope-0.0.8/datascope/importance/shapley_cy.pyx` & `datascope-0.0.9/datascope/importance/shapley_cy.pyx`

 * *Files identical despite different names*

### Comparing `datascope-0.0.8/datascope.egg-info/PKG-INFO` & `datascope-0.0.9/datascope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope
-Version: 0.0.8
+Version: 0.0.9
 Summary: Measuring data importance over ML pipelines using the Shapley value.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Ease.ml/Datascope: Guiding your Data-centric Data Iterations, over End-to-end ML pipelines
         
         [![PyPI version](https://badge.fury.io/py/datascope.svg)](https://badge.fury.io/py/datascope)
```

### Comparing `datascope-0.0.8/datascope.egg-info/SOURCES.txt` & `datascope-0.0.9/datascope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datascope-0.0.8/setup.py` & `datascope-0.0.9/setup.py`

 * *Files identical despite different names*

