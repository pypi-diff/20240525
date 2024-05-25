# Comparing `tmp/pypose-0.6.7.tar.gz` & `tmp/pypose-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypose-0.6.7.tar", last modified: Sat Jan 13 20:23:03 2024, max compression
+gzip compressed data, was "pypose-0.6.8.tar", last modified: Sat May 25 07:58:11 2024, max compression
```

## Comparing `pypose-0.6.7.tar` & `pypose-0.6.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.399897 pypose-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-01-13 20:22:52.000000 pypose-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-01-13 20:23:03.399897 pypose-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-01-13 20:22:52.000000 pypose-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.387897 pypose-0.6.7/pypose/
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.391897 pypose-0.6.7/pypose/basics/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/basics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/basics/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.391897 pypose-0.6.7/pypose/func/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/func/jac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.391897 pypose-0.6.7/pypose/function/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/function/checking.py
--rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/function/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/function/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/function/spline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.391897 pypose-0.6.7/pypose/lietensor/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/lietensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/lietensor/basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    33747 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/lietensor/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    44616 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/lietensor/lietensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    36241 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/lietensor/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)   109672 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/lietensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.395897 pypose-0.6.7/pypose/module/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25532 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/ekf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/icp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/imu_preintegrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17901 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/lqr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/mpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/pf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/pnp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/module/ukf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.395897 pypose-0.6.7/pypose/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/corrector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    28738 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/optim/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.395897 pypose-0.6.7/pypose/sparse/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/sparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/sparse/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.395897 pypose-0.6.7/pypose/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/testing/comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.399897 pypose-0.6.7/pypose/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-01-13 20:22:52.000000 pypose-0.6.7/pypose/utils/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.399897 pypose-0.6.7/pypose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-01-13 20:23:03.000000 pypose-0.6.7/pypose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-01-13 20:23:03.000000 pypose-0.6.7/pypose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 20:23:03.000000 pypose-0.6.7/pypose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-13 20:23:03.000000 pypose-0.6.7/pypose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-13 20:23:03.000000 pypose-0.6.7/pypose.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 20:23:03.000000 pypose-0.6.7/pypose.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 20:23:03.399897 pypose-0.6.7/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-13 20:22:52.000000 pypose-0.6.7/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-13 20:22:52.000000 pypose-0.6.7/requirements/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 20:23:03.399897 pypose-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-01-13 20:22:52.000000 pypose-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.802808 pypose-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-25 07:58:06.000000 pypose-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-25 07:58:11.802808 pypose-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-05-25 07:58:06.000000 pypose-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.790808 pypose-0.6.8/pypose/
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.790808 pypose-0.6.8/pypose/basics/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/basics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/basics/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.790808 pypose-0.6.8/pypose/func/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/func/jac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.794808 pypose-0.6.8/pypose/function/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/function/checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14273 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/function/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/function/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/function/spline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.794808 pypose-0.6.8/pypose/lietensor/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/lietensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12621 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/lietensor/basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33747 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/lietensor/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44730 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/lietensor/lietensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36241 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/lietensor/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109672 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/lietensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.798808 pypose-0.6.8/pypose/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25532 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/icp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22422 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/imu_preintegrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17901 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/lqr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/mpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/pf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/pnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/module/ukf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.798808 pypose-0.6.8/pypose/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/corrector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8413 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28738 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14519 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/optim/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.798808 pypose-0.6.8/pypose/sparse/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/sparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/sparse/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.798808 pypose-0.6.8/pypose/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/testing/comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.798808 pypose-0.6.8/pypose/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17052 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-25 07:58:06.000000 pypose-0.6.8/pypose/utils/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.798808 pypose-0.6.8/pypose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-25 07:58:11.000000 pypose-0.6.8/pypose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-25 07:58:11.000000 pypose-0.6.8/pypose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:58:11.000000 pypose-0.6.8/pypose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-25 07:58:11.000000 pypose-0.6.8/pypose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 07:58:11.000000 pypose-0.6.8/pypose.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:58:11.000000 pypose-0.6.8/pypose.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:58:11.798808 pypose-0.6.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-25 07:58:06.000000 pypose-0.6.8/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 07:58:06.000000 pypose-0.6.8/requirements/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:58:11.802808 pypose-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-25 07:58:06.000000 pypose-0.6.8/setup.py
```

### Comparing `pypose-0.6.7/LICENSE` & `pypose-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/PKG-INFO` & `pypose-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.6.7
+Version: 0.6.8
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang and PyPose Team
 Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
