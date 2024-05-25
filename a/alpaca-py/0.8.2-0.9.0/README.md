# Comparing `tmp/alpaca_py-0.8.2.tar.gz` & `tmp/alpaca_py-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_py-0.8.2.tar", max compression
+gzip compressed data, was "alpaca_py-0.9.0.tar", max compression
```

## Comparing `alpaca_py-0.8.2.tar` & `alpaca_py-0.9.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
--rw-r--r--   0        0        0    10872 2023-03-20 15:12:59.606686 alpaca_py-0.8.2/LICENSE
--rw-r--r--   0        0        0     9810 2023-04-03 17:13:32.842661 alpaca_py-0.8.2/README.md
--rw-r--r--   0        0        0       22 2023-04-26 13:55:31.165406 alpaca_py-0.8.2/alpaca/__init__.py
--rw-r--r--   0        0        0      100 2023-03-20 15:12:59.607787 alpaca_py-0.8.2/alpaca/broker/__init__.py
--rw-r--r--   0        0        0    64825 2023-04-11 19:21:35.937449 alpaca_py-0.8.2/alpaca/broker/client.py
--rw-r--r--   0        0        0    11012 2023-03-20 15:12:59.608585 alpaca_py-0.8.2/alpaca/broker/enums.py
--rw-r--r--   0        0        0      138 2023-03-20 15:12:59.608839 alpaca_py-0.8.2/alpaca/broker/models/__init__.py
--rw-r--r--   0        0        0    13998 2023-04-03 17:13:32.844395 alpaca_py-0.8.2/alpaca/broker/models/accounts.py
--rw-r--r--   0        0        0    14499 2023-03-20 15:12:59.609458 alpaca_py-0.8.2/alpaca/broker/models/cip.py
--rw-r--r--   0        0        0     6266 2023-03-20 15:12:59.609667 alpaca_py-0.8.2/alpaca/broker/models/documents.py
--rw-r--r--   0        0        0     4372 2023-03-20 15:12:59.609845 alpaca_py-0.8.2/alpaca/broker/models/funding.py
--rw-r--r--   0        0        0     3216 2023-04-03 17:13:32.845068 alpaca_py-0.8.2/alpaca/broker/models/journals.py
--rw-r--r--   0        0        0      305 2023-03-20 15:12:59.610382 alpaca_py-0.8.2/alpaca/broker/models/trading.py
--rw-r--r--   0        0        0    43935 2023-04-03 17:13:32.846078 alpaca_py-0.8.2/alpaca/broker/requests.py
--rw-r--r--   0        0        0      136 2023-03-20 15:12:59.610982 alpaca_py-0.8.2/alpaca/common/__init__.py
--rw-r--r--   0        0        0      347 2023-03-20 15:12:59.611141 alpaca_py-0.8.2/alpaca/common/constants.py
--rw-r--r--   0        0        0     1705 2023-04-03 17:13:32.846674 alpaca_py-0.8.2/alpaca/common/enums.py
--rw-r--r--   0        0        0      987 2023-03-20 15:12:59.611559 alpaca_py-0.8.2/alpaca/common/exceptions.py
--rw-r--r--   0        0        0      403 2023-03-20 15:12:59.611781 alpaca_py-0.8.2/alpaca/common/models.py
--rw-r--r--   0        0        0     1991 2023-03-20 15:12:59.612115 alpaca_py-0.8.2/alpaca/common/requests.py
--rw-r--r--   0        0        0    13960 2023-04-11 19:21:35.938278 alpaca_py-0.8.2/alpaca/common/rest.py
--rw-r--r--   0        0        0      173 2023-03-20 15:12:59.612704 alpaca_py-0.8.2/alpaca/common/types.py
--rw-r--r--   0        0        0     1916 2023-03-20 15:12:59.612900 alpaca_py-0.8.2/alpaca/common/utils.py
--rw-r--r--   0        0        0    17332 2023-03-20 15:12:59.613119 alpaca_py-0.8.2/alpaca/common/websocket.py
--rw-r--r--   0        0        0      118 2023-03-20 15:12:59.613409 alpaca_py-0.8.2/alpaca/data/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-03 14:46:59.759940 alpaca_py-0.8.2/alpaca/data/enums.py
--rw-r--r--   0        0        0       92 2023-03-20 15:12:59.613798 alpaca_py-0.8.2/alpaca/data/historical/__init__.py
--rw-r--r--   0        0        0    14142 2023-04-03 14:46:59.761182 alpaca_py-0.8.2/alpaca/data/historical/crypto.py
--rw-r--r--   0        0        0    12392 2023-03-20 15:12:59.614199 alpaca_py-0.8.2/alpaca/data/historical/stock.py
--rw-r--r--   0        0        0     4474 2023-03-20 15:12:59.614356 alpaca_py-0.8.2/alpaca/data/historical/utils.py
--rw-r--r--   0        0        0       72 2023-03-20 15:12:59.614560 alpaca_py-0.8.2/alpaca/data/live/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-03 17:13:34.312258 alpaca_py-0.8.2/alpaca/data/live/crypto.py
--rw-r--r--   0        0        0     1935 2023-03-20 15:12:59.614841 alpaca_py-0.8.2/alpaca/data/live/stock.py
--rw-r--r--   0        0        0     1012 2023-03-20 15:12:59.614987 alpaca_py-0.8.2/alpaca/data/mappings.py
--rw-r--r--   0        0        0      115 2023-03-20 15:12:59.615222 alpaca_py-0.8.2/alpaca/data/models/__init__.py
--rw-r--r--   0        0        0     2304 2023-03-20 15:12:59.615411 alpaca_py-0.8.2/alpaca/data/models/bars.py
--rw-r--r--   0        0        0     1752 2023-03-20 15:12:59.615552 alpaca_py-0.8.2/alpaca/data/models/base.py
--rw-r--r--   0        0        0     1643 2023-03-20 15:12:59.615704 alpaca_py-0.8.2/alpaca/data/models/orderbooks.py
--rw-r--r--   0        0        0     2581 2023-03-20 15:12:59.615907 alpaca_py-0.8.2/alpaca/data/models/quotes.py
--rw-r--r--   0        0        0     1979 2023-03-20 15:12:59.616060 alpaca_py-0.8.2/alpaca/data/models/snapshots.py
--rw-r--r--   0        0        0     2318 2023-03-20 15:12:59.616284 alpaca_py-0.8.2/alpaca/data/models/trades.py
--rw-r--r--   0        0        0    12288 2023-04-03 17:13:32.848638 alpaca_py-0.8.2/alpaca/data/requests.py
--rw-r--r--   0        0        0     4303 2023-03-20 15:12:59.616739 alpaca_py-0.8.2/alpaca/data/timeframe.py
--rw-r--r--   0        0        0        0 2023-03-20 15:12:59.616869 alpaca_py-0.8.2/alpaca/py.typed
--rw-r--r--   0        0        0       89 2023-03-20 15:12:59.617081 alpaca_py-0.8.2/alpaca/trading/__init__.py
--rw-r--r--   0        0        0    21010 2023-03-20 15:12:59.617276 alpaca_py-0.8.2/alpaca/trading/client.py
--rw-r--r--   0        0        0     7780 2023-04-26 13:54:12.682339 alpaca_py-0.8.2/alpaca/trading/enums.py
--rw-r--r--   0        0        0    25517 2023-04-11 19:30:55.555410 alpaca_py-0.8.2/alpaca/trading/models.py
--rw-r--r--   0        0        0    19232 2023-03-20 15:12:59.617974 alpaca_py-0.8.2/alpaca/trading/requests.py
--rw-r--r--   0        0        0     7505 2023-03-20 15:12:59.618140 alpaca_py-0.8.2/alpaca/trading/stream.py
--rw-r--r--   0        0        0      915 2023-04-26 13:55:28.655204 alpaca_py-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 alpaca_py-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    10872 2023-04-18 01:08:49.988181 alpaca_py-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9810 2023-04-18 01:08:49.988267 alpaca_py-0.9.0/README.md
+-rw-r--r--   0        0        0       22 2023-08-02 17:04:46.130477 alpaca_py-0.9.0/alpaca/__init__.py
+-rw-r--r--   0        0        0      100 2023-08-02 17:04:21.634237 alpaca_py-0.9.0/alpaca/broker/__init__.py
+-rw-r--r--   0        0        0    64825 2023-08-02 17:04:21.635303 alpaca_py-0.9.0/alpaca/broker/client.py
+-rw-r--r--   0        0        0    11106 2023-07-16 15:49:01.428684 alpaca_py-0.9.0/alpaca/broker/enums.py
+-rw-r--r--   0        0        0      138 2023-04-18 01:08:49.988763 alpaca_py-0.9.0/alpaca/broker/models/__init__.py
+-rw-r--r--   0        0        0    13998 2023-08-02 17:04:21.635768 alpaca_py-0.9.0/alpaca/broker/models/accounts.py
+-rw-r--r--   0        0        0    14499 2023-04-18 01:08:49.988966 alpaca_py-0.9.0/alpaca/broker/models/cip.py
+-rw-r--r--   0        0        0     6317 2023-08-02 17:04:21.636300 alpaca_py-0.9.0/alpaca/broker/models/documents.py
+-rw-r--r--   0        0        0     4372 2023-08-02 17:04:21.636639 alpaca_py-0.9.0/alpaca/broker/models/funding.py
+-rw-r--r--   0        0        0     3216 2023-08-02 17:04:21.636979 alpaca_py-0.9.0/alpaca/broker/models/journals.py
+-rw-r--r--   0        0        0      350 2023-07-16 15:49:01.428898 alpaca_py-0.9.0/alpaca/broker/models/trading.py
+-rw-r--r--   0        0        0    43935 2023-08-02 17:04:21.637158 alpaca_py-0.9.0/alpaca/broker/requests.py
+-rw-r--r--   0        0        0      136 2023-08-02 17:04:21.637337 alpaca_py-0.9.0/alpaca/common/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-18 01:08:49.989527 alpaca_py-0.9.0/alpaca/common/constants.py
+-rw-r--r--   0        0        0     1705 2023-04-18 01:08:49.989586 alpaca_py-0.9.0/alpaca/common/enums.py
+-rw-r--r--   0        0        0      987 2023-04-18 01:08:49.989652 alpaca_py-0.9.0/alpaca/common/exceptions.py
+-rw-r--r--   0        0        0      403 2023-08-02 17:04:21.638411 alpaca_py-0.9.0/alpaca/common/models.py
+-rw-r--r--   0        0        0     1991 2023-08-02 17:04:21.638850 alpaca_py-0.9.0/alpaca/common/requests.py
+-rw-r--r--   0        0        0    13960 2023-04-18 01:08:49.989887 alpaca_py-0.9.0/alpaca/common/rest.py
+-rw-r--r--   0        0        0      173 2023-04-18 01:08:49.989949 alpaca_py-0.9.0/alpaca/common/types.py
+-rw-r--r--   0        0        0     1916 2023-04-18 01:08:49.990018 alpaca_py-0.9.0/alpaca/common/utils.py
+-rw-r--r--   0        0        0    17332 2023-04-18 01:08:49.990119 alpaca_py-0.9.0/alpaca/common/websocket.py
+-rw-r--r--   0        0        0      118 2023-08-02 17:04:21.639074 alpaca_py-0.9.0/alpaca/data/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-16 15:49:01.429006 alpaca_py-0.9.0/alpaca/data/enums.py
+-rw-r--r--   0        0        0       92 2023-08-02 17:04:21.639214 alpaca_py-0.9.0/alpaca/data/historical/__init__.py
+-rw-r--r--   0        0        0    14142 2023-08-02 17:04:21.639445 alpaca_py-0.9.0/alpaca/data/historical/crypto.py
+-rw-r--r--   0        0        0     2754 2023-08-02 17:04:21.639644 alpaca_py-0.9.0/alpaca/data/historical/screener.py
+-rw-r--r--   0        0        0    12392 2023-04-18 01:08:49.990520 alpaca_py-0.9.0/alpaca/data/historical/stock.py
+-rw-r--r--   0        0        0     4474 2023-04-18 01:08:49.990581 alpaca_py-0.9.0/alpaca/data/historical/utils.py
+-rw-r--r--   0        0        0       72 2023-08-02 17:04:21.639929 alpaca_py-0.9.0/alpaca/data/live/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-18 01:08:49.990712 alpaca_py-0.9.0/alpaca/data/live/crypto.py
+-rw-r--r--   0        0        0     1935 2023-04-18 01:08:49.990769 alpaca_py-0.9.0/alpaca/data/live/stock.py
+-rw-r--r--   0        0        0     1012 2023-04-18 01:08:49.990821 alpaca_py-0.9.0/alpaca/data/mappings.py
+-rw-r--r--   0        0        0      115 2023-08-02 17:04:21.640071 alpaca_py-0.9.0/alpaca/data/models/__init__.py
+-rw-r--r--   0        0        0     2304 2023-04-18 01:08:49.990952 alpaca_py-0.9.0/alpaca/data/models/bars.py
+-rw-r--r--   0        0        0     1752 2023-08-02 17:04:21.640209 alpaca_py-0.9.0/alpaca/data/models/base.py
+-rw-r--r--   0        0        0     1643 2023-08-02 17:04:21.640364 alpaca_py-0.9.0/alpaca/data/models/orderbooks.py
+-rw-r--r--   0        0        0     2581 2023-08-02 17:04:21.640604 alpaca_py-0.9.0/alpaca/data/models/quotes.py
+-rw-r--r--   0        0        0     2041 2023-07-16 15:49:01.429169 alpaca_py-0.9.0/alpaca/data/models/screener.py
+-rw-r--r--   0        0        0     1979 2023-04-18 01:08:49.991231 alpaca_py-0.9.0/alpaca/data/models/snapshots.py
+-rw-r--r--   0        0        0     2318 2023-08-02 17:04:21.640779 alpaca_py-0.9.0/alpaca/data/models/trades.py
+-rw-r--r--   0        0        0    13360 2023-08-02 17:04:21.640958 alpaca_py-0.9.0/alpaca/data/requests.py
+-rw-r--r--   0        0        0     4303 2023-04-18 01:08:49.991442 alpaca_py-0.9.0/alpaca/data/timeframe.py
+-rw-r--r--   0        0        0        0 2023-04-18 01:08:49.991467 alpaca_py-0.9.0/alpaca/py.typed
+-rw-r--r--   0        0        0       89 2023-08-02 17:04:21.641225 alpaca_py-0.9.0/alpaca/trading/__init__.py
+-rw-r--r--   0        0        0    21010 2023-08-02 17:04:21.641395 alpaca_py-0.9.0/alpaca/trading/client.py
+-rw-r--r--   0        0        0     7780 2023-07-16 15:49:01.429823 alpaca_py-0.9.0/alpaca/trading/enums.py
+-rw-r--r--   0        0        0    25878 2023-08-02 17:04:21.642014 alpaca_py-0.9.0/alpaca/trading/models.py
+-rw-r--r--   0        0        0    19359 2023-08-02 17:04:21.642242 alpaca_py-0.9.0/alpaca/trading/requests.py
+-rw-r--r--   0        0        0     7505 2023-04-18 01:08:49.991982 alpaca_py-0.9.0/alpaca/trading/stream.py
+-rw-r--r--   0        0        0      915 2023-08-02 17:04:58.539351 alpaca_py-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 alpaca_py-0.9.0/PKG-INFO
```

### Comparing `alpaca_py-0.8.2/LICENSE` & `alpaca_py-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/README.md` & `alpaca_py-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/broker/client.py` & `alpaca_py-0.9.0/alpaca/broker/client.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/broker/enums.py` & `alpaca_py-0.9.0/alpaca/broker/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,16 @@
     IDENTITY_VERIFICATION = "identity_verification"
     ADDRESS_VERIFICATION = "address_verification"
     DATE_OF_BIRTH_VERIFICATION = "date_of_birth_verification"
     TAX_ID_VERIFICATION = "tax_id_verification"
     ACCOUNT_APPROVAL_LETTER = "account_approval_letter"
     LIMITED_TRADING_AUTHORIZATION = "limited_trading_authorization"
     W8BEN = "w8ben"
