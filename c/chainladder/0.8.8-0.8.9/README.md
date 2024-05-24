# Comparing `tmp/chainladder-0.8.8.tar.gz` & `tmp/chainladder-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainladder-0.8.8.tar", last modified: Mon Sep 13 12:23:18 2021, max compression
+gzip compressed data, was "chainladder-0.8.9.tar", last modified: Sun Oct 24 20:21:14 2021, max compression
```

## Comparing `chainladder-0.8.8.tar` & `chainladder-0.8.9.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.661764 chainladder-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2021-09-13 12:23:10.000000 chainladder-0.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      992 2021-09-13 12:23:10.000000 chainladder-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    10932 2021-09-13 12:23:18.661764 chainladder-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9392 2021-09-13 12:23:10.000000 chainladder-0.8.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.641764 chainladder-0.8.8/chainladder/
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.641764 chainladder-0.8.8/chainladder/adjustments/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7957 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/berqsherm.py
--rw-r--r--   0 runner    (1001) docker     (121)    11227 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4390 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/parallelogram.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.641764 chainladder-0.8.8/chainladder/adjustments/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      538 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/tests/test_berqsherm.py
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/tests/test_parallelogram.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/tests/test_trend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2772 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/adjustments/trend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.645763 chainladder-0.8.8/chainladder/core/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15141 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6154 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     7396 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4518 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/display.py
--rw-r--r--   0 runner    (1001) docker     (121)    14163 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/dunders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    15540 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)    13901 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/slice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.645763 chainladder-0.8.8/chainladder/core/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2696 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/tests/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/tests/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/tests/test_grain.py
--rw-r--r--   0 runner    (1001) docker     (121)     4057 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/tests/test_slicing.py
--rw-r--r--   0 runner    (1001) docker     (121)    10036 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/tests/test_triangle.py
--rw-r--r--   0 runner    (1001) docker     (121)    31185 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/core/triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.645763 chainladder-0.8.8/chainladder/development/
--rw-r--r--   0 runner    (1001) docker     (121)      807 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/barnzehn.py
--rw-r--r--   0 runner    (1001) docker     (121)     5520 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    10791 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/clark.py
--rw-r--r--   0 runner    (1001) docker     (121)     3789 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/constant.py
--rw-r--r--   0 runner    (1001) docker     (121)     7967 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/development.py
--rw-r--r--   0 runner    (1001) docker     (121)     5236 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/glm.py
--rw-r--r--   0 runner    (1001) docker     (121)     6052 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/incremental.py
--rw-r--r--   0 runner    (1001) docker     (121)     8172 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/learning.py
--rw-r--r--   0 runner    (1001) docker     (121)    15048 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/munich.py
--rw-r--r--   0 runner    (1001) docker     (121)     7556 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/development/outstanding.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.645763 chainladder-0.8.8/chainladder/methods/
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5608 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/benktander.py
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/bornferg.py
--rw-r--r--   0 runner    (1001) docker     (121)     7481 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/capecod.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/chainladder.py
--rw-r--r--   0 runner    (1001) docker     (121)     7244 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/mack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.645763 chainladder-0.8.8/chainladder/methods/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/tests/test_benktander.py
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/tests/test_capecod.py
--rw-r--r--   0 runner    (1001) docker     (121)     5571 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/tests/test_mack.py
--rw-r--r--   0 runner    (1001) docker     (121)     4309 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/methods/tests/test_predict.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.649763 chainladder-0.8.8/chainladder/tails/
--rw-r--r--   0 runner    (1001) docker     (121)      389 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6409 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5896 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/bondy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4910 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/clark.py
--rw-r--r--   0 runner    (1001) docker     (121)     2570 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/constant.py
--rw-r--r--   0 runner    (1001) docker     (121)     7856 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/curve.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.649763 chainladder-0.8.8/chainladder/tails/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/tests/test_bondy.py
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/tests/test_constant.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/tails/tests/test_exponential.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.649763 chainladder-0.8.8/chainladder/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/cupy.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.661764 chainladder-0.8.8/chainladder/utils/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/abc.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4348 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/auto.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2994 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/berqsherm.csv
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/cc_sample.csv
--rw-r--r--   0 runner    (1001) docker     (121)  3235366 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/clrd.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/genins.csv
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/ia_sample.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6221 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/liab.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/m3ir5.csv
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/mcl.csv
--rw-r--r--   0 runner    (1001) docker     (121)      898 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/mortgage.csv
--rw-r--r--   0 runner    (1001) docker     (121)      926 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/mw2008.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2780 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/mw2014.csv
--rw-r--r--   0 runner    (1001) docker     (121)  4306791 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/prism.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6912 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/quarterly.csv
--rw-r--r--   0 runner    (1001) docker     (121)      995 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/raa.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/tail_sample.csv
--rw-r--r--   0 runner    (1001) docker     (121)      514 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/ukmotor.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/usaa.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1573 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/usauto.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/data/xyz.csv
--rw-r--r--   0 runner    (1001) docker     (121)     3315 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/sparse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.661764 chainladder-0.8.8/chainladder/utils/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     4598 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/templates/triangle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.661764 chainladder-0.8.8/chainladder/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    13642 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5707 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/utils/weighted_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.661764 chainladder-0.8.8/chainladder/workflow/
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7273 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/workflow/gridsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.661764 chainladder-0.8.8/chainladder/workflow/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/workflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/workflow/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/workflow/tests/test_voting.py
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/workflow/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    13876 2021-09-13 12:23:10.000000 chainladder-0.8.8/chainladder/workflow/voting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-13 12:23:18.641764 chainladder-0.8.8/chainladder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10932 2021-09-13 12:23:18.000000 chainladder-0.8.8/chainladder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2021-09-13 12:23:18.000000 chainladder-0.8.8/chainladder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-13 12:23:18.000000 chainladder-0.8.8/chainladder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-13 12:23:18.000000 chainladder-0.8.8/chainladder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-13 12:23:18.000000 chainladder-0.8.8/chainladder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-09-13 12:23:10.000000 chainladder-0.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-09-13 12:23:18.661764 chainladder-0.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2021-09-13 12:23:10.000000 chainladder-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.396229 chainladder-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    16725 2021-10-24 20:21:02.000000 chainladder-0.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2021-10-24 20:21:02.000000 chainladder-0.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     9714 2021-10-24 20:21:14.396229 chainladder-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9339 2021-10-24 20:21:02.000000 chainladder-0.8.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.376228 chainladder-0.8.9/chainladder/
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.376228 chainladder-0.8.9/chainladder/adjustments/
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7957 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/berqsherm.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11227 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4390 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/parallelogram.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.376228 chainladder-0.8.9/chainladder/adjustments/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/tests/test_berqsherm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/tests/test_parallelogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)      583 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/tests/test_trend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2772 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/adjustments/trend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.380229 chainladder-0.8.9/chainladder/core/
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15285 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6154 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7396 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4518 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/display.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14474 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/dunders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15692 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13878 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/slice.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.380229 chainladder-0.8.9/chainladder/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2696 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/tests/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/tests/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3187 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/tests/test_grain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4057 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/tests/test_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10981 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/tests/test_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31269 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/core/triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.380229 chainladder-0.8.9/chainladder/development/
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2126 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/barnzehn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5642 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10791 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/clark.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3789 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/constant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7967 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/development.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5236 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/glm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6052 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/incremental.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8172 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/learning.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15048 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/munich.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7556 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/development/outstanding.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.380229 chainladder-0.8.9/chainladder/methods/
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5608 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5649 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/benktander.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2741 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/bornferg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7481 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/capecod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/chainladder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7244 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/mack.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.384229 chainladder-0.8.9/chainladder/methods/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1492 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/tests/test_benktander.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1530 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/tests/test_capecod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5788 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/tests/test_mack.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4309 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/methods/tests/test_predict.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.384229 chainladder-0.8.9/chainladder/tails/
+-rw-r--r--   0 runner    (1001) docker     (121)      389 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6466 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5964 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/bondy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4943 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/clark.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2797 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/constant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8482 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/curve.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.384229 chainladder-0.8.9/chainladder/tails/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/tests/test_bondy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/tests/test_constant.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/tails/tests/test_exponential.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.384229 chainladder-0.8.9/chainladder/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/cupy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.392229 chainladder-0.8.9/chainladder/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/abc.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     4348 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/auto.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2994 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/berqsherm.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/cc_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (121)  3235366 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/clrd.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     1116 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/genins.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/ia_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     6221 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/liab.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     1984 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/m3ir5.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/mcl.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/mortgage.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/mw2008.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2780 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/mw2014.csv
+-rw-r--r--   0 runner    (1001) docker     (121)  4306791 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/prism.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     6912 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/quarterly.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/raa.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     1136 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/tail_sample.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      514 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/ukmotor.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/usaa.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     1573 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/usauto.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2392 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/data/xyz.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     2651 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/sparse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.392229 chainladder-0.8.9/chainladder/utils/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     4598 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/templates/triangle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.392229 chainladder-0.8.9/chainladder/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2430 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13642 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5707 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/utils/weighted_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.396229 chainladder-0.8.9/chainladder/workflow/
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7273 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/workflow/gridsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.396229 chainladder-0.8.9/chainladder/workflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/workflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/workflow/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3981 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/workflow/tests/test_voting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2134 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/workflow/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13876 2021-10-24 20:21:02.000000 chainladder-0.8.9/chainladder/workflow/voting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-24 20:21:14.376228 chainladder-0.8.9/chainladder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     9714 2021-10-24 20:21:13.000000 chainladder-0.8.9/chainladder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3624 2021-10-24 20:21:14.000000 chainladder-0.8.9/chainladder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-24 20:21:13.000000 chainladder-0.8.9/chainladder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-24 20:21:13.000000 chainladder-0.8.9/chainladder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-10-24 20:21:13.000000 chainladder-0.8.9/chainladder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-24 20:21:02.000000 chainladder-0.8.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-24 20:21:14.396229 chainladder-0.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2021-10-24 20:21:02.000000 chainladder-0.8.9/setup.py
```

### Comparing `chainladder-0.8.8/LICENSE` & `chainladder-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/MANIFEST.in` & `chainladder-0.8.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/PKG-INFO` & `chainladder-0.8.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,158 +1,161 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: chainladder
-Version: 0.8.8
+Version: 0.8.9
 Summary: Chainladder Package - P&C Loss Reserving package 
 Home-page: https://github.com/casact/chainladder-python
 Maintainer: John Bogaardt
 Maintainer-email: jbogaardt@gmail.com
 License: MPL-2.0
