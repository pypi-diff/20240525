# Comparing `tmp/scoringrules-0.5.0.tar.gz` & `tmp/scoringrules-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoringrules-0.5.0.tar", max compression
+gzip compressed data, was "scoringrules-0.5.1.tar", max compression
```

## Comparing `scoringrules-0.5.0.tar` & `scoringrules-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11348 2023-05-10 12:48:41.343565 scoringrules-0.5.0/LICENSE
--rw-r--r--   0        0        0     2504 2024-05-08 07:29:05.548392 scoringrules-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1158 2024-04-04 18:44:03.729234 scoringrules-0.5.0/scoringrules/__init__.py
--rw-r--r--   0        0        0      952 2024-05-08 07:26:24.480906 scoringrules-0.5.0/scoringrules/_brier.py
--rw-r--r--   0        0        0    13391 2024-05-08 07:26:24.481381 scoringrules-0.5.0/scoringrules/_crps.py
--rw-r--r--   0        0        0     9326 2024-05-08 07:26:24.482229 scoringrules-0.5.0/scoringrules/_energy.py
--rw-r--r--   0        0        0     1455 2024-05-08 07:26:24.482623 scoringrules-0.5.0/scoringrules/_error_spread.py
--rw-r--r--   0        0        0     1121 2024-05-08 07:26:24.483091 scoringrules-0.5.0/scoringrules/_logs.py
--rw-r--r--   0        0        0     9639 2024-05-08 07:26:24.483485 scoringrules-0.5.0/scoringrules/_variogram.py
--rw-r--r--   0        0        0      207 2023-11-21 10:51:34.399740 scoringrules-0.5.0/scoringrules/backend/__init__.py
--rw-r--r--   0        0        0     7880 2024-04-30 08:37:43.267646 scoringrules-0.5.0/scoringrules/backend/base.py
--rw-r--r--   0        0        0     5694 2024-04-30 08:37:43.269594 scoringrules-0.5.0/scoringrules/backend/jax.py
--rw-r--r--   0        0        0     5253 2024-04-30 08:37:43.272167 scoringrules-0.5.0/scoringrules/backend/numpy.py
--rw-r--r--   0        0        0     2423 2024-01-12 19:11:22.760540 scoringrules-0.5.0/scoringrules/backend/registry.py
--rw-r--r--   0        0        0     7083 2024-04-30 08:37:43.275286 scoringrules-0.5.0/scoringrules/backend/tensorflow.py
--rw-r--r--   0        0        0     6262 2024-04-30 08:37:43.277534 scoringrules-0.5.0/scoringrules/backend/torch.py
--rw-r--r--   0        0        0        0 2023-11-01 17:12:40.919839 scoringrules-0.5.0/scoringrules/core/__init__.py
--rw-r--r--   0        0        0      733 2024-05-08 07:26:24.484282 scoringrules-0.5.0/scoringrules/core/brier.py
--rw-r--r--   0        0        0      286 2024-04-04 18:44:03.730806 scoringrules-0.5.0/scoringrules/core/crps/__init__.py
--rw-r--r--   0        0        0     3408 2024-05-08 07:26:24.484679 scoringrules-0.5.0/scoringrules/core/crps/_approx.py
--rw-r--r--   0        0        0     1711 2024-05-08 07:26:24.485021 scoringrules-0.5.0/scoringrules/core/crps/_closed.py
--rw-r--r--   0        0        0     9081 2024-05-08 07:26:24.485435 scoringrules-0.5.0/scoringrules/core/crps/_gufuncs.py
--rw-r--r--   0        0        0      376 2023-11-01 17:12:40.931435 scoringrules-0.5.0/scoringrules/core/energy/__init__.py
--rw-r--r--   0        0        0     2289 2024-05-08 07:26:24.485821 scoringrules-0.5.0/scoringrules/core/energy/_gufuncs.py
--rw-r--r--   0        0        0     2500 2024-05-08 07:26:24.486413 scoringrules-0.5.0/scoringrules/core/energy/_score.py
--rw-r--r--   0        0        0      143 2024-04-30 08:37:43.279924 scoringrules-0.5.0/scoringrules/core/error_spread/__init__.py
--rw-r--r--   0        0        0      763 2024-05-08 07:26:24.486827 scoringrules-0.5.0/scoringrules/core/error_spread/_gufunc.py
--rw-r--r--   0        0        0      617 2024-05-08 07:26:24.487217 scoringrules-0.5.0/scoringrules/core/error_spread/_score.py
--rw-r--r--   0        0        0      677 2024-05-08 07:26:24.487554 scoringrules-0.5.0/scoringrules/core/logarithmic.py
--rw-r--r--   0        0        0     5609 2024-04-30 08:37:43.285897 scoringrules-0.5.0/scoringrules/core/stats.py
--rw-r--r--   0        0        0      476 2024-04-30 08:37:43.287370 scoringrules-0.5.0/scoringrules/core/typing.py
--rw-r--r--   0        0        0     1302 2024-05-08 07:26:24.487885 scoringrules-0.5.0/scoringrules/core/utils.py
--rw-r--r--   0        0        0      397 2023-11-01 17:12:40.944275 scoringrules-0.5.0/scoringrules/core/variogram/__init__.py
--rw-r--r--   0        0        0     2777 2024-05-08 07:26:24.488244 scoringrules-0.5.0/scoringrules/core/variogram/_gufuncs.py
--rw-r--r--   0        0        0     3332 2024-05-08 07:26:24.488585 scoringrules-0.5.0/scoringrules/core/variogram/_score.py
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 scoringrules-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-05-24 14:33:45.077293 scoringrules-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2522 2024-05-25 12:20:56.125394 scoringrules-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1198 2024-05-25 12:20:14.514041 scoringrules-0.5.1/scoringrules/__init__.py
+-rw-r--r--   0        0        0      952 2024-05-16 15:29:48.255457 scoringrules-0.5.1/scoringrules/_brier.py
+-rw-r--r--   0        0        0    15477 2024-05-25 12:20:14.515463 scoringrules-0.5.1/scoringrules/_crps.py
+-rw-r--r--   0        0        0     9326 2024-05-16 15:29:48.258821 scoringrules-0.5.1/scoringrules/_energy.py
+-rw-r--r--   0        0        0     1455 2024-05-16 15:29:48.260068 scoringrules-0.5.1/scoringrules/_error_spread.py
+-rw-r--r--   0        0        0     1121 2024-05-16 15:29:48.260993 scoringrules-0.5.1/scoringrules/_logs.py
+-rw-r--r--   0        0        0     9639 2024-05-16 15:29:48.262279 scoringrules-0.5.1/scoringrules/_variogram.py
+-rw-r--r--   0        0        0      207 2023-12-21 16:44:36.815394 scoringrules-0.5.1/scoringrules/backend/__init__.py
+-rw-r--r--   0        0        0     7880 2024-05-16 15:29:48.263551 scoringrules-0.5.1/scoringrules/backend/base.py
+-rw-r--r--   0        0        0     5694 2024-05-16 15:29:48.264609 scoringrules-0.5.1/scoringrules/backend/jax.py
+-rw-r--r--   0        0        0     5253 2024-05-16 15:29:48.265610 scoringrules-0.5.1/scoringrules/backend/numpy.py
+-rw-r--r--   0        0        0     2423 2024-01-12 21:14:37.070511 scoringrules-0.5.1/scoringrules/backend/registry.py
+-rw-r--r--   0        0        0     7083 2024-05-16 15:29:48.266959 scoringrules-0.5.1/scoringrules/backend/tensorflow.py
+-rw-r--r--   0        0        0     6262 2024-05-16 15:29:48.268258 scoringrules-0.5.1/scoringrules/backend/torch.py
+-rw-r--r--   0        0        0        0 2023-11-10 08:02:17.497880 scoringrules-0.5.1/scoringrules/core/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-16 15:29:48.268876 scoringrules-0.5.1/scoringrules/core/brier.py
+-rw-r--r--   0        0        0      384 2024-05-25 12:20:14.517248 scoringrules-0.5.1/scoringrules/core/crps/__init__.py
+-rw-r--r--   0        0        0     3822 2024-05-25 12:20:14.517831 scoringrules-0.5.1/scoringrules/core/crps/_approx.py
+-rw-r--r--   0        0        0     1711 2024-05-16 15:29:48.269820 scoringrules-0.5.1/scoringrules/core/crps/_closed.py
+-rw-r--r--   0        0        0     9680 2024-05-25 12:20:14.518827 scoringrules-0.5.1/scoringrules/core/crps/_gufuncs.py
+-rw-r--r--   0        0        0      376 2023-11-10 08:02:17.502536 scoringrules-0.5.1/scoringrules/core/energy/__init__.py
+-rw-r--r--   0        0        0     2289 2024-05-16 15:29:48.272647 scoringrules-0.5.1/scoringrules/core/energy/_gufuncs.py
+-rw-r--r--   0        0        0     2500 2024-05-16 15:29:48.273257 scoringrules-0.5.1/scoringrules/core/energy/_score.py
+-rw-r--r--   0        0        0      143 2024-05-16 15:29:48.274084 scoringrules-0.5.1/scoringrules/core/error_spread/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-16 15:29:48.274598 scoringrules-0.5.1/scoringrules/core/error_spread/_gufunc.py
+-rw-r--r--   0        0        0      617 2024-05-16 15:29:48.275036 scoringrules-0.5.1/scoringrules/core/error_spread/_score.py
+-rw-r--r--   0        0        0      677 2024-05-16 15:29:48.275581 scoringrules-0.5.1/scoringrules/core/logarithmic.py
+-rw-r--r--   0        0        0     5609 2024-05-16 15:29:48.276229 scoringrules-0.5.1/scoringrules/core/stats.py
+-rw-r--r--   0        0        0      476 2024-05-16 15:29:48.276660 scoringrules-0.5.1/scoringrules/core/typing.py
+-rw-r--r--   0        0        0     1302 2024-05-16 15:29:48.277041 scoringrules-0.5.1/scoringrules/core/utils.py
+-rw-r--r--   0        0        0      397 2023-11-10 08:02:17.505745 scoringrules-0.5.1/scoringrules/core/variogram/__init__.py
+-rw-r--r--   0        0        0     2777 2024-05-16 15:29:48.277466 scoringrules-0.5.1/scoringrules/core/variogram/_gufuncs.py
+-rw-r--r--   0        0        0     3332 2024-05-16 15:29:48.278010 scoringrules-0.5.1/scoringrules/core/variogram/_score.py
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 scoringrules-0.5.1/PKG-INFO
```

### Comparing `scoringrules-0.5.0/LICENSE` & `scoringrules-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/pyproject.toml` & `scoringrules-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scoringrules"
-version = "0.5.0"
+version = "0.5.1"
 description = "Scoring rules for probabilistic forecast evaluation."
 authors = [
   "Francesco Zanetta <zanetta.francesco@gmail.com>",
   "Sam Allen <sam.allen@unibe.ch>",
 ]
 homepage = "https://github.com/frazane/scoringrules"
 documentation = "https://frazane.github.io/scoringrules/"
