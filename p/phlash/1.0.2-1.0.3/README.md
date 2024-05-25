# Comparing `tmp/phlash-1.0.2.tar.gz` & `tmp/phlash-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlash-1.0.2.tar", last modified: Mon Apr 15 18:04:13 2024, max compression
+gzip compressed data, was "phlash-1.0.3.tar", last modified: Sat May 25 18:49:21 2024, max compression
```

## Comparing `phlash-1.0.2.tar` & `phlash-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,53 @@
--rw-r--r--   0        0        0       54 2024-01-18 15:50:39.314184 phlash-1.0.2/AUTHORS.md
--rw-r--r--   0        0        0     1102 2024-02-23 17:51:48.581326 phlash-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     2176 2024-04-15 15:25:43.833513 phlash-1.0.2/README.md
--rw-r--r--   0        0        0     2480 2024-04-15 18:04:13.809324 phlash-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1089 2024-02-23 17:51:48.581326 phlash-1.0.2/src/phlash/__init__.py
--rw-r--r--   0        0        0      467 2024-03-07 16:19:49.405975 phlash-1.0.2/src/phlash/_version.py
--rw-r--r--   0        0        0      986 2024-03-07 01:41:49.831734 phlash-1.0.2/src/phlash/afs.py
--rw-r--r--   0        0        0     4798 2024-04-15 17:47:41.920951 phlash-1.0.2/src/phlash/cband.py
--rw-r--r--   0        0        0    18202 2024-04-15 17:56:27.355273 phlash-1.0.2/src/phlash/data.py
--rw-r--r--   0        0        0    21860 2024-04-15 17:25:10.586956 phlash-1.0.2/src/phlash/gpu.py
--rw-r--r--   0        0        0     2467 2024-04-15 17:11:30.103462 phlash-1.0.2/src/phlash/hmm.py
--rw-r--r--   0        0        0     2431 2024-02-23 17:51:48.585326 phlash-1.0.2/src/phlash/jax_ppoly.py
--rw-r--r--   0        0        0      794 2024-04-15 17:25:29.551038 phlash-1.0.2/src/phlash/kernel.py
--rw-r--r--   0        0        0     4459 2024-02-25 01:52:38.841162 phlash-1.0.2/src/phlash/liveplot.py
--rw-r--r--   0        0        0    12267 2024-04-15 16:41:29.503757 phlash-1.0.2/src/phlash/mcmc.py
--rw-r--r--   0        0        0     2430 2024-04-15 14:57:48.773013 phlash-1.0.2/src/phlash/model.py
--rw-r--r--   0        0        0      646 2024-02-23 17:51:48.585326 phlash-1.0.2/src/phlash/mp.py
--rw-r--r--   0        0        0     3536 2024-04-15 14:56:43.652824 phlash-1.0.2/src/phlash/params.py
--rw-r--r--   0        0        0      726 2024-02-23 17:51:48.585326 phlash-1.0.2/src/phlash/plot.py
--rw-r--r--   0        0        0    10355 2024-04-15 18:04:01.489269 phlash-1.0.2/src/phlash/sim.py
--rw-r--r--   0        0        0    12105 2024-03-26 00:31:45.400238 phlash-1.0.2/src/phlash/size_history.py
--rw-r--r--   0        0        0     2616 2024-03-25 20:23:13.263219 phlash-1.0.2/src/phlash/transition.py
--rw-r--r--   0        0        0     1301 2024-03-07 01:43:16.655984 phlash-1.0.2/src/phlash/util.py
--rw-r--r--   0        0        0    48861 2024-03-15 16:55:50.847090 phlash-1.0.2/tests/.benchmarks/Linux-CPython-3.10-64bit/0001_gpu_vs_jax.json
--rw-r--r--   0        0        0    53248 2023-12-14 20:24:56.454022 phlash-1.0.2/tests/.coverage
--rw-r--r--   0        0        0       37 2024-02-07 01:57:37.951589 phlash-1.0.2/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-02-07 01:57:37.951589 phlash-1.0.2/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-02-07 01:57:37.951589 phlash-1.0.2/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0     1895 2024-03-15 16:55:50.895090 phlash-1.0.2/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    13396 2024-03-15 16:55:50.851090 phlash-1.0.2/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-03-15 16:55:50.895090 phlash-1.0.2/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      665 2024-04-15 17:12:20.383672 phlash-1.0.2/tests/conftest.py
--rw-r--r--   0        0        0  1306723 2024-02-24 19:03:38.092173 phlash-1.0.2/tests/fixtures/elpd_bug.pkl
--rw-r--r--   0        0        0   131135 2024-01-07 18:27:14.126332 phlash-1.0.2/tests/fixtures/sample.bcf
--rw-r--r--   0        0        0      244 2024-01-07 18:27:14.126332 phlash-1.0.2/tests/fixtures/sample.bcf.csi
--rw-r--r--   0        0        0      105 2024-04-15 17:52:56.714345 phlash-1.0.2/tests/fixtures/sample.psmcfa
--rw-r--r--   0        0        0    17967 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/fixtures/tv_bug.pkl
--rw-r--r--   0        0        0      940 2024-03-07 01:41:49.831734 phlash-1.0.2/tests/test_afs.py
--rw-r--r--   0        0        0     1019 2024-03-11 16:00:58.769990 phlash-1.0.2/tests/test_cband.py
--rw-r--r--   0        0        0     2872 2024-04-15 17:56:27.011272 phlash-1.0.2/tests/test_data.py
--rw-r--r--   0        0        0     1599 2024-04-15 17:12:32.355723 phlash-1.0.2/tests/test_gpu.py
--rw-r--r--   0        0        0      473 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_hmm.py
--rw-r--r--   0        0        0     1628 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_jax_ppoly.py
--rw-r--r--   0        0        0      434 2024-04-15 15:39:57.675107 phlash-1.0.2/tests/test_mcmc.py
--rw-r--r--   0        0        0      574 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_model.py
--rw-r--r--   0        0        0      631 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_sim.py
--rw-r--r--   0        0        0     4518 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_size_history.py
--rw-r--r--   0        0        0     1121 2024-04-15 17:18:55.073344 phlash-1.0.2/tests/test_speed.py
--rw-r--r--   0        0        0      818 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_transition.py
--rw-r--r--   0        0        0     3636 1970-01-01 00:00:00.000000 phlash-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-01-18 15:50:39.314184 phlash-1.0.3/AUTHORS.md
+-rw-r--r--   0        0        0     1102 2024-02-23 17:51:48.581326 phlash-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     2021 2024-05-17 08:52:42.589947 phlash-1.0.3/README.md
+-rw-r--r--   0        0        0     2280 2024-05-25 18:49:21.917285 phlash-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1182 2024-05-18 13:17:12.811708 phlash-1.0.3/src/phlash/__init__.py
+-rw-r--r--   0        0        0      467 2024-03-07 16:19:49.405975 phlash-1.0.3/src/phlash/_version.py
+-rw-r--r--   0        0        0      986 2024-03-07 01:41:49.831734 phlash-1.0.3/src/phlash/afs.py
+-rw-r--r--   0        0        0     4798 2024-04-16 13:01:48.709265 phlash-1.0.3/src/phlash/cband.py
+-rw-r--r--   0        0        0    19159 2024-05-18 13:45:21.200447 phlash-1.0.3/src/phlash/data.py
+-rw-r--r--   0        0        0    21862 2024-05-18 14:20:53.431120 phlash-1.0.3/src/phlash/gpu.py
+-rw-r--r--   0        0        0     2467 2024-04-16 13:01:27.017189 phlash-1.0.3/src/phlash/hmm.py
+-rw-r--r--   0        0        0     2431 2024-02-23 17:51:48.585326 phlash-1.0.3/src/phlash/jax_ppoly.py
+-rw-r--r--   0        0        0      794 2024-04-16 13:01:27.017189 phlash-1.0.3/src/phlash/kernel.py
+-rw-r--r--   0        0        0     4459 2024-02-25 01:52:38.841162 phlash-1.0.3/src/phlash/liveplot.py
+-rw-r--r--   0        0        0    12312 2024-05-18 14:20:53.435121 phlash-1.0.3/src/phlash/mcmc.py
+-rw-r--r--   0        0        0     2430 2024-04-16 13:01:27.009189 phlash-1.0.3/src/phlash/model.py
+-rw-r--r--   0        0        0      646 2024-02-23 17:51:48.585326 phlash-1.0.3/src/phlash/mp.py
+-rw-r--r--   0        0        0     3536 2024-05-18 14:20:53.435121 phlash-1.0.3/src/phlash/params.py
+-rw-r--r--   0        0        0      726 2024-02-23 17:51:48.585326 phlash-1.0.3/src/phlash/plot.py
+-rw-r--r--   0        0        0      896 2024-05-18 14:20:41.491085 phlash-1.0.3/src/phlash/psmc.py
+-rw-r--r--   0        0        0    10355 2024-04-15 18:04:01.489269 phlash-1.0.3/src/phlash/sim.py
+-rw-r--r--   0        0        0    12105 2024-03-26 00:31:45.400238 phlash-1.0.3/src/phlash/size_history.py
+-rw-r--r--   0        0        0     2616 2024-05-18 14:20:53.435121 phlash-1.0.3/src/phlash/transition.py
+-rw-r--r--   0        0        0     1315 2024-05-18 14:20:53.435121 phlash-1.0.3/src/phlash/util.py
+-rw-r--r--   0        0        0    48861 2024-03-15 16:55:50.847090 phlash-1.0.3/tests/.benchmarks/Linux-CPython-3.10-64bit/0001_gpu_vs_jax.json
+-rw-r--r--   0        0        0    53248 2023-12-14 20:24:56.454022 phlash-1.0.3/tests/.coverage
+-rw-r--r--   0        0        0       37 2024-02-07 01:57:37.951589 phlash-1.0.3/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-02-07 01:57:37.951589 phlash-1.0.3/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-02-07 01:57:37.951589 phlash-1.0.3/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0     1895 2024-03-15 16:55:50.895090 phlash-1.0.3/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    13396 2024-03-15 16:55:50.851090 phlash-1.0.3/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-03-15 16:55:50.895090 phlash-1.0.3/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2024-05-16 20:55:59.496787 phlash-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      791 2024-05-18 13:45:20.548446 phlash-1.0.3/tests/conftest.py
+-rw-r--r--   0        0        0  1306723 2024-02-24 19:03:38.092173 phlash-1.0.3/tests/fixtures/elpd_bug.pkl
+-rw-r--r--   0        0        0   131135 2024-01-07 18:27:14.126332 phlash-1.0.3/tests/fixtures/sample.bcf
+-rw-r--r--   0        0        0      244 2024-01-07 18:27:14.126332 phlash-1.0.3/tests/fixtures/sample.bcf.csi
+-rw-r--r--   0        0        0      105 2024-04-16 13:01:48.713265 phlash-1.0.3/tests/fixtures/sample.psmcfa
+-rw-r--r--   0        0        0    17967 2024-02-23 17:51:48.585326 phlash-1.0.3/tests/fixtures/tv_bug.pkl
+-rw-r--r--   0        0        0     1121 2024-04-15 17:18:55.073344 phlash-1.0.3/tests/speed.py
+-rw-r--r--   0        0        0      940 2024-03-07 01:41:49.831734 phlash-1.0.3/tests/test_afs.py
+-rw-r--r--   0        0        0     1051 2024-05-17 08:54:48.950469 phlash-1.0.3/tests/test_cband.py
+-rw-r--r--   0        0        0     2711 2024-05-18 13:45:30.960474 phlash-1.0.3/tests/test_data.py
+-rw-r--r--   0        0        0     1703 2024-05-17 09:06:08.908738 phlash-1.0.3/tests/test_gpu.py
+-rw-r--r--   0        0        0      505 2024-05-17 08:58:06.763204 phlash-1.0.3/tests/test_hmm.py
+-rw-r--r--   0        0        0     1628 2024-02-23 17:51:48.585326 phlash-1.0.3/tests/test_jax_ppoly.py
+-rw-r--r--   0        0        0      949 2024-05-18 13:45:20.768446 phlash-1.0.3/tests/test_mcmc.py
+-rw-r--r--   0        0        0      574 2024-02-23 17:51:48.585326 phlash-1.0.3/tests/test_model.py
+-rw-r--r--   0        0        0      631 2024-02-23 17:51:48.585326 phlash-1.0.3/tests/test_sim.py
+-rw-r--r--   0        0        0     4518 2024-02-23 17:51:48.585326 phlash-1.0.3/tests/test_size_history.py
+-rw-r--r--   0        0        0      818 2024-02-23 17:51:48.585326 phlash-1.0.3/tests/test_transition.py
+-rw-r--r--   0        0        0      557 2024-05-18 14:20:53.435121 phlash-1.0.3/tests/test_util.py
+-rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 phlash-1.0.3/PKG-INFO
```

### Comparing `phlash-1.0.2/LICENSE.txt` & `phlash-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/README.md` & `phlash-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,26 +19,21 @@
 
 phlash can be installed from PyPI using pip:
 
 ```
 $ pip install phlash
 ```
 