+    SOCIAL_SECURITY_NUMBER_VERIFICATION = "social_security_number_verification"
+    NULL = ""
 
 
 class AccountEntities(str, Enum):
     """
     An enum representing the different fields to query for when listing accounts.
 
     ie: asking for CONTACT and IDENTITY will have the api fill those fields when returning the list of Accounts however
```

### Comparing `alpaca_py-0.8.2/alpaca/broker/models/accounts.py` & `alpaca_py-0.9.0/alpaca/broker/models/accounts.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/broker/models/cip.py` & `alpaca_py-0.9.0/alpaca/broker/models/cip.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/broker/models/documents.py` & `alpaca_py-0.9.0/alpaca/broker/models/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,25 @@
         document_type (DocumentType): The type of document uploaded
         document_sub_type (Optional[str]): The specific type of document, e.g. passport
         name (Optional(str)): Name of the document if present
         content (str): Base64 string representing the document
         mime_type (str): The format of content encoded by the string
     """
 
-    id: UUID
-    document_type: DocumentType
+    id: Optional[UUID]
+    document_type: Optional[DocumentType]
     document_sub_type: Optional[str] = None
-    content: str
+    content: Optional[str]
     mime_type: Optional[str] = None
 
     def __init__(self, **data: Any) -> None:
         # validate the incoming id field for uuid
