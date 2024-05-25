# Comparing `tmp/pkscreener-0.45.20240525.414.tar.gz` & `tmp/pkscreener-0.45.20240525.415.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240525.414.tar", last modified: Sat May 25 16:52:09 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240525.415.tar", last modified: Sat May 25 18:49:41 2024, max compression
```

## Comparing `pkscreener-0.45.20240525.414.tar` & `pkscreener-0.45.20240525.415.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:52:09.738425 pkscreener-0.45.20240525.414/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/LICENSE-Others
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-25 16:52:09.738425 pkscreener-0.45.20240525.414/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:52:09.734425 pkscreener-0.45.20240525.414/pkscreener/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:52:09.738425 pkscreener-0.45.20240525.414/pkscreener/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/ArtTexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/Backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/Barometer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/CandlePatterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/Changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)    33644 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/Fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/MarketMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/MarketStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/MenuOptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/OtaUpdater.py
--rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/PKScanRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/PKScheduledTaskProgress.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/PKScheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/PKSpreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/PKTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/Pktalib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/Portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/PortfolioXRay.py
--rw-r--r--   0 runner    (1001) docker     (127)   154008 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/ScreeningStatistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    55902 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/StockScreener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/UserMenuChoicesHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    84541 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/WorkflowManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 16:52:03.000000 pkscreener-0.45.20240525.414/pkscreener/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/classes/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/courbd.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   144558 2024-05-25 16:50:41.000000 pkscreener-0.45.20240525.414/pkscreener/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-25 16:50:42.000000 pkscreener-0.45.20240525.414/pkscreener/pkscreener.ini
--rw-r--r--   0 runner    (1001) docker     (127)    52903 2024-05-25 16:50:42.000000 pkscreener-0.45.20240525.414/pkscreener/pkscreenerbot.py
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-05-25 16:50:42.000000 pkscreener-0.45.20240525.414/pkscreener/pkscreenercli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 16:52:09.734425 pkscreener-0.45.20240525.414/pkscreener.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-25 16:52:09.000000 pkscreener-0.45.20240525.414/pkscreener.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-25 16:52:09.000000 pkscreener-0.45.20240525.414/pkscreener.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:52:09.000000 pkscreener-0.45.20240525.414/pkscreener.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-25 16:52:09.000000 pkscreener-0.45.20240525.414/pkscreener.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 16:52:09.000000 pkscreener-0.45.20240525.414/pkscreener.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-25 16:52:09.000000 pkscreener-0.45.20240525.414/pkscreener.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 16:52:09.000000 pkscreener-0.45.20240525.414/pkscreener.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-25 16:52:09.738425 pkscreener-0.45.20240525.414/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-25 16:50:42.000000 pkscreener-0.45.20240525.414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/LICENSE-Others
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26594 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.359372 pkscreener-0.45.20240525.415/pkscreener/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/pkscreener/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/ArtTexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Barometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16986 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/CandlePatterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33644 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10050 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/MarketMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/MarketStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44414 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/MenuOptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/OtaUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24198 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22357 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKScanRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKSpreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PKTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18470 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Pktalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13876 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47779 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/PortfolioXRay.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154008 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/ScreeningStatistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55902 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/StockScreener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84541 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/WorkflowManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-25 18:49:35.000000 pkscreener-0.45.20240525.415/pkscreener/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/classes/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)   791436 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/courbd.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   144558 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/pkscreener.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    53262 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/pkscreenerbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33987 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/pkscreener/pkscreenercli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 18:49:41.359372 pkscreener-0.45.20240525.415/pkscreener.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27511 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 18:49:41.000000 pkscreener-0.45.20240525.415/pkscreener.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-25 18:49:41.363372 pkscreener-0.45.20240525.415/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5567 2024-05-25 18:48:06.000000 pkscreener-0.45.20240525.415/setup.py
```

### Comparing `pkscreener-0.45.20240525.414/LICENSE` & `pkscreener-0.45.20240525.415/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/LICENSE-Others` & `pkscreener-0.45.20240525.415/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/PKG-INFO` & `pkscreener-0.45.20240525.415/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240525.414
+Version: 0.45.20240525.415
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240525.414.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240525.415.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240525.414/README.md` & `pkscreener-0.45.20240525.415/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240525.414/pkscreener/__init__.py` & `pkscreener-0.45.20240525.415/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 5
         self.maxNumResultRowsInMonitor = 3
         self.calculatersiintraday = False