-If your machine contains an Nvidia GPU, you should install the `gpu` variant in order to enable it.
-In this case, you should run:
+If your machine contains an Nvidia GPU, you should be sure to install the `gpu` variant in order to enable it:
 
 ```
-$ pip install \
-    -f "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html" \
-    --extra-index-url "https://pypi.ngc.nvidia.com" \
-    phlash[gpu]
+$ pip install 'phlash[gpu]'
 ```
 
-I recommend installing phlash into a separate virtual environment: before running the
-above, do
+I recommend installing phlash into a separate virtual environment: before running the above, do
 
 ```
 $ python3 -mvenv /path/to/phlash  # replace with desired path
 $ source /path/to/phlash/bin/activate
 $ pip3 install -U pip setuptools  # recent version of pip and setuptools are required
 ```
 ## Running the program
```

### Comparing `phlash-1.0.2/pyproject.toml` & `phlash-1.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 dynamic = []
 description = "Bayesian inference of population size history from recombining sequence data."
 authors = [
     { name = "Jonathan Terhorst", email = "jonth@umich.edu" },
 ]
 dependencies = [
     "blackjax<2.0.0,>=1.1.0",
-    "cuda-python<13,>=12.3",
-    "cyvcf2<1.0.0,>=0.30.28",
     "intervaltree<4.0.0,>=3.1.0",
-    "jax>=0.4.24",
+    "jax>=0.4.25",
     "loguru<1.0.0,>=0.7.2",
     "matplotlib<4.0.0,>=3.8.2",
     "msprime<2.0.0,>=1.3.0",
     "numpy<2.0.0,>=1.26.3",
     "optax<1.0.0,>=0.1.9",
     "plotly<6.0.0,>=5.18.0",
     "scipy<2.0.0,>=1.12.0",
@@ -23,34 +21,32 @@
     "tskit<1.0.0,>=0.5.6",
     "demes<1.0.0,>=0.2.3",
     "jax-dataclasses<2.0.0,>=1.6.0",
     "tszip<1.0.0,>=0.2.3",
     "jaxtyping<1.0.0,>=0.2.25",
     "pulp>=2.8.0",
     "dinopy>=3.0.0",
+    "pysam>=0.22.1",
 ]
 requires-python = ">=3.10,<4.0"
 readme = "README.md"
