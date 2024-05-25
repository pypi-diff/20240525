# Comparing `tmp/logbesselk-3.2.1.tar.gz` & `tmp/logbesselk-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logbesselk-3.2.1.tar", max compression
+gzip compressed data, was "logbesselk-3.3.0.tar", max compression
```

## Comparing `logbesselk-3.2.1.tar` & `logbesselk-3.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-05-24 04:48:20.673878 logbesselk-3.2.1/LICENSE.txt
--rw-r--r--   0        0        0     2265 2024-05-24 04:48:20.673878 logbesselk-3.2.1/README.md
--rw-r--r--   0        0        0     2190 2024-05-24 04:48:20.689878 logbesselk-3.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/__init__.py
--rw-r--r--   0        0        0      186 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/__init__.py
--rw-r--r--   0        0        0     1826 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/asymptotic.py
--rw-r--r--   0        0        0     1829 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/cfraction.py
--rw-r--r--   0        0        0     2715 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/integral.py
--rw-r--r--   0        0        0     1865 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/math.py
--rw-r--r--   0        0        0      789 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/misc.py
--rw-r--r--   0        0        0     1804 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/sca.py
--rw-r--r--   0        0        0     2482 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/series.py
--rw-r--r--   0        0        0     2375 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/utils.py
--rw-r--r--   0        0        0     2457 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/jax/wrap.py
--rw-r--r--   0        0        0      186 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/__init__.py
--rw-r--r--   0        0        0     2017 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/asymptotic.py
--rw-r--r--   0        0        0     1944 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/cfraction.py
--rw-r--r--   0        0        0     2878 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/integral.py
--rw-r--r--   0        0        0     2218 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/math.py
--rw-r--r--   0        0        0      861 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/misc.py
--rw-r--r--   0        0        0     1890 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/sca.py
--rw-r--r--   0        0        0     2568 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/series.py
--rw-r--r--   0        0        0     3289 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/utils.py
--rw-r--r--   0        0        0     2202 2024-05-24 04:48:20.689878 logbesselk-3.2.1/src/logbesselk/tensorflow/wrap.py
--rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 logbesselk-3.2.1/setup.py
--rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 logbesselk-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-25 17:20:21.509063 logbesselk-3.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2265 2024-05-25 17:20:21.509063 logbesselk-3.3.0/README.md
+-rw-r--r--   0        0        0     2091 2024-05-25 17:20:21.525063 logbesselk-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/__init__.py
+-rw-r--r--   0        0        0     1800 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/asymptotic.py
+-rw-r--r--   0        0        0     1812 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/cfraction.py
+-rw-r--r--   0        0        0     1667 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/ica.py
+-rw-r--r--   0        0        0     2603 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/integral.py
+-rw-r--r--   0        0        0     1714 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/math.py
+-rw-r--r--   0        0        0      781 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/misc.py
+-rw-r--r--   0        0        0     1788 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/sca.py
+-rw-r--r--   0        0        0     2412 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/series.py
+-rw-r--r--   0        0        0     2358 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/utils.py
+-rw-r--r--   0        0        0     2423 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/jax/wrap.py
+-rw-r--r--   0        0        0      283 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/__init__.py
+-rw-r--r--   0        0        0     1977 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/asymptotic.py
+-rw-r--r--   0        0        0     1913 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/cfraction.py
+-rw-r--r--   0        0        0     2729 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/integral.py
+-rw-r--r--   0        0        0     1992 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/math.py
+-rw-r--r--   0        0        0      876 2024-05-25 17:20:21.525063 logbesselk-3.3.0/src/logbesselk/tensorflow/misc.py
+-rw-r--r--   0        0        0     1874 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/sca.py
+-rw-r--r--   0        0        0     2485 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/series.py
+-rw-r--r--   0        0        0     3272 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/utils.py
+-rw-r--r--   0        0        0     2194 2024-05-25 17:20:21.529063 logbesselk-3.3.0/src/logbesselk/tensorflow/wrap.py
+-rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 logbesselk-3.3.0/setup.py
+-rw-r--r--   0        0        0     2979 1970-01-01 00:00:00.000000 logbesselk-3.3.0/PKG-INFO
```

### Comparing `logbesselk-3.2.1/LICENSE.txt` & `logbesselk-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.1/README.md` & `logbesselk-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `logbesselk-3.2.1/pyproject.toml` & `logbesselk-3.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "logbesselk"
-version = "3.2.1"
+version = "3.3.0"
 description = "Provide function to calculate the modified Bessel function of the second kind"
 license = "Apache-2.0"
 authors = ["TAKEKAWA Takashi <takekawa@tk2lab.org>"]
 readme = "README.md"
 repository = "https://github.com/tk2lab/logbesselk"
 
 [build-system]
@@ -14,86 +14,78 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 #tensorflow = ">=2.6,<2.12"
 #jax = "^0.2+cuda"
 
 [tool.isort]
 profile = "black"
+multi_line_output = 3
+force_grid_wrap = 1
 
-[tool.black]
-line-length = 79
+[tool.flake8]
+max-line-length = 88
+extend-ignore = ["E203"]
 
 [tool.pytest.ini_options]
 markers = [
     "vec",
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 min_version = 4.0
 isolated_build = True
 env_list = 
-    py{38,39,310,}-tf{26,27,28,29,210,211}
-    py{38,39,310,311,}-jax{3,4}
+    py{310,311,312}-jax{3,4}
+    py{310,311,312}-tf{29,210,211,212,213,214,215,216}
     lint
     eval_tf
     eval_jax
 
 [gh-actions]
 python =
-    3.8: py38-tf26, py38-tf211, py38-jax3, py38-jax4
-    3.9: py39-tf26
-    3.10: py310-tf29, py310-tf211
-    3.11: py311-jax3, py311-jax4
+    3.10: py310-jax3, py310-tf29
+    3.12: py312-jax4, py312-tf216
 
-[testenv:lint]
-skip_install = True
+[testenv:py{310,311,312}-jax{3,4}]
 deps =
-    isort
-    black
-    autoflake
-commands =
-    isort --sl src
-    autoflake -ri --remove-all-unused-imports --ignore-init-module-imports src
-    black src
-
-[testenv:eval_jax]
-deps =
-    jax[cuda]
+    jax3: jax[cuda] (>=0.3,<0.4)
+    jax4: jax[cuda] (>=0.4,<0.5)
+    pytest
     pandas
 install_command =
     pip install --upgrade -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html {opts} {packages}
 commands =
-    {envpython} eval/eval_jax.py
+    {envpython} -m pytest tests/test_jax.py {posargs}
 
-[testenv:eval_tf]
+[testenv:py{310,311,312}-tf{29,210,211,212,213,214,215,216}]
 deps =
-    tensorflow
+    tf29: tensorflow (>=2.9,<2.10)
+    tf210: tensorflow (>=2.10,<2.11)
+    tf211: tensorflow (>=2.11,<2.12)
+    tf212: tensorflow (>=2.12,<2.13)
+    tf213: tensorflow (>=2.13,<2.14)
+    tf214: tensorflow (>=2.14,<2.15)
+    tf215: tensorflow (>=2.15,<2.16)
+    tf216: tensorflow (>=2.16,<2.17)
+    pytest
     pandas
 commands =
-    {envpython} eval/eval_tensorflow.py
+    {envpython} -m pytest tests/test_tensorflow.py {posargs}
 
-[testenv:py{38,39,310,311,}-jax{3,4}]
+[testenv:eval_jax]
 deps =
-    jax3: jax[cuda] (>=0.3,<0.4)
-    jax4: jax[cuda] (>=0.4,<0.5)
-    pytest
+    jax[cuda]
     pandas
 install_command =
     pip install --upgrade -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html {opts} {packages}
 commands =
-    {envpython} -m pytest tests/test_jax.py {posargs}
+    {envpython} eval/eval_jax.py
 
-[testenv:py{38,39,310,}-tf{26,27,28,29,210,211}]
+[testenv:eval_tf]
 deps =
-    tf26: tensorflow (>=2.6,<2.7)
-    tf27: tensorflow (>=2.7,<2.8)
-    tf28: tensorflow (>=2.8,<2.9)
-    tf29: tensorflow (>=2.9,<2.10)
-    tf210: tensorflow (>=2.10,<2.11)
-    tf211: tensorflow (>=2.11,<2.12)
-    pytest
+    tensorflow
     pandas
 commands =
-    {envpython} -m pytest tests/test_tensorflow.py {posargs}
+    {envpython} eval/eval_tensorflow.py
 """
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/asymptotic.py` & `logbesselk-3.3.0/src/logbesselk/jax/asymptotic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import math
 
 import jax.lax as lax
 import jax.numpy as jnp
 
-from .math import fabs
-from .math import log
-from .math import sqrt
-from .math import square
-from .utils import epsilon
-from .utils import result_type
-from .wrap import wrap_log_bessel_k
+from .math import (
+    fabs,
+    log,
+    sqrt,
+    square,
+)
+from .utils import (
+    epsilon,
+    result_type,
+)
+from .wrap import (
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
 ]
 
 
 @wrap_log_bessel_k
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/cfraction.py` & `logbesselk-3.3.0/src/logbesselk/jax/cfraction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 import math
 
 import jax.lax as lax
 
-from .math import fabs
-from .math import fround
-from .math import log
-from .math import square
-from .misc import log_bessel_recurrence
-from .utils import epsilon
-from .utils import result_type
-from .wrap import wrap_log_bessel_k
+from .math import (
+    fabs,
+    fround,
+    log,
+    square,
+)
+from .misc import (
+    log_bessel_recurrence,
+)
+from .utils import (
+    epsilon,
+    result_type,
+)
+from .wrap import (
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
 ]
 
 
 @wrap_log_bessel_k
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/integral.py` & `logbesselk-3.3.0/src/logbesselk/jax/integral.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import jax.lax as lax
 import jax.numpy as jnp
-from jax import grad
-
-from .math import cosh
-from .math import is_finite
-from .math import log
-from .math import log_cosh
-from .math import log_sinh
-from .math import maximum
-from .math import square
-from .utils import epsilon
-from .utils import extend
-from .utils import find_zero
-from .utils import log_integrate
-from .utils import result_type
-from .wrap import wrap_bessel_ke
-from .wrap import wrap_bessel_kratio
-from .wrap import wrap_log_abs_deriv_bessel_k
+from jax import (
+    grad,
+)
+
+from .math import (
+    cosh,
+    is_finite,
+    log,
+    log_cosh,
+    log_sinh,
+    maximum,
+    square,
+)
+from .utils import (
+    epsilon,
+    extend,
+    find_zero,
+    log_integrate,
+    result_type,
+)
+from .wrap import (
+    wrap_bessel_ke,
+    wrap_bessel_kratio,
+    wrap_log_abs_deriv_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
     "bessel_ke",
     "bessel_kratio",
     "log_abs_deriv_bessel_k",
 ]
@@ -54,14 +62,17 @@
             out += log_sinh(v * t)
         if m > 0:
             out += m * log(t)
         if n > 0:
             out += n * log_cosh(t)
         return out
 
+    def mfunc(t):
+        return func(t) - th
+
     scale = 0.1
     tol = 1.0
     max_iter = 10
     bins = 32
 
     dtype = result_type(v, x)
     eps = epsilon(dtype)
@@ -81,15 +92,14 @@
 
     start = zero
     delta = lax.cond(deriv_at_zero_is_positive, lambda: scale, lambda: zero)
     start, delta = extend(deriv, start, delta)
     tp = find_zero(deriv, start, delta, tol, max_iter)
 
     th = func(tp) + log(eps) - tol
-    mfunc = lambda t: func(t) - th
     tpl = maximum(tp - bins * eps, zero)
     tpr = maximum(tp + bins * eps, tp * (1 + bins * eps))
     mfunc_at_zero_is_negative = out_is_finite & (mfunc(zero) < 0)
     mfunc_at_tpr_is_positive = out_is_finite & (mfunc(tpr) > 0)
 
     start = zero
     delta = lax.cond(mfunc_at_zero_is_negative, lambda: tpl, lambda: zero)
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/misc.py` & `logbesselk-3.3.0/src/logbesselk/jax/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import jax.lax as lax
 
-from .math import log
-from .math import log_add_exp
-from .math import sign
-from .utils import result_type
+from .math import (
+    log,
+    log_add_exp,
+    sign,
+)
+from .utils import (
+    result_type,
+)
 
 __all__ = [
     "sign_deriv_bessel_k",
     "log_bessel_recurrence",
 ]
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/sca.py` & `logbesselk-3.3.0/src/logbesselk/jax/sca.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import jax.lax as lax
 
 from .asymptotic import log_bessel_k_naive as log_k_large_v
 from .cfraction import log_bessel_ku as log_ku_large_x
-from .math import fround
-from .math import is_finite
-from .math import log
-from .misc import log_bessel_recurrence
+from .math import (
+    fround,
+    is_finite,
+    log,
+)
+from .misc import (
+    log_bessel_recurrence,
+)
 from .series import log_bessel_ku as log_ku_small_x
-from .utils import result_type
-from .wrap import wrap_bessel_ke
-from .wrap import wrap_bessel_kratio
-from .wrap import wrap_log_bessel_k
+from .utils import (
+    result_type,
+)
+from .wrap import (
+    wrap_bessel_ke,
+    wrap_bessel_kratio,
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
     "bessel_kratio",
     "bessel_ke",
 ]
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/series.py` & `logbesselk-3.3.0/src/logbesselk/jax/series.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import jax.lax as lax
 
-from .math import cosh
-from .math import exp
-from .math import fabs
-from .math import fround
-from .math import log
-from .math import sinc
-from .math import sinhc
-from .math import square
-from .misc import log_bessel_recurrence
-from .utils import epsilon
-from .utils import result_type
-from .wrap import wrap_log_bessel_k
+from .math import (
+    cosh,
+    exp,
+    fabs,
+    fround,
+    log,
+    sinc,
+    sinhc,
+    square,
+)
+from .misc import (
+    log_bessel_recurrence,
+)
+from .utils import (
+    epsilon,
+    result_type,
+)
+from .wrap import (
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
 ]
 
 
 @wrap_log_bessel_k
@@ -29,15 +37,14 @@
     n = fround(v)
     u = v - n
     log_ku, log_kup1 = log_bessel_ku(u, x)
     return log_bessel_recurrence(log_ku, log_kup1, u, n, x)[0]
 
 
 def log_bessel_ku(u, x):
-
     def cond(args):
         ku, kn, i, p, q, r, s = args
         update = fabs(r * s) > eps * fabs(ku)
         return (i < 10) | (update & (i < max_iter))
 
     def body(args):
         ku, kn, i, p, q, r, s = args
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/utils.py` & `logbesselk-3.3.0/src/logbesselk/jax/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 
-from .math import exp
-from .math import fabs
-from .math import log
+from .math import (
+    exp,
+    fabs,
+    log,
+)
 
 __all__ = [
     "result_type",
     "epsilon",
     "extend",
     "find_zero",
     "log_integrate",
```

