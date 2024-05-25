# Comparing `tmp/quad5-0.1.8.tar.gz` & `tmp/quad5-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quad5-0.1.8.tar", last modified: Thu May 23 09:59:23 2024, max compression
+gzip compressed data, was "quad5-0.1.9.tar", last modified: Thu May 23 15:02:02 2024, max compression
```

## Comparing `quad5-0.1.8.tar` & `quad5-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:59:23.735702 quad5-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 09:58:49.000000 quad5-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-23 09:59:23.735702 quad5-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-23 09:58:49.000000 quad5-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:59:23.735702 quad5-0.1.8/quad5/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-23 09:58:49.000000 quad5-0.1.8/quad5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-23 09:58:49.000000 quad5-0.1.8/quad5/quadratic_approximation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:59:23.735702 quad5-0.1.8/quad5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4362 2024-05-23 09:59:23.000000 quad5-0.1.8/quad5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-23 09:59:23.000000 quad5-0.1.8/quad5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:59:23.000000 quad5-0.1.8/quad5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 09:59:23.000000 quad5-0.1.8/quad5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 09:59:23.000000 quad5-0.1.8/quad5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 09:59:23.735702 quad5-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-23 09:58:49.000000 quad5-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:59:23.735702 quad5-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 09:58:49.000000 quad5-0.1.8/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:02.398640 quad5-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-23 15:01:26.000000 quad5-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-23 15:02:02.398640 quad5-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-23 15:01:26.000000 quad5-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:02.394640 quad5-0.1.9/quad5/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-23 15:01:26.000000 quad5-0.1.9/quad5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-23 15:01:26.000000 quad5-0.1.9/quad5/quadratic_approximation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:02.398640 quad5-0.1.9/quad5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-23 15:02:02.000000 quad5-0.1.9/quad5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-23 15:02:02.000000 quad5-0.1.9/quad5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:02:02.000000 quad5-0.1.9/quad5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 15:02:02.000000 quad5-0.1.9/quad5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 15:02:02.000000 quad5-0.1.9/quad5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 15:02:02.398640 quad5-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-23 15:01:26.000000 quad5-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:02:02.394640 quad5-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-23 15:01:26.000000 quad5-0.1.9/tests/test.py
```

### Comparing `quad5-0.1.8/LICENSE` & `quad5-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `quad5-0.1.8/PKG-INFO` & `quad5-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quad5
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quadratic Approximation custom step sampler for PYMC.
 Home-page: https://github.com/carsten-j/quad5
 Author: Carsten Jørgensen
 Author-email: carstenj@gmail.com
 License: MIT
 Keywords: Bayesian Statistics,Probabalistic Programming Language,Python
 Classifier: Programming Language :: Python :: 3
@@ -28,24 +28,34 @@
 ## Word of warning
 This package is not production-grade code. It is primarily meant for educational purposes. Secondary for the author to learn more about the internals of the PYMC library.
 
 I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit either a PR or create a issue for such cases.
 
 ## Example
 ``` python
+
+        import arviz as az
+        import numpy as np
+        import pymc as pm
+        import quad5 as quad5
+
         y = np.array([2642, 3503, 4358], dtype=np.float64)
 
         with pm.Model() as m:
             logsigma = pm.Uniform("logsigma", 1, 100)
             mu = pm.Uniform("mu", 0, 10000)
             _ = pm.Normal("y", mu=mu, sigma=pm.math.exp(logsigma), observed=y)
-            custom_step = QuadraticApproximation([mu, logsigma], m)
+            custom_step = quad5.QuadraticApproximation([mu, logsigma], m)
             trace = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
+
+        az.plot_posterior(trace)    
 ```
 
+![Posterior Distribution](posterior.png)
+
 See more examples in this [notebook](https://colab.research.google.com/github/carsten-j/Rethinking/blob/main/chapter4.ipynb) with examples from chapter 4 in Statistical Rethinking.
 
 [^1]: [The Bernstein-Von Mises Theorem](https://en.wikipedia.org/wiki/Bernstein%E2%80%93von_Mises_theorem) states that under some regularity conditions the posterior distribution is asymptotically normal. If the distribution is unimodal with most of the probability mass located symmetric around the peak then quite often you will get a faily good approximation using Quadratic Approximation.
 
 [^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC. Optimizers works better when provided with a good initial guess and hence a (optional) starting point has been added to function arguments. Please see [Github](https://github.com/pymc-devs/pymc/issues/5443#issuecomment-1030609090) for a discussion about the differences between PYMC version 3 and 5 for computing the Hessian and in particular the for loop `for var in vars:` used when computing the Hessian.
 
 [^3]:The NumPyro documentation refers to "Automatic Guide Generation" and as I understand it this is a kind
```