-        if isinstance(data["id"], str):
-            data["id"] = UUID(data["id"])
+        _id = data.get("id", None)
+        if isinstance(_id, str):
+            data["id"] = UUID(_id)
 
         super().__init__(**data)
 
 
 class TradeDocument(BaseModel):
     """
     Similar to the AccountDocument model but this represents documents having to do with a TradeAccount not a regular
```

### Comparing `alpaca_py-0.8.2/alpaca/broker/models/funding.py` & `alpaca_py-0.9.0/alpaca/broker/models/funding.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/broker/models/journals.py` & `alpaca_py-0.9.0/alpaca/broker/models/journals.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/broker/requests.py` & `alpaca_py-0.9.0/alpaca/broker/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/common/enums.py` & `alpaca_py-0.9.0/alpaca/common/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/common/exceptions.py` & `alpaca_py-0.9.0/alpaca/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/common/requests.py` & `alpaca_py-0.9.0/alpaca/common/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/common/rest.py` & `alpaca_py-0.9.0/alpaca/common/rest.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/common/utils.py` & `alpaca_py-0.9.0/alpaca/common/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/common/websocket.py` & `alpaca_py-0.9.0/alpaca/common/websocket.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/enums.py` & `alpaca_py-0.9.0/alpaca/data/enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -88,7 +88,35 @@
     Crypto location
 
     Attributes:
         US (str): United States crypto feed
     """
 
     US = "us"