### Comparing `logbesselk-3.2.1/src/logbesselk/jax/wrap.py` & `logbesselk-3.3.0/src/logbesselk/jax/wrap.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import functools
 
 import jax
 import jax.lax as lax
 
-from .math import exp
-from .math import fabs
-from .math import inf
-from .math import nan
-from .math import sign
-from .utils import result_type
+from .math import (
+    exp,
+    fabs,
+    inf,
+    nan,
+    sign,
+)
+from .utils import (
+    result_type,
+)
 
 __all__ = [
     "wrap_log_bessel_k",
     "wrap_log_abs_deriv_bessel_k",
     "wrap_bessel_ke",
     "wrap_bessel_kratio",
 ]
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/asymptotic.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/asymptotic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import math
 
 import tensorflow as tf
 
-from .math import fabs
-from .math import log
-from .math import sqrt
-from .math import square
-from .utils import epsilon
-from .utils import result_shape
-from .utils import result_type
-from .wrap import wrap_log_bessel_k
+from .math import (
+    fabs,
+    log,
+    sqrt,
+    square,
+)
+from .utils import (
+    epsilon,
+    result_shape,
+    result_type,
+)
+from .wrap import (
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
 ]
 
 
 @wrap_log_bessel_k
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/cfraction.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/cfraction.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import math
 
 import tensorflow as tf
 