-Download-URL: https://github.com/casact/chainladder-python/archive/v0.8.8.tar.gz
-Description: .. -*- mode: rst -*-
-        
-        chainladder (python)
-        ====================
-        
-        |PyPI version| |Conda Version| |Build Status| |codecov io| |Documentation Status|
-        
-        chainladder - Property and Casualty Loss Reserving in Python
-        ------------------------------------------------------------
-        
-        This package gets inspiration from the popular `R ChainLadder package`_.
-        
-        This package strives to be minimalistic in needing its own API. Think in
-        `pandas`_ for data manipulation and `scikit-learn`_ for model
-        construction. An actuary already versed in these tools will pick up this
-        package with ease. Save your mental energy for actuarial work.
-        
-        
-        Documentation
-        -------------
-        
-        Please visit the `Documentation`_ page for examples, how-tos, and source
-        code documentation.
-        
-        
-        Available Estimators
-        --------------------
-        
-        ``chainladder`` has an ever growing list of estimators that work seemlessly together:
-        
-        .. _R ChainLadder package: https://github.com/mages/ChainLadder
-        .. _pandas: https://pandas.pydata.org/
-        .. _scikit-learn: https://scikit-learn.org/stable/index.html
-        
-        .. |PyPI version| image:: https://badge.fury.io/py/chainladder.svg
-           :target: https://badge.fury.io/py/chainladder
-        
-        .. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/chainladder.svg
-           :target: https://anaconda.org/conda-forge/chainladder
-        
-        .. |Build Status| image:: https://github.com/casact/chainladder-python/workflows/Unit%20Tests/badge.svg
-        
-        .. |Documentation Status| image:: https://readthedocs.org/projects/chainladder-python/badge/?version=latest
-           :target: http://chainladder-python.readthedocs.io/en/latest/?badge=latest
-        
-        .. |codecov io| image:: https://codecov.io/github/casact/chainladder-python/coverage.svg?branch=master
-           :target: https://codecov.io/github/casact/chainladder-python?branch=master
-        
-        
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | Loss                         | Tails Factors    | IBNR Models             | Adjustments           | Workflow              |
-        | Development                  |                  |                         |                       |                       |
-        +==============================+==================+=========================+=======================+=======================+
-        | `Development`_               | `TailCurve`_     | `Chainladder`_          | `BootstrapODPSample`_ | `VotingChainladder`_  |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `DevelopmentConstant`_       | `TailConstant`_  | `MackChainladder`_      | `BerquistSherman`_    |  `Pipeline`_          |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `MunichAdjustment`_          | `TailBondy`_     | `BornhuettterFerguson`_ | `ParallelogramOLF`_   | `GridSearch`_         |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `ClarkLDF`_                  | `TailClark`_     | `Benktander`_           | `Trend`_              |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `IncrementalAdditive`_       |                  | `CapeCod`_              |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `CaseOutstanding`_           |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `TweedieGLM`_                |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `DevelopmentML`_             |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `BarnettZehnwirth`_          |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        
-        
-        .. _Development: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#basic-development
-        .. _TailCurve: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#ldf-curve-fitting
-        .. _Chainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#basic-chainladder
-        .. _BootstrapODPSample: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#bootstrap-sampling
-        .. _DevelopmentConstant: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#external-patterns
-        .. _TailConstant: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#external-data
-        .. _MackChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#mack-chainladder
-        .. _BerquistSherman: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#berquist-sherman
-        .. _MunichAdjustment: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#munich-adjustment
-        .. _TailBondy: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#the-bondy-tail
-        .. _BornhuettterFerguson: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#bornhuetter-ferguson
-        .. _Pipeline: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#pipeline
-        .. _ClarkLDF: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#growth-curve-fitting
-        .. _TailClark: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#growth-curve-extrapolation
-        .. _Benktander: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#benktander
-        .. _GridSearch: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#gridsearch
-        .. _IncrementalAdditive: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#incremental-additive
-        .. _CapeCod: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#cape-cod
-        .. _ParallelogramOLF: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#parallelogramolf
-        .. _VotingChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#votingchainladder
-        .. _Trend: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#trend
-        .. _CaseOutstanding: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#caseoutstanding
-        .. _TweedieGLM: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#tweedieglm
-        .. _DevelopmentML: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentml
-        .. _BarnettZehnwirth: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#barnettzehnwirth
-        .. _Documentation: https://chainladder-python.readthedocs.io/en/latest/
-        
-        Getting Started Tutorials
-        -------------------------
-        
-        Tutorial notebooks are available for download `here`_.
-        
-        * `Working with Triangles`_
-        * `Selecting Development Patterns`_
-        * `Extending Development Patterns with Tails`_
-        * `Applying Deterministic Methods`_
-        * `Applying Stochastic Methods`_
-        * `Large Datasets`_
-        
-        Installation
-        ------------
-        
-        To install using pip: ``pip install chainladder``
-        
-        To instal using conda: ``conda install -c conda-forge chainladder``
-        
-        Alternatively for pre-release functionality, install directly from github:
-        ``pip install git+https://github.com/casact/chainladder-python/``
-        
-        Note: This package requires Python>=3.5 pandas 0.23.0 and later,
-        sparse 0.9 and later, scikit-learn 0.23.0 and later.
-        
-        Questions or Ideas?
-        --------------------
-        
-        Join in on the `github discussions`_.  Your question is more likely to get answered
-        here than on Stack Overflow.  We're always happy to answer any usage
-        questions or hear ideas on how to make ``chainladder`` better.
-        
-        
-        Want to contribute?
-        -------------------
-        
-        Check out our `contributing guidelines`_.
-        
-        .. _here: https://github.com/casact/chainladder-python/tree/master/docs/tutorials
-        .. _Working with Triangles: https://chainladder-python.readthedocs.io/en/latest/tutorials/triangle-tutorial.html
-        .. _Selecting Development Patterns: https://chainladder-python.readthedocs.io/en/latest/tutorials/development-tutorial.html
-        .. _Extending Development Patterns with Tails: https://chainladder-python.readthedocs.io/en/latest/tutorials/tail-tutorial.html
-        .. _Applying Deterministic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/deterministic-tutorial.html
-        .. _Applying Stochastic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/stochastic-tutorial.html
-        .. _Large Datasets: https://chainladder-python.readthedocs.io/en/latest/tutorials/large-datasets.html
-        .. _github discussions: https://github.com/casact/chainladder-python/discussions
-        .. _contributing guidelines: https://chainladder-python.readthedocs.io/en/latest/contributing.html
-        
+Download-URL: https://github.com/casact/chainladder-python/archive/v0.8.9.tar.gz
 Platform: UNKNOWN
