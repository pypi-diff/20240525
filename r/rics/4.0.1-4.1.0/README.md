# Comparing `tmp/rics-4.0.1.tar.gz` & `tmp/rics-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rics-4.0.1.tar", max compression
+gzip compressed data, was "rics-4.1.0.tar", max compression
```

## Comparing `rics-4.0.1.tar` & `rics-4.1.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0     1077 2024-03-21 22:56:26.764852 rics-4.0.1/LICENSE.md
--rw-r--r--   0        0        0     3592 2024-03-21 22:56:26.764852 rics-4.0.1/README.md
--rw-r--r--   0        0        0     4870 2024-03-21 22:56:26.776852 rics-4.0.1/pyproject.toml
--rw-r--r--   0        0        0      276 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_internal_support/__init__.py
--rw-r--r--   0        0        0     5154 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_internal_support/_local_or_remote.py
--rw-r--r--   0        0        0      473 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_internal_support/changelog/__init__.py
--rw-r--r--   0        0        0     2540 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_internal_support/changelog/_patch_notes.py
--rw-r--r--   0        0        0      615 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_internal_support/changelog/_split_changelog.py
--rw-r--r--   0        0        0     1730 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_internal_support/changelog/_write_changelog.py
--rw-r--r--   0        0        0      344 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_internal_support/types.py
--rw-r--r--   0        0        0     3058 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/_just_the_way_i_like_it.py
--rw-r--r--   0        0        0     4297 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/action_level.py
--rw-r--r--   0        0        0       28 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/collections/__init__.py
--rw-r--r--   0        0        0    10256 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/collections/dicts.py
--rw-r--r--   0        0        0      854 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/collections/misc.py
--rw-r--r--   0        0        0     3015 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/envinterp/__init__.py
--rw-r--r--   0        0        0      544 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/envinterp/_file_utils.py
--rw-r--r--   0        0        0     4623 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/envinterp/_variable.py
--rw-r--r--   0        0        0     4039 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/logs.py
--rw-r--r--   0        0        0    14078 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/misc.py
--rw-r--r--   0        0        0      125 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/__init__.py
--rw-r--r--   0        0        0     4769 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/__init__.py
--rw-r--r--   0        0        0      134 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_backend/__init__.py
--rw-r--r--   0        0        0     2204 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_backend/_available.py
--rw-r--r--   0        0        0      487 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_backend/_datetime_index_like.py
--rw-r--r--   0        0        0     4930 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_backend/_limits.py
--rw-r--r--   0        0        0     2643 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_backend/_schedule.py
--rw-r--r--   0        0        0     3744 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_backend/_span.py
--rw-r--r--   0        0        0     5663 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_backend/_splitter.py
--rw-r--r--   0        0        0     1514 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_docstrings.py
--rw-r--r--   0        0        0      261 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_frontend/__init__.py
--rw-r--r--   0        0        0    11831 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_frontend/_plot.py
--rw-r--r--   0        0        0     5103 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_frontend/_progress.py
--rw-r--r--   0        0        0     1043 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_frontend/_split.py
--rw-r--r--   0        0        0     3001 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_frontend/_to_string.py
--rw-r--r--   0        0        0     2171 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_frontend/_weight.py
--rw-r--r--   0        0        0      420 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/_support.py
--rw-r--r--   0        0        0       62 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/integration/__init__.py
--rw-r--r--   0        0        0      953 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/integration/_log_progress.py
--rw-r--r--   0        0        0     1808 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/integration/pandas/__init__.py
--rw-r--r--   0        0        0     2809 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/integration/pandas/_impl.py
--rw-r--r--   0        0        0     2424 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/integration/polars/__init__.py
--rw-r--r--   0        0        0     1891 2024-03-21 22:56:26.776852 rics-4.0.1/src/rics/ml/time_split/integration/polars/_impl.py
--rw-r--r--   0        0        0      131 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/ml/time_split/integration/sklearn/__init__.py
--rw-r--r--   0        0        0     5721 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/ml/time_split/integration/sklearn/_impl.py
--rw-r--r--   0        0        0     2566 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/ml/time_split/integration/split_data.py
--rw-r--r--   0        0        0     6153 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/ml/time_split/settings.py
--rw-r--r--   0        0        0      564 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/ml/time_split/support/__init__.py
--rw-r--r--   0        0        0     2002 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/ml/time_split/types.py
--rw-r--r--   0        0        0      415 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/__init__.py
--rw-r--r--   0        0        0     2546 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/_format_perf_counter.py
--rw-r--r--   0        0        0     7081 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/_multi_case_timer.py
--rw-r--r--   0        0        0     6329 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/_util.py
--rw-r--r--   0        0        0     1869 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/_wrapper.py
--rw-r--r--   0        0        0     7942 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/cli.py
--rw-r--r--   0        0        0      398 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/plot/__init__.py
--rw-r--r--   0        0        0     6523 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/plot/_params.py
--rw-r--r--   0        0        0     1661 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/plot/_plot.py
--rw-r--r--   0        0        0     1314 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/plot/_postprocessors.py
--rw-r--r--   0        0        0      555 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/plot/types.py
--rw-r--r--   0        0        0      600 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/templates/candidates.py.txt
--rw-r--r--   0        0        0      455 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/templates/test_data.py.txt
--rw-r--r--   0        0        0      408 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/performance/types.py
--rw-r--r--   0        0        0     4172 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/plotting.py
--rw-r--r--   0        0        0        0 2024-03-21 22:56:26.780852 rics-4.0.1/src/rics/py.typed
--rw-r--r--   0        0        0     4946 1970-01-01 00:00:00.000000 rics-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-25 18:18:55.886805 rics-4.1.0/LICENSE.md
+-rw-r--r--   0        0        0     3942 2024-05-25 18:18:55.886805 rics-4.1.0/README.md
+-rw-r--r--   0        0        0     4667 2024-05-25 18:18:55.894805 rics-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-05-25 18:18:55.894805 rics-4.1.0/src/rics/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 18:18:55.894805 rics-4.1.0/src/rics/_internal_support/__init__.py
+-rw-r--r--   0        0        0     5172 2024-05-25 18:18:55.894805 rics-4.1.0/src/rics/_internal_support/_local_or_remote.py
+-rw-r--r--   0        0        0      473 2024-05-25 18:18:55.894805 rics-4.1.0/src/rics/_internal_support/changelog/__init__.py
+-rw-r--r--   0        0        0     2540 2024-05-25 18:18:55.894805 rics-4.1.0/src/rics/_internal_support/changelog/_patch_notes.py
+-rw-r--r--   0        0        0      604 2024-05-25 18:18:55.894805 rics-4.1.0/src/rics/_internal_support/changelog/_split_changelog.py
+-rw-r--r--   0        0        0     1724 2024-05-25 18:18:55.894805 rics-4.1.0/src/rics/_internal_support/changelog/_write_changelog.py
+-rw-r--r--   0        0        0     3106 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/_just_the_way_i_like_it.py
+-rw-r--r--   0        0        0     4297 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/action_level.py
+-rw-r--r--   0        0        0       28 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/collections/__init__.py
+-rw-r--r--   0        0        0    17565 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/collections/dicts.py
+-rw-r--r--   0        0        0      863 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/collections/misc.py
+-rw-r--r--   0        0        0     3015 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/envinterp/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/envinterp/_file_utils.py
+-rw-r--r--   0        0        0     4623 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/envinterp/_variable.py
+-rw-r--r--   0        0        0     4039 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/logs.py
+-rw-r--r--   0        0        0    14196 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/misc.py
+-rw-r--r--   0        0        0      125 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/__init__.py
+-rw-r--r--   0        0        0     5035 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/__init__.py
+-rw-r--r--   0        0        0      134 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_backend/__init__.py
+-rw-r--r--   0        0        0     2204 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_backend/_available.py
+-rw-r--r--   0        0        0      487 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_backend/_datetime_index_like.py
+-rw-r--r--   0        0        0     4930 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_backend/_limits.py
+-rw-r--r--   0        0        0     2643 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_backend/_schedule.py
+-rw-r--r--   0        0        0     3744 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_backend/_span.py
+-rw-r--r--   0        0        0     5663 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_backend/_splitter.py
+-rw-r--r--   0        0        0     1514 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_docstrings.py
+-rw-r--r--   0        0        0      261 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_frontend/__init__.py
+-rw-r--r--   0        0        0    11831 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_frontend/_plot.py
+-rw-r--r--   0        0        0     5103 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_frontend/_progress.py
+-rw-r--r--   0        0        0     1043 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_frontend/_split.py
+-rw-r--r--   0        0        0     3001 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_frontend/_to_string.py
+-rw-r--r--   0        0        0     2171 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_frontend/_weight.py
+-rw-r--r--   0        0        0      420 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/_support.py
+-rw-r--r--   0        0        0       62 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/_log_progress.py
+-rw-r--r--   0        0        0     1808 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/pandas/__init__.py
+-rw-r--r--   0        0        0     2809 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/pandas/_impl.py
+-rw-r--r--   0        0        0     2424 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/polars/__init__.py
+-rw-r--r--   0        0        0     1891 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/polars/_impl.py
+-rw-r--r--   0        0        0      131 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/sklearn/__init__.py
+-rw-r--r--   0        0        0     5721 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/sklearn/_impl.py
+-rw-r--r--   0        0        0     2566 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/integration/split_data.py
+-rw-r--r--   0        0        0     6153 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/settings.py
+-rw-r--r--   0        0        0      564 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/support/__init__.py
+-rw-r--r--   0        0        0     2002 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/ml/time_split/types.py
+-rw-r--r--   0        0        0     3879 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/paths.py
+-rw-r--r--   0        0        0      415 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/_format_perf_counter.py
+-rw-r--r--   0        0        0     7073 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/_multi_case_timer.py
+-rw-r--r--   0        0        0     6356 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/_util.py
+-rw-r--r--   0        0        0     1869 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/_wrapper.py
+-rw-r--r--   0        0        0     7942 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/cli.py
+-rw-r--r--   0        0        0      398 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/plot/__init__.py
+-rw-r--r--   0        0        0     6550 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/plot/_params.py
+-rw-r--r--   0        0        0     1661 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/plot/_plot.py
+-rw-r--r--   0        0        0     1314 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/plot/_postprocessors.py
+-rw-r--r--   0        0        0      555 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/plot/types.py
+-rw-r--r--   0        0        0      600 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/templates/candidates.py.txt
+-rw-r--r--   0        0        0      455 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/templates/test_data.py.txt
+-rw-r--r--   0        0        0      408 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/performance/types.py
+-rw-r--r--   0        0        0     4172 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/plotting.py
+-rw-r--r--   0        0        0        0 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/py.typed
+-rw-r--r--   0        0        0     6031 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/strings.py
+-rw-r--r--   0        0        0      229 2024-05-25 18:18:55.898805 rics-4.1.0/src/rics/types.py
+-rw-r--r--   0        0        0     5296 1970-01-01 00:00:00.000000 rics-4.1.0/PKG-INFO
```

### Comparing `rics-4.0.1/LICENSE.md` & `rics-4.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/README.md` & `rics-4.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,38 +7,52 @@
 # RiCS: my personal little ML engineering library. <!-- omit in toc -->
 [![PyPI - Version](https://img.shields.io/pypi/v/rics.svg)](https://pypi.python.org/pypi/rics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rics.svg)](https://pypi.python.org/pypi/rics)
 [![Tests](https://github.com/rsundqvist/rics/workflows/tests/badge.svg)](https://github.com/rsundqvist/rics/actions?workflow=tests)
 [![Codecov](https://codecov.io/gh/rsundqvist/rics/branch/master/graph/badge.svg)](https://codecov.io/gh/rsundqvist/rics)
 [![Read the Docs](https://readthedocs.org/projects/rics/badge/)](https://rics.readthedocs.io/)
 [![PyPI - License](https://img.shields.io/pypi/l/rics.svg)](https://pypi.python.org/pypi/rics)
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 ## What is it?
-An assorted collections of generic functions that used to live in a Dropbox folder where I used to keep useful snippets.
-RiCS, pronounced _"rix_", is short for _**Ri**chard's **C**ode **S**tash_. I started this project with the purpose of 
-learning more about Python best practices, typing and the Python ecosystem. It has grown organically since then, and now
-provides a wide variety of utility functions. The [id-translation](https://pypi.org/project/id-translation/) suite 
-(installed separately) relies heavily on [rics.mapping][mapping], as well as a number of other functions provided herein.
+An assorted collection of reusable functions that used to live in a Dropbox folder. RiCS, pronounced _"rix_", is short 
+for _**Ri**chard's **C**ode **S**tash_. I started this project with the purpose of learning more about Python best 
+practices, typing and the Python ecosystem.
+
+It has grown organically since then, and now provides a wide variety of small utility functions. Large submodules are
+typically converted to [stand-alone PyPI packages](#related-libraries) once they begin to mature.
 
 ## Highlighted Features
-- Multivariate [performance testing][perf].
-- Various other [utilities][utility], ranging from [logging] to [plotting] to specialized [dict] functions.
-- [Time-based cross-validation][time-split] splitter for heterogeneous data, 
-  including ``pandas`` and ``scikit-learn`` integrations.
+- Multivariate [performance testing][perf] and [plotting][perf-plot].
+- [get_by_full_name()]: Import functions, objects and classes by name.
+- [rics.collections.dicts]: Extended functionality for the built-in `dict` type.
+- [basic_config()]: Configure logging for development.
+- And much more; click [here](https://rics.readthedocs.io/en/stable/_autosummary/rics.html) for the full API.
+
+## Related libraries
+The following packages started life as RiCS submodules.
+
+* ID Translation
+  [![PyPI - Version](https://img.shields.io/pypi/v/id-translation.svg)](https://pypi.python.org/pypi/id-translation) 
+  [![Read the Docs](https://readthedocs.org/projects/id-translation/badge/)](https://id-translation.readthedocs.io/)
+
+  **_Turn meaningless IDs into human-readable labels._**
+
+* Time Split
+  [![PyPI - Version](https://img.shields.io/pypi/v/time-split.svg)](https://pypi.python.org/pypi/time-split)
+  [![Read the Docs](https://readthedocs.org/projects/time-split/badge/)](https://time-split.readthedocs.io/)
+
+  **_Time-based k-fold validation splits for heterogeneous data._**
 
 [perf]: https://rics.readthedocs.io/en/stable/_autosummary/rics.performance.html#rics.performance.run_multivariate_test
 [perf-plot]: https://rics.readthedocs.io/en/stable/_autosummary/rics.performance.html#rics.performance.plot_run
 
-[utility]: https://rics.readthedocs.io/en/stable/_autosummary/rics.misc.html
-[logging]: https://rics.readthedocs.io/en/stable/_autosummary/rics.logs.html
-[plotting]: https://rics.readthedocs.io/en/stable/_autosummary/rics.plotting.html
-[dict]: https://rics.readthedocs.io/en/stable/_autosummary/rics.collections.dicts.html
-[time-split]: https://rics.readthedocs.io/en/stable/_autosummary/rics.ml.time_split.html
+[get_by_full_name()]: https://rics.readthedocs.io/en/stable/_autosummary/rics.misc.html#rics.misc.get_by_full_name
+
+[basic_config()]: https://rics.readthedocs.io/en/stable/_autosummary/rics.logs.html#rics.logs.basic_config
+[rics.collections.dicts]: https://rics.readthedocs.io/en/stable/_autosummary/rics.collections.dicts.html
 
 ## Installation
 The package is published through the [Python Package Index (PyPI)]. Source code
 is available on GitHub: https://github.com/rsundqvist/rics
 
 ```sh
 pip install -U rics
```

### Comparing `rics-4.0.1/pyproject.toml` & `rics-4.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rics"
-version = "4.0.1"
+version = "4.1.0"
 description = "My personal little ML engineering library."
 authors = ["Richard Sundqvist <richard.sundqvist@live.se>"]
 
 readme = "README.md"
 homepage = "https://github.com/rsundqvist/rics"
 repository = "https://github.com/rsundqvist/rics"
 documentation = "https://rics.readthedocs.io"
@@ -46,15 +46,15 @@
 [tool.poetry.extras]
 cli = ["click"]
 plotting = ["matplotlib", "seaborn"]
 
 [tool.poetry.group.manual-extras.dependencies]
 # Extras that must be available for docs + tests go here. Doc/test-only deps go in their respective groups.
 croniter = "^2.0.1"
-pyarrow = "^15.0.0"
+pyarrow = "^16.0.0"
 polars = { version = "^0.20.16", extras = ["pandas"] }
 
 [tool.poetry.group.docs]
 [tool.poetry.group.docs.dependencies]
 # duplicate object warnings for sphinx>=4
 # description: https://github.com/astropy/astropy/issues/11723
 # https://github.com/astropy/astropy/pull/12270
@@ -75,20 +75,16 @@
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 xdoctest = "^1.1.1"
 coverage = "^7.3.0"
 pytest-cov = "^4.1.0"
 
-scikit-learn = "^1.4.0"
-# TODO Unpin.
-# dask.datasets.timeseries() warns:
-#     UserWarning: dask_expr does not support the DataFrameIOFunction protocol for column projection
-# on dask == 2024.3.1
-dask = { version = "==2024.2.1", extras = ["dataframe"] }
+scikit-learn = "^1.4.2"
+dask = { version = "^2024.5.0 ", extras = ["dataframe"] }
 
 [tool.poetry.group.devops.dependencies]
 invoke = "^2.2.0"
 mypy = "^1.9.0"
 ruff = "^0.3.3"
 
 safety = "^3.0.1"
@@ -177,15 +173,15 @@
 max-line-length = 150
 
 [tool.pytest]
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
     "ignore:Matplotlib is currently using agg:UserWarning",
-    "ignore:.*utcfromtimestamp.*:DeprecationWarning", # Detta är farligt - ta bort
+    "ignore:.*rics.ml.time_split:DeprecationWarning",
 ]
 log_file_level = 10
 log_file = "pytest.log"
 norecursedirs = [
     "**/cli_modules/*",
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rics-4.0.1/src/rics/_internal_support/_local_or_remote.py` & `rics-4.1.0/src/rics/_internal_support/_local_or_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import logging
 import pickle
 from collections.abc import Callable, Iterable
 from pathlib import Path
 from typing import Any, BinaryIO
 from urllib.parse import urljoin
 
-from .types import PathLikeType
-
 try:
     from tqdm.auto import tqdm
 
     TQDM_INSTALLED = True
 except ModuleNotFoundError:
     TQDM_INSTALLED = False
 
 _CHUNK_SIZE: int = 1024
 
 LOGGER = logging.getLogger("rics.utility.misc")
 _GLOR_LOGGER = LOGGER.getChild("get_local_or_remote")
 
 
 def get_local_or_remote(
-    file: PathLikeType,
+    file: str,
     *,
-    remote_root: PathLikeType,
-    local_root: PathLikeType,
+    remote_root: str,
+    local_root: str,
     force: bool = False,
     postprocessor: Callable[[str], Any] | None = None,
-    show_progress: bool = TQDM_INSTALLED,
+    show_progress: bool | None = TQDM_INSTALLED,
 ) -> Path:
     """Retrieve a file from a local or remove (HTTP/HTTPS) source.
 
     Args:
         file: Name of an object to retrieve.
         remote_root: Remote location where the `file` may be downloaded.
         local_root: Local storage location for `file`.
@@ -40,15 +38,17 @@
             Returned value must be pickleable.
         show_progress: If ``True``, show a progress bar.
 
     Returns:
         Location where `file` may be accessed locally. Transformations are applied if a `postprocessor` is given, in
         which case the returned ``Path`` will point to a transformed result.
     """
-    if show_progress and not TQDM_INSTALLED:
+    if show_progress is None:
+        show_progress = TQDM_INSTALLED
+    elif show_progress and not TQDM_INSTALLED:
         raise ModuleNotFoundError("The tqdm package is not installed; cannot show progress.")
 
     return _get_file(
         file=str(file),
         remote_root=str(remote_root),
         local_root=Path(str(local_root)).absolute(),
         force=force,
```

### Comparing `rics-4.0.1/src/rics/_internal_support/changelog/_patch_notes.py` & `rics-4.1.0/src/rics/_internal_support/changelog/_patch_notes.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/_internal_support/changelog/_split_changelog.py` & `rics-4.1.0/src/rics/_internal_support/changelog/_split_changelog.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
-from ..types import PathLikeType
+from rics.paths import AnyPath
+
 from ._patch_notes import PatchNotes
 from ._write_changelog import write_changelog
 
 
-def split_changelog(output_dir: PathLikeType, changelog: PathLikeType = "CHANGELOG.md") -> None:
+def split_changelog(output_dir: AnyPath, changelog: AnyPath = "CHANGELOG.md") -> None:
     """Split a Markdown changelog into multiple pages.
 
     Args:
         output_dir: Output directory where pages will be placed. Only ``index.rst`` needs to be manually imported.
         changelog: The changelog to split.
 
     """
```

### Comparing `rics-4.0.1/src/rics/_internal_support/changelog/_write_changelog.py` & `rics-4.1.0/src/rics/_internal_support/changelog/_write_changelog.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import shutil
-from pathlib import Path
 
-from ..types import PathLikeType
+from rics.paths import AnyPath, any_path_to_path
+
 from ._patch_notes import PatchNotes
 
 BASE_LINES: list[str] = [
     "Changelog",
     "=========",
     "All notable changes to this project will be documented in this file.",
     "The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_",
@@ -14,27 +14,27 @@
     ".. toctree::",
     "   :hidden:",
     "",
 ]
 
 
 def write_changelog(
-    output_dir: PathLikeType,
+    output_dir: AnyPath,
     notes: list[PatchNotes],
     refs: dict[str, str],
 ) -> None:
     """Write changelog parts to several pages in an output directory.
 
     Args:
         output_dir: Output directory where pages will be placed. Only ``index.rst`` needs to be manually imported.
         notes: A list of patch notes, in the order in which they should be added to the TOC.
         refs: Title references.
 
     """
-    root = Path(str(output_dir))
+    root = any_path_to_path(output_dir)
     shutil.rmtree(root, ignore_errors=True)
     root.mkdir()
 
     index_lines = BASE_LINES.copy()
 
     for note in notes:
         page = note.title.replace("[", "").replace("]", "").replace("#", "").lower().strip()
```

### Comparing `rics-4.0.1/src/rics/_just_the_way_i_like_it.py` & `rics-4.1.0/src/rics/_just_the_way_i_like_it.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-import contextlib
-import logging
-import os
-import sys
-import traceback
-from multiprocessing import process
 from typing import Any
 
-from .logs import basic_config
-
 _SKIP_WARNING: bool = False
 
 
 def configure_stuff(
     level: int | str = "INFO",
     rics_level: int | str = "INFO",
     id_translation_level: int | str = "INFO",
@@ -29,14 +21,18 @@
         level: Log level for the root logger. Default is ``logging.INFO``.
         rics_level: Log level for the :mod:`rics` package. Default is ``logging.INFO``.
         id_translation_level: Log level for the :mod:`id_translation` package. Default is ``logging.INFO``.
         matplotlib_level: Log level for the :mod:`matplotlib` package. Default is ``logging.WARNING``.
         **kwargs: Keyword arguments for :func:`rics.logs.basic_config` and :py:func:`logging.basicConfig`.
 
     """
+    import contextlib
+
+    from .logs import basic_config
+
     basic_config(
         level=level,
         rics_level=rics_level,
         id_translation_level=id_translation_level,
         matplotlib_level=matplotlib_level,
         **kwargs,
     )
@@ -54,14 +50,16 @@
 
 def _configure_pandas() -> None:
     try:
         import pandas as pd
     except ModuleNotFoundError:
         return
 
+    import contextlib
+
     pd.options.display.max_columns = 50
     pd.options.display.max_colwidth = 150
     pd.options.display.max_rows = 250
     pd.options.display.width = 0
     pd.options.display.float_format = "{:.6g}".format
 
     pd.options.mode.chained_assignment = "raise"
@@ -69,25 +67,31 @@
         pd.options.mode.copy_on_write = "warn"
 
     with contextlib.suppress(ImportError):
         pd.plotting.register_matplotlib_converters()
 
 
 def _maybe_emit_warning() -> None:  # pragma: no cover
+    import logging
+    import os
+    import sys
+    import traceback
+    from multiprocessing import process
+
     global _SKIP_WARNING  # noqa: PLW0603
     if _SKIP_WARNING:
         return
     _SKIP_WARNING = True
 
+    if os.environ.get("JTWILI", "").lower() == "true":
+        return
+
     if getattr(process.current_process(), "_inheriting", False):
         return  # From multiprocessing.spawn._check_not_importing_main
 
-    if os.environ.get("JTWILI", "false").lower() == "true":
-        return
-
     try:
         get_ipython()  # type: ignore[name-defined]
         return  # noqa: TRY300 # Typically in a console or notebook
     except NameError:
         pass
 
     caller = traceback.format_stack()[-3]
```

### Comparing `rics-4.0.1/src/rics/action_level.py` & `rics-4.1.0/src/rics/action_level.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/collections/misc.py` & `rics-4.1.0/src/rics/collections/misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Miscellaneous utility methods for collections."""
 
-from collections.abc import Iterable
-from typing import Any, TypeVar
+import typing as _t
+from collections.abc import Iterable as _Iterable
 
-ArgType = TypeVar("ArgType")
+ArgType = _t.TypeVar("ArgType")
 """ArgType generic type."""
 
 
-def as_list(arg: ArgType | Iterable[ArgType] | None = None, excl_types: tuple[type[Any]] = (str,)) -> list[ArgType]:
+def as_list(arg: ArgType | _Iterable[ArgType] | None = None, excl_types: tuple[type[_t.Any]] = (str,)) -> list[ArgType]:
     """Create a list or list-wrapping of `arg`.
 
     Args:
         arg: An object to name.
         excl_types: Iterable types that should be treated as single elements, such as strings.
 
     Returns:
         A list representation of `arg`.
 
     Notes:
         For all zero-length arguments, i.e. ``len(arg) == 0``, an empty list is returned.
 
     """
     # https://github.com/python/mypy/issues/10835
-    if isinstance(arg, Iterable) and not isinstance(arg, excl_types):
+    if isinstance(arg, _Iterable) and not isinstance(arg, excl_types):
         return list(arg)
     else:
         return [arg]  # type: ignore[list-item]
```

### Comparing `rics-4.0.1/src/rics/envinterp/__init__.py` & `rics-4.1.0/src/rics/envinterp/__init__.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/envinterp/_file_utils.py` & `rics-4.1.0/src/rics/envinterp/_file_utils.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/envinterp/_variable.py` & `rics-4.1.0/src/rics/envinterp/_variable.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/logs.py` & `rics-4.1.0/src/rics/logs.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/misc.py` & `rics-4.1.0/src/rics/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import typing as _t
 from importlib import import_module as _import_module
 from pathlib import Path as _Path
 from pprint import saferepr as _safe_repr
 from types import ModuleType as _ModuleType
 
-from ._internal_support import _local_or_remote
-from ._internal_support.types import PathLikeType
+from . import paths as _paths
 from .envinterp import UnsetVariableError as _UnsetVariableError
 from .envinterp import Variable as _Variable
+from .types import AnyPath as _AnyPath
 
 
 def interpolate_environment_variables(
     s: str,
     *,
     allow_nested: bool = True,
     allow_blank: bool = False,
@@ -310,35 +310,36 @@
             return value_repr
         return tname(value)
 
     return ", ".join(f"{k}={repr_value(v)}" for k, v in kwargs.items())
 
 
 def get_local_or_remote(
-    file: PathLikeType,
+    file: _AnyPath,
     *,
-    remote_root: PathLikeType,
-    local_root: PathLikeType = ".",
+    remote_root: _AnyPath,
+    local_root: _AnyPath = ".",
     force: bool = False,
     postprocessor: _t.Callable[[str], _t.Any] | None = None,
-    show_progress: bool = _local_or_remote.TQDM_INSTALLED,
+    show_progress: bool | None = None,
 ) -> _Path:
     r"""Retrieve the path of a local file, downloading it if needed.
 
     If `file` is not available at the local root path, it will be downloaded using `requests.get`_. A postprocessor may
     be given in which case the name of the final file will be ``local_root/<name-of-postprocessor>/file``. Removing
     a raw local file (i.e. ``local_root/file``) will invalidate postprocessed files as well.
 
     Args:
         file: A file to retrieve or download.
         remote_root: Remote URL where the data may be retrieved using ``requests.get``.
         local_root: Local directory where the file may be cached.
         force: If ``True``, always download and apply processing (if applicable). Existing files will be overwritten.
         postprocessor: A function which takes a single argument `input_path` and returns a pickleable type.
-        show_progress: If ``True``, show a progress bar. Requires the `tqdm`_ package.
+        show_progress: If ``True``, show a progress bar. Requires the `tqdm`_ package. If ``None``, use only if TQDM
+            is installed.
 
     Returns:
         An absolute path to the data.
 
     Raises:
         ValueError: If local root path does not exist or is not a directory.
         ValueError: If the local file does not exist and ``remote=None``.
@@ -373,18 +374,20 @@
         https://www.imdb.com/interfaces/
     .. _requests.get:
         https://2.python-requests.org/en/master/api/#requests.get
     .. _tqdm:
         https://pypi.org/project/tqdm/
 
     """
-    return _local_or_remote.get_local_or_remote(
-        file=file,
-        local_root=local_root,
-        remote_root=remote_root,
+    from ._internal_support._local_or_remote import get_local_or_remote as _impl
+
+    return _impl(
+        file=_paths.any_path_to_str(file),
+        local_root=_paths.any_path_to_str(local_root),
+        remote_root=_paths.any_path_to_str(remote_root),
         force=force,
         postprocessor=postprocessor,
         show_progress=show_progress,
     )
 
 
 def serializable(obj: object) -> bool:
```

### Comparing `rics-4.0.1/src/rics/ml/time_split/__init__.py` & `rics-4.1.0/src/rics/ml/time_split/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Create temporal k-folds for cross-validation with heterogeneous data.
 
-.. minigallery:: rics.ml.time_split.plot
-    :add-heading: Examples
-    :heading-level: =
+.. warning::
 
-Examples demonstrate usage of :func:`.split` and :func:`.plot`. The :mod:`.integration` functions do not have examples,
-but mostly behave the same way as the :func:`.split`-function.
+   This module is deprecated. Use the :mod:`time_split` |pypi-badge| package instead.
+
+.. |pypi-badge| image:: https://img.shields.io/pypi/v/time-split.svg
+                :target: https://pypi.org/project/time-split/
 
 .. _tsug:
 
 User guide
 ==========
 High-level overview of relevant concepts.
 
@@ -106,14 +106,27 @@
        Pass an :ref:`offset alias <pandas:timeseries.offset_aliases>` specify how limits should be rounded. To specify
        by `how much` limits may be rounded, pass two offset aliases separated by a  ``'<'``.
 
        For example, passing ``flex="d<1h"`` will snap limits to the nearest date, but will not expand limits by more
        than one hour in either direction.
 """
 
+from warnings import warn as _warn
+
 from ._frontend import log_split_progress, plot, split
 
 __all__ = [
     "log_split_progress",
     "plot",
     "split",
 ]
+
+_warn(
+    (
+        f"The `{__package__}` submodule is now a stand-alone package.\n"
+        "Run `python -m pip install time-split` to install, or"
+        " pin `rics==4.0.1` to hide this warning."
+    ),
+    category=DeprecationWarning,
+    stacklevel=2,
+)
+del _warn
```

### Comparing `rics-4.0.1/src/rics/ml/time_split/_backend/_available.py` & `rics-4.1.0/src/rics/ml/time_split/_backend/_available.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_backend/_limits.py` & `rics-4.1.0/src/rics/ml/time_split/_backend/_limits.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_backend/_schedule.py` & `rics-4.1.0/src/rics/ml/time_split/_backend/_schedule.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_backend/_span.py` & `rics-4.1.0/src/rics/ml/time_split/_backend/_span.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_backend/_splitter.py` & `rics-4.1.0/src/rics/ml/time_split/_backend/_splitter.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_docstrings.py` & `rics-4.1.0/src/rics/ml/time_split/_docstrings.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_frontend/_plot.py` & `rics-4.1.0/src/rics/ml/time_split/_frontend/_plot.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_frontend/_progress.py` & `rics-4.1.0/src/rics/ml/time_split/_frontend/_progress.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_frontend/_split.py` & `rics-4.1.0/src/rics/ml/time_split/_frontend/_split.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_frontend/_to_string.py` & `rics-4.1.0/src/rics/ml/time_split/_frontend/_to_string.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/_frontend/_weight.py` & `rics-4.1.0/src/rics/ml/time_split/_frontend/_weight.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/integration/_log_progress.py` & `rics-4.1.0/src/rics/ml/time_split/integration/_log_progress.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/integration/pandas/__init__.py` & `rics-4.1.0/src/rics/ml/time_split/integration/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/integration/pandas/_impl.py` & `rics-4.1.0/src/rics/ml/time_split/integration/pandas/_impl.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/integration/polars/__init__.py` & `rics-4.1.0/src/rics/ml/time_split/integration/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/integration/polars/_impl.py` & `rics-4.1.0/src/rics/ml/time_split/integration/polars/_impl.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/integration/sklearn/_impl.py` & `rics-4.1.0/src/rics/ml/time_split/integration/sklearn/_impl.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/integration/split_data.py` & `rics-4.1.0/src/rics/ml/time_split/integration/split_data.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/settings.py` & `rics-4.1.0/src/rics/ml/time_split/settings.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/support/__init__.py` & `rics-4.1.0/src/rics/ml/time_split/support/__init__.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/ml/time_split/types.py` & `rics-4.1.0/src/rics/ml/time_split/types.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/performance/_multi_case_timer.py` & `rics-4.1.0/src/rics/performance/_multi_case_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import warnings
-from collections.abc import Collection, Mapping
+from collections.abc import Collection, Hashable, Mapping
 from timeit import Timer
-from typing import Any, Generic, Hashable, TypeAlias
+from typing import Any, Generic, TypeAlias
+
+from rics.strings import format_seconds as fmt_time
 
 from ..misc import tname
-from ._format_perf_counter import format_seconds as fmt_time
 from .types import CandFunc, DataType, ResultsDict
 
 CandidateMethodArg: TypeAlias = dict[str, CandFunc[DataType]] | Collection[CandFunc[DataType]] | CandFunc[DataType]
 TestDataArg: TypeAlias = dict[Hashable, DataType] | Collection[DataType]
 
 
 class MultiCaseTimer(Generic[DataType]):
```

### Comparing `rics-4.0.1/src/rics/performance/_util.py` & `rics-4.1.0/src/rics/performance/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Hashable, Iterable, Literal, TypeGuard, cast, get_args
+from collections.abc import Hashable, Iterable
+from typing import Any, Literal, TypeGuard, cast, get_args
 
 import pandas as pd
 
 from .types import ResultsDict
 
 
 def to_dataframe(run_results: ResultsDict, names: Iterable[str] = ()) -> pd.DataFrame:
```

### Comparing `rics-4.0.1/src/rics/performance/_wrapper.py` & `rics-4.1.0/src/rics/performance/_wrapper.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/performance/cli.py` & `rics-4.1.0/src/rics/performance/cli.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/performance/plot/_params.py` & `rics-4.1.0/src/rics/performance/plot/_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Hashable, Iterable, Mapping
 from dataclasses import dataclass, field, fields
-from typing import Any, ClassVar, Hashable, Iterable, Literal, Mapping, Self
+from typing import Any, ClassVar, Literal, Self
 
 import numpy as np
 import pandas as pd
 
 from ...collections.dicts import compute_if_absent
 from ..types import ResultsDict
 from .types import Candidate, FuncOrData, Kind, TestData, Unit
```

### Comparing `rics-4.0.1/src/rics/performance/plot/_plot.py` & `rics-4.1.0/src/rics/performance/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/performance/plot/_postprocessors.py` & `rics-4.1.0/src/rics/performance/plot/_postprocessors.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/performance/plot/types.py` & `rics-4.1.0/src/rics/performance/plot/types.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/performance/templates/candidates.py.txt` & `rics-4.1.0/src/rics/performance/templates/candidates.py.txt`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/src/rics/plotting.py` & `rics-4.1.0/src/rics/plotting.py`

 * *Files identical despite different names*

### Comparing `rics-4.0.1/PKG-INFO` & `rics-4.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rics
-Version: 4.0.1
+Version: 4.1.0
 Summary: My personal little ML engineering library.
 Home-page: https://github.com/rsundqvist/rics
 Keywords: rics
 Author: Richard Sundqvist
 Author-email: richard.sundqvist@live.se
 Requires-Python: >=3.11
 Classifier: Development Status :: 5 - Production/Stable
@@ -40,38 +40,52 @@
 # RiCS: my personal little ML engineering library. <!-- omit in toc -->
 [![PyPI - Version](https://img.shields.io/pypi/v/rics.svg)](https://pypi.python.org/pypi/rics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rics.svg)](https://pypi.python.org/pypi/rics)
 [![Tests](https://github.com/rsundqvist/rics/workflows/tests/badge.svg)](https://github.com/rsundqvist/rics/actions?workflow=tests)
 [![Codecov](https://codecov.io/gh/rsundqvist/rics/branch/master/graph/badge.svg)](https://codecov.io/gh/rsundqvist/rics)
 [![Read the Docs](https://readthedocs.org/projects/rics/badge/)](https://rics.readthedocs.io/)
 [![PyPI - License](https://img.shields.io/pypi/l/rics.svg)](https://pypi.python.org/pypi/rics)
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 ## What is it?
-An assorted collections of generic functions that used to live in a Dropbox folder where I used to keep useful snippets.
-RiCS, pronounced _"rix_", is short for _**Ri**chard's **C**ode **S**tash_. I started this project with the purpose of 
-learning more about Python best practices, typing and the Python ecosystem. It has grown organically since then, and now
-provides a wide variety of utility functions. The [id-translation](https://pypi.org/project/id-translation/) suite 
-(installed separately) relies heavily on [rics.mapping][mapping], as well as a number of other functions provided herein.
+An assorted collection of reusable functions that used to live in a Dropbox folder. RiCS, pronounced _"rix_", is short 
+for _**Ri**chard's **C**ode **S**tash_. I started this project with the purpose of learning more about Python best 
+practices, typing and the Python ecosystem.
+
+It has grown organically since then, and now provides a wide variety of small utility functions. Large submodules are
+typically converted to [stand-alone PyPI packages](#related-libraries) once they begin to mature.
 
 ## Highlighted Features
-- Multivariate [performance testing][perf].
-- Various other [utilities][utility], ranging from [logging] to [plotting] to specialized [dict] functions.
-- [Time-based cross-validation][time-split] splitter for heterogeneous data, 
-  including ``pandas`` and ``scikit-learn`` integrations.
+- Multivariate [performance testing][perf] and [plotting][perf-plot].
+- [get_by_full_name()]: Import functions, objects and classes by name.
+- [rics.collections.dicts]: Extended functionality for the built-in `dict` type.
+- [basic_config()]: Configure logging for development.
+- And much more; click [here](https://rics.readthedocs.io/en/stable/_autosummary/rics.html) for the full API.
+
+## Related libraries
+The following packages started life as RiCS submodules.
+
+* ID Translation
+  [![PyPI - Version](https://img.shields.io/pypi/v/id-translation.svg)](https://pypi.python.org/pypi/id-translation) 
+  [![Read the Docs](https://readthedocs.org/projects/id-translation/badge/)](https://id-translation.readthedocs.io/)
+
+  **_Turn meaningless IDs into human-readable labels._**
+
+* Time Split
+  [![PyPI - Version](https://img.shields.io/pypi/v/time-split.svg)](https://pypi.python.org/pypi/time-split)
+  [![Read the Docs](https://readthedocs.org/projects/time-split/badge/)](https://time-split.readthedocs.io/)
+
+  **_Time-based k-fold validation splits for heterogeneous data._**
 
 [perf]: https://rics.readthedocs.io/en/stable/_autosummary/rics.performance.html#rics.performance.run_multivariate_test
 [perf-plot]: https://rics.readthedocs.io/en/stable/_autosummary/rics.performance.html#rics.performance.plot_run
 
-[utility]: https://rics.readthedocs.io/en/stable/_autosummary/rics.misc.html
-[logging]: https://rics.readthedocs.io/en/stable/_autosummary/rics.logs.html
-[plotting]: https://rics.readthedocs.io/en/stable/_autosummary/rics.plotting.html
-[dict]: https://rics.readthedocs.io/en/stable/_autosummary/rics.collections.dicts.html
-[time-split]: https://rics.readthedocs.io/en/stable/_autosummary/rics.ml.time_split.html
+[get_by_full_name()]: https://rics.readthedocs.io/en/stable/_autosummary/rics.misc.html#rics.misc.get_by_full_name
+
+[basic_config()]: https://rics.readthedocs.io/en/stable/_autosummary/rics.logs.html#rics.logs.basic_config
+[rics.collections.dicts]: https://rics.readthedocs.io/en/stable/_autosummary/rics.collections.dicts.html
 
 ## Installation
 The package is published through the [Python Package Index (PyPI)]. Source code
 is available on GitHub: https://github.com/rsundqvist/rics
 
 ```sh
 pip install -U rics
```