-version = "1.0.2"
+version = "1.0.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/jthlab/phlash"
 "Bug Reports" = "https://github.com/jthlab/phlash/issues"
 Source = "https://github.com/jthlab/phlash/"
 
 [project.optional-dependencies]
-webui = [
-    "jupyter>=1.0.0",
-    "notebook>=7.1.1",
-]
 gpu = [
-    "jax[cuda12_pip]>=0.4.24",
+    "jax[cuda12]>=0.4.25",
+    "cuda-python<13,>=12.3",
     "nvidia-cuda-nvrtc-cu12>=12.3",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
@@ -61,25 +57,14 @@
 
 [tool.pdm.build]
 includes = []
 
 [tool.pdm.version]
 source = "scm"
 
-[[tool.pdm.source]]
-name = "jax"
-url = "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html"
-type = "find_links"
-verify_ssl = true
-
-[[tool.pdm.source]]
-name = "nvidia"
-url = "https://pypi.ngc.nvidia.com"
-verify_ssl = true
-
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=8.0.0",
     "flake8>=7.0.0",
     "flake8-pyproject>=1.2.3",
 ]
 
@@ -124,7 +109,12 @@
     "if __name__ == .__main__.:",
     "@(abc\\.)?abstractmethod",
 ]
 ignore_errors = true
 
 [tool.coverage.html]
 directory = "coverage_html_report"
+
+[tool.pytest.ini_options]
+markers = [
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+]
```

### Comparing `phlash-1.0.2/src/phlash/__init__.py` & `phlash-1.0.3/src/phlash/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import warnings
 
 # ignore some annoying warnings that show up in the packages we rely on
 warnings.filterwarnings(action="ignore", module="stdpopsim", category=FutureWarning)
 
 # this needs to occur before jax loads
 os.environ["XLA_PYTHON_CLIENT_PREALLOCATE"] = "false"
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
 import sys
 
 import jax
 
 jax.config.update("jax_enable_x64", True)
 
 from phlash.data import contig
 from phlash.mcmc import fit