@@ -12,14 +12,15 @@
 
 [tool.poetry.urls]
 "Homepage" = "https://github.com/frazane/scoringrules"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "^1.23.4"
+scipy = "^1.10.0"
 numba = "^0.57.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.3"
 mkdocstrings = { extras = ["python"], version = "^0.24.0" }
 jupyter = "^1.0.0"
```

### Comparing `scoringrules-0.5.0/scoringrules/__init__.py` & `scoringrules-0.5.1/scoringrules/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from scoringrules._brier import brier_score
 from scoringrules._crps import (
     crps_ensemble,
     crps_logistic,
     crps_lognormal,
     crps_normal,
+    crps_quantile,
     owcrps_ensemble,
     twcrps_ensemble,
     vrcrps_ensemble,
 )
 from scoringrules._energy import (
     energy_score,
     owenergy_score,
@@ -32,14 +33,15 @@
 __all__ = [
     "register_backend",
     "backends",
     "crps_ensemble",
     "crps_normal",
     "crps_lognormal",
     "crps_logistic",
+    "crps_quantile",
     "owcrps_ensemble",
     "twcrps_ensemble",
     "vrcrps_ensemble",
     "logs_normal",
     "brier_score",
     "error_spread_score",
     "energy_score",
```

### Comparing `scoringrules-0.5.0/scoringrules/_brier.py` & `scoringrules-0.5.1/scoringrules/_brier.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/_crps.py` & `scoringrules-0.5.1/scoringrules/_crps.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,14 +122,78 @@
         axis=axis,
         sorted_ensemble=sorted_ensemble,
         estimator=estimator,
         backend=backend,
     )
 
 
+def crps_quantile(
+    observations: "ArrayLike",
+    forecasts: "Array",
+    alpha: "Array",
+    /,
+    axis: int = -1,
+    *,
+    backend: "Backend" = None,
+) -> "Array":
+    r"""Approximate the CRPS from quantile predictions via the Pinball Loss.
+
+    It is based on the notation in [Berrisch & Ziel, 2022](https://arxiv.org/pdf/2102.00968)
+
+    The CRPS can be approximated as the mean pinball loss for all
+    quantile forecasts $F_q$ with level $q \in Q$:
+
+    $$\text{quantileCRPS} = \frac{2}{|Q|} \sum_{q \in Q} PB_q$$
+
+    where the pinball loss is defined as:
+
+    $$\text{PB}_q = \begin{cases}
+        q(y - F_q) &\text{if} & y \geq F_q  \\
+        (1-q)(F_q - y) &\text{else.} &  \\
+    \end{cases} $$
+
+    Parameters
+    ----------
+    observations: ArrayLike
+        The observed values.
+    forecasts: Array
+        The predicted forecast ensemble, where the ensemble dimension is by default
+        represented by the last axis.
+    alpha: Array
+        The percentile levels. We expect the quantile array to match the axis (see below) of the forecast array.
+    axis: int
+        The axis corresponding to the ensemble. Default is the last axis.
+    backend: str
+        The name of the backend used for computations. Defaults to 'numba' if available, else 'numpy'.
+
+    Returns
+    -------
+    qcrps: Array
+        An array of CRPS scores for each forecast, which should be averaged to get meaningful values.
+
+    Examples
+    --------
+    >>> import scoringrules as sr
+    >>> sr.crps_quantile(obs, fct, alpha)
+    """
+    B = backends.active if backend is None else backends[backend]
+    observations, forecasts, alpha = map(B.asarray, (observations, forecasts, alpha))
+
+    if axis != -1:
+        forecasts = B.moveaxis(forecasts, axis, -1)
+
+    if not forecasts.shape[-1] == alpha.shape[-1]:
+        raise ValueError("Expected matching length of forecasts and alpha values.")
+
+    if B.name == "numba":
+        return crps.quantile_pinball_gufunc(observations, forecasts, alpha)
+
+    return crps.quantile_pinball(observations, forecasts, alpha, backend=backend)
+
+
 def owcrps_ensemble(
     observations: "ArrayLike",
     forecasts: "Array",
     w_func: tp.Callable[["ArrayLike"], "ArrayLike"],
     /,
     axis: int = -1,
     *,
```

### Comparing `scoringrules-0.5.0/scoringrules/_energy.py` & `scoringrules-0.5.1/scoringrules/_energy.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/_error_spread.py` & `scoringrules-0.5.1/scoringrules/_error_spread.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/_logs.py` & `scoringrules-0.5.1/scoringrules/_logs.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/_variogram.py` & `scoringrules-0.5.1/scoringrules/_variogram.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/backend/base.py` & `scoringrules-0.5.1/scoringrules/backend/base.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/backend/jax.py` & `scoringrules-0.5.1/scoringrules/backend/jax.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/backend/numpy.py` & `scoringrules-0.5.1/scoringrules/backend/numpy.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/backend/registry.py` & `scoringrules-0.5.1/scoringrules/backend/registry.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/backend/tensorflow.py` & `scoringrules-0.5.1/scoringrules/backend/tensorflow.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/backend/torch.py` & `scoringrules-0.5.1/scoringrules/backend/torch.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/brier.py` & `scoringrules-0.5.1/scoringrules/core/brier.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/crps/_approx.py` & `scoringrules-0.5.1/scoringrules/core/crps/_approx.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,24 @@
     M: int = fct.shape[-1]
     expected_diff = B.sum(B.abs(obs[..., None] - fct), axis=-1) / M
     β_0 = B.sum(fct, axis=-1) / M
     β_1 = B.sum(fct * B.arange(M), axis=-1) / (M * (M - 1.0))
     return expected_diff + β_0 - 2.0 * β_1
 
 
+def quantile_pinball(
+    obs: "Array", fct: "Array", alpha: "Array", backend: "Backend" = None
+) -> "Array":
+    """CRPS approximation via Pinball Loss."""
+    B = backends.active if backend is None else backends[backend]
+    below = (fct <= obs[..., None]) * alpha * (obs[..., None] - fct)
+    above = (fct > obs[..., None]) * (1 - alpha) * (fct - obs[..., None])
+    return 2 * B.mean(below + above, axis=-1)
+
+
 def ow_ensemble(
     obs: "Array",
     fct: "Array",
     ow: "Array",
     fw: "Array",
     backend: "Backend" = None,
 ) -> "Array":
```

### Comparing `scoringrules-0.5.0/scoringrules/core/crps/_closed.py` & `scoringrules-0.5.1/scoringrules/core/crps/_closed.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/crps/_gufuncs.py` & `scoringrules-0.5.1/scoringrules/core/crps/_gufuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,33 @@
 
 INV_SQRT_PI = 1 / np.sqrt(np.pi)
 EPSILON = 1e-6
 
 
 @guvectorize(
     [
+        "void(float32[:], float32[:], float32[:], float32[:])",
+        "void(float64[:], float64[:], float64[:], float64[:])",
+    ],
+    "(),(a),(a)->()",
+)
+def quantile_pinball_gufunc(
+    obs: np.ndarray, fct: np.ndarray, alpha: np.ndarray, out: np.ndarray
+):
+    """Pinball loss based estimator for the CRPS from quantiles."""
+    obs = obs[0]
+    Q = fct.shape[0]
+    pb = 0
+    for fc, level in zip(fct, alpha):  # noqa: B905
+        pb += (obs > fc) * level * (obs - fc) + (obs <= fc) * (1 - level) * (fc - obs)
+    out[0] = 2 * (pb / Q)
+
+
+@guvectorize(
+    [
         "void(float32[:], float32[:], float32[:])",
         "void(float64[:], float64[:], float64[:])",
     ],
     "(),(n)->()",
 )
 def _crps_ensemble_int_gufunc(obs: np.ndarray, fct: np.ndarray, out: np.ndarray):
     """CRPS estimator based on the integral form."""
@@ -343,8 +362,9 @@
     "_crps_ensemble_int_gufunc",
     "_crps_ensemble_nrg_gufunc",
     "_crps_ensemble_pwm_gufunc",
     "_crps_ensemble_qd_gufunc",
     "_crps_normal_ufunc",
     "_crps_lognormal_ufunc",
     "_crps_logistic_ufunc",
+    "quantile_pinball_gufunc",
 ]
```

### Comparing `scoringrules-0.5.0/scoringrules/core/energy/_gufuncs.py` & `scoringrules-0.5.1/scoringrules/core/energy/_gufuncs.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/energy/_score.py` & `scoringrules-0.5.1/scoringrules/core/energy/_score.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/error_spread/_gufunc.py` & `scoringrules-0.5.1/scoringrules/core/error_spread/_gufunc.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/error_spread/_score.py` & `scoringrules-0.5.1/scoringrules/core/error_spread/_score.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/logarithmic.py` & `scoringrules-0.5.1/scoringrules/core/logarithmic.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/stats.py` & `scoringrules-0.5.1/scoringrules/core/stats.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/utils.py` & `scoringrules-0.5.1/scoringrules/core/utils.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/variogram/_gufuncs.py` & `scoringrules-0.5.1/scoringrules/core/variogram/_gufuncs.py`

 * *Files identical despite different names*

### Comparing `scoringrules-0.5.0/scoringrules/core/variogram/_score.py` & `scoringrules-0.5.1/scoringrules/core/variogram/_score.py`

 * *Files identical despite different names*

