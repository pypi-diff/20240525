# Comparing `tmp/tinyticker-0.7.3.tar.gz` & `tmp/tinyticker-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.7.3.tar", max compression
+gzip compressed data, was "tinyticker-0.7.4.tar", max compression
```

## Comparing `tinyticker-0.7.3.tar` & `tinyticker-0.7.4.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0     1068 2024-05-24 13:56:27.147646 tinyticker-0.7.3/LICENSE
--rw-r--r--   0        0        0     3955 2024-05-24 13:56:27.147646 tinyticker-0.7.3/README.md
--rw-r--r--   0        0        0      917 2024-05-24 13:56:27.147646 tinyticker-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      465 2024-05-24 13:56:27.147646 tinyticker-0.7.3/tinyticker/__init__.py
--rw-r--r--   0        0        0     5967 2024-05-24 13:56:27.147646 tinyticker-0.7.3/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-24 13:56:27.147646 tinyticker-0.7.3/tinyticker/config.py
--rw-r--r--   0        0        0     9000 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/paths.py
--rw-r--r--   0        0        0     5483 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2915 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    21091 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in7.py
--rw-r--r--   0        0        0    19697 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1551 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2895 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     8457 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/app.py
--rw-r--r--   0        0        0     3656 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/command.py
--rw-r--r--   0        0        0      593 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/startup.py
--rw-r--r--   0        0        0   274777 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    14743 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-24 13:56:27.151646 tinyticker-0.7.3/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-24 13:56:27.155646 tinyticker-0.7.3/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-24 13:56:27.155646 tinyticker-0.7.3/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2449 2024-05-24 13:56:27.155646 tinyticker-0.7.3/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     3173 2024-05-24 13:56:27.155646 tinyticker-0.7.3/tinyticker/web/templates/startup.html
--rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-25 17:14:32.547655 tinyticker-0.7.4/LICENSE
+-rw-r--r--   0        0        0     3955 2024-05-25 17:14:32.547655 tinyticker-0.7.4/README.md
+-rw-r--r--   0        0        0      917 2024-05-25 17:14:32.547655 tinyticker-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      518 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/__init__.py
+-rw-r--r--   0        0        0     4712 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/config.py
+-rw-r--r--   0        0        0     4813 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/display.py
+-rw-r--r--   0        0        0     5247 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/layouts.py
+-rw-r--r--   0        0        0      345 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/paths.py
+-rw-r--r--   0        0        0     5483 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     2584 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-25 17:14:32.551655 tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1558 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2895 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     8428 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3656 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/command.py
+-rw-r--r--   0        0        0      593 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/startup.py
+-rw-r--r--   0        0        0   274777 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    14743 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2449 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     3173 2024-05-25 17:14:32.555655 tinyticker-0.7.4/tinyticker/web/templates/startup.html
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 tinyticker-0.7.4/PKG-INFO
```

### Comparing `tinyticker-0.7.3/LICENSE` & `tinyticker-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/README.md` & `tinyticker-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/pyproject.toml` & `tinyticker-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.7.3"
+version = "0.7.4"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.7.3/tinyticker/__main__.py` & `tinyticker-0.7.4/tinyticker/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from watchdog.observers import Observer
 
 from . import __version__, logger
 from .config import load_config_safe
 from .display import Display
 from .paths import CONFIG_FILE, PID_FILE
 from .sequence import Sequence
-from .tickers._base import TickerBase, TickerResponse
 from .utils import RawTextArgumentDefaultsHelpFormatter, set_verbosity
 
 
 def parse_args(args: List[str]) -> argparse.Namespace:
     """Parse the command line arguments."""
     parser = argparse.ArgumentParser(
         prog="tinyticker",
@@ -48,46 +47,14 @@
         help="Show the version and exit.",
         action="version",
         version="%(prog)s {version}".format(version=__version__),
     )
     return parser.parse_args(args)
 
 
-def show_ticker(ticker: TickerBase, resp: TickerResponse, display: Display):
-    delta_range_start = resp.historical.iloc[0]["Open"]
-    delta_range = 100 * (resp.current_price - delta_range_start) / delta_range_start
-
-    top_string = f"{ticker.config.symbol}: $ {resp.current_price:.2f}"
-    if ticker.config.avg_buy_price is not None:
-        # calculate the delta from the average buy price
-        delta_abp = (
-            100
-            * (resp.current_price - ticker.config.avg_buy_price)
-            / ticker.config.avg_buy_price
-        )
-        top_string += f" {delta_abp:+.2f}%"
-
-    xlim = None
-    # if incomplete data, leave space for the missing data
-    if len(resp.historical) < ticker.lookback:
-        # the floats are to leave padding left and right of the edge candles
-        xlim = (-0.75, ticker.lookback - 0.25)
-    logger.debug("xlim: %s", xlim)
-    display.plot(
-        resp.historical,
-        top_string=top_string,
-        sub_string=f"{len(resp.historical)}x{ticker.config.interval} {delta_range:+.2f}%",
-        show=True,
-        xlim=xlim,
-        type=ticker.config.plot_type,
-        mav=ticker.config.mav,
-        volume=ticker.config.volume,
-    )
-
-
 async def start_ticker(config_file: Path) -> None:
     """Start ticking.
 
     Args:
         config_file: config file path.
     """
     logger.info("Starting ticker process")
