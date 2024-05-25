# Comparing `tmp/py_alpaca_api-0.5.6.tar.gz` & `tmp/py_alpaca_api-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.5.6.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.5.8.tar", max compression
```

## Comparing `py_alpaca_api-0.5.6.tar` & `py_alpaca_api-0.5.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.6/LICENSE
--rw-r--r--   0        0        0    16791 2024-05-19 11:02:34.884010 py_alpaca_api-0.5.6/README.md
--rw-r--r--   0        0        0        0 2024-05-19 01:27:26.322892 py_alpaca_api-0.5.6/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2490 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     4672 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.6/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     3789 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    20726 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.6/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     8341 2024-05-23 02:44:37.096464 py_alpaca_api-0.5.6/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2141 2024-05-20 23:00:54.419417 py_alpaca_api-0.5.6/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    13186 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0    14989 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.6/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     8824 2024-05-22 22:57:11.657657 py_alpaca_api-0.5.6/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    14951 2024-05-20 02:57:54.840513 py_alpaca_api-0.5.6/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1344 2024-05-23 02:45:38.106461 py_alpaca_api-0.5.6/pyproject.toml
--rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-24 01:31:49.350968 py_alpaca_api-0.5.8/LICENSE
+-rw-r--r--   0        0        0    16791 2024-05-24 01:31:49.350968 py_alpaca_api-0.5.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-24 01:31:49.354302 py_alpaca_api-0.5.8/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-24 01:31:49.354302 py_alpaca_api-0.5.8/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6216 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     3324 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    22112 2024-05-24 02:26:00.502180 py_alpaca_api-0.5.8/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     8465 2024-05-24 02:26:07.905556 py_alpaca_api-0.5.8/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2985 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    13542 2024-05-24 02:26:23.698984 py_alpaca_api-0.5.8/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0    13633 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     9202 2024-05-24 02:26:38.579074 py_alpaca_api-0.5.8/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    15411 2024-05-24 02:24:59.025171 py_alpaca_api-0.5.8/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1344 2024-05-25 16:14:06.398947 py_alpaca_api-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0    17593 1970-01-01 00:00:00.000000 py_alpaca_api-0.5.8/PKG-INFO
```

### Comparing `py_alpaca_api-0.5.6/LICENSE` & `py_alpaca_api-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.6/README.md` & `py_alpaca_api-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.5.6/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.5.8/py_alpaca_api/src/asset.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,51 +63,35 @@
         else:
             raise ValueError(f"Failed to get asset information. Response: {response.text}")
 
     #####################################################
     # \\\\\\\\\\\\\\\\\\\  Get Asset ////////////////////#
     #####################################################
     def get(self, symbol: str) -> AssetClass:
-        """Get asset information from Alpaca API
+        """
+        Gets the asset information for a given symbol using the Alpaca API.
 
-        Parameters:
-        ___________
-        symbol: str
-                Asset symbol required
+        Args:
+            symbol (str): The symbol of the asset.
 
         Returns:
-        ________
-        AssetClass: Asset information as an AssetClass object
+            AssetClass: The asset information as an AssetClass object.
 
         Raises:
-        _______
-        ValueError: If the response is not successful
+            ValueError: If the request to the Alpaca API fails.
 
         Example:
-        ________
-        >>> from py_alpaca_api.alpaca import PyAlpacaApi
-            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-            asset = api.asset.get(symbol="AAPL")
-            print(asset)
-
-        AssetClass(
-            asset_id="375f6b6e-3b5f-4b2b-8f6b-2e6b2a6b2e6b",
-            class="us_equity",
-            easy_to_borrow=True,
-            exchange="NASDAQ",
-            id="375f6b6e-3b5f-4b2b-8f6b-2e6b2a6b2e6b",
-            marginable=True,
-            name="Apple Inc",
-            shortable=True,
-            status="active",
-            symbol="AAPL",
-            tradable=True
-        )
-        """  # noqa
-
+            >>> asset = self.get("AAPL")
+            >>> asset.symbol
+            'AAPL'
+            >>> asset.name
+            'Apple Inc.'
+            >>> asset.exchange
+            'NASDAQ'
+        """
         # Alpaca API URL for asset information
         url = f"{self.trade_url}/assets/{symbol}"
         # Get request to Alpaca API for asset information
         response = requests.get(url, headers=self.headers)
         # Check if response is successful
         if response.status_code == 200:
             # Convert JSON response to dictionary
```

### Comparing `py_alpaca_api-0.5.6/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.5.8/py_alpaca_api/src/data_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -301,15 +301,17 @@
     name: str
     assets: object
 
 
 def watchlist_class_from_dict(data_dict: dict) -> WatchlistClass:
     return WatchlistClass(
         id=str(data_dict["id"] if data_dict["id"] else ""),
-        account_id=str(data_dict["account_id"] if data_dict["account_id"] else ""),
+        account_id=str(
+            data_dict["account_id"] if data_dict["account_id"] else ""
+        ),
         created_at=(
             datetime.strptime(
                 data_dict["created_at"].split(".")[0].replace("T", " "),
                 "%Y-%m-%d %H:%M:%S",
             )
             if data_dict["created_at"]
             else datetime.date(0, 0, 0)
@@ -319,15 +321,23 @@
                 data_dict["updated_at"].split(".")[0].replace("T", " "),
                 "%Y-%m-%d %H:%M:%S",
             )
             if data_dict["updated_at"]
             else datetime.date(0, 0, 0)
         ),
         name=str(data_dict["name"] if data_dict["name"] else ""),