+from phlash.psmc import psmc
+from phlash.size_history import DemographicModel, SizeHistory
 
-__all__ = ["fit", "contig"]
+__all__ = ["fit", "contig", "psmc", "DemographicModel", "SizeHistory"]
 
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import PackageNotFoundError, version  # pragma: no cover
 else:
     from importlib_metadata import PackageNotFoundError, version  # pragma: no cover
```

### Comparing `phlash-1.0.2/src/phlash/afs.py` & `phlash-1.0.3/src/phlash/afs.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/cband.py` & `phlash-1.0.3/src/phlash/cband.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/data.py` & `phlash-1.0.3/src/phlash/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 "Classes for importing data"
 
 import re
 from abc import ABC, abstractmethod
+from collections.abc import Iterable
 from concurrent.futures import as_completed
 from dataclasses import asdict, dataclass, field
 from typing import NamedTuple
 
-import cyvcf2
 import dinopy
 import numpy as np
+import pysam
 import tqdm.auto as tqdm
 import tskit
 import tszip
 from intervaltree import IntervalTree
 from jaxtyping import Array, Int, Int8
 from loguru import logger
 
@@ -116,41 +117,42 @@
 class RawContig(Contig):
     "A contig with pre-computed het matrix and afs."
     het_matrix: Int8[Array, "N L"]
     afs: Int[Array, "n"]
     window_size: int
 
     @classmethod
-    def from_psmcfa(
-        cls, psmcfa_path: str, contig: str, window_size: int
-    ) -> "RawContig":
-        """Construct a contig from a PSMC FASTA (.psmcfa) file.
+    def from_psmcfa_iter(
+        cls, psmcfa_path: str, window_size: int
+    ) -> Iterable["RawContig"]:
+        """Construct a list of contigs from a PSMC FASTA (.psmcfa) file.
 
         Args:
             psmcfa_path: The path to the .psmcfa file.
-            contig: The name of the contig to read in.
             window_size: The size of the window that was used when binning entries
                 to construct the FASTA file.
 
         Notes:
             The `window_size` parameter corresponds to the `-s` option that was passed
             to the `fq2psmcfa` utility when creating the .psmcfa file, and is usually
             set to 100bp.
         """
         # parse psmcfa file
         far = dinopy.FastaReader(psmcfa_path)
-        try:
-            c = next(far.chromosomes(contig))
-        except StopIteration:
-            raise ValueError(f"A contig named {contig} was not found in {psmcfa_path}")
-        seq = np.frombuffer(c.sequence, dtype="c")
-        data = (seq == b"K").astype(np.uint8)
-        (L,) = data.shape
-        afs = np.ones(1)
-        return cls(het_matrix=data[None], afs=afs, window_size=window_size)
+        for record in far.entries():
+            contig_name = record.name
+            logger.debug(
+                f"Reading contig {contig_name.decode('ascii')} from {psmcfa_path}"
+            )
+            seq = np.frombuffer(record.sequence, dtype="c")
+            data = (seq == b"K").astype(np.int8)
+            data[seq == b"N"] = -1  # account for missing data
+            (L,) = data.shape
+            afs = np.ones(1)
+            yield cls(het_matrix=data[None], afs=afs, window_size=window_size)
 
     @property
     def N(self):
         # the het matrix has one row per diploid pair, so the number of ploids
         # is twice its first dimension.
         if self.het_matrix is None:
             return None
@@ -269,14 +271,48 @@
         for v in pbar:
             g = v.genotypes.reshape(-1, 2)
             ell = int(v.position / window_size)
             G[:, ell] += g[:, 0] != g[:, 1]
     return G
 
 
+class _VCFFile:
+    def __init__(self, file_path, samples: list[str]):
+        self.file_path = file_path
+        self.samples = samples
+        self.vcf = pysam.VariantFile(file_path)  # opens the VCF or BCF file
+        self.vcf.subset_samples(samples)
+        self._contigs = {name: c.length for name, c in self.vcf.header.contigs.items()}
+
+    @property
+    def header(self):
+        return self.vcf.header
+
+    @property
+    def contigs(self):
+        return self._contigs
+
+    def fetch(self, **kwargs):
+        # Check if the samples are in the VCF header
+        def variant_iterator():
+            for record in self.vcf.fetch(**kwargs):
+                het = np.zeros(len(self.samples), dtype=np.int8)
+                nd = 0  # number of derived alleles
+                for i, sample in enumerate(self.samples):
+                    gt = record.samples[sample]["GT"]
+                    if gt is None or None in gt:
+                        het[i] = -1
+                    else:
+                        het[i] = gt[0] != gt[1]
+                    nd += sum([g != 0 and g is not None for g in gt])
+                yield {"pos": record.pos, "ref": record.ref, "nd": nd, "het": het}
+
+        return variant_iterator()
+
+
 @dataclass(frozen=True)
 class VcfContig(Contig):
     """Read data from a VCF file.
 
     Args:
         vcf_file: path to VCF file
         contig: contig name
@@ -300,18 +336,18 @@
 
     @property
     def L(self):
         "Length of sequence"
         if self.interval is None:
             v = self._vcf
             if self.contig is None:
-                assert len(v.seqnames) == 1
-                return v.seqlens[0]
+                assert len(v.contigs) == 1
+                return list(v.contigs.values())[0]
             else:
