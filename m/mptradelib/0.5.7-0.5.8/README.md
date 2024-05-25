# Comparing `tmp/mptradelib-0.5.7.tar.gz` & `tmp/mptradelib-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.5.7.tar", max compression
+gzip compressed data, was "mptradelib-0.5.8.tar", max compression
```

## Comparing `mptradelib-0.5.7.tar` & `mptradelib-0.5.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.7/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.7/mptradelib/__init__.py
--rw-r--r--   0        0        0     4515 2024-05-21 20:24:35.631241 mptradelib-0.5.7/mptradelib/backtest.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.7/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0    11073 2024-05-09 18:27:16.773912 mptradelib-0.5.7/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.7/mptradelib/broker/session.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.7/mptradelib/broker/shoonya.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.7/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.7/mptradelib/cli/__init__.py
--rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.7/mptradelib/cli/new.py
--rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.7/mptradelib/cli/templates/strategy/__init__.py.jinja
--rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.7/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
--rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.7/mptradelib/cli/templates/strategy/livetrade.py.jinja
--rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.7/mptradelib/feed.py
--rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.7/mptradelib/livetrade.py
--rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.7/mptradelib/optimizers/__init__.py
--rw-r--r--   0        0        0     8569 2024-05-23 19:20:16.364263 mptradelib-0.5.7/mptradelib/optimizers/walkforward.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.7/mptradelib/test_renko.py
--rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.7/mptradelib/utils/__init__.py
--rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.7/mptradelib/utils/simulated_trades.py
--rw-r--r--   0        0        0    10818 2024-05-24 03:38:04.967978 mptradelib-0.5.7/mptradelib/utils/tearsheet.py
--rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.7/mptradelib/utils/utils.py
--rw-r--r--   0        0        0        0 2024-05-23 19:19:31.018101 mptradelib-0.5.7/mptradelib/widgets/__init__.py
--rw-r--r--   0        0        0     2005 2024-05-23 19:19:52.537757 mptradelib-0.5.7/mptradelib/widgets/daterangepicker.py
--rw-r--r--   0        0        0      822 2024-05-24 03:38:23.532168 mptradelib-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     3137 2024-05-03 13:20:41.913077 mptradelib-0.5.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.5.8/mptradelib/__init__.py
+-rw-r--r--   0        0        0     4786 2024-05-25 17:34:22.689097 mptradelib-0.5.8/mptradelib/backtest.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.5.8/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0    11072 2024-05-25 17:30:54.602294 mptradelib-0.5.8/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5808 2024-05-09 18:04:15.841857 mptradelib-0.5.8/mptradelib/broker/session.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.5.8/mptradelib/broker/shoonya.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.5.8/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0        0 2024-05-03 11:19:20.268249 mptradelib-0.5.8/mptradelib/cli/__init__.py
+-rw-r--r--   0        0        0     2342 2024-05-09 18:05:58.447254 mptradelib-0.5.8/mptradelib/cli/new.py
+-rw-r--r--   0        0        0      953 2024-05-09 18:11:12.323673 mptradelib-0.5.8/mptradelib/cli/templates/strategy/__init__.py.jinja
+-rw-r--r--   0        0        0     2984 2024-05-04 12:28:56.516490 mptradelib-0.5.8/mptradelib/cli/templates/strategy/backtest.ipynb.jinja
+-rw-r--r--   0        0        0      614 2024-05-03 12:29:43.201283 mptradelib-0.5.8/mptradelib/cli/templates/strategy/livetrade.py.jinja
+-rw-r--r--   0        0        0     5394 2024-05-09 18:03:46.504439 mptradelib-0.5.8/mptradelib/feed.py
+-rw-r--r--   0        0        0     2007 2024-05-09 18:25:26.040938 mptradelib-0.5.8/mptradelib/livetrade.py
+-rw-r--r--   0        0        0       36 2024-05-16 13:40:16.707824 mptradelib-0.5.8/mptradelib/optimizers/__init__.py
+-rw-r--r--   0        0        0     8569 2024-05-23 19:20:16.364263 mptradelib-0.5.8/mptradelib/optimizers/walkforward.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.5.8/mptradelib/test_renko.py
+-rw-r--r--   0        0        0       77 2024-05-06 16:16:12.200968 mptradelib-0.5.8/mptradelib/utils/__init__.py
+-rw-r--r--   0        0        0     1316 2024-05-25 17:35:22.328037 mptradelib-0.5.8/mptradelib/utils/downloader.py
+-rw-r--r--   0        0        0      902 2024-05-06 16:14:19.221626 mptradelib-0.5.8/mptradelib/utils/simulated_trades.py
+-rw-r--r--   0        0        0    10818 2024-05-24 03:38:04.967978 mptradelib-0.5.8/mptradelib/utils/tearsheet.py
+-rw-r--r--   0        0        0      910 2024-05-06 16:15:09.786235 mptradelib-0.5.8/mptradelib/utils/utils.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:19:31.018101 mptradelib-0.5.8/mptradelib/widgets/__init__.py
+-rw-r--r--   0        0        0     2005 2024-05-23 19:19:52.537757 mptradelib-0.5.8/mptradelib/widgets/daterangepicker.py
+-rw-r--r--   0        0        0      822 2024-05-25 17:35:29.870447 mptradelib-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3974 1970-01-01 00:00:00.000000 mptradelib-0.5.8/PKG-INFO
```

### Comparing `mptradelib-0.5.7/README.md` & `mptradelib-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/backtest.py` & `mptradelib-0.5.8/mptradelib/backtest.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,40 +15,50 @@
 
     def __init__(self, 
                  data: pd.DataFrame, 
                  compute: Callable[[pd.DataFrame, dict], 
                  pd.DataFrame]=None, 
                  tp=2, sl=1,
                  intraday_exit_time: dt.time = dt.time(15,10,0),
+                 exit_func: Callable[[pd.DataFrame, dict], None]=None,
                  intraday=True):
         self.data = data
         self.compute = compute
         self.params['tp'] = tp
         self.params['sl'] = sl
         self.intraday = intraday
         self.intraday_exit_time = intraday_exit_time