-        assets=([asset_class_from_dict(sym) for sym in data_dict["assets"] if len(data_dict["assets"]) > 0] if data_dict["assets"] else None),
+        assets=(
+            [
+                asset_class_from_dict(sym)
+                for sym in data_dict["assets"]
+                if len(data_dict["assets"]) > 0
+            ]
+            if data_dict["assets"]
+            else None
+        ),
     )
 
 
 ############################################
 # Data Class Clock Conversion Functions
 ############################################
 def clock_class_from_dict(data_dict: dict) -> ClockClass:
@@ -359,15 +369,17 @@
                 "%Y-%m-%d %H:%M:%S",
             )
             if data_dict["next_open"]
             else datetime.date(0, 0, 0)
         ),
         next_close=(
             datetime.strptime(
-                data_dict["next_close"].replace("-04:00", "").replace("T", " "),
+                data_dict["next_close"]
+                .replace("-04:00", "")
+                .replace("T", " "),
                 "%Y-%m-%d %H:%M:%S",
             )
             if data_dict["next_close"]
             else datetime.date(0, 0, 0)
         ),
     )
 
@@ -423,58 +435,138 @@
     AccountClass
         An AccountClass object.
     """  # noqa
     return AccountClass(
         id=str(data_dict["id"] if data_dict["id"] else ""),
         account_number=str(data_dict["account_number"]),
         status=str(data_dict["status"] if data_dict["status"] else ""),
-        crypto_status=str(data_dict["crypto_status"] if data_dict["crypto_status"] else ""),
-        options_approved_level=int(data_dict["options_approved_level"] if data_dict["options_approved_level"] else 0),
-        options_trading_level=int(data_dict["options_trading_level"] if data_dict["options_trading_level"] else 0),
+        crypto_status=str(
+            data_dict["crypto_status"] if data_dict["crypto_status"] else ""
+        ),
+        options_approved_level=int(
+            data_dict["options_approved_level"]
+            if data_dict["options_approved_level"]
+            else 0
+        ),
+        options_trading_level=int(
+            data_dict["options_trading_level"]
+            if data_dict["options_trading_level"]
+            else 0
+        ),
         currency=str(data_dict["currency"] if data_dict["currency"] else ""),
-        buying_power=float(data_dict["buying_power"] if data_dict["buying_power"] else 0),
-        regt_buying_power=float(data_dict["regt_buying_power"] if data_dict["regt_buying_power"] else 0),
-        daytrading_buying_power=float(data_dict["daytrading_buying_power"] if data_dict["daytrading_buying_power"] else 0),
-        effective_buying_power=float(data_dict["effective_buying_power"] if data_dict["effective_buying_power"] else 0),
-        non_marginable_buying_power=float(data_dict["non_marginable_buying_power"] if data_dict["non_marginable_buying_power"] else 0),
-        options_buying_power=float(data_dict["options_buying_power"] if data_dict["options_buying_power"] else 0),
+        buying_power=float(
+            data_dict["buying_power"] if data_dict["buying_power"] else 0
+        ),
+        regt_buying_power=float(
+            data_dict["regt_buying_power"]
+            if data_dict["regt_buying_power"]
+            else 0
+        ),
+        daytrading_buying_power=float(
+            data_dict["daytrading_buying_power"]
+            if data_dict["daytrading_buying_power"]
+            else 0
+        ),
+        effective_buying_power=float(
+            data_dict["effective_buying_power"]
+            if data_dict["effective_buying_power"]
+            else 0
+        ),
+        non_marginable_buying_power=float(
+            data_dict["non_marginable_buying_power"]
+            if data_dict["non_marginable_buying_power"]
+            else 0
+        ),
+        options_buying_power=float(
+            data_dict["options_buying_power"]
+            if data_dict["options_buying_power"]
+            else 0
+        ),
         bod_dtbp=float(data_dict["bod_dtbp"] if data_dict["bod_dtbp"] else 0),
         cash=float(data_dict["cash"] if data_dict["cash"] else 0),
-        accrued_fees=float(data_dict["accrued_fees"] if data_dict["accrued_fees"] else 0),
-        pending_transfer_in=float(data_dict["pending_transfer_in"] if data_dict["pending_transfer_in"] else 0),
-        portfolio_value=float(data_dict["portfolio_value"] if data_dict["portfolio_value"] else 0),
+        accrued_fees=float(
+            data_dict["accrued_fees"] if data_dict["accrued_fees"] else 0
+        ),
+        pending_transfer_in=float(
+            data_dict["pending_transfer_in"]
+            if data_dict["pending_transfer_in"]
+            else 0
+        ),
+        portfolio_value=float(
+            data_dict["portfolio_value"] if data_dict["portfolio_value"] else 0
+        ),
         pattern_day_trader=bool(data_dict["pattern_day_trader"]),
         trading_blocked=bool(data_dict["trading_blocked"]),
         transfers_blocked=bool(data_dict["transfers_blocked"]),
         account_blocked=bool(data_dict["account_blocked"]),
         created_at=(
             datetime.strptime(
                 data_dict["created_at"].split(".")[0].replace("T", " "),
                 "%Y-%m-%d %H:%M:%S",
             )
             if data_dict["created_at"]
             else datetime.date(0, 0, 0)
         ),
         trade_suspended_by_user=bool(data_dict["trade_suspended_by_user"]),
-        multiplier=int(data_dict["multiplier"] if data_dict["multiplier"] else 0),
+        multiplier=int(
+            data_dict["multiplier"] if data_dict["multiplier"] else 0
+        ),
         shorting_enabled=bool(data_dict["shorting_enabled"]),
         equity=float(data_dict["equity"] if data_dict["equity"] else 0),
-        last_equity=float(data_dict["last_equity"] if data_dict["last_equity"] else 0),
-        long_market_value=float(data_dict["long_market_value"] if data_dict["long_market_value"] else 0),
-        short_market_value=float(data_dict["short_market_value"] if data_dict["short_market_value"] else 0),
-        position_market_value=float(data_dict["position_market_value"] if data_dict["position_market_value"] else 0),
-        initial_margin=float(data_dict["initial_margin"] if data_dict["initial_margin"] else 0),
-        maintenance_margin=float(data_dict["maintenance_margin"] if data_dict["maintenance_margin"] else 0),
-        last_maintenance_margin=float(data_dict["last_maintenance_margin"] if data_dict["last_maintenance_margin"] else 0),
+        last_equity=float(
+            data_dict["last_equity"] if data_dict["last_equity"] else 0
+        ),
+        long_market_value=float(
+            data_dict["long_market_value"]
+            if data_dict["long_market_value"]
+            else 0
+        ),
+        short_market_value=float(
+            data_dict["short_market_value"]
+            if data_dict["short_market_value"]
+            else 0
+        ),
+        position_market_value=float(
+            data_dict["position_market_value"]
+            if data_dict["position_market_value"]
+            else 0
+        ),
+        initial_margin=float(
+            data_dict["initial_margin"] if data_dict["initial_margin"] else 0
+        ),
+        maintenance_margin=float(
+            data_dict["maintenance_margin"]
+            if data_dict["maintenance_margin"]
+            else 0
+        ),
+        last_maintenance_margin=float(
+            data_dict["last_maintenance_margin"]
+            if data_dict["last_maintenance_margin"]
+            else 0
+        ),
         sma=float(data_dict["sma"] if data_dict["sma"] else 0),
-        daytrade_count=int(data_dict["daytrade_count"] if data_dict["daytrade_count"] else 0),
-        balance_asof=str(data_dict["balance_asof"] if data_dict["balance_asof"] else ""),
-        crypto_tier=int(data_dict["crypto_tier"] if data_dict["crypto_tier"] else 0),
-        intraday_adjustments=int(data_dict["intraday_adjustments"] if data_dict["intraday_adjustments"] else 0),
-        pending_reg_taf_fees=float(data_dict["pending_reg_taf_fees"] if data_dict["pending_reg_taf_fees"] else 0),
+        daytrade_count=int(
+            data_dict["daytrade_count"] if data_dict["daytrade_count"] else 0
+        ),
+        balance_asof=str(
+            data_dict["balance_asof"] if data_dict["balance_asof"] else ""
+        ),
+        crypto_tier=int(
+            data_dict["crypto_tier"] if data_dict["crypto_tier"] else 0
+        ),
+        intraday_adjustments=int(
+            data_dict["intraday_adjustments"]
+            if data_dict["intraday_adjustments"]
+            else 0
+        ),
+        pending_reg_taf_fees=float(
+            data_dict["pending_reg_taf_fees"]
+            if data_dict["pending_reg_taf_fees"]
+            else 0
+        ),
     )
 
 
 ############################################
 # Data Class Asset Conversion Functions
 ############################################
 def asset_class_from_dict(data_dict: dict) -> AssetClass:
@@ -492,15 +584,19 @@
     """  # noqa
     return AssetClass(
         id=str(data_dict["id"]) if data_dict["id"] else "",
         asset_class=str(data_dict["class"]) if data_dict["class"] else "",
         easy_to_borrow=bool(data_dict["easy_to_borrow"]),
         exchange=str(data_dict["exchange"]) if data_dict["exchange"] else "",
         fractionable=bool(data_dict["fractionable"]),
-        maintenance_margin_requirement=(float(data_dict["maintenance_margin_requirement"]) if data_dict["maintenance_margin_requirement"] else 0),
+        maintenance_margin_requirement=(
+            float(data_dict["maintenance_margin_requirement"])
+            if data_dict["maintenance_margin_requirement"]
+            else 0
+        ),
         marginable=bool(data_dict["marginable"]),
         name=str(data_dict["name"]) if data_dict["name"] else "",
         shortable=bool(data_dict["shortable"]),
         status=str(data_dict["status"]) if data_dict["status"] else "",
         symbol=str(data_dict["symbol"]) if data_dict["symbol"] else "",
         tradable=bool(data_dict["tradable"]),
     )
