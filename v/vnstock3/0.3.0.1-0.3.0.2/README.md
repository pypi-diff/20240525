# Comparing `tmp/vnstock3-0.3.0.1.tar.gz` & `tmp/vnstock3-0.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnstock3-0.3.0.1.tar", last modified: Sun May 12 00:39:59 2024, max compression
+gzip compressed data, was "vnstock3-0.3.0.2.tar", last modified: Sat May 25 03:09:40 2024, max compression
```

## Comparing `vnstock3-0.3.0.1.tar` & `vnstock3-0.3.0.2.tar`

### file list

```diff
@@ -1,71 +1,101 @@
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.779986 vnstock3-0.3.0.1/
--rw-r--r--   0 mrthinh    (501) staff       (20)     8376 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/LICENSE.md
--rw-r--r--   0 mrthinh    (501) staff       (20)    15455 2024-05-12 00:39:59.779606 vnstock3-0.3.0.1/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)     5406 2024-05-11 14:12:50.000000 vnstock3-0.3.0.1/README.md
--rw-r--r--   0 mrthinh    (501) staff       (20)     1019 2024-05-11 14:13:03.000000 vnstock3-0.3.0.1/pyproject.toml
--rw-r--r--   0 mrthinh    (501) staff       (20)       38 2024-05-12 00:39:59.780034 vnstock3-0.3.0.1/setup.cfg
--rw-r--r--   0 mrthinh    (501) staff       (20)     1231 2024-05-11 14:12:02.000000 vnstock3-0.3.0.1/setup.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.766580 vnstock3-0.3.0.1/vnstock3/
--rw-r--r--   0 mrthinh    (501) staff       (20)      104 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.767696 vnstock3-0.3.0.1/vnstock3/common/
--rw-r--r--   0 mrthinh    (501) staff       (20)      168 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/common/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.768581 vnstock3-0.3.0.1/vnstock3/common/data/
--rw-r--r--   0 mrthinh    (501) staff       (20)       28 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/common/data/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    16025 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/common/data/data_explorer.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.768975 vnstock3-0.3.0.1/vnstock3/core/
--rw-r--r--   0 mrthinh    (501) staff       (20)      110 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.769489 vnstock3-0.3.0.1/vnstock3/core/config/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/config/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)       16 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/config/auth.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      725 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/config/const.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.769790 vnstock3-0.3.0.1/vnstock3/core/converter/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/converter/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      453 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/converter/export.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.771697 vnstock3-0.3.0.1/vnstock3/core/utils/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1160 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/env.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1651 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/ext.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1056 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/help.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1487 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/launcher.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     3202 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/logger.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     5617 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/parser.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1747 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/core/utils/user_agent.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.771873 vnstock3-0.3.0.1/vnstock3/explorer/
--rw-r--r--   0 mrthinh    (501) staff       (20)       56 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/__init__.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.772420 vnstock3-0.3.0.1/vnstock3/explorer/misc/
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/misc/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1438 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/misc/exchange_rate.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2605 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/misc/gold_price.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.774368 vnstock3-0.3.0.1/vnstock3/explorer/msn/
--rw-r--r--   0 mrthinh    (501) staff       (20)       43 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/msn/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     4105 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/msn/const.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     1814 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/msn/helper.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2832 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/msn/listing.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/msn/models.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     7302 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/msn/quote.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.776617 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/
--rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)       53 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/analysis.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    14574 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/company.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     3576 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/const.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     9466 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/financial.py
--rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/listing.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      738 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/models.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     9684 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/quote.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2267 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/tcbs/trading.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.778617 vnstock3-0.3.0.1/vnstock3/explorer/vci/
--rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/__init__.py
--rw-r--r--   0 mrthinh    (501) staff       (20)       23 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/analysis.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     5722 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/company.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     2340 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/const.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    13079 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/financial.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    10679 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/listing.py
--rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/models.py
--rw-r--r--   0 mrthinh    (501) staff       (20)    11513 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/quote.py
--rw-r--r--   0 mrthinh    (501) staff       (20)     4148 2024-05-11 09:52:19.000000 vnstock3-0.3.0.1/vnstock3/explorer/vci/trading.py
-drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-12 00:39:59.779046 vnstock3-0.3.0.1/vnstock3.egg-info/
--rw-r--r--   0 mrthinh    (501) staff       (20)    15455 2024-05-12 00:39:59.000000 vnstock3-0.3.0.1/vnstock3.egg-info/PKG-INFO
--rw-r--r--   0 mrthinh    (501) staff       (20)     1687 2024-05-12 00:39:59.000000 vnstock3-0.3.0.1/vnstock3.egg-info/SOURCES.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-12 00:39:59.000000 vnstock3-0.3.0.1/vnstock3.egg-info/dependency_links.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)      146 2024-05-12 00:39:59.000000 vnstock3-0.3.0.1/vnstock3.egg-info/requires.txt
--rw-r--r--   0 mrthinh    (501) staff       (20)        9 2024-05-12 00:39:59.000000 vnstock3-0.3.0.1/vnstock3.egg-info/top_level.txt
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.963868 vnstock3-0.3.0.2/
+-rw-r--r--   0 mrthinh    (501) staff       (20)     8376 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/LICENSE.md
+-rw-r--r--   0 mrthinh    (501) staff       (20)    15714 2024-05-25 03:09:40.963513 vnstock3-0.3.0.2/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)     5665 2024-05-24 20:48:14.000000 vnstock3-0.3.0.2/README.md
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1019 2024-05-24 17:09:16.000000 vnstock3-0.3.0.2/pyproject.toml
+-rw-r--r--   0 mrthinh    (501) staff       (20)       38 2024-05-25 03:09:40.963909 vnstock3-0.3.0.2/setup.cfg
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1231 2024-05-24 17:09:06.000000 vnstock3-0.3.0.2/setup.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.952639 vnstock3-0.3.0.2/tests/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:36:22.000000 vnstock3-0.3.0.2/tests/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.953069 vnstock3-0.3.0.2/tests/common/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/common/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     7575 2024-05-25 03:08:48.000000 vnstock3-0.3.0.2/tests/common/test_data_explorer.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1783 2024-05-24 20:39:40.000000 vnstock3-0.3.0.2/tests/config.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.953694 vnstock3-0.3.0.2/tests/core/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/test_config.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/test_converter.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/core/test_utils.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.953794 vnstock3-0.3.0.2/tests/explorer/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.954126 vnstock3-0.3.0.2/tests/explorer/misc/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/misc/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/misc/test_exchange_rate.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/misc/test_gold_price.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.954320 vnstock3-0.3.0.2/tests/explorer/msn/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/msn/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/msn/test_quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.954769 vnstock3-0.3.0.2/tests/explorer/tcbs/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/test_analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/test_company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/tcbs/test_quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.955300 vnstock3-0.3.0.2/tests/explorer/vci/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/test_analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/test_company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-24 16:43:04.000000 vnstock3-0.3.0.2/tests/explorer/vci/test_quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.955428 vnstock3-0.3.0.2/vnstock3/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      104 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.956291 vnstock3-0.3.0.2/vnstock3/common/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      168 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/common/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.956522 vnstock3-0.3.0.2/vnstock3/common/data/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       28 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/common/data/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    17660 2024-05-25 02:32:16.000000 vnstock3-0.3.0.2/vnstock3/common/data/data_explorer.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.956996 vnstock3-0.3.0.2/vnstock3/core/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      110 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.957421 vnstock3-0.3.0.2/vnstock3/core/config/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/config/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)       16 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/config/auth.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      725 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/config/const.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.957651 vnstock3-0.3.0.2/vnstock3/core/converter/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/converter/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      453 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/converter/export.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.958694 vnstock3-0.3.0.2/vnstock3/core/utils/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1160 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/env.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1651 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/ext.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1056 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/help.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1487 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/launcher.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     3202 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/logger.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     5617 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/parser.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1747 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/core/utils/user_agent.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.958836 vnstock3-0.3.0.2/vnstock3/explorer/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       56 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/__init__.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.959198 vnstock3-0.3.0.2/vnstock3/explorer/misc/
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/misc/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1438 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/misc/exchange_rate.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2605 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/misc/gold_price.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.960010 vnstock3-0.3.0.2/vnstock3/explorer/msn/
+-rw-r--r--   0 mrthinh    (501) staff       (20)       43 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     4105 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/const.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     1814 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/helper.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2832 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/listing.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/models.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     7301 2024-05-24 18:33:19.000000 vnstock3-0.3.0.2/vnstock3/explorer/msn/quote.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.961357 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)       53 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    14574 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     3576 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/const.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     9466 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/financial.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)        0 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/listing.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      738 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/models.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     9684 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/quote.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2267 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/tcbs/trading.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.962720 vnstock3-0.3.0.2/vnstock3/explorer/vci/
+-rw-r--r--   0 mrthinh    (501) staff       (20)      138 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/__init__.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)       23 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/analysis.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     5722 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/company.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2340 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/const.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    13079 2024-05-25 01:53:24.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/financial.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    10702 2024-05-24 16:17:17.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/listing.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)      276 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/models.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)    11513 2024-05-16 18:32:12.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/quote.py
+-rw-r--r--   0 mrthinh    (501) staff       (20)     4147 2024-05-24 18:33:49.000000 vnstock3-0.3.0.2/vnstock3/explorer/vci/trading.py
+drwxr-xr-x   0 mrthinh    (501) staff       (20)        0 2024-05-25 03:09:40.962984 vnstock3-0.3.0.2/vnstock3.egg-info/
+-rw-r--r--   0 mrthinh    (501) staff       (20)    15714 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/PKG-INFO
+-rw-r--r--   0 mrthinh    (501) staff       (20)     2362 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/SOURCES.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)        1 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/dependency_links.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)      146 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/requires.txt
+-rw-r--r--   0 mrthinh    (501) staff       (20)       15 2024-05-25 03:09:40.000000 vnstock3-0.3.0.2/vnstock3.egg-info/top_level.txt
```

### Comparing `vnstock3-0.3.0.1/LICENSE.md` & `vnstock3-0.3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/PKG-INFO` & `vnstock3-0.3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock3
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: A comprehensive and transparent solution for Vietnamese stock market analysis.
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 License: **GIẤY PHÉP SỬ DỤNG PHẦN MỀM VNSTOCK3**
         -----------------------------------
         
