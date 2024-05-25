# Comparing `tmp/schwab_api_wrapper-0.0.4.tar.gz` & `tmp/schwab_api_wrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.0.4.tar", last modified: Fri May 24 21:25:54 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.0.5.tar", last modified: Sat May 25 01:13:13 2024, max compression
```

## Comparing `schwab_api_wrapper-0.0.4.tar` & `schwab_api_wrapper-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.437221 schwab_api_wrapper-0.0.4/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-04-28 01:20:00.000000 schwab_api_wrapper-0.0.4/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-24 21:25:54.436955 schwab_api_wrapper-0.0.4/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-04-28 01:37:25.000000 schwab_api_wrapper-0.0.4/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-24 21:25:03.000000 schwab_api_wrapper-0.0.4/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.430768 schwab_api_wrapper-0.0.4/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-04-28 01:29:21.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.434346 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-24 21:24:24.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    36520 2024-05-08 01:27:40.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.435849 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     7461 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     5463 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.436661 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-24 21:25:54.437262 schwab_api_wrapper-0.0.4/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.436148 schwab_api_wrapper-0.0.4/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    44497 2024-04-28 01:49:49.000000 schwab_api_wrapper-0.0.4/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.592563 schwab_api_wrapper-0.0.5/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-04-28 01:20:00.000000 schwab_api_wrapper-0.0.5/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-25 01:13:13.592337 schwab_api_wrapper-0.0.5/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-04-28 01:37:25.000000 schwab_api_wrapper-0.0.5/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-25 01:12:33.000000 schwab_api_wrapper-0.0.5/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.587845 schwab_api_wrapper-0.0.5/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-04-28 01:29:21.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.589766 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-24 21:24:24.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    36520 2024-05-08 01:27:40.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.591190 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 01:11:28.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     5463 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.592103 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-25 01:13:13.592605 schwab_api_wrapper-0.0.5/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.591569 schwab_api_wrapper-0.0.5/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    44497 2024-04-28 01:49:49.000000 schwab_api_wrapper-0.0.5/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.0.4/LICENSE` & `schwab_api_wrapper-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/PKG-INFO` & `schwab_api_wrapper-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.4/pyproject.toml` & `schwab_api_wrapper-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/schwab.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,41 +188,62 @@
     mutualFundValue: float
     regTCall: float
     shortMarginValue: float
     shortOptionMarketValue: float
     shortStockValue: float
     totalCash: float
     isInCall: float
-    unsettledCash: float
+    unsettledCash: Optional[float] = None
     pendingDeposits: float
     marginBalance: float
     shortBalance: float
     accountValue: float
 
 
 class MarginBalance(BaseModel):
+    accruedInterest: float
+    cashBalance: float
+    cashReceipts: float
+    longOptionMarketValue: float
+    liquidationValue: float
+    longMarketValue: float
+    moneyMarketFund: float
+    savings: float
+    shortMarketValue: float
+    pendingDeposits: float
+    mutualFundValue: float
+    bondValue: float
+    shortOptionMarketValue: float
     availableFunds: float
     availableFundsNonMarginableTrade: float
     buyingPower: float
     buyingPowerNonMarginableTrade: float
     dayTradingBuyingPower: float
-    dayTradingBuyingPowerCall: float
     equity: float
     equityPercentage: float
     longMarginValue: float
     maintenanceCall: float
     maintenanceRequirement: float
     marginBalance: float
     regTCall: float
     shortBalance: float
     shortMarginValue: float
     sma: float
+
+
+class MarginProjectedBalance(BaseModel):
+    availableFunds: float
+    availableFundsNonMarginableTrade: float
+    buyingPower: float
+    dayTradingBuyingPower: float
+    dayTradingBuyingPowerCall: float
+    maintenanceCall: float
+    regTCall: float
     isInCall: float
     stockBuyingPower: float
-    optionBuyingPower: float
 
 
 class CashInitialBalance(BaseModel):
     accruedInterest: float
     cashAvailableForTrading: float
     cashAvailableForWithdrawal: float
     cashBalance: float
@@ -279,15 +300,15 @@
     pfcbFlag: bool = False
     positions: Optional[List[Position]] = None
 
 
 class MarginAccount(BaseAccount):
     initialBalances: MarginInitialBalance
     currentBalances: MarginBalance
-    projectedBalances: MarginBalance
+    projectedBalances: MarginProjectedBalance
 
 
 class CashAccount(BaseAccount):
     initialBalances: CashInitialBalance
     currentBalances: CashBalance
     projectedBalances: CashProjectedBalance
```

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.4/tests/test_schawb_api.py` & `schwab_api_wrapper-0.0.5/tests/test_schawb_api.py`

 * *Files identical despite different names*

