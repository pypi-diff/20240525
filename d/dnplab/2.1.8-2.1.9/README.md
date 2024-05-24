# Comparing `tmp/dnplab-2.1.8.tar.gz` & `tmp/dnplab-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-lbcyaa71\dnplab-2.1.8.tar", last modified: Fri Oct 13 19:21:08 2023, max compression
+gzip compressed data, was "D:\Users\tkeller\Repositories\DNPLab\dist\.tmp-1kr8ptjm\dnplab-2.1.9.tar", last modified: Wed Oct 18 17:37:07 2023, max compression
```

## Comparing `dnplab-2.1.8.tar` & `dnplab-2.1.9.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.469547 dnplab-2.1.8/
--rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     2519 2023-10-13 19:21:08.469547 dnplab-2.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1556 2023-08-18 19:29:56.000000 dnplab-2.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:07.805011 dnplab-2.1.8/dnplab/
--rw-rw-rw-   0        0        0      636 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:07.829669 dnplab-2.1.8/dnplab/analysis/
--rw-rw-rw-   0        0        0      170 2023-04-28 19:23:06.000000 dnplab-2.1.8/dnplab/analysis/__init__.py
--rw-rw-rw-   0        0        0    19691 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/analysis/hydration.py
--rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.8/dnplab/analysis/relaxation_fit.py
--rw-rw-rw-   0        0        0     3743 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/analysis/simulate_enhancement_profiles.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:07.860435 dnplab-2.1.8/dnplab/config/
--rw-rw-rw-   0        0        0        0 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/config/__init__.py
--rw-rw-rw-   0        0        0     2442 2023-08-18 19:29:56.000000 dnplab-2.1.8/dnplab/config/config.py
--rw-rw-rw-   0        0        0     7919 2023-09-15 22:15:44.000000 dnplab-2.1.8/dnplab/config/dnplab.cfg
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:07.867416 dnplab-2.1.8/dnplab/constants/
--rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.8/dnplab/constants/__init__.py
--rw-rw-rw-   0        0        0      553 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/constants/constants.py
--rw-rw-rw-   0        0        0    13795 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/constants/mrProperties.py
--rw-rw-rw-   0        0        0     5150 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/constants/radicalProperties.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:07.949449 dnplab-2.1.8/dnplab/core/
--rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.8/dnplab/core/__init__.py
--rw-rw-rw-   0        0        0    41843 2023-09-15 22:15:44.000000 dnplab-2.1.8/dnplab/core/base.py
--rw-rw-rw-   0        0        0     6815 2023-06-21 13:34:20.000000 dnplab-2.1.8/dnplab/core/coord.py
--rw-rw-rw-   0        0        0    10720 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/core/data.py
--rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.8/dnplab/core/ufunc.py
--rw-rw-rw-   0        0        0     3757 2023-08-18 19:29:56.000000 dnplab-2.1.8/dnplab/core/util.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:07.963383 dnplab-2.1.8/dnplab/fitting/
--rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.8/dnplab/fitting/__init__.py
--rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.8/dnplab/fitting/general.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.165419 dnplab-2.1.8/dnplab/io/
--rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.8/dnplab/io/__init__.py
--rw-rw-rw-   0        0        0    15086 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/io/bes3t.py
--rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.8/dnplab/io/cnsi.py
--rw-rw-rw-   0        0        0     5943 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/io/delta.py
--rw-rw-rw-   0        0        0     7003 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/io/h5.py
--rw-rw-rw-   0        0        0    10819 2023-09-15 22:15:44.000000 dnplab-2.1.8/dnplab/io/load.py
--rw-rw-rw-   0        0        0     3269 2023-04-28 19:23:06.000000 dnplab-2.1.8/dnplab/io/load_csv.py
--rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.8/dnplab/io/power.py
--rw-rw-rw-   0        0        0    10272 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/io/prospa.py
--rw-rw-rw-   0        0        0      824 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/io/random.py
--rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.8/dnplab/io/save.py
--rw-rw-rw-   0        0        0     5027 2023-04-28 19:23:06.000000 dnplab-2.1.8/dnplab/io/specman.py
--rw-rw-rw-   0        0        0     2799 2023-05-31 16:23:10.000000 dnplab-2.1.8/dnplab/io/tnmr.py
--rw-rw-rw-   0        0        0    16104 2023-09-15 22:15:44.000000 dnplab-2.1.8/dnplab/io/topspin.py
--rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.8/dnplab/io/vna.py
--rw-rw-rw-   0        0        0     7831 2023-09-15 22:15:44.000000 dnplab-2.1.8/dnplab/io/vnmrj.py
--rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.8/dnplab/io/winepr.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.179398 dnplab-2.1.8/dnplab/math/
--rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.8/dnplab/math/__init__.py
--rw-rw-rw-   0        0        0     2417 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/math/lineshape.py
--rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.8/dnplab/math/relaxation.py
--rw-rw-rw-   0        0        0     4083 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/math/window.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.217518 dnplab-2.1.8/dnplab/plotting/
--rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.8/dnplab/plotting/__init__.py
--rw-rw-rw-   0        0        0     9363 2023-09-29 20:57:37.000000 dnplab-2.1.8/dnplab/plotting/general.py
--rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.8/dnplab/plotting/image.py
--rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.8/dnplab/plotting/stack_plot.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.296702 dnplab-2.1.8/dnplab/processing/
--rw-rw-rw-   0        0        0      294 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/processing/__init__.py
--rw-rw-rw-   0        0        0     2334 2023-09-29 20:57:37.000000 dnplab-2.1.8/dnplab/processing/align.py
--rw-rw-rw-   0        0        0     3129 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/processing/apodization.py
--rw-rw-rw-   0        0        0      651 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/processing/average.py
--rw-rw-rw-   0        0        0     6887 2023-09-15 22:15:44.000000 dnplab-2.1.8/dnplab/processing/conversion.py
--rw-rw-rw-   0        0        0     5181 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/processing/fft.py
--rw-rw-rw-   0        0        0    14078 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/processing/helpers.py
--rw-rw-rw-   0        0        0     3605 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/processing/integration.py
--rw-rw-rw-   0        0        0     2301 2023-06-09 16:57:10.000000 dnplab-2.1.8/dnplab/processing/offset.py
--rw-rw-rw-   0        0        0    17191 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/processing/phase.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.300720 dnplab-2.1.8/dnplab/reporting/
--rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.8/dnplab/reporting/__init__.py
--rw-rw-rw-   0        0        0       23 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/version.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.320476 dnplab-2.1.8/dnplab/widgets/
--rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.8/dnplab/widgets/__init__.py
--rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.8/dnplab/widgets/align_widget.py
--rw-rw-rw-   0        0        0     3591 2023-10-13 19:20:39.000000 dnplab-2.1.8/dnplab/widgets/phase_widget.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:07.817733 dnplab-2.1.8/dnplab.egg-info/
--rw-rw-rw-   0        0        0     2519 2023-10-13 19:21:07.000000 dnplab-2.1.8/dnplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1966 2023-10-13 19:21:07.000000 dnplab-2.1.8/dnplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-13 19:21:07.000000 dnplab-2.1.8/dnplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-10-13 19:21:07.000000 dnplab-2.1.8/dnplab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-10-13 19:21:07.000000 dnplab-2.1.8/dnplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-13 19:21:08.470547 dnplab-2.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1413 2023-06-09 16:57:10.000000 dnplab-2.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-13 19:21:08.468058 dnplab-2.1.8/unittests/
--rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.8/unittests/__init__.py
--rw-rw-rw-   0        0        0     2904 2023-09-15 22:15:44.000000 dnplab-2.1.8/unittests/test_data_class.py
--rw-rw-rw-   0        0        0     1758 2023-09-15 22:15:44.000000 dnplab-2.1.8/unittests/test_dnp_nmr.py
--rw-rw-rw-   0        0        0     5833 2023-09-29 20:57:37.000000 dnplab-2.1.8/unittests/test_dnp_tools.py
--rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.8/unittests/test_general_fit.py
--rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.8/unittests/test_hydration.py
--rw-rw-rw-   0        0        0    11768 2023-09-15 22:15:44.000000 dnplab-2.1.8/unittests/test_io.py
--rw-rw-rw-   0        0        0     1916 2023-08-18 19:29:56.000000 dnplab-2.1.8/unittests/test_load.py
--rw-rw-rw-   0        0        0    12294 2023-09-15 22:15:44.000000 dnplab-2.1.8/unittests/test_nddata_core.py
--rw-rw-rw-   0        0        0      914 2023-08-18 19:29:09.000000 dnplab-2.1.8/unittests/test_save.py
--rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.8/unittests/testing.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.600195 dnplab-2.1.9/
+-rw-rw-rw-   0        0        0     1105 2022-08-30 17:05:30.000000 dnplab-2.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     2519 2023-10-18 17:37:07.599228 dnplab-2.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1556 2023-08-18 19:29:56.000000 dnplab-2.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:06.883837 dnplab-2.1.9/dnplab/
+-rw-rw-rw-   0        0        0      636 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:06.940324 dnplab-2.1.9/dnplab/analysis/
+-rw-rw-rw-   0        0        0      170 2023-04-28 19:23:06.000000 dnplab-2.1.9/dnplab/analysis/__init__.py
+-rw-rw-rw-   0        0        0    19691 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/analysis/hydration.py
+-rw-rw-rw-   0        0        0      660 2023-03-24 14:33:33.000000 dnplab-2.1.9/dnplab/analysis/relaxation_fit.py
+-rw-rw-rw-   0        0        0     3743 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/analysis/simulate_enhancement_profiles.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:06.957612 dnplab-2.1.9/dnplab/config/
+-rw-rw-rw-   0        0        0        0 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/config/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-08-18 19:29:56.000000 dnplab-2.1.9/dnplab/config/config.py
+-rw-rw-rw-   0        0        0     7919 2023-09-15 22:15:44.000000 dnplab-2.1.9/dnplab/config/dnplab.cfg
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:06.994130 dnplab-2.1.9/dnplab/constants/
+-rw-rw-rw-   0        0        0      133 2022-08-30 17:05:30.000000 dnplab-2.1.9/dnplab/constants/__init__.py
+-rw-rw-rw-   0        0        0      553 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/constants/constants.py
+-rw-rw-rw-   0        0        0    13795 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/constants/mrProperties.py
+-rw-rw-rw-   0        0        0     5150 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/constants/radicalProperties.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.071597 dnplab-2.1.9/dnplab/core/
+-rw-rw-rw-   0        0        0      132 2022-08-30 17:05:30.000000 dnplab-2.1.9/dnplab/core/__init__.py
+-rw-rw-rw-   0        0        0    41843 2023-09-15 22:15:44.000000 dnplab-2.1.9/dnplab/core/base.py
+-rw-rw-rw-   0        0        0     6815 2023-06-21 13:34:20.000000 dnplab-2.1.9/dnplab/core/coord.py
+-rw-rw-rw-   0        0        0    10720 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/core/data.py
+-rw-rw-rw-   0        0        0     1456 2023-03-16 14:57:24.000000 dnplab-2.1.9/dnplab/core/ufunc.py
+-rw-rw-rw-   0        0        0     3757 2023-08-18 19:29:56.000000 dnplab-2.1.9/dnplab/core/util.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.083273 dnplab-2.1.9/dnplab/fitting/
+-rw-rw-rw-   0        0        0       76 2022-08-30 17:05:30.000000 dnplab-2.1.9/dnplab/fitting/__init__.py
+-rw-rw-rw-   0        0        0     2653 2023-03-16 14:57:24.000000 dnplab-2.1.9/dnplab/fitting/general.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.279578 dnplab-2.1.9/dnplab/io/
+-rw-rw-rw-   0        0        0      379 2023-03-24 14:33:33.000000 dnplab-2.1.9/dnplab/io/__init__.py
+-rw-rw-rw-   0        0        0    15086 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/io/bes3t.py
+-rw-rw-rw-   0        0        0     5180 2023-03-16 14:57:24.000000 dnplab-2.1.9/dnplab/io/cnsi.py
+-rw-rw-rw-   0        0        0     5943 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/io/delta.py
+-rw-rw-rw-   0        0        0     7003 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/io/h5.py
+-rw-rw-rw-   0        0        0    10819 2023-09-15 22:15:44.000000 dnplab-2.1.9/dnplab/io/load.py
+-rw-rw-rw-   0        0        0     3269 2023-04-28 19:23:06.000000 dnplab-2.1.9/dnplab/io/load_csv.py
+-rw-rw-rw-   0        0        0     3263 2023-03-16 14:57:24.000000 dnplab-2.1.9/dnplab/io/power.py
+-rw-rw-rw-   0        0        0    10272 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/io/prospa.py
+-rw-rw-rw-   0        0        0      824 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/io/random.py
+-rw-rw-rw-   0        0        0     1344 2023-03-24 14:33:33.000000 dnplab-2.1.9/dnplab/io/save.py
+-rw-rw-rw-   0        0        0     5027 2023-04-28 19:23:06.000000 dnplab-2.1.9/dnplab/io/specman.py
+-rw-rw-rw-   0        0        0     2799 2023-05-31 16:23:10.000000 dnplab-2.1.9/dnplab/io/tnmr.py
+-rw-rw-rw-   0        0        0    16104 2023-09-15 22:15:44.000000 dnplab-2.1.9/dnplab/io/topspin.py
+-rw-rw-rw-   0        0        0     1897 2023-03-24 14:33:33.000000 dnplab-2.1.9/dnplab/io/vna.py
+-rw-rw-rw-   0        0        0     7831 2023-09-15 22:15:44.000000 dnplab-2.1.9/dnplab/io/vnmrj.py
+-rw-rw-rw-   0        0        0     5637 2023-03-24 14:33:33.000000 dnplab-2.1.9/dnplab/io/winepr.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.298030 dnplab-2.1.9/dnplab/math/
+-rw-rw-rw-   0        0        0      136 2022-09-30 17:23:14.000000 dnplab-2.1.9/dnplab/math/__init__.py
+-rw-rw-rw-   0        0        0     2417 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/math/lineshape.py
+-rw-rw-rw-   0        0        0     3057 2023-03-16 14:57:24.000000 dnplab-2.1.9/dnplab/math/relaxation.py
+-rw-rw-rw-   0        0        0     4084 2023-10-18 17:32:46.000000 dnplab-2.1.9/dnplab/math/window.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.330358 dnplab-2.1.9/dnplab/plotting/
+-rw-rw-rw-   0        0        0      138 2022-08-30 17:05:30.000000 dnplab-2.1.9/dnplab/plotting/__init__.py
+-rw-rw-rw-   0        0        0     9363 2023-09-29 20:57:37.000000 dnplab-2.1.9/dnplab/plotting/general.py
+-rw-rw-rw-   0        0        0     1042 2023-03-16 14:57:24.000000 dnplab-2.1.9/dnplab/plotting/image.py
+-rw-rw-rw-   0        0        0     1797 2023-03-16 14:57:24.000000 dnplab-2.1.9/dnplab/plotting/stack_plot.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.434404 dnplab-2.1.9/dnplab/processing/
+-rw-rw-rw-   0        0        0      294 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/processing/__init__.py
+-rw-rw-rw-   0        0        0     2334 2023-09-29 20:57:37.000000 dnplab-2.1.9/dnplab/processing/align.py
+-rw-rw-rw-   0        0        0     3129 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/processing/apodization.py
+-rw-rw-rw-   0        0        0      651 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/processing/average.py
+-rw-rw-rw-   0        0        0     6887 2023-09-15 22:15:44.000000 dnplab-2.1.9/dnplab/processing/conversion.py
+-rw-rw-rw-   0        0        0     5181 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/processing/fft.py
+-rw-rw-rw-   0        0        0    14078 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/processing/helpers.py
+-rw-rw-rw-   0        0        0     3605 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/processing/integration.py
+-rw-rw-rw-   0        0        0     2301 2023-06-09 16:57:10.000000 dnplab-2.1.9/dnplab/processing/offset.py
+-rw-rw-rw-   0        0        0    17191 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/processing/phase.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.438425 dnplab-2.1.9/dnplab/reporting/
+-rw-rw-rw-   0        0        0       39 2022-08-30 17:05:30.000000 dnplab-2.1.9/dnplab/reporting/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-10-18 17:35:53.000000 dnplab-2.1.9/dnplab/version.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.469926 dnplab-2.1.9/dnplab/widgets/
+-rw-rw-rw-   0        0        0      151 2023-03-24 14:33:33.000000 dnplab-2.1.9/dnplab/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2023 2023-03-24 14:33:33.000000 dnplab-2.1.9/dnplab/widgets/align_widget.py
+-rw-rw-rw-   0        0        0     3591 2023-10-13 19:20:39.000000 dnplab-2.1.9/dnplab/widgets/phase_widget.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:06.894225 dnplab-2.1.9/dnplab.egg-info/
+-rw-rw-rw-   0        0        0     2519 2023-10-18 17:37:06.000000 dnplab-2.1.9/dnplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1966 2023-10-18 17:37:06.000000 dnplab-2.1.9/dnplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-18 17:37:06.000000 dnplab-2.1.9/dnplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-10-18 17:37:06.000000 dnplab-2.1.9/dnplab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-10-18 17:37:06.000000 dnplab-2.1.9/dnplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-18 17:37:07.600195 dnplab-2.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1413 2023-06-09 16:57:10.000000 dnplab-2.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-18 17:37:07.597231 dnplab-2.1.9/unittests/
+-rw-rw-rw-   0        0        0        0 2022-08-30 17:05:30.000000 dnplab-2.1.9/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2904 2023-09-15 22:15:44.000000 dnplab-2.1.9/unittests/test_data_class.py
+-rw-rw-rw-   0        0        0     1758 2023-09-15 22:15:44.000000 dnplab-2.1.9/unittests/test_dnp_nmr.py
+-rw-rw-rw-   0        0        0     5833 2023-09-29 20:57:37.000000 dnplab-2.1.9/unittests/test_dnp_tools.py
+-rw-rw-rw-   0        0        0      793 2023-03-24 14:33:33.000000 dnplab-2.1.9/unittests/test_general_fit.py
+-rw-rw-rw-   0        0        0     4590 2023-03-24 14:33:33.000000 dnplab-2.1.9/unittests/test_hydration.py
+-rw-rw-rw-   0        0        0    11768 2023-09-15 22:15:44.000000 dnplab-2.1.9/unittests/test_io.py
+-rw-rw-rw-   0        0        0     1916 2023-08-18 19:29:56.000000 dnplab-2.1.9/unittests/test_load.py
+-rw-rw-rw-   0        0        0    12294 2023-09-15 22:15:44.000000 dnplab-2.1.9/unittests/test_nddata_core.py
+-rw-rw-rw-   0        0        0      914 2023-08-18 19:29:09.000000 dnplab-2.1.9/unittests/test_save.py
+-rw-rw-rw-   0        0        0      602 2023-03-24 14:33:33.000000 dnplab-2.1.9/unittests/testing.py
```

### Comparing `dnplab-2.1.8/LICENSE.txt` & `dnplab-2.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/PKG-INFO` & `dnplab-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.8
+Version: 2.1.9
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.8/README.md` & `dnplab-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/__init__.py` & `dnplab-2.1.9/dnplab/__init__.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/analysis/hydration.py` & `dnplab-2.1.9/dnplab/analysis/hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/analysis/relaxation_fit.py` & `dnplab-2.1.9/dnplab/analysis/relaxation_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/analysis/simulate_enhancement_profiles.py` & `dnplab-2.1.9/dnplab/analysis/simulate_enhancement_profiles.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/config/config.py` & `dnplab-2.1.9/dnplab/config/config.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/config/dnplab.cfg` & `dnplab-2.1.9/dnplab/config/dnplab.cfg`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/constants/constants.py` & `dnplab-2.1.9/dnplab/constants/constants.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/constants/mrProperties.py` & `dnplab-2.1.9/dnplab/constants/mrProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/constants/radicalProperties.py` & `dnplab-2.1.9/dnplab/constants/radicalProperties.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/core/base.py` & `dnplab-2.1.9/dnplab/core/base.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/core/coord.py` & `dnplab-2.1.9/dnplab/core/coord.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/core/data.py` & `dnplab-2.1.9/dnplab/core/data.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/core/ufunc.py` & `dnplab-2.1.9/dnplab/core/ufunc.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/core/util.py` & `dnplab-2.1.9/dnplab/core/util.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/fitting/general.py` & `dnplab-2.1.9/dnplab/fitting/general.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/bes3t.py` & `dnplab-2.1.9/dnplab/io/bes3t.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/cnsi.py` & `dnplab-2.1.9/dnplab/io/cnsi.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/delta.py` & `dnplab-2.1.9/dnplab/io/delta.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/h5.py` & `dnplab-2.1.9/dnplab/io/h5.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/load.py` & `dnplab-2.1.9/dnplab/io/load.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/load_csv.py` & `dnplab-2.1.9/dnplab/io/load_csv.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/power.py` & `dnplab-2.1.9/dnplab/io/power.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/prospa.py` & `dnplab-2.1.9/dnplab/io/prospa.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/random.py` & `dnplab-2.1.9/dnplab/io/random.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/save.py` & `dnplab-2.1.9/dnplab/io/save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/specman.py` & `dnplab-2.1.9/dnplab/io/specman.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/tnmr.py` & `dnplab-2.1.9/dnplab/io/tnmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/topspin.py` & `dnplab-2.1.9/dnplab/io/topspin.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/vna.py` & `dnplab-2.1.9/dnplab/io/vna.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/vnmrj.py` & `dnplab-2.1.9/dnplab/io/vnmrj.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/io/winepr.py` & `dnplab-2.1.9/dnplab/io/winepr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/math/lineshape.py` & `dnplab-2.1.9/dnplab/math/lineshape.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/math/relaxation.py` & `dnplab-2.1.9/dnplab/math/relaxation.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/math/window.py` & `dnplab-2.1.9/dnplab/math/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     Returns:
         array: exponential window function
 
     .. math::
         \mathrm{exponential} =  e^{-\pi * x * lw}
     """
-    return _np.exp(_const.pi * (x - x[0]) * lw)
+    return _np.exp(-_const.pi * (x - x[0]) * lw)
 
 
 def gaussian(x, lw):
     r"""Calculate gaussian window function
 
     Args:
         x (array_like): vector of points
```