@@ -585,32 +681,56 @@
             datetime.strptime(
                 data_dict["replaced_at"].split(".")[0].replace("T", " "),
                 "%Y-%m-%d %H:%M:%S",
             )
             if data_dict["replaced_at"]
             else datetime(1, 1, 1, 0, 0)
         ),
-        replaced_by=str(data_dict["replaced_by"] if data_dict["replaced_by"] else ""),
+        replaced_by=str(
+            data_dict["replaced_by"] if data_dict["replaced_by"] else ""
+        ),
         replaces=str(data_dict["replaces"] if data_dict["replaces"] else ""),
         asset_id=str(data_dict["asset_id"] if data_dict["asset_id"] else ""),
         symbol=str(data_dict["symbol"] if data_dict["symbol"] else ""),
-        asset_class=str(data_dict["asset_class"] if data_dict["asset_class"] else ""),
+        asset_class=str(
+            data_dict["asset_class"] if data_dict["asset_class"] else ""
+        ),
         notional=float(data_dict["notional"] if data_dict["notional"] else 0),
         qty=float(data_dict["qty"] if data_dict["qty"] else 0),
-        filled_qty=float(data_dict["filled_qty"] if data_dict["filled_qty"] else 0),
-        filled_avg_price=float(data_dict["filled_avg_price"] if data_dict["filled_avg_price"] else 0),
-        order_class=str(data_dict["order_class"] if data_dict["order_class"] else ""),
-        order_type=str(data_dict["order_type"] if data_dict["order_type"] else ""),
+        filled_qty=float(
+            data_dict["filled_qty"] if data_dict["filled_qty"] else 0
+        ),
+        filled_avg_price=float(
+            data_dict["filled_avg_price"]
+            if data_dict["filled_avg_price"]
+            else 0
+        ),
+        order_class=str(
+            data_dict["order_class"] if data_dict["order_class"] else ""
+        ),
+        order_type=str(
+            data_dict["order_type"] if data_dict["order_type"] else ""
+        ),
         type=str(data_dict["type"] if data_dict["type"] else ""),
         side=str(data_dict["side"] if data_dict["side"] else ""),