-from .math import fabs
-from .math import fround
-from .math import log
-from .math import square
-from .misc import log_bessel_recurrence
-from .utils import epsilon
-from .utils import result_shape
-from .utils import result_type
-from .wrap import wrap_log_bessel_k
+from .math import (
+    fabs,
+    fround,
+    log,
+    square,
+)
+from .misc import (
+    log_bessel_recurrence,
+)
+from .utils import (
+    epsilon,
+    result_shape,
+    result_type,
+)
+from .wrap import (
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
 ]
 
 
 @wrap_log_bessel_k
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/integral.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/integral.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import tensorflow as tf
 
-from .math import cosh
-from .math import is_finite
-from .math import log
-from .math import log_cosh
-from .math import log_sinh
-from .math import maximum
-from .math import square
-from .utils import epsilon
-from .utils import extend
-from .utils import find_zero
-from .utils import grad
-from .utils import log_integrate
-from .utils import result_shape
-from .utils import result_type
-from .wrap import wrap_bessel_ke
-from .wrap import wrap_bessel_kratio
-from .wrap import wrap_log_abs_deriv_bessel_k
+from .math import (
+    cosh,
+    is_finite,
+    log,
+    log_cosh,
+    log_sinh,
+    maximum,
+    square,
+)
+from .utils import (
+    epsilon,
+    extend,
+    find_zero,
+    grad,
+    log_integrate,
+    result_shape,
+    result_type,
+)
+from .wrap import (
+    wrap_bessel_ke,
+    wrap_bessel_kratio,
+    wrap_log_abs_deriv_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
     "bessel_ke",
     "bessel_kratio",
     "log_abs_deriv_bessel_k",
 ]