+License-File: LICENSE
+
+.. -*- mode: rst -*-
+
+chainladder (python)
+====================
+
+|PyPI version| |Conda Version| |Build Status| |codecov io| |Documentation Status|
+
+chainladder - Property and Casualty Loss Reserving in Python
+------------------------------------------------------------
+
+This package gets inspiration from the popular `R ChainLadder package`_.
+
+This package strives to be minimalistic in needing its own API. Think in
+`pandas`_ for data manipulation and `scikit-learn`_ for model
+construction. An actuary already versed in these tools will pick up this
+package with ease. Save your mental energy for actuarial work.
+
+
+Documentation
+-------------
+
+Please visit the `Documentation`_ page for examples, how-tos, and source
+code documentation.
+
+
+Available Estimators
+--------------------
+
+``chainladder`` has an ever growing list of estimators that work seemlessly together:
+
+.. _R ChainLadder package: https://github.com/mages/ChainLadder
+.. _pandas: https://pandas.pydata.org/
+.. _scikit-learn: https://scikit-learn.org/latest/index.html
+
+.. |PyPI version| image:: https://badge.fury.io/py/chainladder.svg
+   :target: https://badge.fury.io/py/chainladder
+
+.. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/chainladder.svg
+   :target: https://anaconda.org/conda-forge/chainladder
+
+.. |Build Status| image:: https://github.com/casact/chainladder-python/workflows/Unit%20Tests/badge.svg
+
+.. |Documentation Status| image:: https://readthedocs.org/projects/chainladder-python/badge/?version=latest
+   :target: http://chainladder-python.readthedocs.io/en/latest/?badge=latest
+
+.. |codecov io| image:: https://codecov.io/github/casact/chainladder-python/coverage.svg?branch=latest
+   :target: https://codecov.io/github/casact/chainladder-python?branch=latest
+
+
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| Loss                         | Tails Factors    | IBNR Models             | Adjustments           | Workflow              |
+| Development                  |                  |                         |                       |                       |
++==============================+==================+=========================+=======================+=======================+
+| `Development`_               | `TailCurve`_     | `Chainladder`_          | `BootstrapODPSample`_ | `VotingChainladder`_  |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `DevelopmentConstant`_       | `TailConstant`_  | `MackChainladder`_      | `BerquistSherman`_    |  `Pipeline`_          |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `MunichAdjustment`_          | `TailBondy`_     | `BornhuettterFerguson`_ | `ParallelogramOLF`_   | `GridSearch`_         |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `ClarkLDF`_                  | `TailClark`_     | `Benktander`_           | `Trend`_              |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `IncrementalAdditive`_       |                  | `CapeCod`_              |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `CaseOutstanding`_           |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `TweedieGLM`_                |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `DevelopmentML`_             |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `BarnettZehnwirth`_          |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+
+
+.. _Development: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#development
+.. _TailCurve: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailcurve
+.. _Chainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#chainladder
+.. _BootstrapODPSample: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#bootstrapodpsample
+.. _DevelopmentConstant: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentconstant
+.. _TailConstant: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailconstant
+.. _MackChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#mackchainladder
+.. _BerquistSherman: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#berquistsherman
+.. _MunichAdjustment: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#munichadjustment
+.. _TailBondy: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailbondy
+.. _BornhuettterFerguson: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#bornhuetterferguson
+.. _Pipeline: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#pipeline
+.. _ClarkLDF: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#clarkldf
+.. _TailClark: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailclark
+.. _Benktander: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#benktander
+.. _GridSearch: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#gridsearch
+.. _IncrementalAdditive: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#incrementaladditive
+.. _CapeCod: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#capecod
+.. _ParallelogramOLF: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#parallelogramolf
+.. _VotingChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#votingchainladder
+.. _Trend: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#trend
+.. _CaseOutstanding: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#caseoutstanding
+.. _TweedieGLM: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#tweedieglm
+.. _DevelopmentML: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentml
+.. _BarnettZehnwirth: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#barnettzehnwirth
+.. _Documentation: https://chainladder-python.readthedocs.io/en/latest/
+
+Getting Started Tutorials
+-------------------------
+
+Tutorial notebooks are available for download `here`_.
+
+* `Working with Triangles`_
+* `Selecting Development Patterns`_
+* `Extending Development Patterns with Tails`_
+* `Applying Deterministic Methods`_
+* `Applying Stochastic Methods`_
+* `Large Datasets`_
+
+Installation
+------------
+
+To install using pip: ``pip install chainladder``
+
+To instal using conda: ``conda install -c conda-forge chainladder``
+
+Alternatively for pre-release functionality, install directly from github:
+``pip install git+https://github.com/casact/chainladder-python/``
+
+Note: This package requires Python>=3.5 pandas 0.23.0 and later,
+sparse 0.9 and later, scikit-learn 0.23.0 and later.
+
+Questions or Ideas?
+--------------------
+
+Join in on the `github discussions`_.  Your question is more likely to get answered
+here than on Stack Overflow.  We're always happy to answer any usage
+questions or hear ideas on how to make ``chainladder`` better.
+
+
+Want to contribute?
+-------------------
+
+Check out our `contributing guidelines`_.
+
+.. _here: https://github.com/casact/chainladder-python/tree/latest/docs/tutorials
+.. _Working with Triangles: https://chainladder-python.readthedocs.io/en/latest/tutorials/triangle-tutorial.html
+.. _Selecting Development Patterns: https://chainladder-python.readthedocs.io/en/latest/tutorials/development-tutorial.html
+.. _Extending Development Patterns with Tails: https://chainladder-python.readthedocs.io/en/latest/tutorials/tail-tutorial.html
+.. _Applying Deterministic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/deterministic-tutorial.html
+.. _Applying Stochastic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/stochastic-tutorial.html
+.. _Large Datasets: https://chainladder-python.readthedocs.io/en/latest/tutorials/large-datasets.html
+.. _github discussions: https://github.com/casact/chainladder-python/discussions
+.. _contributing guidelines: https://chainladder-python.readthedocs.io/en/latest/contributing.html
+
+
```

### Comparing `chainladder-0.8.8/README.rst` & `chainladder-0.8.9/chainladder.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: chainladder
+Version: 0.8.9
+Summary: Chainladder Package - P&C Loss Reserving package 
+Home-page: https://github.com/casact/chainladder-python
+Maintainer: John Bogaardt
+Maintainer-email: jbogaardt@gmail.com
+License: MPL-2.0
+Download-URL: https://github.com/casact/chainladder-python/archive/v0.8.9.tar.gz
+Platform: UNKNOWN
+License-File: LICENSE
+
 .. -*- mode: rst -*-
 
 chainladder (python)
 ====================
 
 |PyPI version| |Conda Version| |Build Status| |codecov io| |Documentation Status|
 
@@ -26,29 +38,29 @@
 Available Estimators
 --------------------
 
 ``chainladder`` has an ever growing list of estimators that work seemlessly together:
 
 .. _R ChainLadder package: https://github.com/mages/ChainLadder
 .. _pandas: https://pandas.pydata.org/
-.. _scikit-learn: https://scikit-learn.org/stable/index.html
+.. _scikit-learn: https://scikit-learn.org/latest/index.html
 
 .. |PyPI version| image:: https://badge.fury.io/py/chainladder.svg
    :target: https://badge.fury.io/py/chainladder
 
 .. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/chainladder.svg
    :target: https://anaconda.org/conda-forge/chainladder
 
 .. |Build Status| image:: https://github.com/casact/chainladder-python/workflows/Unit%20Tests/badge.svg
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/chainladder-python/badge/?version=latest
    :target: http://chainladder-python.readthedocs.io/en/latest/?badge=latest
 
-.. |codecov io| image:: https://codecov.io/github/casact/chainladder-python/coverage.svg?branch=master
-   :target: https://codecov.io/github/casact/chainladder-python?branch=master
+.. |codecov io| image:: https://codecov.io/github/casact/chainladder-python/coverage.svg?branch=latest
+   :target: https://codecov.io/github/casact/chainladder-python?branch=latest
 
 
 +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
 | Loss                         | Tails Factors    | IBNR Models             | Adjustments           | Workflow              |
 | Development                  |                  |                         |                       |                       |
 +==============================+==================+=========================+=======================+=======================+
 | `Development`_               | `TailCurve`_     | `Chainladder`_          | `BootstrapODPSample`_ | `VotingChainladder`_  |
@@ -67,32 +79,32 @@
 +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
 | `DevelopmentML`_             |                  |                         |                       |                       |
 +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
 | `BarnettZehnwirth`_          |                  |                         |                       |                       |
 +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
 
 
-.. _Development: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#basic-development
-.. _TailCurve: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#ldf-curve-fitting
-.. _Chainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#basic-chainladder
-.. _BootstrapODPSample: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#bootstrap-sampling
-.. _DevelopmentConstant: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#external-patterns
-.. _TailConstant: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#external-data
-.. _MackChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#mack-chainladder
-.. _BerquistSherman: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#berquist-sherman
-.. _MunichAdjustment: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#munich-adjustment
-.. _TailBondy: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#the-bondy-tail
-.. _BornhuettterFerguson: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#bornhuetter-ferguson
+.. _Development: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#development
+.. _TailCurve: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailcurve
+.. _Chainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#chainladder
+.. _BootstrapODPSample: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#bootstrapodpsample
+.. _DevelopmentConstant: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentconstant
+.. _TailConstant: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailconstant
+.. _MackChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#mackchainladder
+.. _BerquistSherman: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#berquistsherman
+.. _MunichAdjustment: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#munichadjustment
+.. _TailBondy: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailbondy
+.. _BornhuettterFerguson: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#bornhuetterferguson
 .. _Pipeline: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#pipeline
-.. _ClarkLDF: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#growth-curve-fitting
-.. _TailClark: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#growth-curve-extrapolation
+.. _ClarkLDF: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#clarkldf
+.. _TailClark: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailclark
 .. _Benktander: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#benktander
 .. _GridSearch: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#gridsearch