+
+
+class MostActivesBy(str, Enum):
+    """
+    Most actives possible filters.
+
+    Attributes:
+        volume (str):
+            Retrieve most actives by trading volume.
+        trades (str):
+            Retrieve most actives by number of trades.
+    """
+
+    VOLUME = "volume"
+    TRADES = "trades"
+
+
+class MarketType(str, Enum):
+    """
+    Most actives possible filters.
+
+    Attributes:
+        stocks (str)
+        crypto (str)
+    """
+
+    STOCKS = "stocks"
+    CRYPTO = "crypto"
```

### Comparing `alpaca_py-0.8.2/alpaca/data/historical/crypto.py` & `alpaca_py-0.9.0/alpaca/data/historical/crypto.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/historical/stock.py` & `alpaca_py-0.9.0/alpaca/data/historical/stock.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/historical/utils.py` & `alpaca_py-0.9.0/alpaca/data/historical/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/live/crypto.py` & `alpaca_py-0.9.0/alpaca/data/live/crypto.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/live/stock.py` & `alpaca_py-0.9.0/alpaca/data/live/stock.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/mappings.py` & `alpaca_py-0.9.0/alpaca/data/mappings.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/models/bars.py` & `alpaca_py-0.9.0/alpaca/data/models/bars.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/models/base.py` & `alpaca_py-0.9.0/alpaca/data/models/base.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/models/orderbooks.py` & `alpaca_py-0.9.0/alpaca/data/models/orderbooks.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/models/quotes.py` & `alpaca_py-0.9.0/alpaca/data/models/quotes.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/models/snapshots.py` & `alpaca_py-0.9.0/alpaca/data/models/snapshots.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/models/trades.py` & `alpaca_py-0.9.0/alpaca/data/models/trades.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/data/requests.py` & `alpaca_py-0.9.0/alpaca/data/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import Optional, Union, List, Any
 import pytz
 from alpaca.common.enums import SupportedCurrencies
 from alpaca.common.requests import NonEmptyRequest