@@ -136,15 +136,21 @@
 # I. 🎤 Giới thiệu
 
 `Vnstock3` là phiên bản phần mềm Vnstock thế hệ thứ 3 được giới thiệu công khai vào 10/5/2024. 
 Đây là thế hệ Vnstock với nhiều nâng cấp giá trị, chia sẻ tầm nhìn rõ ràng hơn về Vnstock với vai trò một giải pháp phân tích thị trường chứng khoán mã nguồn mở mang nhiều dấu ấn của tương lai công nghệ.
 
 Vnstock sẽ luôn là giải pháp miễn phí để bạn tiếp cận dữ liệu chứng khoán, tài chính toàn diện, miễn phí với các nhu cầu thiết yếu và làm quen với bộ giải phép Python linh hoạt. Chúc mừng bạn là một phần của sự thay đổi trong hành trình chuyển đổi số thị trường chứng khoán tại Việt Nam.
 
-# II. 📔 Tài liệu hướng dẫn
+# II. ⏱️ Cập nhật đáng chú ý
+
+- 10-05-2024: Ra mắt phiên bản Vnstock `0.3.0.1` với tên gói cài đặt `vnstock3`
+
+Chi tiết cập nhật phần mềm và phiên bản [tại đây](https://vnstocks.com/docs/tai-lieu/lich-su-phien-ban)
+
+# III. 📔 Tài liệu hướng dẫn
 
 Trước khi bắt đầu, hãy đánh dấu yêu thích để giúp dự án có thể tiếp cận tới nhiều người hơn. Cám ơn bạn!
 
 ![star_project](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/images/github_star_guide.png)
 
 Cài đặt thư viện với câu lệnh sau:
 
@@ -170,15 +176,15 @@
 ```
 Chúc các bạn thành công và có nhiều trải nghiệm thú vị với Vnstock3!
 
 <!-- [![vnstock docs - Xem Thêm](https://img.shields.io/badge/vnstock_docs-Xem_Thêm-2ea44f?style=for-the-badge&logo=Github)](https://thinh-vu.github.io/vnstock) -->
 
 <!-- [![vnstock_docs_home](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/images/vnstock_docs_home.png)](https://thinh-vu.github.io/vnstock) -->
 
-# III. 🙋‍♂️ Thông tin liên hệ
+# IV. 🙋‍♂️ Thông tin liên hệ
 
 Bạn có thể kết nối với tác giả qua các hình thức sau. Trong trường hợp cần hỗ trợ nhanh, bạn có thể chọn nhắn tin qua Messenger hoặc Linkedin, tôi sẽ phản hồi ngay lập tức nếu có thể trong hầu hết các trường hợp.
 
 <div id="badges" align="center">
   <a href="https://www.linkedin.com/in/thinh-vu">
     <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
   </a>
@@ -189,18 +195,18 @@
   </a>
   </a>
     <a href="https://github.com/thinh-vu">
     <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Github Badge"/>
   </a>
 </div>
 
-# IV. 🔑 Giấy phép sử dụng (License)
+# V. 🔑 Giấy phép sử dụng (License)
 
 `Vnstock3` được phát hành theo giấy phép tuỳ chỉnh hướng đến cá nhân, không dành cho mục đích thương mại. Quyền sử dụng được quy định cụ thể trong [giấy phép](LICENSE.md) kèm theo. Nếu bạn hoặc tổ chức bạn đang làm việc muốn sử dụng Vnstock có thể liên hệ tác giả để hiểu rõ phạm vi sử dụng và được cấp phép chính thức.
 
 Khi sử dụng Vnstock trong dự án của mình, bạn cần trích dẫn thông tin về tác giả và dự án theo hướng dẫn của Vnstock.
 
-# V. Lịch sử lượt yêu thích
+# VI. Lịch sử lượt yêu thích
 
 Bạn có thể hỗ trợ dự án bằng cách cực kỳ đơn giản là đánh dấu yêu thích để giúp dự án có thể tiếp cận tới nhiều người hơn. Dưới đây là lịch sử lượt yêu thích của dự án.
 
 [![Star History Chart](https://api.star-history.com/svg?repos=thinh-vu/vnstock&type=Date)](https://star-history.com/#thinh-vu/vnstock&Date)
```

### Comparing `vnstock3-0.3.0.1/README.md` & `vnstock3-0.3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 # I. 🎤 Giới thiệu
 
 `Vnstock3` là phiên bản phần mềm Vnstock thế hệ thứ 3 được giới thiệu công khai vào 10/5/2024. 
 Đây là thế hệ Vnstock với nhiều nâng cấp giá trị, chia sẻ tầm nhìn rõ ràng hơn về Vnstock với vai trò một giải pháp phân tích thị trường chứng khoán mã nguồn mở mang nhiều dấu ấn của tương lai công nghệ.
 
 Vnstock sẽ luôn là giải pháp miễn phí để bạn tiếp cận dữ liệu chứng khoán, tài chính toàn diện, miễn phí với các nhu cầu thiết yếu và làm quen với bộ giải phép Python linh hoạt. Chúc mừng bạn là một phần của sự thay đổi trong hành trình chuyển đổi số thị trường chứng khoán tại Việt Nam.
 
-# II. 📔 Tài liệu hướng dẫn
+# II. ⏱️ Cập nhật đáng chú ý
+
+- 10-05-2024: Ra mắt phiên bản Vnstock `0.3.0.1` với tên gói cài đặt `vnstock3`
+
+Chi tiết cập nhật phần mềm và phiên bản [tại đây](https://vnstocks.com/docs/tai-lieu/lich-su-phien-ban)
+
+# III. 📔 Tài liệu hướng dẫn
 
 Trước khi bắt đầu, hãy đánh dấu yêu thích để giúp dự án có thể tiếp cận tới nhiều người hơn. Cám ơn bạn!
 
 ![star_project](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/images/github_star_guide.png)
 
 Cài đặt thư viện với câu lệnh sau:
 
@@ -53,15 +59,15 @@
 ```
 Chúc các bạn thành công và có nhiều trải nghiệm thú vị với Vnstock3!
 
 <!-- [![vnstock docs - Xem Thêm](https://img.shields.io/badge/vnstock_docs-Xem_Thêm-2ea44f?style=for-the-badge&logo=Github)](https://thinh-vu.github.io/vnstock) -->
 
 <!-- [![vnstock_docs_home](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/images/vnstock_docs_home.png)](https://thinh-vu.github.io/vnstock) -->
 
-# III. 🙋‍♂️ Thông tin liên hệ
+# IV. 🙋‍♂️ Thông tin liên hệ
 
 Bạn có thể kết nối với tác giả qua các hình thức sau. Trong trường hợp cần hỗ trợ nhanh, bạn có thể chọn nhắn tin qua Messenger hoặc Linkedin, tôi sẽ phản hồi ngay lập tức nếu có thể trong hầu hết các trường hợp.
 
 <div id="badges" align="center">
   <a href="https://www.linkedin.com/in/thinh-vu">
     <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
   </a>
@@ -72,18 +78,18 @@
   </a>
   </a>
     <a href="https://github.com/thinh-vu">
     <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Github Badge"/>
   </a>
 </div>
 
-# IV. 🔑 Giấy phép sử dụng (License)
+# V. 🔑 Giấy phép sử dụng (License)
 
 `Vnstock3` được phát hành theo giấy phép tuỳ chỉnh hướng đến cá nhân, không dành cho mục đích thương mại. Quyền sử dụng được quy định cụ thể trong [giấy phép](LICENSE.md) kèm theo. Nếu bạn hoặc tổ chức bạn đang làm việc muốn sử dụng Vnstock có thể liên hệ tác giả để hiểu rõ phạm vi sử dụng và được cấp phép chính thức.
 
 Khi sử dụng Vnstock trong dự án của mình, bạn cần trích dẫn thông tin về tác giả và dự án theo hướng dẫn của Vnstock.
 
-# V. Lịch sử lượt yêu thích
+# VI. Lịch sử lượt yêu thích
 
 Bạn có thể hỗ trợ dự án bằng cách cực kỳ đơn giản là đánh dấu yêu thích để giúp dự án có thể tiếp cận tới nhiều người hơn. Dưới đây là lịch sử lượt yêu thích của dự án.
 
 [![Star History Chart](https://api.star-history.com/svg?repos=thinh-vu/vnstock&type=Date)](https://star-history.com/#thinh-vu/vnstock&Date)
```

#### html2text {}

```diff
@@ -7,44 +7,47 @@
 rÃµ rÃ ng hÆ¡n vá» Vnstock vá»i vai trÃ² má»t giáº£i phÃ¡p phÃ¢n tÃ­ch thá»
 trÆ°á»ng chá»©ng khoÃ¡n mÃ£ nguá»n má» mang nhiá»u dáº¥u áº¥n cá»§a tÆ°Æ¡ng
 lai cÃ´ng nghá». Vnstock sáº½ luÃ´n lÃ  giáº£i phÃ¡p miá»n phÃ­ Äá» báº¡n
 tiáº¿p cáº­n dá»¯ liá»u chá»©ng khoÃ¡n, tÃ i chÃ­nh toÃ n diá»n, miá»n phÃ­
 vá»i cÃ¡c nhu cáº§u thiáº¿t yáº¿u vÃ  lÃ m quen vá»i bá» giáº£i phÃ©p Python
 linh hoáº¡t. ChÃºc má»«ng báº¡n lÃ  má»t pháº§n cá»§a sá»± thay Äá»i trong
 hÃ nh trÃ¬nh chuyá»n Äá»i sá» thá» trÆ°á»ng chá»©ng khoÃ¡n táº¡i Viá»t
-Nam. # II. ð TÃ i liá»u hÆ°á»ng dáº«n TrÆ°á»c khi báº¯t Äáº§u, hÃ£y
-ÄÃ¡nh dáº¥u yÃªu thÃ­ch Äá» giÃºp dá»± Ã¡n cÃ³ thá» tiáº¿p cáº­n tá»i
-nhiá»u ngÆ°á»i hÆ¡n. CÃ¡m Æ¡n báº¡n! ![star_project](https://
-raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/images/
-github_star_guide.png) CÃ i Äáº·t thÆ° viá»n vá»i cÃ¢u lá»nh sau: ``` pip
-install -U vnstock3 ``` Äá» hiá»u rÃµ hÆ¡n vá» vnstock vÃ  hÆ°á»ng dáº«n
-sá»­ dá»¥ng toÃ n diá»n, báº¡n cÃ³ thá» truy cáº­p [vnstock.site](https://
-vnstock.site). Báº¡n cáº§n má» Vnstock3 tá»« Terminal hoáº·c Jupyter Notebook
-vÃ  náº¡p thÆ° viá»n láº§n Äáº§u cÃ i Äáº·t Äá» cháº¥p nháº­n Äiá»u
-khoáº£n & Äiá»u kiá»n sá»­ dá»¥ng trÆ°á»c khi tiáº¿p tá»¥c. ``` from
-vnstock3 import Vnstock ``` ThÃ´ng bÃ¡o hiá»n ra, báº¡n chá» cáº§n áº¥n phÃ­m
-Enter Äá» Äá»ng Ã½. Lá»i nháº¯c nÃ y chá» há»i 1 láº§n duy nháº¥t khi
-báº¡n cÃ i Äáº·t trÃªn thiáº¿t bá» láº§n Äáº§u tiÃªn. Äá» bá» qua lá»i
-nháº¯c vÃ  tá»± Äá»ng cháº¥p nháº­n Äiá»u khoáº£n, báº¡n cÃ³ thá» chÃ¨n
-Äoáº¡n code sau vÃ o Äáº§u dá»± Ã¡n cá»§a mÃ¬nh khi thá»±c thi. ``` import os
-if "ACCEPT_TC" not in os.environ: os.environ["ACCEPT_TC"] = "tÃ´i Äá»ng Ã½"
-``` ChÃºc cÃ¡c báº¡n thÃ nh cÃ´ng vÃ  cÃ³ nhiá»u tráº£i nghiá»m thÃº vá»
-vá»i Vnstock3! # III. ðââï¸ ThÃ´ng tin liÃªn há» Báº¡n cÃ³ thá»
-káº¿t ná»i vá»i tÃ¡c giáº£ qua cÃ¡c hÃ¬nh thá»©c sau. Trong trÆ°á»ng há»£p
-cáº§n há» trá»£ nhanh, báº¡n cÃ³ thá» chá»n nháº¯n tin qua Messenger hoáº·c
-Linkedin, tÃ´i sáº½ pháº£n há»i ngay láº­p tá»©c náº¿u cÃ³ thá» trong háº§u
-háº¿t cÃ¡c trÆ°á»ng há»£p.
+Nam. # II. â±ï¸ Cáº­p nháº­t ÄÃ¡ng chÃº Ã½ - 10-05-2024: Ra máº¯t phiÃªn
+báº£n Vnstock `0.3.0.1` vá»i tÃªn gÃ³i cÃ i Äáº·t `vnstock3` Chi tiáº¿t cáº­p
+nháº­t pháº§n má»m vÃ  phiÃªn báº£n [táº¡i ÄÃ¢y](https://vnstocks.com/docs/
+tai-lieu/lich-su-phien-ban) # III. ð TÃ i liá»u hÆ°á»ng dáº«n TrÆ°á»c khi
+báº¯t Äáº§u, hÃ£y ÄÃ¡nh dáº¥u yÃªu thÃ­ch Äá» giÃºp dá»± Ã¡n cÃ³ thá»
+tiáº¿p cáº­n tá»i nhiá»u ngÆ°á»i hÆ¡n. CÃ¡m Æ¡n báº¡n! ![star_project]
+(https://raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/
+images/github_star_guide.png) CÃ i Äáº·t thÆ° viá»n vá»i cÃ¢u lá»nh sau:
+``` pip install -U vnstock3 ``` Äá» hiá»u rÃµ hÆ¡n vá» vnstock vÃ  hÆ°á»ng
+dáº«n sá»­ dá»¥ng toÃ n diá»n, báº¡n cÃ³ thá» truy cáº­p [vnstock.site]
+(https://vnstock.site). Báº¡n cáº§n má» Vnstock3 tá»« Terminal hoáº·c Jupyter
+Notebook vÃ  náº¡p thÆ° viá»n láº§n Äáº§u cÃ i Äáº·t Äá» cháº¥p nháº­n
+Äiá»u khoáº£n & Äiá»u kiá»n sá»­ dá»¥ng trÆ°á»c khi tiáº¿p tá»¥c. ```
+from vnstock3 import Vnstock ``` ThÃ´ng bÃ¡o hiá»n ra, báº¡n chá» cáº§n áº¥n
+phÃ­m Enter Äá» Äá»ng Ã½. Lá»i nháº¯c nÃ y chá» há»i 1 láº§n duy nháº¥t
+khi báº¡n cÃ i Äáº·t trÃªn thiáº¿t bá» láº§n Äáº§u tiÃªn. Äá» bá» qua
+lá»i nháº¯c vÃ  tá»± Äá»ng cháº¥p nháº­n Äiá»u khoáº£n, báº¡n cÃ³ thá»
+chÃ¨n Äoáº¡n code sau vÃ o Äáº§u dá»± Ã¡n cá»§a mÃ¬nh khi thá»±c thi. ```
+import os if "ACCEPT_TC" not in os.environ: os.environ["ACCEPT_TC"] = "tÃ´i
+Äá»ng Ã½" ``` ChÃºc cÃ¡c báº¡n thÃ nh cÃ´ng vÃ  cÃ³ nhiá»u tráº£i nghiá»m
+thÃº vá» vá»i Vnstock3! # IV. ðââï¸ ThÃ´ng tin liÃªn há» Báº¡n cÃ³
+thá» káº¿t ná»i vá»i tÃ¡c giáº£ qua cÃ¡c hÃ¬nh thá»©c sau. Trong trÆ°á»ng
+há»£p cáº§n há» trá»£ nhanh, báº¡n cÃ³ thá» chá»n nháº¯n tin qua Messenger
+hoáº·c Linkedin, tÃ´i sáº½ pháº£n há»i ngay láº­p tá»©c náº¿u cÃ³ thá» trong
+háº§u háº¿t cÃ¡c trÆ°á»ng há»£p.
         _[_L_i_n_k_e_d_I_n_ _B_a_d_g_e_]_[_M_e_s_s_e_n_g_e_r_ _B_a_d_g_e_]_[_Y_o_u_t_u_b_e_ _B_a_d_g_e_]_[_G_i_t_h_u_b_ _B_a_d_g_e_]
-# IV. ð Giáº¥y phÃ©p sá»­ dá»¥ng (License) `Vnstock3` ÄÆ°á»£c phÃ¡t hÃ nh
+# V. ð Giáº¥y phÃ©p sá»­ dá»¥ng (License) `Vnstock3` ÄÆ°á»£c phÃ¡t hÃ nh
 theo giáº¥y phÃ©p tuá»³ chá»nh hÆ°á»ng Äáº¿n cÃ¡ nhÃ¢n, khÃ´ng dÃ nh cho
 má»¥c ÄÃ­ch thÆ°Æ¡ng máº¡i. Quyá»n sá»­ dá»¥ng ÄÆ°á»£c quy Äá»nh cá»¥
 thá» trong [giáº¥y phÃ©p](LICENSE.md) kÃ¨m theo. Náº¿u báº¡n hoáº·c tá»
 chá»©c báº¡n Äang lÃ m viá»c muá»n sá»­ dá»¥ng Vnstock cÃ³ thá» liÃªn há»
 tÃ¡c giáº£ Äá» hiá»u rÃµ pháº¡m vi sá»­ dá»¥ng vÃ  ÄÆ°á»£c cáº¥p phÃ©p
 chÃ­nh thá»©c. Khi sá»­ dá»¥ng Vnstock trong dá»± Ã¡n cá»§a mÃ¬nh, báº¡n cáº§n
 trÃ­ch dáº«n thÃ´ng tin vá» tÃ¡c giáº£ vÃ  dá»± Ã¡n theo hÆ°á»ng dáº«n cá»§a
-Vnstock. # V. Lá»ch sá»­ lÆ°á»£t yÃªu thÃ­ch Báº¡n cÃ³ thá» há» trá»£ dá»±
+Vnstock. # VI. Lá»ch sá»­ lÆ°á»£t yÃªu thÃ­ch Báº¡n cÃ³ thá» há» trá»£ dá»±
 Ã¡n báº±ng cÃ¡ch cá»±c ká»³ ÄÆ¡n giáº£n lÃ  ÄÃ¡nh dáº¥u yÃªu thÃ­ch Äá»
 giÃºp dá»± Ã¡n cÃ³ thá» tiáº¿p cáº­n tá»i nhiá»u ngÆ°á»i hÆ¡n. DÆ°á»i
 ÄÃ¢y lÃ  lá»ch sá»­ lÆ°á»£t yÃªu thÃ­ch cá»§a dá»± Ã¡n. [![Star History
 Chart](https://api.star-history.com/svg?repos=thinh-vu/vnstock&type=Date)]
 (https://star-history.com/#thinh-vu/vnstock&Date)
```

### Comparing `vnstock3-0.3.0.1/pyproject.toml` & `vnstock3-0.3.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 # Metadata Information
 [project]
 name = "vnstock3"
-version = "0.3.0.1"
+version = "0.3.0.2"
 description = "A comprehensive and transparent solution for Vietnamese stock market analysis."
 authors = [
     { name = "Thinh Vu", email = "mrthinh@live.com" },
     ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
```

### Comparing `vnstock3-0.3.0.1/setup.py` & `vnstock3-0.3.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 import subprocess
 from setuptools import setup, find_packages, Command
 from setuptools.command.install import install
 
 setup(
     name="vnstock3",
-    version="0.3.0.1",
+    version="0.3.0.2",
     description="A comprehensive and transparent solution for Vietnamese stock market analysis.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     author="Thinh Vu",
     author_email="mrthinh@live.com",
     url="https://github.com/thinh-vu/vnstock",
     classifiers=[
```

### Comparing `vnstock3-0.3.0.1/vnstock3/common/data/data_explorer.py` & `vnstock3-0.3.0.2/vnstock3/common/data/data_explorer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,110 @@
 import importlib
 from typing import Optional
 from vnstock3.core.utils.logger import get_logger
 from vnstock3.explorer.msn.const import _CURRENCY_ID_MAP, _GLOBAL_INDICES, _CRYPTO_ID_MAP
+from vnstock3.core.utils.parser import get_asset_type
 from functools import wraps
 
 logger = get_logger(__name__)
 
-# def property(func):
-#     @wraps(func)
-#     def wrapper(*args, **kwargs):
-#         try:
-#             result = func(*args, **kwargs)
-#             print(f"Completed property: {func.__name__}")
-#             return result
-#         except Exception as e:
-#             print(f"property failed: {func.__name__}, Error: {e}")
-#             raise
-#     return wrapper
-
 class Vnstock:
     """
     Class (lớp) chính quản lý các chức năng của thư viện Vnstock.
     """
+    
+    SUPPORTED_SOURCES = ["VCI", "TCBS", "MSN"]
+    msn_symbol_map = {**_CURRENCY_ID_MAP, **_GLOBAL_INDICES, **_CRYPTO_ID_MAP}
+
     def __init__(self, source:str="VCI"):
-        if source.upper() not in ["VCI", "TCBS", "VND"]:
-            raise ValueError("Hiện tại chỉ có nguồn dữ liệu từ VCI và TCBS được hỗ trợ.")
+        self.source = source.upper()
+        if self.source not in self.SUPPORTED_SOURCES:
+            raise ValueError(F"Hiện tại chỉ có nguồn dữ liệu từ {', '.join(self.SUPPORTED_SOURCES)} được hỗ trợ.")
         self.source = source.upper()
         # self.utils = Utils(self)
 
-    def stock(self, symbol: Optional[str], source: Optional[str] = "VCI"):
-        return StockComponents(symbol, source)
+    def stock(self, symbol: Optional[str]=None, source: Optional[str] = "VCI"):
+        if symbol is None:
+            self.symbol = 'VN30F1M'
+            logger.info("Mã chứng khoán không được chỉ định, chương trình mặc định sử dụng VN30F1M")
+        else:
+            self.symbol = symbol
+        return StockComponents(self.symbol, source)
     
     def fx(self, symbol: Optional[str]='EURUSD', source: Optional[str] = "MSN"):
-        return MSNComponents(symbol, source)
+        if symbol:
+            self.symbol = self.msn_symbol_map[symbol]
+        return MSNComponents(self.symbol, source)
     
     def crypto(self, symbol: Optional[str]='BTC', source: Optional[str] = "MSN"):
-        return MSNComponents(symbol, source)
+        if symbol:
+            self.symbol = self.msn_symbol_map[symbol]
+        return MSNComponents(self.symbol, source)
     
     def world_index(self, symbol: Optional[str]='DJI', source: Optional[str] = "MSN"):
-        return MSNComponents(symbol, source)
+        if symbol:
+            self.symbol = self.msn_symbol_map[symbol]
+        return MSNComponents(self.symbol, source)
 
 
 class StockComponents:
     """
     Class (lớp) quản lý các chức năng của thư viện Vnstock liên quan đến cổ phiếu.
     """
+    SUPPORTED_SOURCES = ["VCI", "TCBS", "MSN"]
+
     def __init__(self, symbol: str, source: str = "VCI"):
         self.symbol = symbol.upper()
-        if source.upper() not in ["VCI", "TCBS", "VND"]:
-            raise ValueError("Hiện tại chỉ có nguồn dữ liệu từ VCI và TCBS được hỗ trợ.")
         self.source = source.upper()
+        if self.source not in self.SUPPORTED_SOURCES:
+            raise ValueError(f"Hiện tại chỉ có nguồn dữ liệu từ {', '.join(self.SUPPORTED_SOURCES)} được hỗ trợ.")
         self._initialize_components()
 
     def _initialize_components(self):
         # Initialize each sub-component with the current symbol
         self.quote = Quote(self.symbol, self.source)
         
         if self.source not in ["VCI", "TCBS"]:
             self.listing = Listing(source='VCI')
             self.trading = Trading(self.symbol, source='VCI')
             logger.warning("Thông tin niêm yết & giao dịch sẽ được truy xuất từ VCI")
         elif self.source == "TCBS":
             self.listing = Listing(source='VCI')
             self.trading = Trading(self.symbol, source=self.source)
             self.company = Company(self.symbol, source=self.source)
-            logger.warning("Thông tin niêm yết sẽ được truy xuất từ TCBS")
+            if get_asset_type(self.symbol) == "stock":
+                self.finance = Finance(self.symbol, source=self.source)
         else:
             self.listing = Listing(source=self.source)
             self.trading = Trading(self.symbol, source=self.source)
+            if get_asset_type(self.symbol) == "stock":
+                self.finance = Finance(self.symbol, source=self.source)
+            logger.warning("Thông tin niêm yết & giao dịch sẽ được truy xuất từ TCBS")
 
     def update_symbol(self, symbol: str):
         """
         Update the symbol for all sub-components.
         """
         self.symbol = symbol.upper()
         self._initialize_components()
 
 # Các class (lớp) dưới đây sẽ được sử dụng để điều hướng nguồn dữ liệu cụ thể từ các nguồn dữ liệu khác nhau.
 class Quote:
     """
     Class (lớp) quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho dữ liệu đồ thị nến, dữ liệu trả về tuỳ thuộc vào nguồn dữ liệu sẵn có được chọn.
     """
+    SUPPORTED_SOURCES = ["VCI", "TCBS", "MSN"]
+
     def __init__(self, symbol: str, source: str = "VCI"):
         """
         Class (lớp) quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho dữ liệu đồ thị nến, dữ liệu trả về tuỳ thuộc vào nguồn dữ liệu sẵn có được chọn.
         """
         self.source = source.upper()
-        if self.source not in ["VCI", "TCBS", "VND", "MSN"]:
-            raise ValueError("Hiện tại chỉ có nguồn dữ liệu từ VCI, TCBS, VND, và MSN được hỗ trợ.")
+        if self.source not in self.SUPPORTED_SOURCES:
+            raise ValueError(f"Hiện tại chỉ có nguồn dữ liệu từ {', '.join(self.SUPPORTED_SOURCES)} được hỗ trợ.")
         self.symbol = symbol.upper()
         self.source_module = f"vnstock3.explorer.{source.lower()}"
         self.data_source = self._load_data_source()
 
     def _load_data_source(self):
         """
         Điều hướng lớp (class) nguồn dữ liệu được lựa chọn.
@@ -108,65 +121,64 @@
         """
         if self.source != 'MSN':
             if symbol:
                 self.symbol = symbol.upper()
                 self.data_source = self._load_data_source()
         else:
             self.data_source = self._load_data_source()
-
-    def history(self, symbol:Optional[str]='VN30F1M', **kwargs):
+        
+    def history(self, symbol: Optional[str] = None, **kwargs):
         """
         Truy xuất dữ liệu giá lịch sử từ nguồn dữ liệu được chọn.
         """
         if self.source == "MSN":
             symbol_map = {**_CURRENCY_ID_MAP, **_GLOBAL_INDICES, **_CRYPTO_ID_MAP}
-            if symbol is not None:
-                original_symbol = self.symbol
-                self.symbol = symbol_map[self.symbol]
+            if symbol:
+                self.symbol = symbol_map[symbol]
+                logger.info(f"Chuyển đổi mã chứng khoán {symbol} sang mã chứng khoán MSN: {self.symbol}")
                 self._update_data_source(symbol=self.symbol)
                 return self.data_source.history(**kwargs)
         else:
-            # if symbol is provided, override the symbol
-            if symbol is not None:
+            if symbol:
                 self.symbol = symbol.upper()
-            self._update_data_source(symbol)
+            self._update_data_source(self.symbol)
             return self.data_source.history(**kwargs)
+        
+        self._update_data_source(self.symbol)
+        return self.data_source.history(**kwargs)
     
-    def intraday(self, symbol:Optional[str], **kwargs):
+    def intraday(self, symbol: Optional[str] = None, **kwargs):
         """
         Truy xuất dữ liệu giao dịch trong ngày từ nguồn dữ liệu được chọn.
         """
         # if symbol is provided, override the symbol
-        if symbol is not None:
-            self.symbol = symbol.upper()
         self._update_data_source(symbol)
         return self.data_source.intraday(**kwargs)
     
-    def price_depth(self, symbol:Optional[str], **kwargs):
+    def price_depth(self, symbol: Optional[str] = None, **kwargs):
         """
         Truy xuất dữ liệu KLGD theo bước giá từ nguồn dữ liệu được chọn.
         """
-        # if symbol is provided, override the symbol
-        if symbol is not None:
-            self.symbol = symbol.upper()
         self._update_data_source(symbol)
         return self.data_source.price_depth(**kwargs)
     
 class Listing:
     """
     Class (lớp) quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho thông tin niêm yết, dữ liệu trả về tuỳ thuộc vào nguồn dữ liệu sẵn có được chọn.
     """
+    
+    SUPPORTED_SOURCES = ["VCI", "MSN"]
     def __init__(self, source: str = "VCI"):
         """
-        Initializes the DataExplorer with the specified source and symbol.
+        Khởi tạo lớp (class) với nguồn dữ liệu được chọn.
         """
-        # validate the source to only VCI are available so far
-        if source.upper() not in ["VCI", "MSN"]:
-            raise ValueError("Hiện tại chỉ có nguồn dữ liệu từ VCI được hỗ trợ.")
-        self.source_module = f"vnstock3.explorer.{source.lower()}"
+        self.source = source.upper()
+        if self.source not in self.SUPPORTED_SOURCES:
+            raise ValueError(f"Hiện tại chỉ có nguồn dữ liệu từ {', '.join(self.SUPPORTED_SOURCES)} được hỗ trợ.")
+        self.source_module = f"vnstock3.explorer.{self.source.lower()}"
         self.data_source = self._load_data_source()
 
     def _load_data_source(self):
         """
         Điều hướng lớp (class) nguồn dữ liệu được lựa chọn.
         """
         module = importlib.import_module(self.source_module)
@@ -226,39 +238,40 @@
         """
         return self.data_source.all_government_bonds(**kwargs)
     
 class Trading:
     """
     Class (lớp) quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho thông tin giao dịch.
     """
+    SUPPORTED_SOURCES = ["VCI", "TCBS"]
     def __init__(self, symbol:Optional[str]='VN30F1M', source: str = "VCI"):
         """
-        Initializes the DataExplorer with the specified source and symbol.
+        Khởi tạo lớp (class) với nguồn dữ liệu được chọn.
         """
         self.symbol = symbol.upper()
-        # validate the source to only VCI are available so far
-        if source.upper() not in ["VCI", "TCBS"]:
-            raise ValueError("Hiện tại chỉ có nguồn dữ liệu từ VCI và TCBS được hỗ trợ.")
+        self.source = source.upper()
+        if self.source not in self.SUPPORTED_SOURCES:
+            raise ValueError(f"Hiện tại chỉ có nguồn dữ liệu từ {', '.join(self.SUPPORTED_SOURCES)} được hỗ trợ.")
         self.source_module = f"vnstock3.explorer.{source.lower()}"
         self.data_source = self._load_data_source()
 
     def _load_data_source(self):
         """
         Điều hướng lớp (class) nguồn dữ liệu được lựa chọn.
         """
         module = importlib.import_module(self.source_module)
         return module.Trading(self.symbol)
     
     def _update_data_source(self, symbol: Optional[str] = None):
         """
-        Update the data source if a new symbol is provided.
+        Cập nhật nguồn dữ liệu nếu mã chứng khoán mới được nhập.
         """
         if symbol:
             self.symbol = symbol.upper()
-            self.data_source = self._load_data_source()
+        self.data_source = self._load_data_source()
     
     def price_board(self, symbols_list:list, **kwargs):
         """
         Truy xuất dữ liệu giao dịch trong ngày từ nguồn dữ liệu được chọn.
         """
         return self.data_source.price_board(symbols_list, **kwargs)
     
@@ -282,20 +295,26 @@
         Điều hướng lớp (class) nguồn dữ liệu được lựa chọn.
         """
         module = importlib.import_module(self.source_module)
         return module.Company(self.symbol)
     
     def _update_data_source(self, symbol: Optional[str] = None):
         """
-        Update the data source if a new symbol is provided.
+        Cập nhật nguồn dữ liệu nếu mã chứng khoán mới được nhập.
         """
         if symbol:
             self.symbol = symbol.upper()
             self.data_source = self._load_data_source()
 
+    def overview(self, **kwargs):
+        """
+        Truy xuất thông tin giới thiệu công ty.
+        """
+        return self.data_source.overview(**kwargs)
+
     def profile(self, **kwargs):
         """
         Truy xuất thông tin giới thiệu công ty.
         """
         return self.data_source.profile(**kwargs)
     
     def shareholders(self, **kwargs):
@@ -340,43 +359,64 @@
         """
         return self.data_source.dividends(**kwargs)
 
 class Finance:
     """
     Lớp quản lý các nguồn dữ liệu được tiêu chuẩn hoá cho thông tin tài chính doanh nghiệp.
     """
-    def __init__(self, symbol:str, period:Optional[str]='quarter', source:Optional[str]='TCBS', get_all:Optional[bool]=True):
+    SUPPORTED_SOURCES = ["TCBS", "VCI"]
+
+    def __init__(self, symbol: str, period: Optional[str] = 'quarter', source: Optional[str] = 'TCBS', get_all: Optional[bool] = True):
         self.symbol = symbol.upper()
         self.period = period
         self.get_all = get_all
-        if source.upper() not in ["TCBS" , "VCI"]:
-            raise ValueError("Hiện tại chỉ có nguồn dữ liệu từ TCBS và VCI được hỗ trợ thông tin báo cáo tài chính.")
-        self.source_module = f"vnstock3.explorer.{source.lower()}"
+        self.source = source.upper()
+        if self.source not in self.SUPPORTED_SOURCES:
+            raise ValueError(f"Hiện tại chỉ có nguồn dữ liệu từ {', '.join(self.SUPPORTED_SOURCES)} được hỗ trợ thông tin báo cáo tài chính.")
+        self.source_module = f"vnstock3.explorer.{self.source.lower()}"
         self.data_source = self._load_data_source()
 
     def _load_data_source(self):
         """
         Điều hướng lớp (class) nguồn dữ liệu được lựa chọn.
         """
         module = importlib.import_module(self.source_module)
         return module.Finance(self.symbol)
     
     def _update_data_source(self, symbol: Optional[str] = None):
         """
-        Update the data source if a new symbol is provided.
+        Cập nhật nguồn dữ liệu nếu mã chứng khoán mới được nhập.
         """
         if symbol:
             self.symbol = symbol.upper()
             self.data_source = self._load_data_source()
 
     def balance_sheet(self, **kwargs):
         """
         Truy xuất bảng cân đối kế toán.
         """
         return self.data_source.balance_sheet(**kwargs)
+    
+    def income_statement(self, **kwargs):
+        """
+        Truy xuất báo cáo doanh thu.
+        """
+        return self.data_source.income_statement(**kwargs)
+    
+    def cash_flow(self, **kwargs):
+        """
+        Truy xuất báo cáo dòng tiền.
+        """
+        return self.data_source.cash_flow(**kwargs)
+    
+    def ratio(self, **kwargs):
+        """
+        Truy xuất các chỉ số tài chính.
+        """
+        return self.data_source.ratio(**kwargs)
 
 class MSNComponents:
     """
     Class (lớp) quản lý các chức năng của thư viện Vnstock liên quan đến thị trường ngoại hối.
     """
     def __init__(self, symbol: Optional[str]='EURUSD', source: str = "MSN"):
         self.symbol = symbol.upper()
```

### Comparing `vnstock3-0.3.0.1/vnstock3/core/config/const.py` & `vnstock3-0.3.0.2/vnstock3/core/config/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/core/utils/env.py` & `vnstock3-0.3.0.2/vnstock3/core/utils/env.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/core/utils/ext.py` & `vnstock3-0.3.0.2/vnstock3/core/utils/ext.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/core/utils/help.py` & `vnstock3-0.3.0.2/vnstock3/core/utils/help.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/core/utils/launcher.py` & `vnstock3-0.3.0.2/vnstock3/core/utils/launcher.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/core/utils/logger.py` & `vnstock3-0.3.0.2/vnstock3/core/utils/logger.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/core/utils/parser.py` & `vnstock3-0.3.0.2/vnstock3/core/utils/parser.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/core/utils/user_agent.py` & `vnstock3-0.3.0.2/vnstock3/core/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/misc/exchange_rate.py` & `vnstock3-0.3.0.2/vnstock3/explorer/misc/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/misc/gold_price.py` & `vnstock3-0.3.0.2/vnstock3/explorer/misc/gold_price.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/msn/const.py` & `vnstock3-0.3.0.2/vnstock3/explorer/msn/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/msn/helper.py` & `vnstock3-0.3.0.2/vnstock3/explorer/msn/helper.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/msn/listing.py` & `vnstock3-0.3.0.2/vnstock3/explorer/msn/listing.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/msn/quote.py` & `vnstock3-0.3.0.2/vnstock3/explorer/msn/quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .const import _BASE_URL, _RESAMPLE_MAP, _OHLC_MAP, _OHLC_DTYPE
 from .models import TickerModel
 
 logger = get_logger(__name__)
 
 class Quote:
     """
-    TCBS data source for fetching stock market data, accommodating requests with large date ranges.
+    MSN data source for fetching stock market data, accommodating requests with large date ranges.
     """
     def __init__(self, symbol_id:str, random_agent:Optional[bool]=False):
         self.data_source = 'MSN'
         self.symbol_id = symbol_id.lower()
         self.asset_type = get_asset_type(symbol_id)
         self.base_url = _BASE_URL
         self.headers = get_headers(data_source=self.data_source, random_agent=random_agent)
```

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/tcbs/company.py` & `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/company.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/tcbs/const.py` & `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/tcbs/financial.py` & `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/financial.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/tcbs/models.py` & `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/models.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/tcbs/quote.py` & `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/quote.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/tcbs/trading.py` & `vnstock3-0.3.0.2/vnstock3/explorer/tcbs/trading.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/vci/company.py` & `vnstock3-0.3.0.2/vnstock3/explorer/vci/company.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/vci/const.py` & `vnstock3-0.3.0.2/vnstock3/explorer/vci/const.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/vci/financial.py` & `vnstock3-0.3.0.2/vnstock3/explorer/vci/financial.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/vci/listing.py` & `vnstock3-0.3.0.2/vnstock3/explorer/vci/listing.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             return json_data
         
     def symbols_by_group (self, group: str ='VN30', show_log:Optional[bool]=False, to_df:Optional[bool]=True):
         """
         Truy xuất danh sách các mã cổ phiếu theo tên nhóm trên thị trường Việt Nam.
 
         Tham số:
-            - group (tùy chọn): Tên nhóm cổ phiếu. Mặc định là 'VN30'. Các mã có thể là: HOSE, VN30, VNMidCap, VNSmallCap, VNAllShare, VN100, ETF, HNX, HNX30, HNXCon, HNXFin, HNXLCap, HNXMSCap, HNXMan, UPCOM, FU_INDEX (mã chỉ số hợp đồng tương lai)
+            - group (tùy chọn): Tên nhóm cổ phiếu. Mặc định là 'VN30'. Các mã có thể là: HOSE, VN30, VNMidCap, VNSmallCap, VNAllShare, VN100, ETF, HNX, HNX30, HNXCon, HNXFin, HNXLCap, HNXMSCap, HNXMan, UPCOM, FU_INDEX (mã chỉ số hợp đồng tương lai), CW (chứng quyền).
             - show_log (tùy chọn): Hiển thị thông tin log giúp debug dễ dàng. Mặc định là False.
             - to_df (tùy chọn): Chuyển đổi dữ liệu danh sách mã cổ phiếu trả về dưới dạng DataFrame. Mặc định là True. Đặt là False để trả về dữ liệu dạng JSON.
         """
         if group not in _GROUP_CODE:
             raise ValueError(f"Invalid group. Group must be in {_GROUP_CODE}")
         url = f'https://mt.vietcap.com.vn/api/price/symbols/getByGroup?group={group}'
```

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/vci/quote.py` & `vnstock3-0.3.0.2/vnstock3/explorer/vci/quote.py`

 * *Files identical despite different names*

### Comparing `vnstock3-0.3.0.1/vnstock3/explorer/vci/trading.py` & `vnstock3-0.3.0.2/vnstock3/explorer/vci/trading.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """
     Truy xuất dữ liệu giao dịch của mã chứng khoán từ nguồn dữ liệu VCI.
     """
     def __init__(self, symbol:Optional[str], random_agent=False):
         self.symbol = symbol.upper()
         self.asset_type = get_asset_type(self.symbol)
         self.base_url = _BASE_URL
-        self.headers = get_headers(data_source='TCBS', random_agent=random_agent)
+        self.headers = get_headers(data_source='VCI', random_agent=random_agent)
         
     def price_board (self, symbols_list: List[str], to_df:Optional[bool]=True, show_log:Optional[bool]=False):
         """
         Truy xuất thông tin bảng giá của các mã chứng khoán tuỳ chọn từ nguồn dữ liệu VCI.
         """
         url = f'{self.base_url}price/symbols/getList'
         payload = json.dumps({"symbols": symbols_list})
```

### Comparing `vnstock3-0.3.0.1/vnstock3.egg-info/PKG-INFO` & `vnstock3-0.3.0.2/vnstock3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnstock3
-Version: 0.3.0.1
+Version: 0.3.0.2
 Summary: A comprehensive and transparent solution for Vietnamese stock market analysis.
 Home-page: https://github.com/thinh-vu/vnstock
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 License: **GIẤY PHÉP SỬ DỤNG PHẦN MỀM VNSTOCK3**
         -----------------------------------
         
@@ -136,15 +136,21 @@
 # I. 🎤 Giới thiệu
 
 `Vnstock3` là phiên bản phần mềm Vnstock thế hệ thứ 3 được giới thiệu công khai vào 10/5/2024. 
 Đây là thế hệ Vnstock với nhiều nâng cấp giá trị, chia sẻ tầm nhìn rõ ràng hơn về Vnstock với vai trò một giải pháp phân tích thị trường chứng khoán mã nguồn mở mang nhiều dấu ấn của tương lai công nghệ.
 
 Vnstock sẽ luôn là giải pháp miễn phí để bạn tiếp cận dữ liệu chứng khoán, tài chính toàn diện, miễn phí với các nhu cầu thiết yếu và làm quen với bộ giải phép Python linh hoạt. Chúc mừng bạn là một phần của sự thay đổi trong hành trình chuyển đổi số thị trường chứng khoán tại Việt Nam.
 
-# II. 📔 Tài liệu hướng dẫn
+# II. ⏱️ Cập nhật đáng chú ý
+
+- 10-05-2024: Ra mắt phiên bản Vnstock `0.3.0.1` với tên gói cài đặt `vnstock3`
+
+Chi tiết cập nhật phần mềm và phiên bản [tại đây](https://vnstocks.com/docs/tai-lieu/lich-su-phien-ban)
+
+# III. 📔 Tài liệu hướng dẫn
 
 Trước khi bắt đầu, hãy đánh dấu yêu thích để giúp dự án có thể tiếp cận tới nhiều người hơn. Cám ơn bạn!
 
 ![star_project](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/images/github_star_guide.png)
 
 Cài đặt thư viện với câu lệnh sau:
 
@@ -170,15 +176,15 @@
 ```
 Chúc các bạn thành công và có nhiều trải nghiệm thú vị với Vnstock3!
 
 <!-- [![vnstock docs - Xem Thêm](https://img.shields.io/badge/vnstock_docs-Xem_Thêm-2ea44f?style=for-the-badge&logo=Github)](https://thinh-vu.github.io/vnstock) -->
 
 <!-- [![vnstock_docs_home](https://raw.githubusercontent.com/thinh-vu/vnstock/beta/docs/docs/assets/images/vnstock_docs_home.png)](https://thinh-vu.github.io/vnstock) -->
 
-# III. 🙋‍♂️ Thông tin liên hệ
+# IV. 🙋‍♂️ Thông tin liên hệ
 
 Bạn có thể kết nối với tác giả qua các hình thức sau. Trong trường hợp cần hỗ trợ nhanh, bạn có thể chọn nhắn tin qua Messenger hoặc Linkedin, tôi sẽ phản hồi ngay lập tức nếu có thể trong hầu hết các trường hợp.
 
 <div id="badges" align="center">
   <a href="https://www.linkedin.com/in/thinh-vu">
     <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
   </a>
@@ -189,18 +195,18 @@
   </a>
   </a>
     <a href="https://github.com/thinh-vu">
     <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="Github Badge"/>
   </a>
 </div>
 
-# IV. 🔑 Giấy phép sử dụng (License)
+# V. 🔑 Giấy phép sử dụng (License)
 
 `Vnstock3` được phát hành theo giấy phép tuỳ chỉnh hướng đến cá nhân, không dành cho mục đích thương mại. Quyền sử dụng được quy định cụ thể trong [giấy phép](LICENSE.md) kèm theo. Nếu bạn hoặc tổ chức bạn đang làm việc muốn sử dụng Vnstock có thể liên hệ tác giả để hiểu rõ phạm vi sử dụng và được cấp phép chính thức.
 
 Khi sử dụng Vnstock trong dự án của mình, bạn cần trích dẫn thông tin về tác giả và dự án theo hướng dẫn của Vnstock.
 
-# V. Lịch sử lượt yêu thích
+# VI. Lịch sử lượt yêu thích
 
 Bạn có thể hỗ trợ dự án bằng cách cực kỳ đơn giản là đánh dấu yêu thích để giúp dự án có thể tiếp cận tới nhiều người hơn. Dưới đây là lịch sử lượt yêu thích của dự án.
 
 [![Star History Chart](https://api.star-history.com/svg?repos=thinh-vu/vnstock&type=Date)](https://star-history.com/#thinh-vu/vnstock&Date)
```