+        if exit_func is None:
+            self.exit_func = self._exit_func
+        else:
+            self.exit_func = exit_func
+
+            
+    def _exit_func(self, df: pd.DataFrame, params: dict):
+        df.loc[df.entries == 1, 'sl'] = df.close * (1 - params['sl']/100)
+        df.loc[df.entries == 1, 'tp'] = df.close * (1 + params['tp']/100)
+
+        df.loc[df.entries == -1, 'sl'] = df.close * (1 + params['sl']/100)
+        df.loc[df.entries == -1, 'tp'] = df.close * (1 - params['tp']/100)
+        
 
     def run(self, **kwargs):
         self.params.update(kwargs)
 
         data = self.data.copy()
         
         data = self.compute(data, self.params)
         
         if 'entries' not in data.columns.to_list():
             raise KeyError('column "entries" not found.')
         
         data.loc[data.entries != 0, 'entry_price'] = data.open.shift(-1)
 
-        data.loc[data.entries == 1, 'sl'] = data.close * (1 - self.params['sl']/100)
-        data.loc[data.entries == 1, 'tp'] = data.close * (1 + self.params['tp']/100)
+        self.exit_func(data, self.params)
 
-        data.loc[data.entries == -1, 'sl'] = data.close * (1 + self.params['sl']/100)
-        data.loc[data.entries == -1, 'tp'] = data.close * (1 - self.params['tp']/100)
-        
         data['exit_price'] = data.open.shift(-1)
         data['trade_time'] = data.datetime.shift(-1)
 
         orders = self._generate_orders(data)
         out_df = pd.DataFrame([o.model_dump() for o in orders])
         return out_df, data
 
@@ -104,14 +114,15 @@
 
     def _objective(self, params):
         r, _ = self.run(**params)
         os, rdf = self._get_overfitting_score(r.copy())
         if os > 10:
             r = rdf
             print("removing event effect - ", params)
+
         return {'params': params, 'trades': r}
 
 
     @retry(tries=10)
     def optimize(self, kwargs):
         opt_params, constant_params = self._define_space(kwargs)
```

### Comparing `mptradelib-0.5.7/mptradelib/broker/broker.py` & `mptradelib-0.5.8/mptradelib/broker/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 "cont_flag": "1",
             }
             
             data = self._client.history(data=payload)
             try:
                 final_data += data["candles"]
             except IndexError as e:
-                continue
+                raise e
             curr += delta + dt.timedelta(days=1)
         df = pd.DataFrame(final_data, columns=["datetime", "open", "high", "low", "close", "volume"])
         df.index = pd.to_datetime(df["datetime"], unit="s", utc=True)
         df.index = df.index.tz_convert("Asia/Kolkata")
         df.datetime = df.index
         df = df.sort_index()
         return df
```

### Comparing `mptradelib-0.5.7/mptradelib/broker/session.py` & `mptradelib-0.5.8/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/broker/shoonya.py` & `mptradelib-0.5.8/mptradelib/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/broker/ticker.py` & `mptradelib-0.5.8/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/cli/new.py` & `mptradelib-0.5.8/mptradelib/cli/new.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/cli/templates/strategy/__init__.py.jinja` & `mptradelib-0.5.8/mptradelib/cli/templates/strategy/__init__.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/cli/templates/strategy/backtest.ipynb.jinja` & `mptradelib-0.5.8/mptradelib/cli/templates/strategy/backtest.ipynb.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/cli/templates/strategy/livetrade.py.jinja` & `mptradelib-0.5.8/mptradelib/cli/templates/strategy/livetrade.py.jinja`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/feed.py` & `mptradelib-0.5.8/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/livetrade.py` & `mptradelib-0.5.8/mptradelib/livetrade.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/optimizers/walkforward.py` & `mptradelib-0.5.8/mptradelib/optimizers/walkforward.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/test_renko.py` & `mptradelib-0.5.8/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/utils/simulated_trades.py` & `mptradelib-0.5.8/mptradelib/utils/simulated_trades.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/utils/tearsheet.py` & `mptradelib-0.5.8/mptradelib/utils/tearsheet.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/utils/utils.py` & `mptradelib-0.5.8/mptradelib/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/mptradelib/widgets/daterangepicker.py` & `mptradelib-0.5.8/mptradelib/widgets/daterangepicker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.5.7/pyproject.toml` & `mptradelib-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.5.7"
+version = "0.5.8"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.5.7/PKG-INFO` & `mptradelib-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.5.7
+Version: 0.5.8
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