-from alpaca.data.enums import Adjustment, DataFeed
+from alpaca.data.enums import Adjustment, DataFeed, MarketType, MostActivesBy
 from alpaca.data.timeframe import TimeFrame
 
 
 class BaseTimeseriesDataRequest(NonEmptyRequest):
     """
     A base class for requests for time series data between a start and an end. This shouldn't be
     instantiated directly. Instead, you should use one of the data type specific classes.
@@ -311,7 +311,45 @@
     This request class is used to submit a request for latest orderbook data for crypto.
 
     Attributes:
         symbol_or_symbols (Union[str, List[str]]): The ticker identifier or list of ticker identifiers.
     """
 
     symbol_or_symbols: Union[str, List[str]]
+
+
+# ############################## Screener #################################### #
+
+
+class ScreenerRequest(NonEmptyRequest):
+    """
+    This request class is used to submit a request for screener endpoints.
+
+    Attributes:
+        top (int): Number of top most active stocks to fetch per day.
+    """
+
+    top: int = 10
+
+
+class MostActivesRequest(ScreenerRequest):
+    """
+    This request class is used to submit a request for most actives screener endpoint.
+
+    Attributes:
+        by (MostActivesBy): The metric used for ranking the most active stocks.
+        top (int): Number of top most active stocks to fetch per day.
+    """
+
+    by: MostActivesBy = MostActivesBy.VOLUME
+
+
+class MarketMoversRequest(ScreenerRequest):
+    """
+    This request class is used to submit a request for most actives screener endpoint.
+
+    Attributes:
+        market_type (MarketType): Screen specific market (stocks or crypto).
+        top (int): Number of top most active stocks to fetch per day.
+    """
+
+    market_type: MarketType = MarketType.STOCKS
```

### Comparing `alpaca_py-0.8.2/alpaca/data/timeframe.py` & `alpaca_py-0.9.0/alpaca/data/timeframe.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/trading/client.py` & `alpaca_py-0.9.0/alpaca/trading/client.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/trading/enums.py` & `alpaca_py-0.9.0/alpaca/trading/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/alpaca/trading/models.py` & `alpaca_py-0.9.0/alpaca/trading/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         name (Optional[str]): The name of the asset.
         status (AssetStatus): The active status of the asset.
         tradable (bool): Whether the asset can be traded.
         marginable (bool): Whether the asset can be traded on margin.
         shortable (bool): Whether the asset can be shorted.
         easy_to_borrow (bool): When shorting, whether the asset is easy to borrow
         fractionable (bool): Whether fractional shares are available