@@ -49,14 +55,17 @@
     def func(t):
         out = -x * cosh(t)
         out += tf.where(tf.equal(m % 2, 0), log_cosh(v * t), log_sinh(v * t))
         out = tf.where(m > 0, out + tf.cast(m, dtype) * log(t), out)
         out = tf.where(n > 0, out + tf.cast(n, dtype) * log_cosh(t), out)
         return out
 
+    def mfunc(t):
+        return func(t) - th
+
     scale = 0.1
     tol = 1.0
     max_iter = 10
     bins = 32
 
     shape = result_shape(v, x)
     dtype = result_type(v, x)
@@ -76,15 +85,14 @@
 
     start = tf.zeros(shape, dtype)
     delta = tf.where(deriv_at_zero_is_positive, scale, zero)
     start, delta = extend(deriv, start, delta)
     tp = find_zero(deriv, start, delta, tol, max_iter)
 
     th = func(tp) + log(eps) - tol
-    mfunc = lambda t: func(t) - th
     tpl = maximum(tp - bins * eps, zero)
     tpr = maximum(tp + bins * eps, tp * (1 + bins * eps))
     mfunc_at_zero_is_negative = out_is_finite & (mfunc(zero) < 0)
     mfunc_at_tpr_is_positive = out_is_finite & (mfunc(tpr) > 0)
 
     start = zero
     delta = tf.where(mfunc_at_zero_is_negative, tpl, zero)
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/math.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/math.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import functools
 import math
 
 import tensorflow as tf