@@ -28,31 +28,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytest==7.*
+Requires-Dist: pytest>=7
 Requires-Dist: torch==2.*
 Provides-Extra: runtime
-Requires-Dist: pytest==7.*; extra == "runtime"
+Requires-Dist: pytest>=7; extra == "runtime"
 Requires-Dist: torch==2.*; extra == "runtime"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.0.0; extra == "docs"
 Requires-Dist: sphinxcontrib.katex; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: pypose_sphinx_theme; extra == "docs"
 Provides-Extra: all
+Requires-Dist: pytest>=7; extra == "all"
 Requires-Dist: torch==2.*; extra == "all"
-Requires-Dist: pypose_sphinx_theme; extra == "all"
-Requires-Dist: pytest==7.*; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: sphinx==5.0.0; extra == "all"
+Requires-Dist: pypose_sphinx_theme; extra == "all"
 Requires-Dist: sphinxcontrib.katex; extra == "all"
+Requires-Dist: sphinx==5.0.0; extra == "all"
 
 ## PyPose: A Library for Robot Learning with Physics-based Optimization
 
 ![robot](https://user-images.githubusercontent.com/8695500/193484553-2da66824-4461-4aca-ad8c-b17c05bef067.png)
 
 -----
```

### Comparing `pypose-0.6.7/README.md` & `pypose-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/__init__.py` & `pypose-0.6.8/pypose/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/basics/ops.py` & `pypose-0.6.8/pypose/basics/ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,30 +28,36 @@
     r'''
         Inplace version of :meth:`pypose.cumops`
     '''
     L, v = input.shape[dim], input
     assert dim != -1 or dim != v.shape[-1], "Invalid dim"
     for i in torch.pow(2, torch.arange(math.log2(L)+1, device=v.device, dtype=torch.int64)):
         index = torch.arange(i, L, device=v.device, dtype=torch.int64)
-        v.index_copy_(dim, index, ops(v.index_select(dim, index), v.index_select(dim, index-i)))
+        v.index_copy_(dim, index, ops(v.index_select(dim, index-i), v.index_select(dim, index)))
     return v
 
 
-def cummul_(input, dim):
+def cummul_(input, dim, left = True):
     r'''
         Inplace version of :meth:`pypose.cummul`
     '''
-    return cumops_(input, dim, lambda a, b : a * b)
+    if left:
+        return cumops_(input, dim, lambda a, b : b * a)
+    else:
+        return cumops_(input, dim, lambda a, b : a * b)
 
 
-def cumprod_(input, dim):
+def cumprod_(input, dim, left = True):
     r'''
         Inplace version of :meth:`pypose.cumprod`
     '''
-    return cumops_(input, dim, lambda a, b : a @ b)
+    if left:
+        return cumops_(input, dim, lambda a, b : b @ a)
+    else:
+        return cumops_(input, dim, lambda a, b : a @ b)
 
 
 def cumops(input, dim, ops):
     r"""Returns the cumulative user-defined operation of LieTensor along a dimension.
 
     .. math::
         y_i = x_1~\mathrm{\circ}~x_2 ~\mathrm{\circ}~ \cdots ~\mathrm{\circ}~ x_i,
@@ -72,20 +78,21 @@
         - The users are supposed to provide meaningful operation.
         - This function doesn't check whether the results are valid for mathematical
           definition of LieTensor, e.g., quaternion.
         - The time complexity of the function is :math:`\mathcal{O}(\log N)`, where
           :math:`N` is the LieTensor size along the :obj:`dim` dimension.
 
     Examples:
+        >>> # The following operations are equivalent.
         >>> input = pp.randn_SE3(2)
-        >>> input.cumprod(dim = 0)
+        >>> input.cumprod(dim = 0, left=True)
         SE3Type LieTensor:
         tensor([[-0.6466,  0.2956,  2.4055, -0.4428,  0.1893,  0.3933,  0.7833],
                 [ 1.2711,  1.2020,  0.0651, -0.0685,  0.6732,  0.7331, -0.0685]])
-        >>> pp.cumops(input, 0, lambda a, b : a @ b)
+        >>> pp.cumops(input, 0, lambda a, b : b @ a) # Left multiplication
         SE3Type LieTensor:
         tensor([[-0.6466,  0.2956,  2.4055, -0.4428,  0.1893,  0.3933,  0.7833],
                 [ 1.2711,  1.2020,  0.0651, -0.0685,  0.6732,  0.7331, -0.0685]])
     """
     return cumops_(input.clone(), dim, ops)
 
 
@@ -134,17 +141,17 @@
         >>> input = pp.randn_SO3(1,2)
         >>> pp.cummul(input, dim=1, left=False)
         SO3Type LieTensor:
         tensor([[[-1.8252e-01,  1.6198e-01,  8.3683e-01,  4.9007e-01],
                 [ 2.0905e-04,  5.2031e-01,  8.4301e-01, -1.3642e-01]]])
     """
     if left:
-        return cumops(input, dim, lambda a, b : a * b)
-    else:
         return cumops(input, dim, lambda a, b : b * a)
+    else:
+        return cumops(input, dim, lambda a, b : a * b)
 
 
 def cumprod(input, dim, left = True):
     r"""Returns the cumulative product (``@``) of LieTensor along a dimension.
 
     * Left product:
 
@@ -188,10 +195,10 @@
         >>> input = pp.randn_SO3(1,2)
         >>> pp.cumprod(input, dim=1, left=False)
         SO3Type LieTensor:
         tensor([[[ 0.5798, -0.1189, -0.2429,  0.7686],
                 [ 0.7515, -0.1920,  0.5072,  0.3758]]])
     """
     if left:
-        return cumops(input, dim, lambda a, b : a @ b)
-    else:
         return cumops(input, dim, lambda a, b : b @ a)
+    else:
+        return cumops(input, dim, lambda a, b : a @ b)
```

### Comparing `pypose-0.6.7/pypose/func/jac.py` & `pypose-0.6.8/pypose/func/jac.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/function/checking.py` & `pypose-0.6.8/pypose/function/checking.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/function/geometry.py` & `pypose-0.6.8/pypose/function/geometry.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/function/linalg.py` & `pypose-0.6.8/pypose/function/linalg.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/function/spline.py` & `pypose-0.6.8/pypose/function/spline.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/lietensor/__init__.py` & `pypose-0.6.8/pypose/lietensor/__init__.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/lietensor/basics.py` & `pypose-0.6.8/pypose/lietensor/basics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/lietensor/convert.py` & `pypose-0.6.8/pypose/lietensor/convert.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/lietensor/lietensor.py` & `pypose-0.6.8/pypose/lietensor/lietensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,32 +152,32 @@
         raise NotImplementedError("randn not implemented yet")
 
     @classmethod
     def cumops(self, X, dim, ops):
         return cumops(X, dim, ops)
 
     @classmethod
-    def cummul(self, X, dim):
-        return cummul(X, dim)
+    def cummul(self, X, dim, left = True):
+        return cummul(X, dim, left)
 
     @classmethod
     def cumprod(self, X, dim, left = True):
         return cumprod(X, dim, left)
 
     @classmethod
     def cumops_(self, X, dim, ops):
         return cumops_(X, dim, ops)
 
     @classmethod
-    def cummul_(self, X, dim):
-        return cummul_(X, dim)
+    def cummul_(self, X, dim, left = True):
+        return cummul_(X, dim, left)
 
     @classmethod
-    def cumprod_(self, X, dim):
-        return cumprod_(X, dim)
+    def cumprod_(self, X, dim, left = True):
+        return cumprod_(X, dim, left)
 
 
 class SO3Type(LieType):
     def __init__(self):
         super().__init__(4, 4, 3)
 
     def Log(self, X):
@@ -1148,43 +1148,43 @@
 
     def cumops(self, dim, ops):
         r"""
         See :func:`pypose.cumops`
         """
         return self.ltype.cumops(self, dim, ops)
 
-    def cummul(self, dim):
+    def cummul(self, dim, left = True):
         r"""
         See :func:`pypose.cummul`
         """
-        return self.ltype.cummul(self, dim)
+        return self.ltype.cummul(self, dim, left)
 
     def cumprod(self, dim, left = True):
         r"""
         See :func:`pypose.cumprod`
         """
         return self.ltype.cumprod(self, dim, left)
 
     def cumops_(self, dim, ops):
         r"""
         Inplace version of :func:`pypose.cumops`
         """
         return self.ltype.cumops_(self, dim, ops)
 
-    def cummul_(self, dim):
+    def cummul_(self, dim, left = True):
         r"""
         Inplace version of :func:`pypose.cummul`
         """
-        return self.ltype.cummul_(self, dim)
+        return self.ltype.cummul_(self, dim, left)
 
-    def cumprod_(self, dim):
+    def cumprod_(self, dim, left = True):
         r"""
         Inplace version of :func:`pypose.cumprod`
         """
-        return self.ltype.cumprod_(self, dim)
+        return self.ltype.cumprod_(self, dim, left)
 
 
 class Parameter(LieTensor, nn.Parameter):
     r'''
     A kind of LieTensor that is to be considered a module parameter.
 
     Parameters are of :meth:`LieTensor` and :meth:`torch.nn.Parameter`,
```

### Comparing `pypose-0.6.7/pypose/lietensor/operation.py` & `pypose-0.6.8/pypose/lietensor/operation.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/lietensor/utils.py` & `pypose-0.6.8/pypose/lietensor/utils.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/dynamics.py` & `pypose-0.6.8/pypose/module/dynamics.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/ekf.py` & `pypose-0.6.8/pypose/module/ekf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/icp.py` & `pypose-0.6.8/pypose/module/icp.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/imu_preintegrator.py` & `pypose-0.6.8/pypose/module/imu_preintegrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         >>> p = torch.zeros(3)    # Initial Position
         >>> r = pp.identity_SO3() # Initial rotation
         >>> v = torch.zeros(3)    # Initial Velocity
         >>> integrator = pp.module.IMUPreintegrator(p, r, v)
 
         2. Get IMU measurement
 
-        >>> ang = torch.tensor([0.1,0.1,0.1]) # angular velocity 
+        >>> ang = torch.tensor([0.1,0.1,0.1]) # angular velocity
         >>> acc = torch.tensor([0.1,0.1,0.1]) # acceleration
         >>> rot = pp.mat2SO3(torch.eye(3))    # Rotation (Optional)
         >>> dt = torch.tensor([0.002])        # Time difference between two measurements
 
         3. Preintegrating IMU measurements.
         Takes as input the IMU values and calculates the preintegrated IMU measurements.
 
@@ -99,15 +99,15 @@
         super().__init__()
         self.reset, self.prop_cov = reset, prop_cov
 
         if isinstance(acc_cov, float):
             acc_cov = torch.tensor([[acc_cov, acc_cov, acc_cov]])
         if isinstance(gyro_cov, float):
             gyro_cov = torch.tensor([[gyro_cov, gyro_cov, gyro_cov]])
-        
+
         # Initial status of IMU: (pos)ition, (rot)ation, (vel)ocity, (cov)ariance
         self.register_buffer('gravity', torch.tensor([0, 0, gravity]), persistent=False)
         self.register_buffer('pos', self._check(pos).clone(), persistent=False)
         self.register_buffer('rot', self._check(rot).clone(), persistent=False)
         self.register_buffer('vel', self._check(vel).clone(), persistent=False)
         self.register_buffer('cov', torch.zeros(1, 9, 9), persistent=False)
         self.register_buffer('gyro_cov', gyro_cov, persistent=False)
@@ -182,15 +182,15 @@
             - :math:`{\Delta}p_{ik}` is the preintegrated position between the :math:`i`-th
               and :math:`k`-th time step.
 
             - :math:`a_k` is linear acceleration at the :math:`k`-th time step.
 
             - :math:`w_k` is angular rate at the :math:`k`-th time step.
 
-            - :math:`{\Delta}t` is the time interval from time step :math:`k`-th to time 
+            - :math:`{\Delta}t` is the time interval from time step :math:`k`-th to time
               step :math:`{k+1}`-th time step.
 
         Uncertainty Propagation:
 
         .. math::
             \begin{align*}
                 C_{ik+1} &= A C_{ik} A^T + B \mathrm{diag}(C_g, C_a) B^T \\
@@ -209,15 +209,15 @@
         .. math::
             B = [B_g, B_a] \\
 
         .. math::
             B_g = \begin{bmatrix}
                     J_r^k \Delta t  \\
                     0_{3*3}  \\
-                    0_{3*3} 
+                    0_{3*3}
                 \end{bmatrix},
 
             B_a = \begin{bmatrix}
                     0_{3*3} \\
                     {\Delta}R_{ik} {\Delta}t  \\
                     1/2 {\Delta}R_{ik} {\Delta}t^2
                 \end{bmatrix},
@@ -289,15 +289,15 @@
             else:
                 Rij = inte_state['Dr']
 
             cov_input_state ={
                 'Rij': Rij.detach(),
                 'Rk': inte_state['w'].detach(),
                 'Ha': vec2skew(inte_state['a'].detach()),
-                'dt': dt.detach() 
+                'dt': dt.detach()
             }
             cov = self.propagate_cov(cov_input = cov_input_state, init_cov = init_cov,
                                     gyro_cov = gyro_cov, acc_cov = acc_cov)
         else:
             cov = {'cov': None}
 
         if not self.reset:
@@ -336,15 +336,15 @@
 
         Shape:
             - input (:obj:`dt`, :obj:`gyro`, :obj:`acc`): This layer supports the input shape
               with :math:`(B, F, H_{in})`, :math:`(F, H_{in})` and :math:`(H_{in})`, where
               :math:`B` is the batch size (or the number of IMU), :math:`F` is the number of
               frames (measurements), and :math:`H_{in}` is the raw sensor signals.
 
-            - init_rot: The initial orientation of the integration, which helps to 
+            - init_rot: The initial orientation of the integration, which helps to
               compensate for the gravity. It contains the shape :math:`(B, H_{in})`. d
 
             - rot: The ground truth orientation of the integration. If this parameter is
               given, the integrator will use the ground truth orientation to compensate the
               gravity.
 
         Return:
@@ -380,15 +380,15 @@
 
         return {'a':a, 'Dp':incre_p[:,1:,:], 'Dv':incre_v[...,1:,:], 'Dr':incre_r[:,1:,:],
                 'Dt':incre_t[...,1:,:], 'w': w[:,1:,:]}
 
     @classmethod
     def predict(cls, init_state, integrate):
         r"""
-        Propogate the next IMU state from the initial IMU state (:obj:`init_state`) with 
+        Propogate the next IMU state from the initial IMU state (:obj:`init_state`) with
         the preintegrated IMU measurements (:math:`\Delta{p}`, :math:`\Delta{v}` and
         :math:`\Delta{r}`).
 
         .. math::
             \begin{align*}
                 R_j &= {\Delta}R_{ij} * R_i                                                     \\
                 v_j &= R_i * {\Delta}v_{ij}   + v_i + g \Delta t_{ij}                           \\
@@ -428,19 +428,19 @@
         ## The input acc_cov and gyro cov should be a vector of 3
         B, F = cov_input['dt'].shape[:2]
         device = cov_input['dt'].device; dtype = cov_input['dt'].dtype
 
         Cg = torch.diag_embed(gyro_cov)
         Ca = torch.diag_embed(acc_cov)
 
-        # constructing the propagate 
+        # constructing the propagate
         A = torch.eye(9, device=device, dtype=dtype).repeat([B, F+1, 1, 1])
         Bg = torch.zeros(B, F, 9, 3, device=device, dtype=dtype)
         Ba = torch.zeros(B, F, 9, 3, device=device, dtype=dtype)
-        
+
         A[:, :-1, 0:3, 0:3] = cov_input['Rk'].matrix().mT # R_{k,k+1}^T
         A[:, :-1, 3:6, 0:3] = torch.einsum('...xy,...t -> ...xy', \
             - cov_input['Rij'].matrix() @ cov_input['Ha'], cov_input['dt'])
         A[:, :-1, 6:9, 0:3] = torch.einsum('...xy,...t -> ...xy', \
             - 0.5 * cov_input['Rij'].matrix() @ cov_input['Ha'], cov_input['dt']**2)
         A[:, :-1, 6:9, 3:6] = torch.einsum('...xy,...t -> ...xy', \
             torch.eye(3, device=device, dtype=dtype).repeat([B, F, 1, 1]), cov_input['dt'])
```

### Comparing `pypose-0.6.7/pypose/module/lqr.py` & `pypose-0.6.8/pypose/module/lqr.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/mpc.py` & `pypose-0.6.8/pypose/module/mpc.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/pf.py` & `pypose-0.6.8/pypose/module/pf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/pnp.py` & `pypose-0.6.8/pypose/module/pnp.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/module/ukf.py` & `pypose-0.6.8/pypose/module/ukf.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/optim/corrector.py` & `pypose-0.6.8/pypose/optim/corrector.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/optim/functional.py` & `pypose-0.6.8/pypose/optim/functional.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/optim/kernel.py` & `pypose-0.6.8/pypose/optim/kernel.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/optim/optimizer.py` & `pypose-0.6.8/pypose/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/optim/scheduler.py` & `pypose-0.6.8/pypose/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/optim/solver.py` & `pypose-0.6.8/pypose/optim/solver.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/optim/strategy.py` & `pypose-0.6.8/pypose/optim/strategy.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/sparse/ops.py` & `pypose-0.6.8/pypose/sparse/ops.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/testing/comparison.py` & `pypose-0.6.8/pypose/testing/comparison.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/utils/collect_env.py` & `pypose-0.6.8/pypose/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose/utils/stepper.py` & `pypose-0.6.8/pypose/utils/stepper.py`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/pypose.egg-info/PKG-INFO` & `pypose-0.6.8/pypose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypose
-Version: 0.6.7
+Version: 0.6.8
 Summary: To connect classic robotics with modern learning methods.
 Home-page: https://pypose.org
 Download-URL: https://github.com/pypose/pypose
 Author: Chen Wang and PyPose Team
 Author-email: admin@pypose.org
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/pypose/pypose/issues
@@ -28,31 +28,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytest==7.*
+Requires-Dist: pytest>=7
 Requires-Dist: torch==2.*
 Provides-Extra: runtime
-Requires-Dist: pytest==7.*; extra == "runtime"
+Requires-Dist: pytest>=7; extra == "runtime"
 Requires-Dist: torch==2.*; extra == "runtime"
 Provides-Extra: docs
 Requires-Dist: sphinx==5.0.0; extra == "docs"
 Requires-Dist: sphinxcontrib.katex; extra == "docs"
 Requires-Dist: sphinx_rtd_theme; extra == "docs"
 Requires-Dist: pypose_sphinx_theme; extra == "docs"
 Provides-Extra: all
+Requires-Dist: pytest>=7; extra == "all"
 Requires-Dist: torch==2.*; extra == "all"
-Requires-Dist: pypose_sphinx_theme; extra == "all"
-Requires-Dist: pytest==7.*; extra == "all"
 Requires-Dist: sphinx_rtd_theme; extra == "all"
-Requires-Dist: sphinx==5.0.0; extra == "all"
+Requires-Dist: pypose_sphinx_theme; extra == "all"
 Requires-Dist: sphinxcontrib.katex; extra == "all"
+Requires-Dist: sphinx==5.0.0; extra == "all"
 
 ## PyPose: A Library for Robot Learning with Physics-based Optimization
 
 ![robot](https://user-images.githubusercontent.com/8695500/193484553-2da66824-4461-4aca-ad8c-b17c05bef067.png)
 
 -----
```

### Comparing `pypose-0.6.7/pypose.egg-info/SOURCES.txt` & `pypose-0.6.8/pypose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypose-0.6.7/setup.py` & `pypose-0.6.8/setup.py`

 * *Files identical despite different names*