+        attributes (bool): One of ptp_no_exception or ptp_with_exception. It will include unique characteristics of the asset here.
     """
 
     id: UUID
     asset_class: AssetClass = Field(
         alias="class"
     )  # using a pydantic alias to allow parsing data with the `class` keyword field
     exchange: AssetExchange
@@ -60,14 +61,15 @@
     shortable: bool
     easy_to_borrow: bool
     fractionable: bool
     min_order_size: Optional[float] = None
     min_trade_increment: Optional[float] = None
     price_increment: Optional[float] = None
     maintenance_margin_requirement: Optional[float] = None
+    attributes: Optional[list] = None
 
 
 class USDPositionValues(BaseModel):
     """
     Represents an open long or short holding in an asset in USD.
 
     Attributes:
@@ -535,23 +537,25 @@
         dtbp_check (DTBPCheck): Day Trade Buying Power Check. Controls Day Trading Margin Call (DTMC) checks.
         fractional_trading (bool): If true, account is able to participate in fractional trading
         max_margin_multiplier (str): A number between 1-4 that represents your max margin multiplier
         no_shorting (bool): If true then Account becomes long-only mode.
         pdt_check (PDTCheck): Controls Pattern Day Trader (PDT) checks.
         suspend_trade (bool): If true Account becomes unable to submit new orders
         trade_confirm_email (TradeConfirmationEmail): Controls whether Trade confirmation emails are sent.