-from tensorflow import where
+from tensorflow import (
+    where,
+)
 from tensorflow.math import abs as fabs
-from tensorflow.math import cosh
-from tensorflow.math import exp
-from tensorflow.math import expm1
-from tensorflow.math import is_finite
-from tensorflow.math import log
-from tensorflow.math import log1p
-from tensorflow.math import maximum
+from tensorflow.math import (
+    cosh,
+    exp,
+    expm1,
+    is_finite,
+    log,
+    log1p,
+    maximum,
+)
 from tensorflow.math import round as fround
-from tensorflow.math import sign
-from tensorflow.math import sin
-from tensorflow.math import sinh
-from tensorflow.math import sqrt
-from tensorflow.math import square
-from tensorflow.math import tanh
+from tensorflow.math import (
+    sign,
+    sin,
+    sinh,
+    sqrt,
+    square,
+    tanh,
+)
 
 __all__ = [
     "fabs",
     "cosh",
     "exp",
     "expm1",
     "is_finite",
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/misc.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import tensorflow as tf
 
-from .math import log
-from .math import log_add_exp
-from .utils import result_type
+from .math import (
+    log,
+    log_add_exp,
+    sign,
+)
+from .utils import (
+    result_type,
+)
 
 __all__ = [
     "sign_deriv_bessel_k",
     "log_bessel_recurrence",
 ]
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/sca.py` & `logbesselk-3.3.0/src/logbesselk/jax/ica.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,68 @@
-import tensorflow as tf
+import jax.lax as lax
 
-from .asymptotic import log_bessel_k as log_k_large_v
-from .cfraction import log_bessel_ku as log_ku_large_x
-from .math import fround
-from .math import is_finite
-from .math import log
-from .misc import log_bessel_recurrence
-from .series import log_bessel_ku as log_ku_small_x
-from .utils import result_type
-from .wrap import wrap_bessel_ke
-from .wrap import wrap_bessel_kratio
-from .wrap import wrap_log_bessel_k
+from .asymptotic import log_bessel_k_naive as log_k_large_v
+from .cfraction import log_bessel_ku as log_ku_small_v
+from .integral import log_abs_deriv_bessel_k as log_k_small_x
+from .math import (
+    fround,
+    is_finite,
+)
+from .misc import (
+    log_bessel_recurrence,
+)
+from .utils import (
+    result_type,
+)
+from .wrap import (
+    wrap_bessel_ke,
+    wrap_bessel_kratio,
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
     "bessel_kratio",
     "bessel_ke",
 ]
 
 
 @wrap_log_bessel_k
 def log_bessel_k(v, x):
     """
-    Combination of Series, Continued fraction and Asymptotic expansion.
+    Combination of Integrate, Continued fraction and Asymptotic expansion.
     """
 
-    def large_v_case():
-        v_ = tf.where(large_v, v, tf.constant(0, dtype))
-        return log_k_large_v(v_, x)
-
-    def small_v_case():
-        def large_x_ku():
-            u_ = tf.where(large_x, u, tf.constant(1 / 2, dtype))
-            x_ = tf.where(large_x, x, tf.constant(1, dtype))
-            return log_ku_large_x(u_, x_)
-
-        def small_x_ku():
-            u_ = tf.where(small_x, u, tf.constant(1 / 2, dtype))
-            return log_ku_small_x(u_, x)
-
-        n = fround(v)
-        u = v - n
-        logk0l, logk1l = large_x_ku()
-        logk0s, logk1s = small_x_ku()
-        logk0 = tf.where(large_x, logk0l, logk0s)
-        logk1 = tf.where(large_x, logk1l, logk1s)
-        return log_bessel_recurrence(logk0, logk1, u, n, x)[0]
+    def small_x_case():
+        return log_k_small_x(v, x)
+
+    def large_x_case():
+        def small_v_case():
+            n = fround(v)
+            u = (v - n).astype(dtype)
+            u_ = lax.cond(small_v, lambda: u, lambda: dtype(1 / 2))
+            logk0, logk1 = log_ku_small_v(u_, x)
+            return log_bessel_recurrence(logk0, logk1, u, n, x)[0]
+
+        def large_v_case():
+            v_ = lax.cond(large_v, lambda: v.astype(dtype), lambda: dtype(0))
+            return log_k_large_v(v_, x)
+
+        return lax.cond(small_v, small_v_case, large_v_case)
 
     dtype = result_type(v, x)
     finite = is_finite(v) & is_finite(x) & (x > 0)
     large_v_ = v >= 25
-    large_x_ = x >= 1.6 + (1 / 2) * log(v + 1)
+    large_x_ = x >= 100
 
-    large_v = finite & large_v_
-    large_x = finite & ~large_v_ & large_x_
-    small_x = finite & ~large_v_ & ~large_x_
-    return tf.where(large_v, large_v_case(), small_v_case())
+    small_x = finite & ~large_x_
+    small_v = finite & large_x_ & ~large_v_
+    large_v = finite & large_x_ & large_v_
+    return lax.cond(small_x, small_x_case, large_x_case)
 
 
-def bessel_kratio(v, x, d: int = 1):
+def bessel_kratio(v, x, d=1):
     return wrap_bessel_kratio(log_bessel_k, v, x, d)
 
 
 def bessel_ke(v, x):
     return wrap_bessel_ke(log_bessel_k, v, x)
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/series.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/series.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 import tensorflow as tf
 
-from .math import cosh
-from .math import exp
-from .math import fabs
-from .math import fround
-from .math import log
-from .math import sinc
-from .math import sinhc
-from .math import square
-from .misc import log_bessel_recurrence
-from .utils import epsilon
-from .utils import result_shape
-from .utils import result_type
-from .wrap import wrap_log_bessel_k
+from .math import (
+    cosh,
+    exp,
+    fabs,
+    fround,
+    log,
+    sinc,
+    sinhc,
+    square,
+)
+from .misc import (
+    log_bessel_recurrence,
+)
+from .utils import (
+    epsilon,
+    result_shape,
+    result_type,
+)
+from .wrap import (
+    wrap_log_bessel_k,
+)
 
 __all__ = [
     "log_bessel_k",
 ]
 
 
 @wrap_log_bessel_k
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/utils.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import numpy as np
 import tensorflow as tf
 
-from .math import exp
-from .math import fabs
-from .math import log
+from .math import (
+    exp,
+    fabs,
+    log,
+)
 
 __all__ = [
     "result_shape",
     "result_type",
     "epsilon",
     "grad",
     "extend",
```

### Comparing `logbesselk-3.2.1/src/logbesselk/tensorflow/wrap.py` & `logbesselk-3.3.0/src/logbesselk/tensorflow/wrap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import functools
 
 import numpy as np
 import tensorflow as tf
 
-from .math import exp
-from .math import fabs
-from .math import sign
-from .utils import result_type
+from .math import (
+    exp,
+    fabs,
+    sign,
+)
+from .utils import (
+    result_type,
+)
 
 __all__ = [
     "wrap_log_bessel_k",
     "wrap_log_abs_deriv_bessel_k",
     "wrap_bessel_ke",
     "wrap_bessel_kratio",
 ]
```

### Comparing `logbesselk-3.2.1/setup.py` & `logbesselk-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['logbesselk', 'logbesselk.jax', 'logbesselk.tensorflow']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'logbesselk',
-    'version': '3.2.1',
+    'version': '3.3.0',
     'description': 'Provide function to calculate the modified Bessel function of the second kind',
     'long_description': '# logbesselk\nProvide function to calculate the modified Bessel function of the second kind\nand its derivatives.\n\n## Reference\nTakashi Takekawa, Fast parallel calculation of modified Bessel function\nof the second kind and its derivatives, SoftwareX, 17, 100923, 2022.\n\n## Author\nTAKEKAWA Takashi <takekawa@tk2lab.org>\n\n\n## For Tensorflow\n\n### Require\n- Python (>=3.8)\n- Tensorflow (>=2.6)\n\n### Installation\n```shell\npip install tensorflow logbesselk\n```\n\n### Examples\n```python\nimport tensorflow as tf\nfrom logbesselk.tensorflow import log_bessel_k as logk\nfrom logbesselk.jax import bessel_ke as ke\nfrom logbesselk.jax import bessel_kratio as kratio\n\nv = 1.0\nx = 1.0\na = logk(v, x)\n\nv = jnp.linspace(1, 10, 10)\nx = jnp.linspace(1, 10, 10)\nb = logk(v, x)\n\n# gradient\nwith tf.GradientTape() as g:\n    g.watch(v, x)\n    f = logk(v, x)\ndlogkdv = g.gradient(f, v)\ndlogkdx = g.gradient(f, x)\n\n# use tf.function\nlogk = tf.function(logk)\n\n# advanced version\nfrom logbesselk.tensorflow import log_abs_deriv_bessel_k\n\nlogk = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 0)\nlogdkdv = lambda v, x: log_abs_deriv_bessel_k(v, x, 1, 0)\nlogdkdx = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 1)\n```\n\n\n## For jax\n\n### Require\n- Python (>=3.8)\n- jax (>=0.3)\n\n### Installation\n```shell\npip install jax[cuda] -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html\npip install logbesselk\n```\n\n### Examples\n```python\nimport jax\nimport jax.numpy as jnp\nfrom logbesselk.jax import log_bessel_k as logk\nfrom logbesselk.jax import bessel_ke as ke\nfrom logbesselk.jax import bessel_kratio as kratio\n\n# scalar func and grad\nv = 1.0\nx = 1.0\na = logk(v, x)\n\n# dlogK/dv = (dK/dv) / K\ndlogkdv = jax.grad(logk, 0)\nb = dlogkdv(v, x)\n\n# dlogK/dx = (dK/dx) / K\ndlogkdx = jax.grad(logk, 1)\nc = dlogkdx(v, x)\n\n# misc\nd = ke(v, x)\ne = kratio(v, x, d=1)\n\n# vectorize\nlogk_vec = jax.vmap(logk)\n\nv = jnp.linspace(1, 10, 10)\nx = jnp.linspace(1, 10, 10)\nf = logk_vec(v)\n\n# use jit\nlogk_vec_jit = jax.jit(logk_vec)\n\n# advanced version\nfrom logbesselk.jax import log_abs_devel_bessel_k\n\nlog_dkdv = lambda v, x: log_abs_deriv_bessel_k(v, x, 1, 0)\nlog_dkdx = lambda v, x: log_abs_deriv_bessel_k(v, x, 0, 1)\n\nlog_dkdv_jit = jax.jit(jax.vmap(log_dkdv))\nlog_dkdx_jit = jax.jit(jax.vmap(log_dkdx))\n```\n',
     'author': 'TAKEKAWA Takashi',
     'author_email': 'takekawa@tk2lab.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tk2lab/logbesselk',
```

### Comparing `logbesselk-3.2.1/PKG-INFO` & `logbesselk-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logbesselk
-Version: 3.2.1
+Version: 3.3.0
 Summary: Provide function to calculate the modified Bessel function of the second kind
 Home-page: https://github.com/tk2lab/logbesselk
 License: Apache-2.0
 Author: TAKEKAWA Takashi
 Author-email: takekawa@tk2lab.org
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
```