-.. _IncrementalAdditive: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#incremental-additive
-.. _CapeCod: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#cape-cod
+.. _IncrementalAdditive: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#incrementaladditive
+.. _CapeCod: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#capecod
 .. _ParallelogramOLF: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#parallelogramolf
 .. _VotingChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#votingchainladder
 .. _Trend: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#trend
 .. _CaseOutstanding: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#caseoutstanding
 .. _TweedieGLM: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#tweedieglm
 .. _DevelopmentML: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentml
 .. _BarnettZehnwirth: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#barnettzehnwirth
@@ -132,16 +144,18 @@
 
 
 Want to contribute?
 -------------------
 
 Check out our `contributing guidelines`_.
 
-.. _here: https://github.com/casact/chainladder-python/tree/master/docs/tutorials
+.. _here: https://github.com/casact/chainladder-python/tree/latest/docs/tutorials
 .. _Working with Triangles: https://chainladder-python.readthedocs.io/en/latest/tutorials/triangle-tutorial.html
 .. _Selecting Development Patterns: https://chainladder-python.readthedocs.io/en/latest/tutorials/development-tutorial.html
 .. _Extending Development Patterns with Tails: https://chainladder-python.readthedocs.io/en/latest/tutorials/tail-tutorial.html
 .. _Applying Deterministic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/deterministic-tutorial.html
 .. _Applying Stochastic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/stochastic-tutorial.html
 .. _Large Datasets: https://chainladder-python.readthedocs.io/en/latest/tutorials/large-datasets.html
 .. _github discussions: https://github.com/casact/chainladder-python/discussions
 .. _contributing guidelines: https://chainladder-python.readthedocs.io/en/latest/contributing.html
+
+
```

### Comparing `chainladder-0.8.8/chainladder/__init__.py` & `chainladder-0.8.9/chainladder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 from chainladder.core import *  # noqa (API Import)
 from chainladder.development import *  # noqa (API Import)
 from chainladder.adjustments import *  # noqa (API Import)
 from chainladder.tails import *  # noqa (API Import)
 from chainladder.methods import *  # noqa (API Import)
 from chainladder.workflow import *  # noqa (API Import)
 
-__version__ = "0.8.8"
+__version__ = "0.8.9"
```

### Comparing `chainladder-0.8.8/chainladder/adjustments/berqsherm.py` & `chainladder-0.8.9/chainladder/adjustments/berqsherm.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/adjustments/bootstrap.py` & `chainladder-0.8.9/chainladder/adjustments/bootstrap.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/adjustments/parallelogram.py` & `chainladder-0.8.9/chainladder/adjustments/parallelogram.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/adjustments/tests/test_berqsherm.py` & `chainladder-0.8.9/chainladder/adjustments/tests/test_berqsherm.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/adjustments/tests/test_parallelogram.py` & `chainladder-0.8.9/chainladder/adjustments/tests/test_parallelogram.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/adjustments/tests/test_trend.py` & `chainladder-0.8.9/chainladder/adjustments/tests/test_trend.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/adjustments/trend.py` & `chainladder-0.8.9/chainladder/adjustments/trend.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/base.py` & `chainladder-0.8.9/chainladder/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,21 +211,27 @@
         freq = "M" if target.nunique() == 1 else TriangleBase._get_grain(target)
         return target.dt.to_period(freq).dt.to_timestamp(how={1: "e", 0: "s"}[period_end])
 
     @staticmethod
     def _development_lag(origin, development):
         """ For tabular format, this will convert the origin/development
             difference to a development lag """