+        ptp_no_exception_entry (bool): If set to true then Alpaca will accept orders for PTP symbols with no exception. Default is false.
     """
 
     dtbp_check: DTBPCheck
     fractional_trading: bool
     max_margin_multiplier: str
     no_shorting: bool
     pdt_check: PDTCheck
     suspend_trade: bool
     trade_confirm_email: TradeConfirmationEmail
+    ptp_no_exception_entry: bool
 
 
 class CorporateActionAnnouncement(BaseModel):
     """
     An announcement of a corporate action. Corporate actions are events like dividend payouts, mergers and stock splits.
 
     Attributes:
@@ -576,16 +580,16 @@
 
     id: UUID
     corporate_action_id: str
     ca_type: CorporateActionType
     ca_sub_type: CorporateActionSubType
     initiating_symbol: str
     initiating_original_cusip: str
-    target_symbol: str
-    target_original_cusip: str
+    target_symbol: Optional[str]
+    target_original_cusip: Optional[str]
     declaration_date: Optional[date]
     ex_date: Optional[date]
     record_date: date
     payable_date: date
     cash: float
     old_rate: float
     new_rate: float
```

### Comparing `alpaca_py-0.8.2/alpaca/trading/requests.py` & `alpaca_py-0.9.0/alpaca/trading/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,19 +117,21 @@
     """
     When querying for available assets, this model provides the parameters that can be filtered by.
 
     Attributes:
         status (Optional[AssetStatus]): The active status of the asset.
         asset_class (Optional[AssetClass]): The type of asset (i.e. us_equity, crypto).
         exchange (Optional[AssetExchange]): The exchange the asset trades on.
+        attributes (Optional[str]): Comma separated values to query for more than one attribute.
     """
 
     status: Optional[AssetStatus]
     asset_class: Optional[AssetClass]
     exchange: Optional[AssetExchange]
+    attributes: Optional[str]
 
 
 class TakeProfitRequest(NonEmptyRequest):
     """
     Used for providing take profit details for a bracket order.
 
     Attributes:
```

### Comparing `alpaca_py-0.8.2/alpaca/trading/stream.py` & `alpaca_py-0.9.0/alpaca/trading/stream.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.2/pyproject.toml` & `alpaca_py-0.9.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "alpaca-py"
-version = "0.8.2"
+version = "0.9.0"
 description = "The Official Python SDK for Alpaca APIs"
 authors = [
     "Rahul Chowdhury <rahul.chowdhury@alpaca.markets>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/alpacahq/alpaca-py"
 documentation = "https://alpaca.markets/docs/python-sdk/"
 packages = [
     { include = "alpaca" }
 ]
 include = [ "alpaca/py.typed" ]
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-requests = "^2.27.1"
+python = "^3.8.0"
+requests = "^2.30.0"
 pydantic = "^1.9.0"
-pandas = "^1.3.5"
+pandas = "^2.0.0"
 msgpack = "^1.0.3"
 websockets = "^10.2"
 sseclient-py = "^1.7.2"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
@@ -33,9 +33,9 @@
 furo = "^2022.2.14"
 Sphinx = "^5.0.1"
 sphinx-copybutton = "^0.5.0"
 enum-tools = "^0.9.0"
 sphinx-toolbox = "^3.1.2"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.4.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alpaca_py-0.8.2/PKG-INFO` & `alpaca_py-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: alpaca-py
-Version: 0.8.2
+Version: 0.9.0
 Summary: The Official Python SDK for Alpaca APIs
 Home-page: https://github.com/alpacahq/alpaca-py
 License: Apache-2.0
 Author: Rahul Chowdhury
 Author-email: rahul.chowdhury@alpaca.markets
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: msgpack (>=1.0.3,<2.0.0)
-Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
 Requires-Dist: websockets (>=10.2,<11.0)
 Project-URL: Documentation, https://alpaca.markets/docs/python-sdk/
 Project-URL: Repository, https://github.com/alpacahq/alpaca-py
 Description-Content-Type: text/markdown
 
 [![Alpaca-py](https://github.com/alpacahq/alpaca-py/blob/master/docs/images/alpaca-py-banner.png?raw=true)](https://alpaca.markets/docs/python-sdk)
```

