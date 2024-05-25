# Comparing `tmp/schwab_api_wrapper-0.0.3.tar.gz` & `tmp/schwab_api_wrapper-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.0.3.tar", last modified: Sun May 12 23:10:55 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.0.4.tar", last modified: Fri May 24 21:25:54 2024, max compression
```

## Comparing `schwab_api_wrapper-0.0.3.tar` & `schwab_api_wrapper-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.187058 schwab_api_wrapper-0.0.3/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-04-28 01:20:00.000000 schwab_api_wrapper-0.0.3/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-12 23:10:55.186763 schwab_api_wrapper-0.0.3/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-04-28 01:37:25.000000 schwab_api_wrapper-0.0.3/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-12 23:09:13.000000 schwab_api_wrapper-0.0.3/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.184285 schwab_api_wrapper-0.0.3/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-04-28 01:29:21.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.185378 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10234 2024-05-12 22:58:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    36520 2024-05-08 01:27:40.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.186025 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     7461 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     5463 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.186392 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-12 23:10:55.187108 schwab_api_wrapper-0.0.3/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.186155 schwab_api_wrapper-0.0.3/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    44497 2024-04-28 01:49:49.000000 schwab_api_wrapper-0.0.3/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.437221 schwab_api_wrapper-0.0.4/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-04-28 01:20:00.000000 schwab_api_wrapper-0.0.4/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-24 21:25:54.436955 schwab_api_wrapper-0.0.4/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-04-28 01:37:25.000000 schwab_api_wrapper-0.0.4/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-24 21:25:03.000000 schwab_api_wrapper-0.0.4/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.430768 schwab_api_wrapper-0.0.4/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-04-28 01:29:21.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.434346 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-24 21:24:24.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    36520 2024-05-08 01:27:40.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.435849 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     7461 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     5463 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.436661 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-24 21:25:54.000000 schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-24 21:25:54.437262 schwab_api_wrapper-0.0.4/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-24 21:25:54.436148 schwab_api_wrapper-0.0.4/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    44497 2024-04-28 01:49:49.000000 schwab_api_wrapper-0.0.4/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.0.3/LICENSE` & `schwab_api_wrapper-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/PKG-INFO` & `schwab_api_wrapper-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.3/pyproject.toml` & `schwab_api_wrapper-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,19 @@
 
     fiftyTwoWeekHigh: float = Field(
         ..., alias="52WeekHigh"
     )  # Highest price traded in the past 12 months, or 52 weeks
     fiftyTwoWeekLow: float = Field(
         ..., alias="52WeekLow"
     )  # Lowest price traded in the past 12 months, or 52 weeks
-    askMICId: str  # ask MIC code
+    askMICId: Optional[str] = None  # ask MIC code
     askPrice: float  # Current Best Ask Price
     askSize: int  # Number of shares for ask
     askTime: int  # Last ask time in milliseconds since Epoch
-    bidMICId: str  # bid MIC code
+    bidMICId: Optional[str] = None  # bid MIC code
     bidPrice: float  # Current Best Bid Price
     bidSize: int  # Number of shares for bid
     bidTime: int  # last bid tim in milliseconds since Epoch
     closePrice: float  # Previous day's closing price
     highPrice: float  # Day's high trade price
     lastMICId: Optional[str] = None  # Last MIC code
     lastPrice: float  # TODO documentation missing on site
```

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/schwab.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.3
+Version: 0.0.4
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.0.4/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.3/tests/test_schawb_api.py` & `schwab_api_wrapper-0.0.4/tests/test_schawb_api.py`

 * *Files identical despite different names*

