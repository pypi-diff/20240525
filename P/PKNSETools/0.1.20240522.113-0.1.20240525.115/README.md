# Comparing `tmp/PKNSETools-0.1.20240522.113.tar.gz` & `tmp/PKNSETools-0.1.20240525.115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240522.113.tar", last modified: Wed May 22 19:31:45 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240525.115.tar", last modified: Sat May 25 05:36:36 2024, max compression
```

## Comparing `PKNSETools-0.1.20240522.113.tar` & `PKNSETools-0.1.20240525.115.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/
--rw-rw-rw-   0        0        0     2663 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10770 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2635 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0    10388 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    17471 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       31 2024-05-22 19:31:40.000000 PKNSETools-0.1.20240522.113/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2663 2024-05-22 19:31:45.000000 PKNSETools-0.1.20240522.113/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-22 19:31:45.000000 PKNSETools-0.1.20240522.113/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:31:45.000000 PKNSETools-0.1.20240522.113/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-22 19:31:38.000000 PKNSETools-0.1.20240522.113/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-22 19:31:45.000000 PKNSETools-0.1.20240522.113/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-22 19:31:45.000000 PKNSETools-0.1.20240522.113/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/README.md
--rw-rw-rw-   0        0        0       86 2024-05-22 19:31:45.523338 PKNSETools-0.1.20240522.113/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-22 19:29:59.000000 PKNSETools-0.1.20240522.113/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/
+-rw-rw-rw-   0        0        0     2663 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0    10388 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    17683 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-25 05:36:31.000000 PKNSETools-0.1.20240525.115/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-25 05:36:36.000000 PKNSETools-0.1.20240525.115/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-25 05:36:36.000000 PKNSETools-0.1.20240525.115/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 05:36:36.000000 PKNSETools-0.1.20240525.115/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-25 05:36:30.000000 PKNSETools-0.1.20240525.115/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-25 05:36:36.000000 PKNSETools-0.1.20240525.115/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-25 05:36:36.000000 PKNSETools-0.1.20240525.115/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-25 05:36:36.917663 PKNSETools-0.1.20240525.115/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-25 05:34:50.000000 PKNSETools-0.1.20240525.115/setup.py
```

### Comparing `PKNSETools-0.1.20240522.113/PKG-INFO` & `PKNSETools-0.1.20240525.115/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240522.113
+Version: 0.1.20240525.115
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240522.113.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240525.115.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240525.115/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240525.115/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240525.115/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240525.115/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240525.115/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240525.115/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240525.115/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240525.115/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240525.115/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240525.115/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,19 @@
         ticker = yf.Ticker(exchange) # ^IXIC
         try:
             info = ticker.info
         except:
             info = {"longName":exchange}
             pass
         try:
-            ticker._lazy_load_price_history()._history_metadata["period"] = '5d' # Ignore the yfinance exception for period being 1wk.
+            history = ticker._lazy_load_price_history()
+            if history is not None:
+                history.history(period="1d",interval="1d",prepost=True, proxy=None)
+            if history._history_metadata is not None:
+                history._history_metadata["period"] = '5d' # Ignore the yfinance exception for period being 1wk.
             md = ticker.get_history_metadata()
             ltd = md["regularMarketTime"]
             ctp = md["currentTradingPeriod"]
             tzName = md["exchangeTimezoneName"]
             lastTradeDate = pd.to_datetime(ltd, unit='s', utc=True).tz_convert(tzName)
         except:
             tzName = "Asia/Kolkata"
```

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240525.115/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240525.115/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240522.113
+Version: 0.1.20240525.115
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240522.113.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240525.115.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240522.113/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240525.115/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/README.md` & `PKNSETools-0.1.20240525.115/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240522.113/setup.py` & `PKNSETools-0.1.20240525.115/setup.py`

 * *Files identical despite different names*