-                return v.seqlens[v.seqnames.index(self.contig)]
+                return v.contigs[self.contig]
         return self.interval[1] - self.interval[0]
 
     def __post_init__(self):
         if self.mask is not None:
             raise NotImplementedError(
                 "masking is not yet implemented for VCF files, please use vcftools or "
                 "a similar method."
@@ -324,60 +360,45 @@
                 )
             if self.interval[0] >= self.interval[1]:
                 raise ValueError("region must be an interval (a,b) with a < b")
         if not all(isinstance(s, str) for s in self.samples):
             raise ValueError(
                 "samples should be a list of (string) sample identifiers in the vcf"
             )
-        diff = set(self.samples) - set(self._vcf.samples)
+        diff = set(self.samples) - set(self._vcf.header.samples)
         if diff:
             raise ValueError(f"the following samples were not found in the vcf: {diff}")
 
     @property
     def _vcf(self):
-        return cyvcf2.VCF(self.vcf_file)
+        return _VCFFile(self.vcf_file, self.samples)
 
     def get_data(self, window_size: int = 100) -> dict[str, np.ndarray]:
-        args = (self.vcf_file, self.samples, window_size)
+        vcf = self._vcf
         if not self._allow_empty_region:
-            args += (self.contig, *self.interval)
-        return _read_vcf(*args)
-
-
-def _read_vcf(
-    vcf_file: str,
-    samples: list[str],
-    window_size: int,
-    contig: str = None,
-    start: int = None,
-    end: int = None,
-    progress: bool = False,
-) -> dict[str, np.ndarray]:
-    vcf = cyvcf2.VCF(vcf_file, samples=samples, gts012=True)
-    if contig and start and end:
-        vcf_iter_args = (f"{contig}:{start}-{end}",)
-    else:
-        vcf_iter_args = ()
-        start = 1
-        assert len(vcf.seqnames) == 1
-        end = vcf.seqlens[0]
-    L = end - start + 1
-    N = len(samples)
-    afs = np.zeros(2 * N + 1, dtype=np.int64)
-    H = np.zeros([N, int(L / window_size)], dtype=np.int8)
-    with tqdm.tqdm(total=L, disable=not progress, desc="Reading VCF") as pbar:
-        for variant in vcf(*vcf_iter_args):
-            x = variant.POS - start
-            pbar.update(x - pbar.n)
+            contig = self.contig
+            start, end = self.interval
+            kwargs = {"contig": contig, "start": start, "stop": end}
+        else:
+            assert len(vcf.contigs) == 1
+            contig, end = next(iter(vcf.contigs.items()))
+            start = 1
+            kwargs = {}
+        L = end - start + 1
+        N = len(self.samples)
+        afs = np.zeros(2 * N + 1, dtype=np.int64)
+        H = np.zeros([N, int(L / window_size)], dtype=np.int8)
+        for rec in self._vcf.fetch(**kwargs):
+            x = rec["pos"] - start
             i = min(H.shape[1] - 1, int(x / window_size))
-            ty = variant.gt_types
-            H[:, i] += ty == 1
+            # ty = variant.gt_types
+            H[:, i] += rec["het"]
             # TODO this doesn't handle missing entries correctly
-            afs[ty[ty < 3].sum()] += 1
-    return dict(het_matrix=H, afs=afs[1:-1])
+            afs[rec["nd"]] += 1
+        return dict(het_matrix=H, afs=afs[1:-1])
 
 
 def contig(
     src: str | tskit.TreeSequence,
     samples: list[str] | list[tuple[int, int]],
     region: str = None,
 ) -> Contig:
```

### Comparing `phlash-1.0.2/src/phlash/gpu.py` & `phlash-1.0.3/src/phlash/gpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import partial, singledispatchmethod
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 import nvidia.cuda_nvrtc.lib
 from cuda import cuda, cudart, nvrtc
-from jax import custom_vjp, tree_map
+from jax import custom_vjp
 from loguru import logger
 
 import phlash.size_history
 from phlash.params import PSMCParams
 
 
 class CudaError(RuntimeError):
@@ -305,19 +305,19 @@
                 pi=dlog[..., 6, :],
             )
             ret = (ll, dll)
         else:
             ret = ll
         # strip off the additional batch dimensions we added earlier
         if added_B and added_S:
-            ret = jax.tree_map(lambda a: a[0, 0, ...], ret)
+            ret = jax.tree.map(lambda a: a[0, 0, ...], ret)
         elif added_B:
-            ret = jax.tree_map(lambda a: a[0, ...], ret)
+            ret = jax.tree.map(lambda a: a[0, ...], ret)
         elif added_S:
-            ret = jax.tree_map(lambda a: a[:, 0, ...], ret)
+            ret = jax.tree.map(lambda a: a[:, 0, ...], ret)
         return ret
 
 
 class PSMCKernel:
     """Spread kernel evalution across multiple devices.
 
     Args:
@@ -346,15 +346,15 @@
     def float_type(self):
         if self.double_precision:
             return np.float64
         return np.float32
 
     @singledispatchmethod
     def loglik(self, pp: PSMCParams, index: int):
-        log_params = tree_map(jnp.log, pp)
+        log_params = jax.tree.map(jnp.log, pp)
         return _psmc_ll(log_params, index=index, kern=self)
 
     # convenience overload mostly to help test code
     @loglik.register
     def _(self, dm: phlash.size_history.DemographicModel, index):
         return self.loglik(PSMCParams.from_dm(dm), index)
 
@@ -378,15 +378,15 @@
     def __call__(
         self, pp: PSMCParams, index: int, grad: bool
     ) -> tuple[float, PSMCParams]:
         def f(a):
             assert np.isfinite(a).all()
 
         try:
-            jax.tree_map(f, pp)
+            jax.tree.map(f, pp)
         except Exception:
             logger.debug("pp:{}", pp)
             raise
         # Split indices array across GPUs
         indices = np.atleast_1d(index)
         D = len(self.devices)
         split_indices = np.array_split(indices, D)
@@ -407,22 +407,22 @@
             logger.trace("spawned thread {}", thread)
 
         for thread in threads:
             thread.join()
 
         ret = self._combine_results(results)
         if index.ndim == 0:
-            ret = jax.tree_map(np.squeeze, ret)
+            ret = jax.tree.map(np.squeeze, ret)
         return ret
 
     def _combine_results(self, results):
         """
         Combine results from all GPUs.
         """
-        return jax.tree_map(lambda *x: np.concatenate(x), *results)
+        return jax.tree.map(lambda *x: np.concatenate(x), *results)
 
     def _compute_on_gpu(
         self, i, device, gpu_kernel, pp, split_index, grad, barrier, results
     ):
         """
         Perform computation on a specific GPU.
         """
@@ -436,15 +436,15 @@
 
 
 def _psmc_ll_fwd(log_params, index, kern):
     return _psmc_ll_helper(log_params, index=index, kern=kern, grad=True)
 
 
 def _psmc_ll_helper(log_params: PSMCParams, index, kern, grad):
-    params = tree_map(jnp.exp, log_params)
+    params = jax.tree.map(jnp.exp, log_params)
     result_shape_dtype = jax.ShapeDtypeStruct(shape=(), dtype=jnp.float64)
     if grad:
         result_shape_dtype = (
             result_shape_dtype,
             PSMCParams(
                 *[
                     jax.ShapeDtypeStruct(shape=(params.M,), dtype=kern.float_type)
@@ -454,15 +454,15 @@
         )
     return jax.pure_callback(
         kern, result_shape_dtype, pp=params, index=index, grad=grad, vectorized=True
     )
 
 
 def _psmc_ll_bwd(kern, df, g):
-    return tree_map(lambda a: g * a, df), None
+    return jax.tree.map(lambda a: g * a, df), None
 
 
 _psmc_ll.defvjp(_psmc_ll_fwd, _psmc_ll_bwd)
 
 
 KERNEL_SRC = r"""
 // Shorthands to index into the global gradient array of shape [M, M, 6]
```

### Comparing `phlash-1.0.2/src/phlash/hmm.py` & `phlash-1.0.3/src/phlash/hmm.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/jax_ppoly.py` & `phlash-1.0.3/src/phlash/jax_ppoly.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/kernel.py` & `phlash-1.0.3/src/phlash/kernel.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/liveplot.py` & `phlash-1.0.3/src/phlash/liveplot.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/mcmc.py` & `phlash-1.0.3/src/phlash/mcmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
             kw["warmup"] = warmup_chunks[inds]
             state1 = step(state, **kw)
 
             def f(x):
                 assert jnp.isfinite(x).all()
                 return x
 
-            state = jax.tree_map(f, state1)
+            state = jax.tree.map(f, state1)
             _particles = state.particles
             if test_data is not None and i % 10 == 0:
                 e = elpd(state.particles)
                 if ema is None:
                     ema = e
                 else:
                     ema = 0.9 * ema + 0.1 * e
@@ -298,15 +298,15 @@
                     logger.info(
                         "The expected log-predictive density has not improved in "
                         f"the last {elpd_cutoff} iterations; exiting."
                     )
                     break
                 pbar.set_description(f"elpd={ema:.2f} a={a}")
             cb(dms())
-
+    logger.info("MCMC finished successfully")
     # notify the live plot that we are done. fails if we are not using liveplot.
     try:
         plotter.finish()
     except Exception:
         pass
 
     # convert to list of dms, easier for the end user who doesn't know jax
```

### Comparing `phlash-1.0.2/src/phlash/model.py` & `phlash-1.0.3/src/phlash/model.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/mp.py` & `phlash-1.0.3/src/phlash/mp.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/params.py` & `phlash-1.0.3/src/phlash/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "Initialize parameters from a demographic model"
         assert dm.M == 16, "require M=16"
         u = 2 * dm.theta * dm.eta.ect()
         emis0 = jnp.exp(-u)
         emis1 = -jnp.expm1(-u)
         pi = dm.eta.pi
         A = phlash.transition.transition_matrix(dm)