-        return ((development - origin) / 
+        return ((development - origin) /
                 np.timedelta64(1, 'M')).round(0).astype(int)
-    
+
     @staticmethod
     def _get_grain(array):
-        return {1: "Y", 2: "S", 4: "Q"}.get(
-            len(set(pd.Series(array.unique()).dt.month)), "M")
+        u = pd.Series(array).dt.month.sort_values().diff().dropna().unique()
+        u = u[u>0]
+        if len(u) > 1:
+            return 'M'
+        elif len(u) == 0:
+            return 'Y'
+        else:
+            return {6: "2Q", 3: "Q"}.get(u[0], "M")
 
     @staticmethod
     def _cartesian_product(*arrays):
         """A fast implementation of cartesian product, used for filling in gaps
         in triangles (if any)"""
         arr = np.empty(
             [len(a) for a in arrays] + [len(arrays)],
```

### Comparing `chainladder-0.8.8/chainladder/core/common.py` & `chainladder-0.8.9/chainladder/core/common.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/correlation.py` & `chainladder-0.8.9/chainladder/core/correlation.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/display.py` & `chainladder-0.8.9/chainladder/core/display.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/dunders.py` & `chainladder-0.8.9/chainladder/core/dunders.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,14 +128,19 @@
         return x, y
 
     def _prep_origin_development(self, obj, other):
         xp = obj.get_array_module()
         is_broadcastable = all(
             (m == n) or (m == 1) or (n == 1)
             for m, n in zip(obj.shape[-2:][::-1], other.shape[-2:][::-1]))
+        if (len(obj.odims), len(obj.ddims)) == (len(other.odims), len(other.ddims)):
+            if np.all(obj.ddims != other.ddims) and len(obj.ddims) > 1:
+                is_broadcastable = False
+            if np.all(obj.odims != other.odims) and len(obj.odims) > 1:
+                is_broadcastable = False
         if len(other.odims) == 1 and len(obj.odims) > 1:
             other.odims = obj.odims
         elif len(obj.odims) == 1 and len(other.odims) > 1:
             obj.odims = other.odims
         if len(other.ddims) == 1 and len(obj.ddims) > 1:
             other.ddims = obj.ddims
         elif len(obj.ddims) == 1 and len(other.ddims) > 1:
```

### Comparing `chainladder-0.8.8/chainladder/core/io.py` & `chainladder-0.8.9/chainladder/core/io.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/pandas.py` & `chainladder-0.8.9/chainladder/core/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
             or columns (1 or ‘columns’).
 
         Returns
         -------
         Triangle
 
         """
+        labels = [labels] if type(labels) is str else list(labels)
         if axis == 1:
             return self[[item for item in self.columns if item not in labels]]
         else:
             raise NotImplementedError("drop only inpemented for column axis")
 
     @property
     def T(self):
@@ -376,14 +377,15 @@
                 obj.kdims = index.values
         if self.axis == 1:
             obj.vdims = pd.DataFrame(self.groups.dtypes.index).values[:, 0]
         if self.axis == 2:
             odims = self.obj._to_datetime(
                 pd.Series(self.groups.indices.keys()).to_frame(), [0])
             obj.origin_grain = self.obj._get_grain(odims)
+            obj.origin_grain = 'S' if obj.origin_grain == '2Q' else obj.origin_grain
             obj.odims = odims.values
         obj._set_slicers()
         if auto_sparse:
             obj = obj._auto_sparse()
         return obj
 
     set_method(cls, agg_func, k)
```

### Comparing `chainladder-0.8.8/chainladder/core/slice.py` & `chainladder-0.8.9/chainladder/core/slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,14 @@
             obj.index = idx
         return obj.values[0, 0, 0, 0]
 
     def __setitem__(self, key, values):
         key = self._check_index(key)
         if self.obj.array_backend == 'sparse':
             key = (key[0][0], key[1][0], key[2][0], key[3][0])
-            print(key)
             self._sparse_setitem(key, values)
         else:
             if isinstance(values, TriangleSlicer):
                 values = values.values
             key = tuple(
                 [slice(item, item + 1) if type(item) is int else item for item in key]
             )
```

### Comparing `chainladder-0.8.8/chainladder/core/tests/test_arithmetic.py` & `chainladder-0.8.9/chainladder/core/tests/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/tests/test_correlation.py` & `chainladder-0.8.9/chainladder/core/tests/test_correlation.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/tests/test_grain.py` & `chainladder-0.8.9/chainladder/core/tests/test_grain.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/tests/test_slicing.py` & `chainladder-0.8.9/chainladder/core/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/core/tests/test_triangle.py` & `chainladder-0.8.9/chainladder/core/tests/test_triangle.py`

 * *Files 10% similar despite different names*

```diff
@@ -352,7 +352,26 @@
     assert a.mean().mean() == b.mean().mean()
 
 def test_inplace(raa):
     t = raa.copy()
     t.dev_to_val(inplace=True)
     t.val_to_dev(inplace=True)
     t.grain('OYDY', inplace=True)
+
+def test_malformed_init():
+    assert cl.Triangle(
+        data=pd.DataFrame({
+            'Accident Date': ['2020-07-23', '2019-07-23', '2018-07-23', '2016-07-23', '2020-08-23', '2019-09-23', '2018-10-23'],
+            'Valuation Date': ['2021-01-01', '2021-01-01', '2021-01-01', '2021-01-01', '2021-01-01', '2021-01-01', '2021-01-01'],
+            'Loss': [10000, 10000, 10000, 10000, 0, 0, 0]}),
+        origin='Accident Date', development='Valuation Date', columns='Loss'
+    ).origin_grain == 'M'
+
+def test_sparse_reassignment_no_mutate(prism):
+    x = prism['Paid'].incr_to_cum()
+    x["Capped 100k Paid"] = cl.minimum(x["Paid"], 100000)
+    x["Excess 100k Paid"] = x["Paid"] - x["Capped 100k Paid"]
+    a = x["Excess 100k Paid"].sum().grain("OYDY")
+    x["Capped 100k Paid"] = cl.minimum(x["Paid"], 100000)
+    x["Excess 100k Paid"] = x["Paid"] - x["Capped 100k Paid"]
+    b = x["Excess 100k Paid"].sum().grain("OYDY")
+    assert a == b
```

### Comparing `chainladder-0.8.8/chainladder/core/triangle.py` & `chainladder-0.8.9/chainladder/core/triangle.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
             return
         index, columns, origin, development = self._input_validation(
             data, index, columns, origin, development)
         data, ult = self._split_ult(data, index, columns, origin, development)
         origin_date = self._to_datetime(
             data, origin, format=origin_format).rename('__origin__')
         self.origin_grain = self._get_grain(origin_date)
+        self.origin_grain = 'S' if self.origin_grain == '2Q' else self.origin_grain
         development_date = self._set_development(
             data, development, development_format, origin_date)
         self.development_grain = (
             self._get_grain(development_date) if development_date.nunique() != 1
             else self.origin_grain)
         data_agg = self._aggregate_data(
             data, origin_date, development_date, index, columns)
```

### Comparing `chainladder-0.8.8/chainladder/development/__init__.py` & `chainladder-0.8.9/chainladder/development/__init__.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/barnzehn.py` & `chainladder-0.8.9/chainladder/development/barnzehn.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/base.py` & `chainladder-0.8.9/chainladder/development/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from chainladder.core.io import EstimatorIO
 from chainladder.core.common import Common
 
 
 class DevelopmentBase(BaseEstimator, TransformerMixin, EstimatorIO, Common):
     def _set_fit_groups(self, X):
         """ Used for assigning group_index in fit """
+        backend = 'numpy' if X.array_backend in ['sparse', 'numpy'] else 'cupy'
         if self.groupby is None:
-            return X
+            return X.set_backend(backend)
         if callable(self.groupby) or type(self.groupby) in [list, str, pd.Series]:
-            return X.groupby(self.groupby).sum()
+            return X.groupby(self.groupby).sum().set_backend(backend)
         else:
             raise ValueError("Cannot determine groupings.")
 
     def _set_transform_groups(self, X):
         """ Used for assigning group_index in transform """
         if self.groupby is None:
             return X.index
```

### Comparing `chainladder-0.8.8/chainladder/development/clark.py` & `chainladder-0.8.9/chainladder/development/clark.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/constant.py` & `chainladder-0.8.9/chainladder/development/constant.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/development.py` & `chainladder-0.8.9/chainladder/development/development.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/glm.py` & `chainladder-0.8.9/chainladder/development/glm.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/incremental.py` & `chainladder-0.8.9/chainladder/development/incremental.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/learning.py` & `chainladder-0.8.9/chainladder/development/learning.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/munich.py` & `chainladder-0.8.9/chainladder/development/munich.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/development/outstanding.py` & `chainladder-0.8.9/chainladder/development/outstanding.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/base.py` & `chainladder-0.8.9/chainladder/methods/base.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/benktander.py` & `chainladder-0.8.9/chainladder/methods/benktander.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/bornferg.py` & `chainladder-0.8.9/chainladder/methods/bornferg.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/capecod.py` & `chainladder-0.8.9/chainladder/methods/capecod.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/chainladder.py` & `chainladder-0.8.9/chainladder/methods/chainladder.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/mack.py` & `chainladder-0.8.9/chainladder/methods/mack.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/tests/test_benktander.py` & `chainladder-0.8.9/chainladder/methods/tests/test_benktander.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/tests/test_capecod.py` & `chainladder-0.8.9/chainladder/methods/tests/test_capecod.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/methods/tests/test_mack.py` & `chainladder-0.8.9/chainladder/methods/tests/test_mack.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,7 +146,14 @@
     r("Paid[seq(1,45,4),] <- qpaid")
     out = r("M <- MackChainLadder(Paid)")
     tri = cl.load_sample("quarterly")["paid"]
     xp = tri.get_array_module()
     assert round(float(xp.array(out.rx("Mack.S.E")[0])[-1, -1]), 2) == round(
         float(cl.MackChainladder().fit(tri).summary_.to_frame().iloc[-1, -1]), 2
     )
+
+def test_mack_malformed():
+    a  = cl.load_sample('raa')
+    b = a.iloc[:, :, :-1]
+    x = cl.MackChainladder().fit(a) 
+    y = cl.MackChainladder().fit(b)
+    assert x.process_risk_.iloc[:,:,:-1] == y.process_risk_
```

### Comparing `chainladder-0.8.8/chainladder/methods/tests/test_predict.py` & `chainladder-0.8.9/chainladder/methods/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/tails/base.py` & `chainladder-0.8.9/chainladder/tails/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,16 @@
         to development objects with an additional set of tail statistics"""
 
     def fit(self, X, y=None, sample_weight=None):
         obj = X.copy()
         if "ldf_" not in obj:
             obj = Development().fit_transform(obj)
         xp = obj.ldf_.get_array_module()
-        self._ave_period = {"Y": (1, 12), "Q": (4, 3), "M": (12, 1)}[
+        m = int(self.projection_period / 12)
+        self._ave_period = {"Y": (1 * m, 12), "Q": (4 * m, 3), "M": (12 * m, 1)}[
             obj.development_grain
         ]
         t_ddims = [
             (item + 1) * self._ave_period[1] + obj.ldf_.ddims[-1]
             for item in range(self._ave_period[0]+1)
         ]
         ddims = np.concatenate((obj.ldf_.ddims, t_ddims), 0,)
```

### Comparing `chainladder-0.8.8/chainladder/tails/bondy.py` & `chainladder-0.8.9/chainladder/tails/bondy.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     .. versionadded:: 0.6.0
 
     Parameters
     ----------
     earliest_age : int
         The earliest age from which the Bondy exponent is to be calculated.
-        Defaults to earliest available in the Triangle. Any available development
+        Defaults to latest age in the Triangle. Any available development
         age can be used.
     attachment_age: int (default=None)
         The age at which to attach the fitted curve.  If None, then the latest
         age is used. Measures of variability from original ``ldf_`` are retained
         when being used in conjunction with the MackChainladder method.
 
     Attributes
@@ -36,27 +36,28 @@
         The Bondy exponent
     earliest_ldf_ : DataFrame
         The LDF associated with the ``earliest_age`` pick.
     sigma_ : Triangle
         sigma with tail factor applied.
     std_err_ : Triangle
         std_err with tail factor applied
-    earliest_ldf_ : DataFrame
-        Based on the ``earliest_age`` selection, this shows the seed ``ldf_`` used
-        in fitting the Bondy exponent.
+    projection_period : int
+        The number of months beyond the latest available development age the
+        `ldf_` and `cdf_` vectors should extend.
 
     See also
     --------
     TailCurve
 
     """
 
-    def __init__(self, earliest_age=None, attachment_age=None):
+    def __init__(self, earliest_age=None, attachment_age=None, projection_period=12):
         self.earliest_age = earliest_age
         self.attachment_age = attachment_age
+        self.projection_period = projection_period
 
     def fit(self, X, y=None, sample_weight=None):
         """Fit the model with X.
 
         Parameters
         ----------
         X : Triangle-like
@@ -76,15 +77,15 @@
             X = X.set_backend("numpy", deep=True)
         else:
             X = X.set_backend("numpy")
         xp = X.get_array_module()
         super().fit(X, y, sample_weight)
 
         if self.earliest_age is None:
-            earliest_age = X.ddims[0]
+            earliest_age = X.ddims[-2]
         else:
             earliest_age = X.ddims[
                 int(
                     self.earliest_age / ({"Y": 12, "Q": 3, "M": 1}[X.development_grain])
                 )
                 - 1
             ]
```

### Comparing `chainladder-0.8.8/chainladder/tails/clark.py` & `chainladder-0.8.9/chainladder/tails/clark.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,20 +38,25 @@
     elr_ : DataFrame
         The Expected Loss Ratio parameter. This only exists when a ``sample_weight``
         is provided to the Estimator.
     scale_ : DataFrame
         The scale parameter of the model.
     norm_resid_ : Triangle
         The "Normalized" Residuals of the model according to Clark.
+    projection_period : int
+        The number of months beyond the latest available development age the
+        `ldf_` and `cdf_` vectors should extend.
     """
 
-    def __init__(self, growth="loglogistic", truncation_age=None, attachment_age=None):
+    def __init__(self, growth="loglogistic", truncation_age=None,
+                 attachment_age=None, projection_period=12):
         self.growth = growth
         self.truncation_age = truncation_age
         self.attachment_age = attachment_age
+        self.projection_period = projection_period
 
     def fit(self, X, y=None, sample_weight=None):
         """Fit the model with X.
 
         Parameters
         ----------
         X : Triangle-like
@@ -71,38 +76,28 @@
         else:
             X = X.copy()
         xp = X.get_array_module()
         super().fit(X, y, sample_weight)
         model = ClarkLDF(growth=self.growth).fit(X, sample_weight=sample_weight)
         xp = X.get_array_module()
         age_offset = {"Y": 6.0, "Q": 1.5, "M": 0.5}[X.development_grain]
-        fitted = 1 / model.G_(
-            xp.array(
-                [
-                    self._ave_period[1] + X.ddims - age_offset
-                    for item in range(self._ave_period[0] + 2)
-                ]
-            )[0]
-        )
+        fitted = 1 / model.G_(self.ldf_.ddims - age_offset)
         fitted = xp.concatenate(
             (
-                fitted.values[..., :-1] / fitted.values[..., -1:],
+                fitted.values[..., :-1] / fitted.values[..., 1:],
                 fitted.values[..., -1:],
             ),
             -1,
         )
         fitted = xp.repeat(fitted, self.ldf_.values.shape[2], 2)
         attachment_age = self.attachment_age if self.attachment_age else X.ddims[-2]
-        self.ldf_.values = xp.concatenate(
-            (
-                self.ldf_.values[..., : sum(X.ddims <= attachment_age)],
-                fitted[..., -sum(X.ddims >= attachment_age) :],
-            ),
-            axis=-1,
-        )
+        self.ldf_.values = xp.concatenate((
+            self.ldf_.values[..., : sum(self.ldf_.ddims < attachment_age)],
+            fitted[..., -sum(self.ldf_.ddims >= attachment_age) :],),
+            axis=-1,)
         self.omega_ = model.omega_
         self.theta_ = model.theta_
         self.G_ = model.G_
         self.scale_ = model.scale_
         self._G = model._G
         self.incremental_fits_ = model.incremental_fits_
         if hasattr(model, "elr_"):
```

### Comparing `chainladder-0.8.8/chainladder/tails/constant.py` & `chainladder-0.8.9/chainladder/tails/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,17 @@
         An exponential decay constant that allows for decay over future
         development periods.  A decay rate of 0.5 sets the development portion
         of each successive LDF to 50% of the previous LDF.
     attachment_age: int (default=None)
         The age at which to attach the fitted curve.  If None, then the latest
         age is used. Measures of variability from original ``ldf_`` are retained
         when being used in conjunction with the MackChainladder method.
+    projection_period : int
+        The number of months beyond the latest available development age the
+        `ldf_` and `cdf_` vectors should extend.
 
     Attributes
     ----------
     ldf_ :
         ldf with tail applied.
     cdf_ :
         cdf with tail applied.
@@ -42,18 +45,19 @@
 
     See also
     --------
     TailCurve
 
     """
 
-    def __init__(self, tail=1.0, decay=0.5, attachment_age=None):
+    def __init__(self, tail=1.0, decay=0.5, attachment_age=None, projection_period=12):
         self.tail = tail
         self.decay = decay
         self.attachment_age = attachment_age
+        self.projection_period = projection_period
 
     def fit(self, X, y=None, sample_weight=None):
         """Fit the model with X.
 
         Parameters
         ----------
         X : Triangle-like
```

### Comparing `chainladder-0.8.8/chainladder/tails/curve.py` & `chainladder-0.8.9/chainladder/tails/curve.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 class TailCurve(TailBase):
     """Allows for extraploation of LDFs to form a tail factor.
 
     Parameters
     ----------
     curve : str ('exponential', 'inverse_power')
         The type of curve extrapolation you'd like to use
-    fit_period : tuple (start, stop)
+    fit_period : tuple (start, stop) or list(bool)
         A tuple representing the range of ldfs to use in the curve fit.
         The use of ``None`` will use the edge of the triangle.  For example,
         (48, None) will use development factors for age 48 and beyond.
+        Alternatively, passing a list of booleans [True, False, ...] will
+        allow for excluding (False) any development patterns from fitting.
     extrap_periods : int
         Then number of development periods from attachment point to extrapolate
         the fit.
     errors : str ('raise' or 'ignore')
         Whether to raise an error or ignore observations that violate the
         distribution being fit.  The most common is ldfs < 1.0 will not work
         in either the ``exponential`` or ``inverse_power`` fits.
@@ -32,14 +34,18 @@
         when being used in conjunction with the MackChainladder method.
     reg_threshold : tuple (lower, upper)
         A tuple representing the lower and upper thresholds for the ldfs to be
         considered in the log regression of the tail fitting. Default lower
         threshold set to 1.00001 to avoid distortion caused by ldfs close to 1.
         Upper threshold can be used as an alternative to the fit_period start,
         to make the selection value based rather then period based.
+    projection_period : int
+        The number of months beyond the latest available development age the
+        `ldf_` and `cdf_` vectors should extend.
+
 
     Attributes
     ----------
     ldf_ : Triangle
         ldf with tail applied.
     cdf_ : Triangle
         cdf with tail applied.
@@ -58,22 +64,24 @@
     def __init__(
         self,
         curve="exponential",
         fit_period=(None, None),
         extrap_periods=100,
         errors="ignore",
         attachment_age=None,
-        reg_threshold=(1.00001,None)
+        reg_threshold=(1.00001,None),
+        projection_period = 12
     ):
         self.curve = curve
         self.fit_period = fit_period
         self.extrap_periods = extrap_periods
         self.errors = errors
         self.attachment_age = attachment_age
         self.reg_threshold = reg_threshold
+        self.projection_period = projection_period
 
     def fit(self, X, y=None, sample_weight=None):
         """Fit the model with X.
 
         Parameters
         ----------
         X : Triangle-like
@@ -91,14 +99,16 @@
         X = X.copy()
         xp = X.get_array_module()
         if type(self.fit_period) == slice:
             warnings.warn(
                 "Slicing for fit_period is deprecated and will be removed. Please use a tuple (start_age, end_age)."
             )
             fit_period = self.fit_period
+        elif type(self.fit_period) is list:
+            fit_period = xp.array(self.fit_period)[None, None, None, :]
         else:
             grain = {"Y": 12, "Q": 3, "M": 1}[X.development_grain]
             start = (
                 None
                 if self.fit_period[0] is None
                 else int(self.fit_period[0] / grain - 1)
             )
@@ -108,41 +118,47 @@
                 else int(self.fit_period[1] / grain - 1)
             )
             fit_period = slice(start, end, None)
         super().fit(X, y, sample_weight)
         xp = self.ldf_.get_array_module()
         _y = self.ldf_.values[..., : X.shape[-1] - 1].copy()
         _w = xp.zeros(_y.shape)
-        _w[..., fit_period] = 1.0
+        if type(fit_period) is slice:
+            _w[..., fit_period] = 1.0
+        else:
+            _w = (_w + 1) * fit_period
         if self.reg_threshold[0] is None:
-            warnings.warn("Lower threshold for ldfs not set. Lower threshold will be set to 1.0 to ensure" \
-                          "valid inputs for regression.")
+            warnings.warn(
+            "Lower threshold for ldfs not set. Lower threshold will be set to 1.0 to ensure",
+            "valid inputs for regression.")
             lower_threshold = 1
         elif self.reg_threshold[0] < 1:
-            warnings.warn("Lower threshold for ldfs set too low (<1). Lower threshold will be set to 1.0 to ensure" \
-                          "valid inputs for regression.")
+            warnings.warn(
+            "Lower threshold for ldfs set too low (<1). Lower threshold will be set to 1.0 to ensure "
+            "valid inputs for regression.")
             lower_threshold = 1
         else:
             lower_threshold = self.reg_threshold[0]
         if self.reg_threshold[1] is not None:
             if self.reg_threshold[1] <= lower_threshold:
-                warnings.warn("Can't set upper threshold for ldfs below lower threshold. Upper threshold will be set to 'None'.")
+                warnings.warn(
+                "Can't set upper threshold for ldfs below lower threshold. Upper threshold will be set to 'None'.")
                 upper_threshold = None
             else:
                 upper_threshold = self.reg_threshold[1]
         else:
             upper_threshold = self.reg_threshold[1]
         if self.errors == "ignore":
             if upper_threshold is None:
                 _w[_y <= lower_threshold] = 0
                 _y[_y <= lower_threshold] = 1.01
             else:
                 _w[(_y <= lower_threshold) | (_y > upper_threshold)] = 0
                 _y[(_y <= lower_threshold) | (_y > upper_threshold)] = 1.01
-        elif self.errors == "raise" and xp.any(y < 1.0):
+        elif self.errors == "raise" and xp.any(_y < 1.0):
             raise ZeroDivisionError("Tail fit requires all LDFs to be greater than 1.0")
         _y = xp.log(_y - 1)
         n_obs = X.shape[-1] - 1
         k, v = X.shape[:2]
         _x = self._get_x(_w, _y)
         # Get LDFs
         coefs = WeightedRegression(axis=3, xp=xp).fit(_x, _y, _w)
```

### Comparing `chainladder-0.8.8/chainladder/tails/tests/test_exponential.py` & `chainladder-0.8.9/chainladder/tails/tests/test_exponential.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/__init__.py` & `chainladder-0.8.9/chainladder/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/cupy.py` & `chainladder-0.8.9/chainladder/utils/cupy.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/dask.py` & `chainladder-0.8.9/chainladder/utils/dask.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/abc.csv` & `chainladder-0.8.9/chainladder/utils/data/abc.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/auto.csv` & `chainladder-0.8.9/chainladder/utils/data/auto.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/berqsherm.csv` & `chainladder-0.8.9/chainladder/utils/data/berqsherm.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/clrd.csv` & `chainladder-0.8.9/chainladder/utils/data/clrd.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/genins.csv` & `chainladder-0.8.9/chainladder/utils/data/genins.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/liab.csv` & `chainladder-0.8.9/chainladder/utils/data/liab.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/m3ir5.csv` & `chainladder-0.8.9/chainladder/utils/data/m3ir5.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/mcl.csv` & `chainladder-0.8.9/chainladder/utils/data/mcl.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/mortgage.csv` & `chainladder-0.8.9/chainladder/utils/data/mortgage.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/mw2008.csv` & `chainladder-0.8.9/chainladder/utils/data/mw2008.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/mw2014.csv` & `chainladder-0.8.9/chainladder/utils/data/mw2014.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/prism.csv` & `chainladder-0.8.9/chainladder/utils/data/prism.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/quarterly.csv` & `chainladder-0.8.9/chainladder/utils/data/quarterly.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/raa.csv` & `chainladder-0.8.9/chainladder/utils/data/raa.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/tail_sample.csv` & `chainladder-0.8.9/chainladder/utils/data/tail_sample.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/ukmotor.csv` & `chainladder-0.8.9/chainladder/utils/data/ukmotor.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/usaa.csv` & `chainladder-0.8.9/chainladder/utils/data/usaa.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/usauto.csv` & `chainladder-0.8.9/chainladder/utils/data/usauto.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/data/xyz.csv` & `chainladder-0.8.9/chainladder/utils/data/xyz.csv`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/sparse.py` & `chainladder-0.8.9/chainladder/utils/sparse.py`

 * *Files 10% similar despite different names*

```diff
@@ -77,40 +77,17 @@
 
 
 def floor(x, *args, **kwargs):
     x.data = np.floor(x.data)
     return x
 
 
-def minimum(x1, x2):
-    if type(x2) in [int, float]:
-        out = x1.copy()
-        out.data = np.minimum(x1.data, x2)
-        return out
-    elif np.all(x1.coords == x2.coords):
-        out = x1.copy()
-        out.data = np.minimum(x1.data, x2.data)
-        return out
-    if x1.shape != x2.shape:
-        raise ValueError("Shapes are not equal")
-    return (x1 < x2) * x1 + (x1 >= x2) * x2
 
-
-def maximum(x1, x2):
-    if np.all(x1.coords == x2.coords):
-        out = x1.copy()
-        out.data = np.maximum(x1.data, x2.data)
-        return out
-    if x1.shape != x2.shape:
-        raise ValueError("Shapes are not equal")
-    return (x1 < x2) * x2 + (x1 >= x2) * x1
-
-
-sp.minimum = minimum
-sp.maximum = maximum
+sp.minimum = np.minimum
+sp.maximum = np.maximum
 sp.floor = floor
 sp.where = where
 sp.arange = arange
 sp.array = array
 sp.nan_to_num = nan_to_num
 sp.ones = ones
 sp.cumprod = cumprod
```

### Comparing `chainladder-0.8.8/chainladder/utils/templates/triangle.yaml` & `chainladder-0.8.9/chainladder/utils/templates/triangle.yaml`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/tests/test_utilities.py` & `chainladder-0.8.9/chainladder/utils/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/utility_functions.py` & `chainladder-0.8.9/chainladder/utils/utility_functions.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/utils/weighted_regression.py` & `chainladder-0.8.9/chainladder/utils/weighted_regression.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/workflow/gridsearch.py` & `chainladder-0.8.9/chainladder/workflow/gridsearch.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/workflow/tests/test_predict.py` & `chainladder-0.8.9/chainladder/workflow/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/workflow/tests/test_voting.py` & `chainladder-0.8.9/chainladder/workflow/tests/test_voting.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/workflow/tests/test_workflow.py` & `chainladder-0.8.9/chainladder/workflow/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder/workflow/voting.py` & `chainladder-0.8.9/chainladder/workflow/voting.py`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/chainladder.egg-info/PKG-INFO` & `chainladder-0.8.9/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,147 @@
-Metadata-Version: 1.2
-Name: chainladder
-Version: 0.8.8
-Summary: Chainladder Package - P&C Loss Reserving package 
-Home-page: https://github.com/casact/chainladder-python
-Maintainer: John Bogaardt
-Maintainer-email: jbogaardt@gmail.com
-License: MPL-2.0
-Download-URL: https://github.com/casact/chainladder-python/archive/v0.8.8.tar.gz
-Description: .. -*- mode: rst -*-
-        
-        chainladder (python)
-        ====================
-        
-        |PyPI version| |Conda Version| |Build Status| |codecov io| |Documentation Status|
-        
-        chainladder - Property and Casualty Loss Reserving in Python
-        ------------------------------------------------------------
-        
-        This package gets inspiration from the popular `R ChainLadder package`_.
-        
-        This package strives to be minimalistic in needing its own API. Think in
-        `pandas`_ for data manipulation and `scikit-learn`_ for model
-        construction. An actuary already versed in these tools will pick up this
-        package with ease. Save your mental energy for actuarial work.
-        
-        
-        Documentation
-        -------------
-        
-        Please visit the `Documentation`_ page for examples, how-tos, and source
-        code documentation.
-        
-        
-        Available Estimators
-        --------------------
-        
-        ``chainladder`` has an ever growing list of estimators that work seemlessly together:
-        
-        .. _R ChainLadder package: https://github.com/mages/ChainLadder
-        .. _pandas: https://pandas.pydata.org/
-        .. _scikit-learn: https://scikit-learn.org/stable/index.html
-        
-        .. |PyPI version| image:: https://badge.fury.io/py/chainladder.svg
-           :target: https://badge.fury.io/py/chainladder
-        
-        .. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/chainladder.svg
-           :target: https://anaconda.org/conda-forge/chainladder
-        
-        .. |Build Status| image:: https://github.com/casact/chainladder-python/workflows/Unit%20Tests/badge.svg
-        
-        .. |Documentation Status| image:: https://readthedocs.org/projects/chainladder-python/badge/?version=latest
-           :target: http://chainladder-python.readthedocs.io/en/latest/?badge=latest
-        
-        .. |codecov io| image:: https://codecov.io/github/casact/chainladder-python/coverage.svg?branch=master
-           :target: https://codecov.io/github/casact/chainladder-python?branch=master
-        
-        
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | Loss                         | Tails Factors    | IBNR Models             | Adjustments           | Workflow              |
-        | Development                  |                  |                         |                       |                       |
-        +==============================+==================+=========================+=======================+=======================+
-        | `Development`_               | `TailCurve`_     | `Chainladder`_          | `BootstrapODPSample`_ | `VotingChainladder`_  |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `DevelopmentConstant`_       | `TailConstant`_  | `MackChainladder`_      | `BerquistSherman`_    |  `Pipeline`_          |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `MunichAdjustment`_          | `TailBondy`_     | `BornhuettterFerguson`_ | `ParallelogramOLF`_   | `GridSearch`_         |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `ClarkLDF`_                  | `TailClark`_     | `Benktander`_           | `Trend`_              |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `IncrementalAdditive`_       |                  | `CapeCod`_              |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `CaseOutstanding`_           |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `TweedieGLM`_                |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `DevelopmentML`_             |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        | `BarnettZehnwirth`_          |                  |                         |                       |                       |
-        +------------------------------+------------------+-------------------------+-----------------------+-----------------------+
-        
-        
-        .. _Development: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#basic-development
-        .. _TailCurve: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#ldf-curve-fitting
-        .. _Chainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#basic-chainladder
-        .. _BootstrapODPSample: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#bootstrap-sampling
-        .. _DevelopmentConstant: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#external-patterns
-        .. _TailConstant: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#external-data
-        .. _MackChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#mack-chainladder
-        .. _BerquistSherman: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#berquist-sherman
-        .. _MunichAdjustment: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#munich-adjustment
-        .. _TailBondy: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#the-bondy-tail
-        .. _BornhuettterFerguson: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#bornhuetter-ferguson
-        .. _Pipeline: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#pipeline
-        .. _ClarkLDF: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#growth-curve-fitting
-        .. _TailClark: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#growth-curve-extrapolation
-        .. _Benktander: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#benktander
-        .. _GridSearch: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#gridsearch
-        .. _IncrementalAdditive: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#incremental-additive
-        .. _CapeCod: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#cape-cod
-        .. _ParallelogramOLF: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#parallelogramolf
-        .. _VotingChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#votingchainladder
-        .. _Trend: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#trend
-        .. _CaseOutstanding: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#caseoutstanding
-        .. _TweedieGLM: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#tweedieglm
-        .. _DevelopmentML: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentml
-        .. _BarnettZehnwirth: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#barnettzehnwirth
-        .. _Documentation: https://chainladder-python.readthedocs.io/en/latest/
-        
-        Getting Started Tutorials
-        -------------------------
-        
-        Tutorial notebooks are available for download `here`_.
-        
-        * `Working with Triangles`_
-        * `Selecting Development Patterns`_
-        * `Extending Development Patterns with Tails`_
-        * `Applying Deterministic Methods`_
-        * `Applying Stochastic Methods`_
-        * `Large Datasets`_
-        
-        Installation
-        ------------
-        
-        To install using pip: ``pip install chainladder``
-        
-        To instal using conda: ``conda install -c conda-forge chainladder``
-        
-        Alternatively for pre-release functionality, install directly from github:
-        ``pip install git+https://github.com/casact/chainladder-python/``
-        
-        Note: This package requires Python>=3.5 pandas 0.23.0 and later,
-        sparse 0.9 and later, scikit-learn 0.23.0 and later.
-        
-        Questions or Ideas?
-        --------------------
-        
-        Join in on the `github discussions`_.  Your question is more likely to get answered
-        here than on Stack Overflow.  We're always happy to answer any usage
-        questions or hear ideas on how to make ``chainladder`` better.
-        
-        
-        Want to contribute?
-        -------------------
-        
-        Check out our `contributing guidelines`_.
-        
-        .. _here: https://github.com/casact/chainladder-python/tree/master/docs/tutorials
-        .. _Working with Triangles: https://chainladder-python.readthedocs.io/en/latest/tutorials/triangle-tutorial.html
-        .. _Selecting Development Patterns: https://chainladder-python.readthedocs.io/en/latest/tutorials/development-tutorial.html
-        .. _Extending Development Patterns with Tails: https://chainladder-python.readthedocs.io/en/latest/tutorials/tail-tutorial.html
-        .. _Applying Deterministic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/deterministic-tutorial.html
-        .. _Applying Stochastic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/stochastic-tutorial.html
-        .. _Large Datasets: https://chainladder-python.readthedocs.io/en/latest/tutorials/large-datasets.html
-        .. _github discussions: https://github.com/casact/chainladder-python/discussions
-        .. _contributing guidelines: https://chainladder-python.readthedocs.io/en/latest/contributing.html
-        
-Platform: UNKNOWN
+.. -*- mode: rst -*-
+
+chainladder (python)
+====================
+
+|PyPI version| |Conda Version| |Build Status| |codecov io| |Documentation Status|
+
+chainladder - Property and Casualty Loss Reserving in Python
+------------------------------------------------------------
+
+This package gets inspiration from the popular `R ChainLadder package`_.
+
+This package strives to be minimalistic in needing its own API. Think in
+`pandas`_ for data manipulation and `scikit-learn`_ for model
+construction. An actuary already versed in these tools will pick up this
+package with ease. Save your mental energy for actuarial work.
+
+
+Documentation
+-------------
+
+Please visit the `Documentation`_ page for examples, how-tos, and source
+code documentation.
+
+
+Available Estimators
+--------------------
+
+``chainladder`` has an ever growing list of estimators that work seemlessly together:
+
+.. _R ChainLadder package: https://github.com/mages/ChainLadder
+.. _pandas: https://pandas.pydata.org/
+.. _scikit-learn: https://scikit-learn.org/latest/index.html
+
+.. |PyPI version| image:: https://badge.fury.io/py/chainladder.svg
+   :target: https://badge.fury.io/py/chainladder
+
+.. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/chainladder.svg
+   :target: https://anaconda.org/conda-forge/chainladder
+
+.. |Build Status| image:: https://github.com/casact/chainladder-python/workflows/Unit%20Tests/badge.svg
+
+.. |Documentation Status| image:: https://readthedocs.org/projects/chainladder-python/badge/?version=latest
+   :target: http://chainladder-python.readthedocs.io/en/latest/?badge=latest
+
+.. |codecov io| image:: https://codecov.io/github/casact/chainladder-python/coverage.svg?branch=latest
+   :target: https://codecov.io/github/casact/chainladder-python?branch=latest
+
+
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| Loss                         | Tails Factors    | IBNR Models             | Adjustments           | Workflow              |
+| Development                  |                  |                         |                       |                       |
++==============================+==================+=========================+=======================+=======================+
+| `Development`_               | `TailCurve`_     | `Chainladder`_          | `BootstrapODPSample`_ | `VotingChainladder`_  |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `DevelopmentConstant`_       | `TailConstant`_  | `MackChainladder`_      | `BerquistSherman`_    |  `Pipeline`_          |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `MunichAdjustment`_          | `TailBondy`_     | `BornhuettterFerguson`_ | `ParallelogramOLF`_   | `GridSearch`_         |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `ClarkLDF`_                  | `TailClark`_     | `Benktander`_           | `Trend`_              |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `IncrementalAdditive`_       |                  | `CapeCod`_              |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `CaseOutstanding`_           |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `TweedieGLM`_                |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `DevelopmentML`_             |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+| `BarnettZehnwirth`_          |                  |                         |                       |                       |
++------------------------------+------------------+-------------------------+-----------------------+-----------------------+
+
+
+.. _Development: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#development
+.. _TailCurve: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailcurve
+.. _Chainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#chainladder
+.. _BootstrapODPSample: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#bootstrapodpsample
+.. _DevelopmentConstant: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentconstant
+.. _TailConstant: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailconstant
+.. _MackChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#mackchainladder
+.. _BerquistSherman: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#berquistsherman
+.. _MunichAdjustment: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#munichadjustment
+.. _TailBondy: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailbondy
+.. _BornhuettterFerguson: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#bornhuetterferguson
+.. _Pipeline: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#pipeline
+.. _ClarkLDF: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#clarkldf
+.. _TailClark: https://chainladder-python.readthedocs.io/en/latest/modules/tails.html#tailclark
+.. _Benktander: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#benktander
+.. _GridSearch: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#gridsearch
+.. _IncrementalAdditive: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#incrementaladditive
+.. _CapeCod: https://chainladder-python.readthedocs.io/en/latest/modules/methods.html#capecod
+.. _ParallelogramOLF: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#parallelogramolf
+.. _VotingChainladder: https://chainladder-python.readthedocs.io/en/latest/modules/workflow.html#votingchainladder
+.. _Trend: https://chainladder-python.readthedocs.io/en/latest/modules/adjustments.html#trend
+.. _CaseOutstanding: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#caseoutstanding
+.. _TweedieGLM: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#tweedieglm
+.. _DevelopmentML: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#developmentml
+.. _BarnettZehnwirth: https://chainladder-python.readthedocs.io/en/latest/modules/development.html#barnettzehnwirth
+.. _Documentation: https://chainladder-python.readthedocs.io/en/latest/
+
+Getting Started Tutorials
+-------------------------
+
+Tutorial notebooks are available for download `here`_.
+
+* `Working with Triangles`_
+* `Selecting Development Patterns`_
+* `Extending Development Patterns with Tails`_
+* `Applying Deterministic Methods`_
+* `Applying Stochastic Methods`_
+* `Large Datasets`_
+
+Installation
+------------
+
+To install using pip: ``pip install chainladder``
+
+To instal using conda: ``conda install -c conda-forge chainladder``
+
+Alternatively for pre-release functionality, install directly from github:
+``pip install git+https://github.com/casact/chainladder-python/``
+
+Note: This package requires Python>=3.5 pandas 0.23.0 and later,
+sparse 0.9 and later, scikit-learn 0.23.0 and later.
+
+Questions or Ideas?
+--------------------
+
+Join in on the `github discussions`_.  Your question is more likely to get answered
+here than on Stack Overflow.  We're always happy to answer any usage
+questions or hear ideas on how to make ``chainladder`` better.
+
+
+Want to contribute?
+-------------------
+
+Check out our `contributing guidelines`_.
+
+.. _here: https://github.com/casact/chainladder-python/tree/latest/docs/tutorials
+.. _Working with Triangles: https://chainladder-python.readthedocs.io/en/latest/tutorials/triangle-tutorial.html
+.. _Selecting Development Patterns: https://chainladder-python.readthedocs.io/en/latest/tutorials/development-tutorial.html
+.. _Extending Development Patterns with Tails: https://chainladder-python.readthedocs.io/en/latest/tutorials/tail-tutorial.html
+.. _Applying Deterministic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/deterministic-tutorial.html
+.. _Applying Stochastic Methods: https://chainladder-python.readthedocs.io/en/latest/tutorials/stochastic-tutorial.html
+.. _Large Datasets: https://chainladder-python.readthedocs.io/en/latest/tutorials/large-datasets.html
+.. _github discussions: https://github.com/casact/chainladder-python/discussions
+.. _contributing guidelines: https://chainladder-python.readthedocs.io/en/latest/contributing.html
```

### Comparing `chainladder-0.8.8/chainladder.egg-info/SOURCES.txt` & `chainladder-0.8.9/chainladder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainladder-0.8.8/setup.py` & `chainladder-0.8.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("README.rst") as f:
     long_desc = f.read()
 
 descr = "Chainladder Package - P&C Loss Reserving package "
 name = 'chainladder'
 url = 'https://github.com/casact/chainladder-python'
-version='0.8.8' # Put this in __init__.py
+version='0.8.9' # Put this in __init__.py
 
 data_path = ''
 setup(
     name=name,
     version=version,
     maintainer='John Bogaardt',
     maintainer_email='jbogaardt@gmail.com',
```