### Comparing `quad5-0.1.8/README.md` & `quad5-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,34 @@
 ## Word of warning
 This package is not production-grade code. It is primarily meant for educational purposes. Secondary for the author to learn more about the internals of the PYMC library.
 
 I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit either a PR or create a issue for such cases.
 
 ## Example
 ``` python
+
+        import arviz as az
+        import numpy as np
+        import pymc as pm
+        import quad5 as quad5
+
         y = np.array([2642, 3503, 4358], dtype=np.float64)
 
         with pm.Model() as m:
             logsigma = pm.Uniform("logsigma", 1, 100)
             mu = pm.Uniform("mu", 0, 10000)
             _ = pm.Normal("y", mu=mu, sigma=pm.math.exp(logsigma), observed=y)
-            custom_step = QuadraticApproximation([mu, logsigma], m)
+            custom_step = quad5.QuadraticApproximation([mu, logsigma], m)
             trace = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
+
+        az.plot_posterior(trace)    
 ```
 
+![Posterior Distribution](posterior.png)
+
 See more examples in this [notebook](https://colab.research.google.com/github/carsten-j/Rethinking/blob/main/chapter4.ipynb) with examples from chapter 4 in Statistical Rethinking.
 
 [^1]: [The Bernstein-Von Mises Theorem](https://en.wikipedia.org/wiki/Bernstein%E2%80%93von_Mises_theorem) states that under some regularity conditions the posterior distribution is asymptotically normal. If the distribution is unimodal with most of the probability mass located symmetric around the peak then quite often you will get a faily good approximation using Quadratic Approximation.
 
 [^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC. Optimizers works better when provided with a good initial guess and hence a (optional) starting point has been added to function arguments. Please see [Github](https://github.com/pymc-devs/pymc/issues/5443#issuecomment-1030609090) for a discussion about the differences between PYMC version 3 and 5 for computing the Hessian and in particular the for loop `for var in vars:` used when computing the Hessian.
 
 [^3]:The NumPyro documentation refers to "Automatic Guide Generation" and as I understand it this is a kind
```

### Comparing `quad5-0.1.8/quad5/quadratic_approximation.py` & `quad5-0.1.9/quad5/quadratic_approximation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 import pymc as pm
-import scipy.stats as st
 from pymc.step_methods.arraystep import ArrayStep
 from pymc.util import get_value_vars_from_user_vars
 
 
 class QuadraticApproximation(ArrayStep):
     def __init__(self, vars, model, start=None, **kwargs):
         self.model = model
@@ -44,10 +43,7 @@
         mean = np.concatenate([np.atleast_1d(map[v.name]) for v in self.vars])
 
         return mean, cov
 
     def astep(self, q0, logp):
         sample = np.random.multivariate_normal(self.mode, self.covariance)
         return sample, []
-
-    def posterior(self):
-        return st.multivariate_normal(mean=self.mean, cov=self.covariance)
```

### Comparing `quad5-0.1.8/quad5.egg-info/PKG-INFO` & `quad5-0.1.9/quad5.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quad5
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quadratic Approximation custom step sampler for PYMC.
 Home-page: https://github.com/carsten-j/quad5
 Author: Carsten Jørgensen
 Author-email: carstenj@gmail.com
 License: MIT
 Keywords: Bayesian Statistics,Probabalistic Programming Language,Python
 Classifier: Programming Language :: Python :: 3
@@ -28,24 +28,34 @@
 ## Word of warning
 This package is not production-grade code. It is primarily meant for educational purposes. Secondary for the author to learn more about the internals of the PYMC library.
 
 I am quite sure there will be valid PYMC models where this package not is able to produce a quadratic approximation for the posterior distribution. You are more than welcome to submit either a PR or create a issue for such cases.
 
 ## Example
 ``` python
+
+        import arviz as az
+        import numpy as np
+        import pymc as pm
+        import quad5 as quad5
+
         y = np.array([2642, 3503, 4358], dtype=np.float64)
 
         with pm.Model() as m:
             logsigma = pm.Uniform("logsigma", 1, 100)
             mu = pm.Uniform("mu", 0, 10000)
             _ = pm.Normal("y", mu=mu, sigma=pm.math.exp(logsigma), observed=y)
-            custom_step = QuadraticApproximation([mu, logsigma], m)
+            custom_step = quad5.QuadraticApproximation([mu, logsigma], m)
             trace = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
+
+        az.plot_posterior(trace)    
 ```
 
+![Posterior Distribution](posterior.png)
+
 See more examples in this [notebook](https://colab.research.google.com/github/carsten-j/Rethinking/blob/main/chapter4.ipynb) with examples from chapter 4 in Statistical Rethinking.
 
 [^1]: [The Bernstein-Von Mises Theorem](https://en.wikipedia.org/wiki/Bernstein%E2%80%93von_Mises_theorem) states that under some regularity conditions the posterior distribution is asymptotically normal. If the distribution is unimodal with most of the probability mass located symmetric around the peak then quite often you will get a faily good approximation using Quadratic Approximation.
 
 [^2]: This work is partly based on the Python package [pymc3-quap](https://github.com/rasmusbergpalm/pymc3-quap) but pymc3-quap is based on PYMC3 and a lot happend bewteen version 3 and 5 of PYMC. Optimizers works better when provided with a good initial guess and hence a (optional) starting point has been added to function arguments. Please see [Github](https://github.com/pymc-devs/pymc/issues/5443#issuecomment-1030609090) for a discussion about the differences between PYMC version 3 and 5 for computing the Hessian and in particular the for loop `for var in vars:` used when computing the Hessian.
 
 [^3]:The NumPyro documentation refers to "Automatic Guide Generation" and as I understand it this is a kind
```

### Comparing `quad5-0.1.8/setup.py` & `quad5-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,25 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="quad5",
-    version="0.1.8",
+    version="0.1.9",
     description="""Quadratic Approximation custom step sampler for PYMC.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Carsten Jørgensen",
     packages=find_packages(include=["quad5"]),
-    keywords=["Bayesian Statistics", "Probabalistic Programming Language", "Python"],
+    keywords=[
+        "Bayesian Statistics",
+        "Probabalistic Programming Language",
+        "Python"
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=["PYMC==5.15.0"],
     license="MIT",
```

### Comparing `quad5-0.1.8/tests/test.py` & `quad5-0.1.9/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,32 @@
 import pymc as pm
 
 from quad5.quadratic_approximation import QuadraticApproximation
 
 
 class TestQuap(unittest.TestCase):
     # Example originates from Bayesian Data Analyses, 3rd Edition
-    # By Andrew Gelman, John Carlin, Hal Stern, David Dunson, Aki Vehtari, and Donald Rubin.
+    # By Andrew Gelman, John Carlin, Hal Stern, David Dunson,
+    # Aki Vehtari, and Donald Rubin.
     # See section. 4.1
     def test_analytical_solution_against_quadratic_approx(
         self,
     ):
         y = np.array([2642, 3503, 4358], dtype=np.float64)
         n = y.size
 
         with pm.Model() as m:
             logsigma = pm.Uniform("logsigma", 1, 100)
             mu = pm.Uniform("mu", 0, 10000)
             _ = pm.Normal("y", mu=mu, sigma=pm.math.exp(logsigma), observed=y)
             custom_step = QuadraticApproximation([mu, logsigma], m)
-            trace = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
+            _ = pm.sample(draws=1000, chains=4, tune=100, step=custom_step)
 
         bda_map = [y.mean(), np.log(y.std())]
         bda_cov = np.array([[y.var() / n, 0], [0, 1 / (2 * n)]])
 
         assert np.allclose(custom_step.mode, bda_map)
         assert np.allclose(custom_step.covariance, bda_cov, atol=1e-3)
 
-        print(trace.posterior.mean()["mu"])
-
 
 if __name__ == "__main__":
     unittest.main()
```