-        emis0, emis1, pi, A = jax.tree_map(
+        emis0, emis1, pi, A = jax.tree.map(
             lambda a: a.clip(1e-20, 1.0 - 1e-20), (emis0, emis1, pi, A)
         )
         b, d, u = (jnp.diag(A, i) for i in [-1, 0, 1])
         v = A[0, 1:] / A[0, 1]
         ut = u / v
         return cls(
             b=jnp.append(b, 0.0),
```

### Comparing `phlash-1.0.2/src/phlash/plot.py` & `phlash-1.0.3/src/phlash/plot.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/sim.py` & `phlash-1.0.3/src/phlash/sim.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/size_history.py` & `phlash-1.0.3/src/phlash/size_history.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/src/phlash/transition.py` & `phlash-1.0.3/src/phlash/transition.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     # upper triangle
     p = {}
     p["R<=i,C>i|T=i"] = P_ect[:, 0, 1] * (
         jnp.append(jnp.exp(-(t[1:] - ect[:-1]) * c_adj[:-1]), 0.0)
     )  # entries above first diagnoal
     p["C>i|C>i-1,T<i"] = jnp.append(jnp.exp(-dt * c_adj[:-1]), 0.0)
     p["C=i|C>i-1,T<i"] = jnp.append(-jnp.expm1(-dt * c_adj[:-1]), 1.0)
-    p = jax.tree_map(lambda a: a.clip(1e-8, 1.0 - 1e-8), p)
+    p = jax.tree.map(lambda a: a.clip(1e-8, 1.0 - 1e-8), p)
     U = (
         p["R<=i,C>i|T=i"][i]
         * jnp.prod(
             p["C>i|C>i-1,T<i"][ell] ** ((i < ell) & (ell < j)), axis=2, keepdims=True
         )
         * p["C=i|C>i-1,T<i"][j]
         * (j > i)
```

### Comparing `phlash-1.0.2/src/phlash/util.py` & `phlash-1.0.3/src/phlash/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+import jax
 import jax.numpy as jnp
-import jax.tree_util as jtu
+import jax.tree_util
 
 
 class Pattern:
     """Class for parsing PSMC-style pattern strings."""
 
     def __init__(self, pattern: str):
         try:
@@ -31,18 +32,18 @@
 
     def expand(self, x):
         assert len(x) == len(self)
         return sum([e * [xx] for e, xx in zip(self._epochs, x)], [])
 
 
 def tree_stack(trees):
-    return jtu.tree_map(lambda *v: jnp.stack(v), *trees)
+    return jax.tree.map(lambda *v: jnp.stack(v), *trees)
 
 
 def tree_unstack(tree):
-    leaves, treedef = jtu.tree_flatten(tree)
+    leaves, treedef = jax.tree_util.tree_flatten(tree)
     return [treedef.unflatten(leaf) for leaf in zip(*leaves, strict=True)]
 
 
 def softplus_inv(y):
     # y > 0
     return y + jnp.log1p(-jnp.exp(-y))
```

### Comparing `phlash-1.0.2/tests/.benchmarks/Linux-CPython-3.10-64bit/0001_gpu_vs_jax.json` & `phlash-1.0.3/tests/.benchmarks/Linux-CPython-3.10-64bit/0001_gpu_vs_jax.json`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/.coverage` & `phlash-1.0.3/tests/.coverage`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/.pytest_cache/v/cache/lastfailed` & `phlash-1.0.3/tests/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/.pytest_cache/v/cache/nodeids` & `phlash-1.0.3/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/conftest.py` & `phlash-1.0.3/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os.path
+
 import jax
 import numpy as np
 from pytest import fixture
 
 from phlash.kernel import get_kernel
 from phlash.params import PSMCParams
 from phlash.size_history import DemographicModel
@@ -28,7 +30,12 @@
 def pp(dm) -> PSMCParams:
     return PSMCParams.from_dm(dm)
 
 
 @fixture
 def kern(data):
     return get_kernel(M=16, data=data, double_precision=True)
+
+
+@fixture
+def psmcfa_file():
+    return os.path.join(os.path.dirname(__file__), "fixtures", "sample.psmcfa")
```

### Comparing `phlash-1.0.2/tests/fixtures/elpd_bug.pkl` & `phlash-1.0.3/tests/fixtures/elpd_bug.pkl`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/fixtures/sample.bcf` & `phlash-1.0.3/tests/fixtures/sample.bcf`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/fixtures/tv_bug.pkl` & `phlash-1.0.3/tests/fixtures/tv_bug.pkl`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/test_afs.py` & `phlash-1.0.3/tests/test_afs.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/test_cband.py` & `phlash-1.0.3/tests/test_cband.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import numpy as np
+import pytest
 
 from phlash.cband import _find_confidence_bands
 
 
+@pytest.mark.slow
 def test_random_sampled_functions(rng):
     """
     Tests the find_confidence_bands function with randomly sampled functions.
     Checks if the solution satisfies basic confidence band criteria.
     Uses a fixture for the random number generator.
     """
     N, K = rng.integers(10, 100, size=(2,))
```

### Comparing `phlash-1.0.2/tests/test_data.py` & `phlash-1.0.3/tests/test_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import os.path
 import tempfile
 
 import msprime
 import numpy as np
-import pytest
 from pytest import fixture
 
 from phlash.data import RawContig, TreeSequenceContig, VcfContig, _chunk_het_matrix
 
 
 @fixture
 def sim():
@@ -24,24 +23,22 @@
     b = 0
     for ch_i in ch:
         q = min(chunk_size + overlap, len(H[0, b:]))
         assert np.all(ch_i[:q] == H[0, b : b + q])
         b += chunk_size
 
 
-def test_psmcfa():
-    fn = os.path.join(os.path.dirname(__file__), "fixtures", "sample.psmcfa")
-    for contig in "1", 0:
-        # allow passing by string name or index
-        rc = RawContig.from_psmcfa(fn, contig, 100)
-        assert rc.het_matrix.shape == (1, 100)
-        assert rc.het_matrix.sum() == 82
-        assert rc.window_size == 100
-    with pytest.raises(ValueError):
-        rc = RawContig.from_psmcfa(fn, "2", 100)
+def test_psmcfa(psmcfa_file):
+    # allow passing by string name or index
+    rc = list(RawContig.from_psmcfa_iter(psmcfa_file, 100))
+    assert len(rc) == 1
+    rc = rc[0]
+    assert rc.het_matrix.shape == (1, 100)
+    assert rc.het_matrix.sum() == 82
+    assert rc.window_size == 100
 
 
 def test_vcf():
     fn = os.path.join(os.path.dirname(__file__), "fixtures", "sample.bcf")
     vcf = VcfContig(
         fn,
         contig="1",
```

### Comparing `phlash-1.0.2/tests/test_gpu.py` & `phlash-1.0.3/tests/test_gpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import jax
 import jax.test_util
 import numpy as np
+import pytest
 from pytest import fixture
 
 from phlash.hmm import psmc_ll
 from phlash.kernel import get_kernel
 from phlash.params import PSMCParams
 
 jax.config.update("jax_enable_x64", True)
@@ -17,40 +18,45 @@
     return data.clip(-1, 1)
 
 
 def rel_err(a, b):
     return np.abs(a - b) / np.abs(a)
 
 
+@pytest.mark.slow
 def test_check_grads(dm, data, kern):
     jax.test_util.check_grads(
         lambda d: kern.loglik(d, 0), (dm,), order=1, modes=["rev"], rtol=1e-2
     )
 
 
+@pytest.mark.slow
 def test_eq_grad_nograd(pp: PSMCParams, data, kern):
     "test that the likelihood is the same using either method"
     inds = np.arange(len(data))
     ll1, _ = kern(pp, inds, grad=True)
     ll2 = kern(pp, inds, grad=False)
     np.testing.assert_allclose(ll1, ll2)
 
 
+@pytest.mark.slow
 def test_pyll_vs_cuda(dm, data, kern):
     ll1 = kern.loglik(dm, 0)
     ll2 = psmc_ll(dm, data[0])[1]
     np.testing.assert_allclose(ll1, ll2, rtol=1e-4)
 
 
+@pytest.mark.slow
 def test_pyll_vs_cuda_missing(dm, missing_data):
     kern = get_kernel(M=16, data=missing_data, double_precision=True)
     ll1 = kern.loglik(dm, 0)
     ll2 = psmc_ll(dm, missing_data[0])[1]
     np.testing.assert_allclose(ll1, ll2, rtol=1e-4)
 
 
+@pytest.mark.slow
 def test_pyll_vg_vs_cuda(dm, data, kern):
     ll1, dll1 = jax.value_and_grad(kern.loglik)(dm, 0)
     ll2, dll2 = jax.value_and_grad(lambda dm: psmc_ll(dm, data[0])[1])(dm)
     np.testing.assert_allclose(ll1, ll2, atol=1e-8, rtol=1e-5)
     for x, y in zip(dll1, dll2):
         np.testing.assert_allclose(x, y, atol=1e-8, rtol=1e-5)
```

### Comparing `phlash-1.0.2/tests/test_jax_ppoly.py` & `phlash-1.0.3/tests/test_jax_ppoly.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/test_model.py` & `phlash-1.0.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/test_sim.py` & `phlash-1.0.3/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/test_size_history.py` & `phlash-1.0.3/tests/test_size_history.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/test_speed.py` & `phlash-1.0.3/tests/speed.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/tests/test_transition.py` & `phlash-1.0.3/tests/test_transition.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.2/PKG-INFO` & `phlash-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: phlash
-Version: 1.0.2
+Version: 1.0.3
 Summary: Bayesian inference of population size history from recombining sequence data.
 Author-Email: Jonathan Terhorst <jonth@umich.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jthlab/phlash
 Project-URL: Bug reports, https://github.com/jthlab/phlash/issues
 Project-URL: Source, https://github.com/jthlab/phlash/
 Requires-Python: <4.0,>=3.10
 Requires-Dist: blackjax<2.0.0,>=1.1.0
-Requires-Dist: cuda-python<13,>=12.3
-Requires-Dist: cyvcf2<1.0.0,>=0.30.28
 Requires-Dist: intervaltree<4.0.0,>=3.1.0
-Requires-Dist: jax>=0.4.24
+Requires-Dist: jax>=0.4.25
 Requires-Dist: loguru<1.0.0,>=0.7.2
 Requires-Dist: matplotlib<4.0.0,>=3.8.2
 Requires-Dist: msprime<2.0.0,>=1.3.0
 Requires-Dist: numpy<2.0.0,>=1.26.3
 Requires-Dist: optax<1.0.0,>=0.1.9
 Requires-Dist: plotly<6.0.0,>=5.18.0
 Requires-Dist: scipy<2.0.0,>=1.12.0
@@ -25,19 +23,18 @@
 Requires-Dist: tskit<1.0.0,>=0.5.6
 Requires-Dist: demes<1.0.0,>=0.2.3
 Requires-Dist: jax-dataclasses<2.0.0,>=1.6.0
 Requires-Dist: tszip<1.0.0,>=0.2.3
 Requires-Dist: jaxtyping<1.0.0,>=0.2.25
 Requires-Dist: pulp>=2.8.0
 Requires-Dist: dinopy>=3.0.0
-Requires-Dist: jupyter>=1.0.0; extra == "webui"
-Requires-Dist: notebook>=7.1.1; extra == "webui"
-Requires-Dist: jax[cuda12_pip]>=0.4.24; extra == "gpu"
+Requires-Dist: pysam>=0.22.1
+Requires-Dist: jax[cuda12]>=0.4.25; extra == "gpu"
+Requires-Dist: cuda-python<13,>=12.3; extra == "gpu"
 Requires-Dist: nvidia-cuda-nvrtc-cu12>=12.3; extra == "gpu"
-Provides-Extra: webui
 Provides-Extra: gpu
 Description-Content-Type: text/markdown
 
 phlash is a program for sampling from the posterior distribution of population size
 history given whole genome sequence data. You can think of it as a Bayesian version
 of Li & Durbin's popular [PSMC](https://github.com/lh3/psmc) program, with a more
 modern interface and GPU acceleration built in.
@@ -58,26 +55,21 @@
 
 phlash can be installed from PyPI using pip:
 
 ```
 $ pip install phlash
 ```
 
-If your machine contains an Nvidia GPU, you should install the `gpu` variant in order to enable it.
-In this case, you should run:
+If your machine contains an Nvidia GPU, you should be sure to install the `gpu` variant in order to enable it:
 
 ```
-$ pip install \
-    -f "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html" \
-    --extra-index-url "https://pypi.ngc.nvidia.com" \
-    phlash[gpu]
+$ pip install 'phlash[gpu]'
 ```
 
-I recommend installing phlash into a separate virtual environment: before running the
-above, do
+I recommend installing phlash into a separate virtual environment: before running the above, do
 
 ```
 $ python3 -mvenv /path/to/phlash  # replace with desired path
 $ source /path/to/phlash/bin/activate
 $ pip3 install -U pip setuptools  # recent version of pip and setuptools are required
 ```
 ## Running the program
```