### Comparing `dnplab-2.1.8/dnplab/plotting/general.py` & `dnplab-2.1.9/dnplab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/plotting/image.py` & `dnplab-2.1.9/dnplab/plotting/image.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/plotting/stack_plot.py` & `dnplab-2.1.9/dnplab/plotting/stack_plot.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/align.py` & `dnplab-2.1.9/dnplab/processing/align.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/apodization.py` & `dnplab-2.1.9/dnplab/processing/apodization.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/average.py` & `dnplab-2.1.9/dnplab/processing/average.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/conversion.py` & `dnplab-2.1.9/dnplab/processing/conversion.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/fft.py` & `dnplab-2.1.9/dnplab/processing/fft.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/helpers.py` & `dnplab-2.1.9/dnplab/processing/helpers.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/integration.py` & `dnplab-2.1.9/dnplab/processing/integration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/offset.py` & `dnplab-2.1.9/dnplab/processing/offset.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/processing/phase.py` & `dnplab-2.1.9/dnplab/processing/phase.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/widgets/align_widget.py` & `dnplab-2.1.9/dnplab/widgets/align_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab/widgets/phase_widget.py` & `dnplab-2.1.9/dnplab/widgets/phase_widget.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/dnplab.egg-info/PKG-INFO` & `dnplab-2.1.9/dnplab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnplab
-Version: 2.1.8
+Version: 2.1.9
 Summary: DNPLab - Bringing the Power of Python to DNP-NMR Spectroscopy
 Home-page: http://dnpLab.net
 Download-URL: 
 Author: DNPLab Team
 License: MIT
 Project-URL: Documentation, http://docs.dnpLab.net
 Project-URL: Examples, http://dnplab.net/auto_examples/index.html
```

### Comparing `dnplab-2.1.8/dnplab.egg-info/SOURCES.txt` & `dnplab-2.1.9/dnplab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/setup.py` & `dnplab-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_data_class.py` & `dnplab-2.1.9/unittests/test_data_class.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_dnp_nmr.py` & `dnplab-2.1.9/unittests/test_dnp_nmr.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_dnp_tools.py` & `dnplab-2.1.9/unittests/test_dnp_tools.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_general_fit.py` & `dnplab-2.1.9/unittests/test_general_fit.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_hydration.py` & `dnplab-2.1.9/unittests/test_hydration.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_io.py` & `dnplab-2.1.9/unittests/test_io.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_load.py` & `dnplab-2.1.9/unittests/test_load.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_nddata_core.py` & `dnplab-2.1.9/unittests/test_nddata_core.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/test_save.py` & `dnplab-2.1.9/unittests/test_save.py`

 * *Files identical despite different names*

### Comparing `dnplab-2.1.8/unittests/testing.py` & `dnplab-2.1.9/unittests/testing.py`

 * *Files identical despite different names*