-        time_in_force=str(data_dict["time_in_force"] if data_dict["time_in_force"] else ""),
-        limit_price=float(data_dict["limit_price"] if data_dict["limit_price"] else 0),
-        stop_price=float(data_dict["stop_price"] if data_dict["stop_price"] else 0),
+        time_in_force=str(
+            data_dict["time_in_force"] if data_dict["time_in_force"] else ""
+        ),
+        limit_price=float(
+            data_dict["limit_price"] if data_dict["limit_price"] else 0
+        ),
+        stop_price=float(
+            data_dict["stop_price"] if data_dict["stop_price"] else 0
+        ),
         status=str(data_dict["status"] if data_dict["status"] else ""),
         extended_hours=bool(data_dict["extended_hours"]),
         legs=data_dict["legs"] if data_dict["legs"] else {},
-        trail_percent=float(data_dict["trail_percent"] if data_dict["trail_percent"] else 0),
-        trail_price=float(data_dict["trail_price"] if data_dict["trail_price"] else 0),
+        trail_percent=float(
+            data_dict["trail_percent"] if data_dict["trail_percent"] else 0
+        ),
+        trail_price=float(
+            data_dict["trail_price"] if data_dict["trail_price"] else 0
+        ),
         hwm=float(data_dict["hwm"] if data_dict["hwm"] else 0),
         subtag=str(data_dict["subtag"] if data_dict["subtag"] else ""),
         source=str(data_dict["source"] if data_dict["source"] else ""),
     )
```

### Comparing `py_alpaca_api-0.5.6/py_alpaca_api/src/history.py` & `py_alpaca_api-0.5.8/py_alpaca_api/src/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import requests
 
 from .asset import Asset
 from .data_classes import AssetClass
 
 
 class History:
-    def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
+    def __init__(
+        self, data_url: str, headers: Dict[str, str], asset: Asset
+    ) -> None:
         """
         Args:
             data_url: A string representing the URL of the data.
             headers: A dictionary containing the headers to be included in the request.
             asset: An instance of the Asset class representing the asset.
 
         """
@@ -72,19 +74,23 @@
             "4h": "4Hour",
             "1d": "1Day",
             "1w": "1Week",
             "1M": "1Month",
         }
 
         if timeframe not in timeframe_mapping:
-            raise ValueError('Invalid timeframe. Must be "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1M"')
+            raise ValueError(
+                'Invalid timeframe. Must be "1m", "5m", "15m", "30m", "1h", "4h", "1d", "1w", or "1M"'
+            )
 
         # Parameters for historical stock data request
         params = {
-            "timeframe": timeframe_mapping[timeframe],  # Timeframe for historical data, default: 1d
+            "timeframe": timeframe_mapping[
+                timeframe
+            ],  # Timeframe for historical data, default: 1d
             "start": start,  # Start date for historical data
             "end": end,  # End date for historical data
             "currency": currency,  # Currency for historical data, default: USD
             "limit": limit,  # Limit number of data points, default: 1000
             "adjustment": adjustment,  # Adjustment for historical data, default: raw
             "feed": feed,  # Data feed source, default: iex
             "sort": sort,  # Sort order, default: asc
@@ -120,15 +126,17 @@
                 raise ValueError(f"{symbol} is not a stock.")
         return asset
 
     ###########################################
     # /////////// PreProcess Data \\\\\\\\\\\ #
     ###########################################
     @staticmethod
-    def preprocess_data(symbol_data: list[defaultdict], symbol: str) -> pd.DataFrame:
+    def preprocess_data(
+        symbol_data: list[defaultdict], symbol: str
+    ) -> pd.DataFrame:
         """Prepross data
         Preprocesses the given symbol data by converting it to a pandas DataFrame and performing various
         data transformations.
 
         Args:
             symbol_data: A list of defaultdict objects representing the JSON response data.
             symbol: A string representing the symbol or ticker for the stock data.
@@ -139,15 +147,17 @@
         """
         # Convert JSON response to dictionary
         bar_data_df = pd.DataFrame(symbol_data)
 
         # Add symbol column to DataFrame
         bar_data_df.insert(0, "symbol", symbol)
         # Reformat date column
-        bar_data_df["t"] = pd.to_datetime(bar_data_df["t"].replace("[A-Za-z]", " ", regex=True))
+        bar_data_df["t"] = pd.to_datetime(
+            bar_data_df["t"].replace("[A-Za-z]", " ", regex=True)
+        )
         # Rename columns for consistency
         bar_data_df.rename(
             columns={
                 "t": "date",
                 "o": "open",
                 "h": "high",
                 "l": "low",
@@ -174,15 +184,17 @@
         )
         # Return historical stock data as a DataFrame
         return bar_data_df
 
     ###########################################
     # ///////// Get Historical Data \\\\\\\\\ #
     ###########################################
-    def get_historical_data(self, symbol: str, url: str, params: dict) -> list[defaultdict]:
+    def get_historical_data(
+        self, symbol: str, url: str, params: dict
+    ) -> list[defaultdict]:
         """Get historical stock data
         Args:
             symbol (str): The symbol of the stock or asset for which historical data is being fetched.
             url (str): The URL of the API endpoint from where the historical data is being fetched.
             params (dict): Additional parameters to be passed along with the API request.
 
         Returns:
```

### Comparing `py_alpaca_api-0.5.6/py_alpaca_api/src/order.py` & `py_alpaca_api-0.5.8/py_alpaca_api/src/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,17 @@
             # Convert JSON response to dictionary
             res = json.loads(response.text)
             # Return order information as an OrderClass object
             return order_class_from_dict(res)
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise ValueError(f'Failed to get order information. Response: {res["message"]}')
+            raise ValueError(
+                f'Failed to get order information. Response: {res["message"]}'
+            )
 
     ########################################################
     # \\\\\\\\\\\\\\\\\ Cancel Order By ID /////////////////#
     ########################################################
     def cancel_by_id(self, order_id: str) -> str:
         """Cancel order by order ID
 
@@ -133,15 +135,17 @@
         # Check if response is successful
         if response.status_code == 204:
             # Convert JSON response to dictionary
             return f"Order {order_id} has been cancelled"
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise Exception(f'Failed to cancel order {order_id}, Response: {res["message"]}')
+            raise Exception(
+                f'Failed to cancel order {order_id}, Response: {res["message"]}'
+            )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Cancel All Orders //////////////////#
     ########################################################
     def cancel_all(self) -> str:
         """Cancel all orders
 
@@ -171,15 +175,17 @@
         if response.status_code == 207:
             # Convert JSON response to dictionary
             res = json.loads(response.text)
             return f"{len(res)} orders have been cancelled"
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise Exception(f'Failed to cancel orders. Response: {res["message"]}')
+            raise Exception(
+                f'Failed to cancel orders. Response: {res["message"]}'
+            )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Market Order ////////////////#
     ########################################################
     def market(
         self,
         symbol: str,
@@ -194,15 +200,21 @@
             raise ValueError("Must provide symbol for trading.")
 
         if not (qty or notional) or (qty and notional):
             raise ValueError("Qty or Notional are required, not both.")
 
         # Return market order using submit order method
         return self.__submit_order(
-            symbol=symbol, side=side, qty=qty, notional=notional, entry_type="market", time_in_force=time_in_force, extended_hours=extended_hours
+            symbol=symbol,
+            side=side,
+            qty=qty,
+            notional=notional,
+            entry_type="market",
+            time_in_force=time_in_force,
+            extended_hours=extended_hours,
         )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Limit Order /////////////////#
     ########################################################
     def limit(
         self,
@@ -254,15 +266,21 @@
         if not stop_price:
             raise ValueError("Must provide stop price for trading.")
 
         if not qty:
             raise ValueError("Qty is required.")
         # Return stop order
         return self.__submit_order(
-            symbol=symbol, side=side, stop_price=stop_price, qty=qty, entry_type="stop", time_in_force=time_in_force, extended_hours=extended_hours
+            symbol=symbol,
+            side=side,
+            stop_price=stop_price,
+            qty=qty,
+            entry_type="stop",
+            time_in_force=time_in_force,
+            extended_hours=extended_hours,
         )
 
     ########################################################
     # \\\\\\\\\\\\\\\\  Submit Stop Order /////////////////#
     ########################################################
     def stop_limit(
         self,
@@ -311,16 +329,23 @@
 
         if not symbol:
             raise ValueError("Must provide symbol for trading.")
 
         if not qty:
             raise ValueError("Qty is required.")
 
-        if trail_percent is None and trail_price is None or trail_percent and trail_price:
-            raise ValueError("Either trail_percent or trail_price must be provided, not both.")
+        if (
+            trail_percent is None
+            and trail_price is None
+            or trail_percent
+            and trail_price
+        ):
+            raise ValueError(
+                "Either trail_percent or trail_price must be provided, not both."
+            )
 
         if trail_percent:
             if trail_percent < 0:
                 raise ValueError("Trail percent must be greater than 0.")
 
         # Return trailing_stop
         return self.__submit_order(
@@ -375,8 +400,10 @@
             # Convert JSON response to dictionary
             res = json.loads(response.text)
             # Return order information as an OrderClass object
             return order_class_from_dict(res)
         # If response is not successful, raise an exception
         else:
             res = json.loads(response.text)
-            raise Exception(f'Failed to submit order. Code: {response.status_code}, Response: {res["message"]}')
+            raise Exception(
+                f'Failed to submit order. Code: {response.status_code}, Response: {res["message"]}'
+            )
```

### Comparing `py_alpaca_api-0.5.6/py_alpaca_api/src/position.py` & `py_alpaca_api-0.5.8/py_alpaca_api/src/position.py`

 * *Files 6% similar despite different names*

```diff
@@ -153,69 +153,30 @@
 
         return pos_data_df
 
     ########################################################
     # \\\\\\\\\\\\\\\\\ Get Position //////////////////////#
     ########################################################
     def get(self, symbol: str = None, symbol_dict: dict = None) -> PositionClass:
-        """Get position information by symbol or asset ID
+        """
+        Get position information for a specific symbol or from a provided symbol dictionary.
 
-        Parameters:
-        -----------
-        symbol:         Asset symbol to get position information
-                        A valid asset symbol string (optional) str
-
-        symbol_dict:    Asset symbol dictionary to get position information
-                        A valid asset symbol dictionary (optional) dict
+        Args:
+            symbol (str): The symbol for which to retrieve position information. Defaults to None.
+            symbol_dict (dict): A dictionary containing position information. Defaults to None.
 
         Returns:
-        --------
-        PositionClass:  Position information as a PositionClass object with attributes:
-                    asset_id, symbol, exchange, asset_class, avg_entry_price, qty, qty_available, side, market_value, cost_basis,
-                    profit_dol, profit_pct, intraday_profit_dol, intraday_profit_pct, portfolio_pct, current_price, lastday_price,
-                    change_today, asset_marginable
+            PositionClass: An object representing the position information.
 
         Raises:
-        -------
-        ValueError:     ValueError if symbol or symbol_dict is not provided
-
-        ValueError:     ValueError if both symbol and symbol_dict are provided
-
-        Exception:      Exception if failed to get position information
-
-        Example:
-        --------
-        >>> from py_alpaca_api.alpaca import PyAlpacaApi
-            api = PyAlpacaApi(api_key="API", api_secret="SECRET", api_paper=True)
-            position = api.position.get(symbol="AAPL")
-            print(position)
-
-        PositionClass(
-            asset_id="375f6b6e-3b5f-4b2b-8f6b-2e6b2a6b2e6b",
-            symbol="AAPL",
-            exchange="NASDAQ",
-            asset_class="us_equity",
-            avg_entry_price=100.0,
-            qty=10.0,
-            qty_available=10.0,
-            side="long",
-            market_value=1000.0,
-            cost_basis=1000.0,
-            profit_dol=0.0,
-            profit_pct=0.0,
-            intraday_profit_dol=0.0,
-            intraday_profit_pct=0.0,
-            portfolio_pct=0.1,
-            current_price=100.0,
-            lastday_price=100.0,
-            change_today=0.0,
-            asset_marginable=True
-        )
-        """  # noqa
+            ValueError: If neither symbol nor symbol_dict is provided.
+            ValueError: If both symbol and symbol_dict are provided.
+            ValueError: If the response from the Alpaca API is not successful.
 
+        """
         # Check if symbol or symbol_dict is provided
         if not symbol and not symbol_dict:
             # Raise ValueError if symbol or symbol_dict is not provided
             raise ValueError("Symbol or symbol_dict is required.")
         # Check if both symbol and symbol_dict are provided
         if symbol and symbol_dict:
             # Raise ValueError if both symbol and symbol_dict are provided
```

### Comparing `py_alpaca_api-0.5.6/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.5.8/py_alpaca_api/src/screener.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 MONDAY = pendulum.MONDAY
 TUESDAY = pendulum.TUESDAY
 FRIDAY = pendulum.FRIDAY
 THURSDAY = pendulum.THURSDAY
 
 
 class Screener:
-    def __init__(self, data_url: str, headers: Dict[str, str], asset: Asset) -> None:
+    def __init__(
+        self, data_url: str, headers: Dict[str, str], asset: Asset
+    ) -> None:
         """Initialize Screener class3
 
         Parameters:
         ___________
         data_url: str
                 Alpaca Data API URL required
 
@@ -71,21 +73,27 @@
             trade_count_greater_than=3000, total_losers_returned=50)
         """
         self.set_dates()
 
         print(f"Yesterday was {self.yesterday}")
         print(f"Day before yesterday was {self.day_before_yesterday}")
 
-        losers_df = self._get_percentages(start=self.day_before_yesterday, end=self.yesterday)
+        losers_df = self._get_percentages(
+            start=self.day_before_yesterday, end=self.yesterday
+        )
 
         losers_df = losers_df[losers_df["price"] > price_greater_than]
         losers_df = losers_df[losers_df["change"] < change_less_than]
         losers_df = losers_df[losers_df["volume"] > volume_greater_than]
         losers_df = losers_df[losers_df["trades"] > trade_count_greater_than]
-        return losers_df.sort_values(by="change", ascending=True).reset_index(drop=True).head(total_losers_returned)
+        return (
+            losers_df.sort_values(by="change", ascending=True)
+            .reset_index(drop=True)
+            .head(total_losers_returned)
+        )
 
     def gainers(
         self,
         price_greater_than: float = 5.0,
         change_greater_than: float = 2.0,
         volume_greater_than: int = 20000,
         trade_count_greater_than: int = 2000,
@@ -107,21 +115,29 @@
         Returns:
             pd.DataFrame: A DataFrame that contains the filtered gainers that satisfy the given thresholds.
             The DataFrame is sorted by the "change" column in descending order and is limited to the specified
             number of gainers.
         """
         self.set_dates()
 
-        gainers_df = self._get_percentages(start=self.day_before_yesterday, end=self.yesterday)
+        gainers_df = self._get_percentages(
+            start=self.day_before_yesterday, end=self.yesterday
+        )
 
         gainers_df = gainers_df[gainers_df["price"] > price_greater_than]
         gainers_df = gainers_df[gainers_df["change"] > change_greater_than]
         gainers_df = gainers_df[gainers_df["volume"] > volume_greater_than]
-        gainers_df = gainers_df[gainers_df["trades"] > trade_count_greater_than]
-        return gainers_df.sort_values(by="change", ascending=False).reset_index(drop=True).head(total_gainers_returned)
+        gainers_df = gainers_df[
+            gainers_df["trades"] > trade_count_greater_than
+        ]
+        return (
+            gainers_df.sort_values(by="change", ascending=False)
+            .reset_index(drop=True)
+            .head(total_gainers_returned)
+        )
 
     def _get_percentages(
         self,
         start: str,
         end: str,
         timeframe: str = "1Day",
     ) -> pd.DataFrame:
@@ -166,15 +182,17 @@
             res = json.loads(response.text)
 
             bars_df = pd.DataFrame.from_dict(res["bars"], orient="index")
             page_token = res["next_page_token"]
 
             while page_token:
                 params["page_token"] = page_token
-                response = requests.get(url, headers=self.headers, params=params)
+                response = requests.get(
+                    url, headers=self.headers, params=params
+                )
                 res = json.loads(response.text)
                 bars_df = pd.concat(
                     [
                         bars_df,
                         pd.DataFrame.from_dict(res["bars"], orient="index"),
                     ]
                 )
@@ -183,34 +201,39 @@
             bars_df.reset_index()
 
             all_bars_df = pd.DataFrame()
 
             for bar in bars_df.iterrows():
                 try:
                     change = round(
-                        ((bar[1][1]["c"] - bar[1][0]["c"]) / bar[1][0]["c"]) * 100,
+                        ((bar[1][1]["c"] - bar[1][0]["c"]) / bar[1][0]["c"])
+                        * 100,
                         2,
                     )
                     symbol = bar[0]
 
                     sym_data = {
                         "symbol": symbol,
                         "change": change,
                         "price": bar[1][1]["c"],
                         "volume": bar[1][1]["v"],
                         "trades": bar[1][1]["n"],
                     }
-                    all_bars_df = pd.concat([all_bars_df, pd.DataFrame([sym_data])])
+                    all_bars_df = pd.concat(
+                        [all_bars_df, pd.DataFrame([sym_data])]
+                    )
 
                 except Exception:
                     pass
             all_bars_df.reset_index(drop=True, inplace=True)
             return all_bars_df
         else:
-            raise ValueError(f"Failed to get assets. Response: {response.text}")
+            raise ValueError(
+                f"Failed to get assets. Response: {response.text}"
+            )
 
     @staticmethod
     def get_previous_date(current_date, day_to_look):
         """
         Get the previous date based on the day_to_look from the current_date.
         """
         return current_date.previous(day_to_look).strftime("%Y-%m-%d")
@@ -233,9 +256,13 @@
         if today.day_of_week in [SUNDAY, MONDAY]:
             self.yesterday = self.get_previous_date(today, FRIDAY)
             self.day_before_yesterday = self.get_previous_date(today, THURSDAY)
         elif today.day_of_week == TUESDAY:
             self.yesterday = self.get_previous_date(today, MONDAY)
             self.day_before_yesterday = self.get_previous_date(today, FRIDAY)
         else:
-            self.yesterday = self.get_previous_date(today, today.day_of_week - 1)
-            self.day_before_yesterday = self.get_previous_date(today, today.day_of_week - 2)
+            self.yesterday = self.get_previous_date(
+                today, today.day_of_week - 1
+            )
+            self.day_before_yesterday = self.get_previous_date(
+                today, today.day_of_week - 2
+            )
```

### Comparing `py_alpaca_api-0.5.6/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.5.8/py_alpaca_api/src/watchlist.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         self.trade_url = trade_url
         self.headers = headers
 
     ########################################################
     # ///////////// Helper functions //////////////////////#
     ########################################################
     @staticmethod
-    def _handle_response(response: dict, no_content_msg: str) -> Union[WatchlistClass, str]:
+    def _handle_response(
+        response: dict, no_content_msg: str
+    ) -> Union[WatchlistClass, str]:
         """
         Handles the response from the API and returns a WatchlistClass object
         if the response is not empty, otherwise returns the specified no_content_msg.
 
         Args:
             response (dict): The response from the API.
             no_content_msg (str): The message to return if the response is empty.
@@ -41,15 +43,17 @@
             return watchlist_class_from_dict(response)
         else:
             return no_content_msg
 
     ########################################################
     # ///////////// Send a request to the API //////////////#
     ########################################################
-    def _request(self, method: str, url: str, payload: dict = None, params: dict = None) -> Dict:
+    def _request(
+        self, method: str, url: str, payload: dict = None, params: dict = None
+    ) -> Dict:
         """
         Sends a request to the specified URL using the specified HTTP method.
 
         Args:
             method (str): The HTTP method to use for the request (e.g., 'GET', 'POST', 'PUT', 'DELETE').
             url (str): The URL to send the request to.
             payload (dict, optional): The payload to include in the request body. Defaults to None.
@@ -74,41 +78,49 @@
             return {}
         else:
             raise Exception(response.text)
 
     ########################################################
     # //////////////// Get a  watchlist ///////////////////#
     ########################################################
-    def get(self, watchlist_id: str = None, watchlist_name: str = None) -> WatchlistClass:
+    def get(
+        self, watchlist_id: str = None, watchlist_name: str = None
+    ) -> WatchlistClass:
         """
         Retrieves a watchlist based on the provided watchlist ID or name.
 
         Args:
             watchlist_id (str, optional): The ID of the watchlist to retrieve.
             watchlist_name (str, optional): The name of the watchlist to retrieve.
 
         Returns:
             WatchlistClass: The retrieved watchlist.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided, or if neither is provided.
 
         """
-        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
+        if (
+            watchlist_id
+            and watchlist_name
+            or (not watchlist_id and not watchlist_name)
+        ):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if watchlist_id:
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             url = f"{self.trade_url}/watchlists:by_name"
 
         params = {"name": watchlist_name} if watchlist_name else None
 
         response = self._request(method="GET", url=url, params=params)
-        return self._handle_response(response=response, no_content_msg="No watchlist was found.")
+        return self._handle_response(
+            response=response, no_content_msg="No watchlist was found."
+        )
 
     ########################################################
     # ///////////// Get all watchlists ////////////////////#
     ########################################################
     def get_all(self) -> list[WatchlistClass]:
         """
         Retrieves all watchlists.
@@ -153,15 +165,17 @@
         # Create the URL
         url = f"{self.trade_url}/watchlists"
         # Split the symbols and remove any spaces
         symbols = symbols.replace(" ", "").split(",") if symbols else []
 
         payload = {"symbols": symbols, "name": name}
         response = self._request(method="POST", url=url, payload=payload)
-        return self._handle_response(response=response, no_content_msg="The watchlist was not created.")
+        return self._handle_response(
+            response=response, no_content_msg="The watchlist was not created."
+        )
 
     ########################################################
     # ///////////// Update a watchlist ////////////////////#
     ########################################################
     def update(
         self,
         watchlist_id: str = None,
@@ -183,15 +197,19 @@
             WatchlistClass: The updated watchlist.
 
         Raises:
             ValueError: If both `watchlist_id` and `watchlist_name` are provided, or if neither `watchlist_id` nor `watchlist_name` are provided.
 
         """
         # Check if both watchlist_id and watchlist_name are provided and raise an error if they are
-        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
+        if (
+            watchlist_id
+            and watchlist_name
+            or (not watchlist_id and not watchlist_name)
+        ):
             raise ValueError("Watchlist ID or Name is required, not both.")
         # Check if watchlist_id is provided
         if watchlist_id:
             watchlist = self.get(watchlist_id=watchlist_id)
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             watchlist = self.get(watchlist_name=watchlist_name)
@@ -203,36 +221,46 @@
             symbols = symbols.replace(" ", "").split(",")
         else:
             symbols = ",".join([o.symbol for o in watchlist.assets])
 
         payload = {"name": name, "symbols": symbols}
         params = {"name": watchlist_name} if watchlist_name else None
 
-        response = self._request(method="PUT", url=url, payload=payload, params=params)
-        return self._handle_response(response=response, no_content_msg="The watchlist was not updated.")
+        response = self._request(
+            method="PUT", url=url, payload=payload, params=params
+        )
+        return self._handle_response(
+            response=response, no_content_msg="The watchlist was not updated."
+        )
 
     ########################################################
     # ///////////// Delete a watchlist ////////////////////#
     ########################################################
-    def delete(self, watchlist_id: str = None, watchlist_name: str = None) -> str:
+    def delete(
+        self, watchlist_id: str = None, watchlist_name: str = None
+    ) -> str:
         """
         Deletes a watchlist.
 
         Args:
             watchlist_id (str, optional): The ID of the watchlist to delete.
             watchlist_name (str, optional): The name of the watchlist to delete.
 
         Returns:
             str: A message indicating the successful deletion of the watchlist.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided or if neither is provided.
 
         """
-        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
+        if (
+            watchlist_id
+            and watchlist_name
+            or (not watchlist_id and not watchlist_name)
+        ):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if watchlist_id:
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             url = f"{self.trade_url}/watchlists:by_name"
 
@@ -263,29 +291,35 @@
 
         Returns:
             WatchlistClass: The updated watchlist object.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided, or if symbol is not provided.
         """
-        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
+        if (
+            watchlist_id
+            and watchlist_name
+            or (not watchlist_id and not watchlist_name)
+        ):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if not symbol:
             raise ValueError("Symbol is required")
 
         if watchlist_id:
             url = f"{self.trade_url}/watchlists/{watchlist_id}"
         else:
             url = f"{self.trade_url}/watchlists:by_name"
 
         params = {"name": watchlist_name} if watchlist_name else None
         payload = {"symbol": symbol}
 
-        response = self._request(method="POST", url=url, payload=payload, params=params)
+        response = self._request(
+            method="POST", url=url, payload=payload, params=params
+        )
         return self._handle_response(
             response=response,
             no_content_msg="Failed to add asset to watchlist.",
         )
 
     ########################################################
     # /////////// Remove a Asset from  watchlist //////////#
@@ -308,15 +342,19 @@
 
         Returns:
             WatchlistClass: The updated watchlist object.
 
         Raises:
             ValueError: If both watchlist_id and watchlist_name are provided, or if symbol is not provided.
         """
-        if watchlist_id and watchlist_name or (not watchlist_id and not watchlist_name):
+        if (
+            watchlist_id
+            and watchlist_name
+            or (not watchlist_id and not watchlist_name)
+        ):
             raise ValueError("Watchlist ID or Name is required, not both.")
 
         if not symbol:
             raise ValueError("Symbol is required")
 
         if not watchlist_id:
             watchlist_id = self.get(watchlist_name=watchlist_name).id
@@ -328,15 +366,17 @@
             response=response,
             no_content_msg="Failed to remove asset from watchlist.",
         )
 
     ########################################################
     # /////////// Get Assets from a watchlist /////////////#
     ########################################################
-    def get_assets(self, watchlist_id: str = None, watchlist_name: str = None) -> list:
+    def get_assets(
+        self, watchlist_id: str = None, watchlist_name: str = None
+    ) -> list:
         """
         Retrieves the symbols of assets in a watchlist.
 
         Args:
             watchlist_id (str, optional): The ID of the watchlist. Either `watchlist_id` or `watchlist_name` should be provided,
             not both. Defaults to None.
             watchlist_name (str, optional): The name of the watchlist. Either `watchlist_id` or `watchlist_name` should be
```

### Comparing `py_alpaca_api-0.5.6/pyproject.toml` & `py_alpaca_api-0.5.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.5.6"
+version = "0.5.8"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.5.6/PKG-INFO` & `py_alpaca_api-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.5.6
+Version: 0.5.8
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