-        self.defaultMonitorOptions = "X:12:9:2.5~X:12:23~X:12:28~X:12:31~|{1}X:0:23:>|X:0:27:>|X:0:31:~|{2}X:0:31:~|{3}X:0:27:~X:12:7:3:.01:1~|{5}X:0:5:0:40:~X:12:7:6:1~X:12:11:~X:12:12:i 5m~X:12:17~X:12:24~X:12:6:7:1~X:12:6:3~X:12:6:8~X:12:6:9~X:12:6:10:1~X:12:7:3:.02:1~X:12:13:i 1m~X:12:2~|{1}X:0:29:"
+        self.defaultMonitorOptions = "X:12:9:2.5~X:12:23~X:12:28~X:12:31~|{1}X:0:23:>|X:0:27:>|X:0:31:~|{2}X:0:31:~|{3}X:0:27:~X:12:7:3:.01:1~|{5}X:0:5:0:35:~X:12:7:6:1~X:12:11:~X:12:12:i 5m~X:12:17~X:12:24~X:12:6:7:1~X:12:6:3~X:12:6:8~X:12:6:9~X:12:6:10:1~X:12:7:3:.02:1~X:12:13:i 1m~X:12:2~|{1}X:0:29:"
         self.minimumChangePercentage = 0
         self.daysToLookback = 22 * self.backtestPeriodFactor  # 1 month
         self.periods = [1,2,3,4,5,10,15,22,30]
         if self.maxBacktestWindow > self.periods[-1]:
             self.periods.extend(self.maxBacktestWindow)
 
     @property
```

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/MarketMonitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,20 +177,23 @@
             headers="keys" if self.isPinnedSingleMonitorMode else (),
             highlightCharacter=colorText.HEAD+"="+colorText.END,
             showindex=self.isPinnedSingleMonitorMode,
             highlightedRows=highlightRows,
             highlightedColumns=highlightCols,
             maxcolwidths=Utility.tools.getMaxColumnWidths(self.monitor_df)
         )
-        self.lines = len(tabulated_results.splitlines()) + 1 # 1 for the progress bar at the bottom and 1 for the chosenMenu option
+        numRecords = len(tabulated_results.splitlines())
+        self.lines = numRecords + 1 # 1 for the progress bar at the bottom and 1 for the chosenMenu option
         OutputControls().printOutput(tabulated_results, enableMultipleLineOutput=True)
         
         if not self.isPinnedSingleMonitorMode:
             if telegram:
                 self.updateIfRunningInTelegramBotMode(screenOptions, chosenMenu, dbTimestamp, telegram, telegram_df)
+            elif screenOptions.split(":")[2] == "5" and numRecords > 1: # RSI conditions met? Sound alert!
+                Utility.tools.alertSound(beeps=5)
         else:
             sleep(30)
 
     def updateDataFrameForTelegramMode(self, telegram, screen_monitor_df):
         telegram_df = None
         if telegram:
             telegram_df = screen_monitor_df[["Stock", "LTP", "Ch%", "Vol"]]
```

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/WorkflowManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,21 @@
                 + branch
                 + '","inputs":{"user":"'
                 + f"{user}"
                 + '","params":"'
                 + f'-a Y -e -p -u {user} -o {options.replace("_",":")}:D:D:D:D:D'.replace("::",":")
                 + '","ref":"main"}}'
             )
-
+    elif workflowType == "R":
+        workflow_name = "w3-workflow-bot.yml"
+        data = (
+                '{"ref":"'
+                + branch
+                + '","inputs":{"branch-name":"main"}}'
+            )
     _, _, _, ghp_token = get_secrets()
     url = f"https://api.github.com/repos/{owner}/{repo}/actions/workflows/{workflow_name}/dispatches"
 
     headers = {
         "Accept": "application/vnd.github+json",
         "Authorization": f"Bearer {ghp_token}",
         "Content-Type": "application/json",
```

### Comparing `pkscreener-0.45.20240525.414/pkscreener/classes/keys.py` & `pkscreener-0.45.20240525.415/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/courbd.ttf` & `pkscreener-0.45.20240525.415/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/globals.py` & `pkscreener-0.45.20240525.415/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240525.415/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240525.415/pkscreener/pkscreenerbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 UNSUPPORTED_COMMAND_MENUS =["22","42","M","Z"]
 SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","31","32"]
 
 def initializeIntradayTimer():
     try:
         if (not PKDateUtilities.isTodayHoliday()[0]):
             now = PKDateUtilities.currentDateTime()
-            marketStartTime = PKDateUtilities.currentDateTime(simulate=True,hour=9,minute=15)
+            marketStartTime = PKDateUtilities.currentDateTime(simulate=True,hour=9,minute=14)
             morning745am = PKDateUtilities.currentDateTime(simulate=True,hour=7,minute=45)
             if now < marketStartTime and now >= morning745am: # Telegram bot might keep running beyond an hour. So let's start watching around 7:45AM
                 difference = (marketStartTime - now).total_seconds() + 1
                 global int_timer
                 int_timer = threading.Timer(difference, launchIntradayMonitor, args=[])
                 int_timer.start()
             elif now >= marketStartTime:
@@ -171,15 +171,16 @@
     # The keyboard is a list of button rows, where each row is in turn
     # a list (hence `[[...]]`).
     if bot_available:
         mns = m0.renderForMenu(asList=True)
         if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()) or sys.argv[0].endswith(".py"):
             mns.append(menu().create(f"MI_{monitorIndex}", "Int. Monitor", 2))
         if user.username == OWNER_USER:
-            mns.append(menu().create(f"DV_0", ("Enbl" if not configManager.logsEnabled else "Dsbl"), 2))
+            mns.append(menu().create(f"DV_0", ("✅" if not configManager.logsEnabled else "🚫"), 2))
+            mns.append(menu().create(f"DV_1", "🔄", 2))
 
         inlineMenus = []
         for mnu in mns:
             if mnu.menuKey[0:2] in TOP_LEVEL_SCANNER_MENUS:
                 inlineMenus.append(
                     InlineKeyboardButton(
                         mnu.menuText.split("(")[0],
@@ -287,15 +288,15 @@
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI").replace("CDV","DV")
     if data[0:2] not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
     if data.startswith("DV"):
         # Dev Mode
         devModeIndex = int(data.split("_")[1])
-        if devModeIndex == 0:
+        if devModeIndex == 0: # Enable/Disable intraday monitor along with logging
             if "PKDevTools_Default_Log_Level" in os.environ.keys():
                 del os.environ['PKDevTools_Default_Log_Level']
                 configManager.maxNumResultRowsInMonitor = 2
                 configManager.logsEnabled = False
             else:
                 # Switch config file
                 configManager.maxNumResultRowsInMonitor = 3
@@ -307,14 +308,17 @@
                 try:
                     monitor_proc.kill()
                 except:
                     pass
             
             launchIntradayMonitor()
             await start(update, context,chosenBotMenuOption=chosenBotMenuOption)
+        elif devModeIndex == 1: # Restart the bot service
+            resp = run_workflow(None, None,None, workflowType="R")
+            await start(update, context,chosenBotMenuOption=f"{resp.status_code}: {resp.text}")
     return START_ROUTES
 
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI")
     if data[0:2] not in TOP_LEVEL_SCANNER_MENUS:
@@ -994,16 +998,15 @@
     for cmd in cmds:
         cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
     reply_markup = default_markup([])
     
     """Send a message when the command /help is issued."""
     if update is not None and update.message is not None:
         await update.message.reply_text(
-            f"You can begin by typing in /start and hit send!\n\nOR\n\nChoose an option:\n{cmdText}",
-            reply_markup=reply_markup
+            f"You can begin by typing in /start (Recommended) and hit send!\n\nOR\n\nChoose an option:\n{cmdText}\n\nWe recommend you start by clicking on this /start"
         )  #  \n\nThis bot restarts every hour starting at 5:30am IST until 10:30pm IST to keep it running on free servers. If it does not respond, please try again in a minutes to avoid the restart duration!
         query = update.message
         message = f"Name: <b>{query.from_user.first_name}</b>, Username:@{query.from_user.username} with ID: <b>@{str(query.from_user.id)}</b> began using the bot!"
         await context.bot.send_message(
             chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
         )
```

### Comparing `pkscreener-0.45.20240525.414/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240525.415/pkscreener/pkscreenercli.py`

 * *Files 2% similar despite different names*

```diff
@@ -577,17 +577,19 @@
         else:
             # We need to switch to daily scan
             args.intraday = None
             configManager.toggleConfig(candleDuration='1d', clearCache=False)
         if monitorOption.startswith("|"):
             monitorOption = monitorOption.replace("|","")
             monitorOptions = monitorOption.split(":")
-            if monitorOptions[1] != "0":
+            if "X" in monitorOptions[0].upper() and monitorOptions[1] != "0":
                 monitorOptions[1] = "0"
                 monitorOption = ":".join(monitorOptions)
+            if "B" in monitorOptions[0].upper() and monitorOptions[1] != "30":
+                monitorOption = ":".join(monitorOptions).upper().replace(f"{monitorOptions[0].upper()}:{monitorOptions[1]}",f"{monitorOptions[0].upper()}:30:{monitorOptions[1]}")
             # We need to pipe the output from previous run into the next one
             if prevOutput is not None and not prevOutput.empty:
                 try:
                     prevOutput.set_index("Stock", inplace=True)
                 except:
                     pass
                 prevOutput_results = prevOutput[~prevOutput.index.duplicated(keep='first')]
```

### Comparing `pkscreener-0.45.20240525.414/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240525.415/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240525.414
+Version: 0.45.20240525.415
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240525.414.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240525.415.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.413/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240525.414/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240525.414/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240525.415/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240525.414/setup.py` & `pkscreener-0.45.20240525.415/setup.py`

 * *Files identical despite different names*