@@ -112,15 +79,15 @@
     sequence = Sequence.from_tinyticker_config(tt_config)
     logger.debug(sequence)
 
     try:
         async for ticker, resp in sequence.start():
             logger.debug("Ticker response len(historical): %s", len(resp.historical))
             logger.debug("Ticker response current_price: %s", resp.current_price)
-            show_ticker(ticker, resp, display)
+            display.show(ticker, resp)
     except Exception as exc:
         logger.error(exc, stack_info=True)
         display.text(
             f"Whoops something broke:\n{exc}",
             show=True,
             weight="bold",
             fontsize="small",
```

### Comparing `tinyticker-0.7.3/tinyticker/config.py` & `tinyticker-0.7.4/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/sequence.py` & `tinyticker-0.7.4/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/tickers/__init__.py` & `tinyticker-0.7.4/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/tickers/_base.py` & `tinyticker-0.7.4/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/tickers/crypto.py` & `tinyticker-0.7.4/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/tickers/stock.py` & `tinyticker-0.7.4/tinyticker/tickers/stock.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class TickerStock(TickerBase):
     @classmethod
     def from_config(cls, tt_config, ticker_config) -> "TickerStock":
         return TickerStock(ticker_config)
 
     def __init__(self, config) -> None:
         super().__init__(config)
+        self._yf_ticker = yfinance.Ticker(self.config.symbol)
 
     def _get_yfinance_start_end(self) -> Tuple[pd.Timestamp, pd.Timestamp]:
         end = utils.now()
         # depending on the interval we need to increase the time range to compensate for the market
         # being closed
         start = end - self.interval_dt * self.lookback
         if self.interval_dt < pd.to_timedelta("1d"):
@@ -38,38 +39,27 @@
         # max(0, start.weekday() - 4) is 0 for Mon-Fri, 1 for Sat, 2 for Sun
         start -= pd.to_timedelta("1d") * max(0, start.weekday() - 4)
         return (start, end)
 
     def _single_tick(self) -> Tuple[pd.DataFrame, Optional[float]]:
         LOGGER.info("Stock tick: %s", self.config.symbol)
         start, end = self._get_yfinance_start_end()
-        current_price_data: pd.DataFrame = yfinance.download(
-            self.config.symbol,
-            start=end - pd.to_timedelta("2m"),
-            end=end,
-            interval="1m",
-            prepost=self.config.prepost,
-            progress=False,
+        current_price: Optional[float] = self._yf_ticker.fast_info.get(
+            "lastPrice", None
         )
-        historical: pd.DataFrame = yfinance.download(
-            self.config.symbol,
+        historical = self._yf_ticker.history(
             start=start,
             end=end,
             interval=self.config.interval,
-            timeout=None,  # type: ignore
+            timeout=None,
             prepost=self.config.prepost,
-            progress=False,
         )
         if historical.empty:
             raise ValueError(
                 f"No historical data returned from yfinance API for {self.config.symbol}."
             )
-        if not current_price_data.empty:
-            current_price = current_price_data.iloc[-1]["Close"]
-        else:
-            current_price = None
         # drop the extra data
         if len(historical) > self.lookback:
             historical = historical.iloc[-self.lookback :]
         if historical.index.tzinfo is None:  # type: ignore
             historical.index = historical.index.tz_localize("utc")  # type: ignore
         return (historical, current_price)
```

### Comparing `tinyticker-0.7.3/tinyticker/utils.py` & `tinyticker-0.7.4/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/device.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in7.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.7.4/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/__main__.py` & `tinyticker-0.7.4/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/app.py` & `tinyticker-0.7.4/tinyticker/web/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,14 @@
 
     @app.errorhandler(500)
     def internal_error(_):
         sys.exit(1)
 
     @app.route("/startup/add", methods=["POST", "GET"])
     def upload_startup_script():
-        print(request.files)
         if request.method == "GET":
             return redirect("/startup")
 
         # this endpoint should receive the script and add it into the startup folder
         # the script should be run on startup
         # check if the post request has the file part
         for _, file in request.files.items():
```

### Comparing `tinyticker-0.7.3/tinyticker/web/command.py` & `tinyticker-0.7.4/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/startup.py` & `tinyticker-0.7.4/tinyticker/web/startup.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.7.4/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.7.4/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.7.4/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.7.4/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/index.html` & `tinyticker-0.7.4/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/js/index.js` & `tinyticker-0.7.4/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.7.4/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.7.4/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/logfiles.html` & `tinyticker-0.7.4/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/tinyticker/web/templates/startup.html` & `tinyticker-0.7.4/tinyticker/web/templates/startup.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.7.3/PKG-INFO` & `tinyticker-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.7.3
+Version: 0.7.4
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.7.3 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.7.4 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

