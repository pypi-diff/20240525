# Comparing `tmp/schwab_api_wrapper-0.0.5.tar.gz` & `tmp/schwab_api_wrapper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.0.5.tar", last modified: Sat May 25 01:13:13 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.0.6.tar", last modified: Sat May 25 03:32:13 2024, max compression
```

## Comparing `schwab_api_wrapper-0.0.5.tar` & `schwab_api_wrapper-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.592563 schwab_api_wrapper-0.0.5/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-04-28 01:20:00.000000 schwab_api_wrapper-0.0.5/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-25 01:13:13.592337 schwab_api_wrapper-0.0.5/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-04-28 01:37:25.000000 schwab_api_wrapper-0.0.5/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-25 01:12:33.000000 schwab_api_wrapper-0.0.5/pyproject.toml
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.587845 schwab_api_wrapper-0.0.5/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-04-28 01:29:21.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.589766 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-24 21:24:24.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    36520 2024-05-08 01:27:40.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.591190 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 01:11:28.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     5463 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.592103 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-25 01:13:13.000000 schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-25 01:13:13.592605 schwab_api_wrapper-0.0.5/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 01:13:13.591569 schwab_api_wrapper-0.0.5/tests/
--rw-r--r--   0 owengordon   (501) staff       (20)    44497 2024-04-28 01:49:49.000000 schwab_api_wrapper-0.0.5/tests/test_schawb_api.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 03:32:13.675516 schwab_api_wrapper-0.0.6/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-25 03:32:13.675202 schwab_api_wrapper-0.0.6/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-25 03:31:43.000000 schwab_api_wrapper-0.0.6/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 03:32:13.672401 schwab_api_wrapper-0.0.6/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 03:32:13.673639 schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10268 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    36788 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 03:32:13.674324 schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8019 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     5497 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 03:32:13.674771 schwab_api_wrapper-0.0.6/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-25 03:32:13.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-25 03:32:13.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-25 03:32:13.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-25 03:32:13.000000 schwab_api_wrapper-0.0.6/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-25 03:32:13.675583 schwab_api_wrapper-0.0.6/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-25 03:32:13.674482 schwab_api_wrapper-0.0.6/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    45372 2024-05-25 03:27:51.000000 schwab_api_wrapper-0.0.6/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.0.5/LICENSE` & `schwab_api_wrapper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/PKG-INFO` & `schwab_api_wrapper-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.5/pyproject.toml` & `schwab_api_wrapper-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/schwab.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import requests
 from requests import Response
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
 from datetime import datetime, timedelta, timezone, date
 from typing import Optional, Union, List
+from collections.abc import Iterable
 import logging
 from devtools import pprint, pformat
 from urllib.parse import quote
 
 from .response_aware_retry import ResponseAwareRetry
 from .utils import *
 
@@ -866,15 +867,15 @@
             return None, AccountsAndTradingError(**response.json())
 
     def get_transactions(
         self,
         encrypted_account_number: str,
         start_date: datetime,
         end_date: datetime,
-        transaction_type: TransactionType,
+        transaction_type: Union[TransactionType, Iterable[TransactionType]],
         symbol: Optional[str] = None,
     ) -> tuple[Optional[TransactionResponse], Optional[AccountsAndTradingError]]:
         """
         Get all transactions information for a specific account
 
         Parameters:
             encrypted_account_number: The encrypted ID of the account
@@ -892,15 +893,20 @@
         if end_date.tzinfo is None or end_date.tzinfo.utcoffset(end_date) is None:
             end_date = end_date.replace(tzinfo=timezone.utc)
 
         params = {
             "startDate": start_date.isoformat(),
             "endDate": end_date.isoformat(),
             "symbol": quote(symbol),
-            "types": transaction_type.value,
+            "types": ",".join(
+                map(
+                    lambda t_type: t_type.value, 
+                    transaction_type
+                )
+            ) if isinstance(transaction_type, Iterable) else transaction_type.value,
         }
 
         logging.getLogger(__name__).debug(
             "Get Transactions Params:\n" + pformat(params)
         )
 
         response = self.__get(url, params=params, headers=self.headers)
```

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,16 +221,16 @@
     description: Optional[str] = None
     accountNumber: str
     type: TransactionType
     status: TransactionStatus
     subAccount: SubAccount
     tradeDate: datetime
     settlementDate: Optional[datetime] = None
-    positionId: int
-    orderId: int
+    positionId: Optional[int] = None
+    orderId: Optional[int] = None
     netAmount: float
     activityType: Optional[ActivityType] = None
     transferItems: List[TransferItem]
 
 
 class TransactionResponse(RootModel):
     root: List[Transaction]
```

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
 Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
 Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `schwab_api_wrapper-0.0.5/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.0.6/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.5/tests/test_schawb_api.py` & `schwab_api_wrapper-0.0.6/tests/test_schawb_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1184,14 +1184,41 @@
             symbol="GM",
         )
 
         self.assertIsInstance(result, TransactionResponse)
         self.assertIsNone(error)
 
     @responses.activate
+    def test_get_transactions_multiple_types_success(self):
+        responses.add(
+            responses.GET,
+            f"{TRADER_API_ENDPOINT}/accounts/{self.encrypted_account_number}/transactions",
+            json=json.load(
+                open(
+                    Path(os.path.dirname(__file__))
+                    / "sample_responses"
+                    / "multi_type_transactions.json",
+                    "r",
+                )
+            ),
+            status=200,
+        )
+
+        result, error = self.api.get_transactions(
+            self.encrypted_account_number,
+            datetime(2024, 3, 1),
+            datetime(2024, 4, 15),
+            [TransactionType.TRADE, TransactionType.CASH_RECEIPT],
+            symbol="GM",
+        )
+
+        self.assertIsInstance(result, TransactionResponse)
+        self.assertIsNone(error)
+
+    @responses.activate
     def test_get_transactions_bad_request(self):
         responses.add(
             responses.GET,
             f"{TRADER_API_ENDPOINT}/accounts/{self.encrypted_account_number}/transactions",
             json={
                 "message": "'2024-04-15T12:00:00+1200' is not a valid value for endDate"
             },
```

