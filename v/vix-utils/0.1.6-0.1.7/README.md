# Comparing `tmp/vix_utils-0.1.6.tar.gz` & `tmp/vix_utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vix_utils-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vix_utils-0.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vix_utils-0.1.6.tar` & `vix_utils-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3306 2024-05-20 23:38:16.423488 vix_utils-0.1.6/README.md
--rw-r--r--   0        0        0     1443 2024-05-20 23:38:16.443489 vix_utils-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      767 2024-05-20 23:38:16.443489 vix_utils-0.1.6/src/vix_utils/__init__.py
--rw-r--r--   0        0        0  1851085 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/cfe-rule-book.pdf
--rw-r--r--   0        0        0     5329 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/continuous_maturity.py
--rw-r--r--   0        0        0     4570 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/data_notes.md
--rw-r--r--   0        0        0    26919 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/download_vix_futures.py
--rw-r--r--   0        0        0      764 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/a_t.ipynb
--rw-r--r--   0        0        0      259 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/hello_x.py
--rw-r--r--   0        0        0     4063 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/sample_load_data.py
--rw-r--r--   0        0        0     4670 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/sample_plots.py
--rw-r--r--   0        0        0    49112 2024-05-20 23:38:16.451489 vix_utils-0.1.6/src/vix_utils/examples/vix_utils xarray.ipynb
--rw-r--r--   0        0        0   264522 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/examples/vix_utils.ipynb
--rw-r--r--   0        0        0     1234 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/futures_utils.py
--rw-r--r--   0        0        0      503 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/location.py
--rw-r--r--   0        0        0    27994 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/old_download_vix_futures.py
--rw-r--r--   0        0        0     3805 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/vix_cash_term_structure.py
--rw-r--r--   0        0        0    12835 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/vix_futures_dates.py
--rw-r--r--   0        0        0     4502 2024-05-20 23:38:16.455489 vix_utils-0.1.6/src/vix_utils/vixutil.py
--rw-r--r--   0        0        0     4269 1970-01-01 00:00:00.000000 vix_utils-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3238 2024-05-25 04:02:37.258651 vix_utils-0.1.7/README.md
+-rw-r--r--   0        0        0     1459 2024-05-25 04:02:37.278651 vix_utils-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      767 2024-05-25 04:02:37.278651 vix_utils-0.1.7/src/vix_utils/__init__.py
+-rw-r--r--   0        0        0  1851085 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/cfe-rule-book.pdf
+-rw-r--r--   0        0        0     5421 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/continuous_maturity.py
+-rw-r--r--   0        0        0     4570 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/data_notes.md
+-rw-r--r--   0        0        0    26919 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/download_vix_futures.py
+-rw-r--r--   0        0        0      764 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/examples/a_t.ipynb
+-rw-r--r--   0        0        0      259 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/examples/hello_x.py
+-rw-r--r--   0        0        0     4063 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/examples/sample_load_data.py
+-rw-r--r--   0        0        0     4670 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/examples/sample_plots.py
+-rw-r--r--   0        0        0    49112 2024-05-25 04:02:37.286651 vix_utils-0.1.7/src/vix_utils/examples/vix_utils xarray.ipynb
+-rw-r--r--   0        0        0   264522 2024-05-25 04:02:37.290651 vix_utils-0.1.7/src/vix_utils/examples/vix_utils.ipynb
+-rw-r--r--   0        0        0     1234 2024-05-25 04:02:37.290651 vix_utils-0.1.7/src/vix_utils/futures_utils.py
+-rw-r--r--   0        0        0      503 2024-05-25 04:02:37.290651 vix_utils-0.1.7/src/vix_utils/location.py
+-rw-r--r--   0        0        0    27994 2024-05-25 04:02:37.290651 vix_utils-0.1.7/src/vix_utils/old_download_vix_futures.py
+-rw-r--r--   0        0        0     3805 2024-05-25 04:02:37.290651 vix_utils-0.1.7/src/vix_utils/vix_cash_term_structure.py
+-rw-r--r--   0        0        0    22447 2024-05-25 04:02:37.290651 vix_utils-0.1.7/src/vix_utils/vix_futures_dates.py
+-rw-r--r--   0        0        0     4502 2024-05-25 04:02:37.290651 vix_utils-0.1.7/src/vix_utils/vixutil.py
+-rw-r--r--   0        0        0     4225 1970-01-01 00:00:00.000000 vix_utils-0.1.7/PKG-INFO
```

### Comparing `vix_utils-0.1.6/README.md` & `vix_utils-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,10 +75,8 @@
 These dates appear to be missing from the CBOE Data.
 At some point they need to be patched in if they exist.
 ```
 [Timestamp('2006-11-10 00:00:00'), Timestamp('2007-01-03 00:00:00'), Timestamp('2021-04-02 00:00:00'), Timestamp('2021-12-24 00:00:00')]
 ```
 There seem to be  a few dates where spot indexes are missing, you will have to workaround by using fill feature of Pandas datafame, or skip those days, in any analysis.
 ~~~
-## Developing
-https://numpydoc.readthedocs.io/en/latest/format.html
```

### Comparing `vix_utils-0.1.6/pyproject.toml` & `vix_utils-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 dependencies= [
     "pandas",
     "pandas-market-calendars >= 4.4.0",
     "aiofiles",
     "aiohttp[speedups]",
     "openpyxl",
     "appdirs",
-    "more_itertools"]
+    "more_itertools",
+    "icecream"]
 
 
 [project.optional-dependencies]
 test=["pytest"]
 
 examples=["matplotlib","scipy"]
```

### Comparing `vix_utils-0.1.6/src/vix_utils/__init__.py` & `vix_utils-0.1.7/src/vix_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A library for preparing   VIX Futures and Cash Term Structures for analysis,
 including a  continuous maturity VIX Futures term structure.
 """
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 
 from .download_vix_futures import  \
 pivot_futures_on_monthly_tenor,select_monthly_futures,async_load_vix_term_structure,load_vix_term_structure
 
 from .vix_cash_term_structure import \
     async_get_vix_index_histories,  \
     get_vix_index_histories,    \
```

### Comparing `vix_utils-0.1.6/src/vix_utils/cfe-rule-book.pdf` & `vix_utils-0.1.7/src/vix_utils/cfe-rule-book.pdf`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/continuous_maturity.py` & `vix_utils-0.1.7/src/vix_utils/continuous_maturity.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,19 +42,19 @@
     as the first level index on axis 1.
     weight_df:  a dataframe with columns that represent the desired weights.
     weights_and_tenors:  a list of tuples of the name of the column weighting and the tenor to be used to find the columns in trades_df.
 
     """
     return sum(do_weight(trades_df,weight_df,n,t) for n,t in weights_and_tenors )
 
-_weights_and_tenors_vix_front_months=[('Front Month Weight',1), ('Next Month Weight',2)]
+_weights_and_tenors_vix_front_months=[(f"T{i}W",i) for i in range(1,4)]
 
-def do_weighting_front_two_months(trades_df : pd.DataFrame,weight_df : pd.DataFrame) -> pd.DataFrame:
+def do_weighting_front_three_months(trades_df : pd.DataFrame,weight_df : pd.DataFrame) -> pd.DataFrame:
     """
-    produces a weighted mean of the two nearest monthly futures resulting in an average of maturity one month.
+    produces a weighted mean of the nearest monthly futures resulting in an average of maturity one month.
     parameters:
     ----------
     trades_df:  a DataFrame indexed by trade date on axis 0, and by Tenor_Monthly (as the first level index) on axis 1.
 
     """
     return do_weighting_months(trades_df,weight_df,_weights_and_tenors_vix_front_months)
 
@@ -113,30 +113,32 @@
 
  
        
 
  
     weights_all=vix_constant_maturity_weights(df)
 
-    #we only need the weigths we for dates we have trades
+    #we only need the weigths  for dates we have trades
     weights=weights_all[weights_all.index.isin(futures_history.index)]
    
-    #select the front two months and the columns that have trade values
+    #select the front three months and the columns that have trade values
+    #we need three because at times teh front month is ignored and the back two contracts are used.
+
     with pd.option_context('display.max_columns',None): 
         logging.debug(f"\n{'*'*50}\nColumns to weight:\n{futures_history}")
-    front_two_months=futures_history[[1,2]]
-    futures_history_trade_value_columns=front_two_months.swaplevel(axis=1)[_weighted_column_names].swaplevel(axis=1)
+    front_three_months=futures_history[[1,2,3]]
+    futures_history_trade_value_columns=front_three_months.swaplevel(axis=1)[_weighted_column_names].swaplevel(axis=1)
  
-    weighted_values=do_weighting_front_two_months(futures_history_trade_value_columns,weights)
+    weighted_values=do_weighting_front_three_months(futures_history_trade_value_columns,weights)
 
     #should have the same number of rows
     assert weighted_values.shape[0]==futures_history_trade_value_columns.shape[0]
 
     
-    df_file=front_two_months.swaplevel(axis=1)["File"]
+    df_file=front_three_months.swaplevel(axis=1)["File"]
     weighted_values["File"]=df_file[1]+"+"+df_file[2] 
     
     weighted_values['Expiry']=weights['Expiry']
 
 
     weighted_values["Tenor_Days"]=(weighted_values['Expiry']-weighted_values.index).dt.days
```

### Comparing `vix_utils-0.1.6/src/vix_utils/data_notes.md` & `vix_utils-0.1.7/src/vix_utils/data_notes.md`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/download_vix_futures.py` & `vix_utils-0.1.7/src/vix_utils/download_vix_futures.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/examples/a_t.ipynb` & `vix_utils-0.1.7/src/vix_utils/examples/a_t.ipynb`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/examples/sample_load_data.py` & `vix_utils-0.1.7/src/vix_utils/examples/sample_load_data.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/examples/sample_plots.py` & `vix_utils-0.1.7/src/vix_utils/examples/sample_plots.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/examples/vix_utils xarray.ipynb` & `vix_utils-0.1.7/src/vix_utils/examples/vix_utils xarray.ipynb`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/examples/vix_utils.ipynb` & `vix_utils-0.1.7/src/vix_utils/examples/vix_utils.ipynb`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/futures_utils.py` & `vix_utils-0.1.7/src/vix_utils/futures_utils.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/old_download_vix_futures.py` & `vix_utils-0.1.7/src/vix_utils/old_download_vix_futures.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/vix_cash_term_structure.py` & `vix_utils-0.1.7/src/vix_utils/vix_cash_term_structure.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/src/vix_utils/vix_futures_dates.py` & `vix_utils-0.1.7/src/vix_utils/vix_futures_dates.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import pandas as pd
 import pandas_market_calendars as mcal
 import functools as func
 import calendar as cal
 import datetime as dt
 import numpy as np
 import vix_utils.futures_utils as u
-
+from icecream import ic
 import logging as logging
 from .location import data_dir
+from typing import Generator
 _cfe_calendar = mcal.get_calendar('CFE')
 _now = dt.datetime.now()
 
-_years_ahead = 5
-_future_date = dt.datetime(_now.year + _years_ahead, 1, 1)
+_years_ahead : int = 5
+_future_date : dt.datetime = dt.datetime(_now.year + _years_ahead, 1, 1)
 # must be 1 year past _future_date
-_last_valid_cfe_day = dt.datetime(_now.year + _years_ahead + 1, 1, 1)
+_last_valid_cfe_day : dt.datetime = dt.datetime(_now.year + _years_ahead + 1, 1, 1)
 
 # generate a range that is beyond any possible Expirys for vix futures in the data
 
 _first_vix_futures_date_date = "2004-03-26"
 #https://www.cboe.com/tradable_products/vix/vix_futures/specifications/
 
 # don't use this for the date range.  _valid_cfe_days should go a year past the last trade date
 
-_valid_cfe_days = pd.DatetimeIndex(
+_valid_cfe_days : pd.DatetimeIndex = pd.DatetimeIndex(
     _cfe_calendar.valid_days(_first_vix_futures_date_date, end_date=_last_valid_cfe_day).date).to_series().sort_index()
 
 
 # days = _valid_cfe_days.date
 # days1 = pd.DatetimeIndex(days).to_series()
 
+minus_one_day=pd.DateOffset(-1)
 
 @func.lru_cache(maxsize=None)  # called repeatedly with the same values, so cache the results.
 def vix_futures_expiry_date_monthly(year: int, month: int):
     """
     Return the date of expiry of Vix Monthly Futures the series expiring in year and month
     :param year: The year of futures expiry
     :param month: The month of futures expiry
@@ -52,38 +54,38 @@
     purposes, the first week of a calendar year is the first week of that year with a Wednesday
     on which a weekly VX futures contract could expire. If that Wednesday or the Friday that
     is thirty days following that Wednesday is a Cboe Options holiday, the final settlement
     date for the contract shall be on the business day immediately preceding that Wednesday.
 
 
     """
-    c = cal.Calendar(firstweekday=cal.SUNDAY)
+    c : cal.Calendar = cal.Calendar(firstweekday=cal.SUNDAY)
     next_month = month + 1
 
     # does the option series the future settles on  settle next year?
     options_next_year = next_month > 12
 
     next_month = next_month % 12 if options_next_year else next_month
     options_year = year + 1 if options_next_year else year  # keep for debugging
 
-    m = c.monthdayscalendar(options_year, next_month)
-    md = c.monthdatescalendar(options_year, next_month)
+    m : list[list[int]] = c.monthdayscalendar(options_year, next_month)
+    md : list[list[dt.date]] = c.monthdatescalendar(options_year, next_month)
 
     friday_index = -2
     # 2 to index the 3d week, 0 based index for m
     week_index = 2 if m[0][friday_index] != 0 else 3
     # third_friday unused, just for easier debugging to have.
-    third_friday = m[week_index][friday_index]              # keep for debugging
-    option_expiry_date = md[week_index][friday_index]
-    friday_expiration = any(_valid_cfe_days.isin([option_expiry_date]))
+    third_friday : int = m[week_index][friday_index]              # keep for debugging
+    option_expiry_date : dt.date = md[week_index][friday_index]
+    friday_expiration : bool = any(_valid_cfe_days.isin([option_expiry_date]))
     if not friday_expiration:
         # the preceding day will be the option expiry date
         option_expiry_date = option_expiry_date - dt.timedelta(days=1)
 
-    futures_expiry_date = option_expiry_date - dt.timedelta(days=30)
+    futures_expiry_date : dt.date = option_expiry_date - dt.timedelta(days=30)
     # also check for a holiday on the 30 days before the 3d friday
     if friday_expiration and not any(_valid_cfe_days.isin([futures_expiry_date])):
         futures_expiry_date = futures_expiry_date - dt.timedelta(days=1)
 
     return futures_expiry_date
 
 
@@ -104,17 +106,19 @@
     months_forward_for_tenor = (0 if day <=  this_calendar_months_expiry.day else 1)
     month_of_expiry = (month + months_forward_for_tenor + tenor - 1) % 12
     year_of_expiry = year + (
         1 if month_of_expiry < month else 0) + (tenor-1)//12
     return vix_futures_expiry_date_monthly(year_of_expiry, month_of_expiry)
 
 
-def vix_constant_maturity_weights(vix_calendar):
+def vix_constant_maturity_weights(vix_calendar : pd.DataFrame, start_date : str|pd.Timestamp=None, end_date : str|pd.Timestamp=None) -> pd.DataFrame:
     """
     :param vix_calendar:  the DataFrame returned by  vix_futures_trade_dates_and_expiry_dates
+    :param date_range: A data range to limit the weights, useful for testing or only need weights for a limited range.
+
     :return: a DataFrame containting the weights required to interpolate between the tenors of trading tenors of
     Vix Futures to have a term structure of constant maturity in months.
 
     This index, for example,
     https://www.spglobal.com/spdji/en/indices/strategy/sp-500-vix-short-term-index-mcap/#overview,
     is based on a 1 month interpolation of the 1st and 2nd month futures.  The DataFrame returned should
     provide the weights required
@@ -140,68 +144,231 @@
     settlement_dates=vix_term_structure["Expiry"]
     vix_term_structure
 
     """
 
     # create a map from Expirys to the previous Expirys
     # this is done by looking at month 2 settlment dates, and finding the month 1 Expiry
+    ic.disable()
+    start_roll_col : str = "Start Roll"
+    end_roll_col : str = "End Roll"
 
-    start_roll_front_month = "Start Roll Front Month"
     sd = "Expiry"
     rptd = "Roll Period Trade Days"
     rpcd = "Roll Period Calendar Days"
+    rrptd = "Remaining Roll Period Trade Days"
+    rrpcd = "Remaining Roll Period Calendar Days"
     settle_dates_map = vix_calendar[sd].drop_duplicates().dropna()
-    month_to_prior_month_settlement_map = settle_dates_map.set_index(2)[1]
-    cols_to_copy = {"Settle 1": vix_calendar['Expiry'][1], "Settle 2": vix_calendar['Expiry'][2]}
-    df_foo = pd.DataFrame(index=vix_calendar.index, data=cols_to_copy)
+    month_to_prior_month_settlement_map_full = settle_dates_map.set_index(2)[1]
+
+    #need to patch the March  2024 settlement  date in.
+    month_to_prior_month_settlement_map_full['2004-04-21']='2004-03-16'
+    month_to_prior_month_settlement_map_full.sort_index(inplace=True)
+
+
+    #avoid looping through months with no data, to facillitate easier debugging.
+    #we need the map from the date of the first trade in the range, to month after.
+    cols_to_copy = {f"Settle {i}": vix_calendar['Expiry'][i] for i in range(1,4)}
+
+    df_foo = pd.DataFrame(index=vix_calendar.index,data=cols_to_copy)
+    if start_date or end_date:
+        #we know that we don't need to look more than 30 days in the future, so limit to 70 days
+        # (to avoid any boundry/edge cases) 
+        # to trip the settlement map.
+        last_trade_of_interest=vix_calendar[start_date:end_date].index[-1]
+
+        date_range=slice(start_date,last_trade_of_interest+pd.DateOffset(70))
+        
+        month_to_prior_month_settlement_map = month_to_prior_month_settlement_map_full.loc[date_range]
+        df_foo=df_foo[start_date:end_date] 
+    else:
+        month_to_prior_month_settlement_map=month_to_prior_month_settlement_map_full
+
+
+
+
+    
 
     df_foo[rptd] = -100001  # just a nonsense number we can identify
 
     df_foo[rptd] = df_foo[rptd].astype(int)
 
+
+    df_foo[rpcd] = -999990  # another nonsense number we can identify
+    df_foo[rpcd] = df_foo[rpcd].astype(int)  # another nonsense number we can identify
+
     # add the start of roll date for front month
 
-    df_foo[start_roll_front_month] = np.nan
-    for second_month_settlement in month_to_prior_month_settlement_map.index:
-        front_month_settlement=month_to_prior_month_settlement_map[second_month_settlement]
-        start_roll = front_month_settlement
-        selected = vix_calendar[sd][1] == front_month_settlement
-        df_foo.loc[selected, start_roll_front_month] = start_roll
-      
-        calendar_day_day_before_settlement=second_month_settlement + pd.DateOffset(-1)
-
-        #roll_period_trade_days is dt in https://www.spglobal.com/spdji/en/documents/methodologies/methodology-sp-vix-futures-indices.pdf page 5
-        roll_period_trade_days = cfe_exchange_open_days(front_month_settlement, calendar_day_day_before_settlement) 
-        df_foo.loc[selected, rptd] = roll_period_trade_days
+    df_foo[start_roll_col] = np.nan
+
+    #useful for debuggin.    
+    df_foo['Day of Week']=df_foo.index.day_of_week
+    df_foo['Day Name']=df_foo.index.day_name()
+    df_foo["First Component"]=1
+    df_foo["Second Component"]=2
+    def roll_periods() -> Generator:
+        """Generator, returns roll periods as tuples start_roll_date, front_month_settlement, end_roll_date-1 day, end_roll_date"""
+
+  
+        for second_month_settlement in month_to_prior_month_settlement_map.index:
+            front_month_settlement=month_to_prior_month_settlement_map[second_month_settlement]
+            #https://www.spglobal.com/spdji/en/documents/methodologies/methodology-sp-vix-futures-indices.pdf page 5
+            #the Roll Period starts after the
+            #close on the Tuesday prior to the monthly Chicago Board Options Exchange (Cboe) VIX Futures 
+            #Settlement Date
+            #a little ambigous if a tuesday is a holiday.
+            day_before_front_month_settlement = front_month_settlement + minus_one_day
+            
+            #days of weeks start at 0 for Monday
+
+            #it is going to be negative, because we are looking for the days until the preceeding tuesday
+            days_until_tuesday_front_month = 1-front_month_settlement.day_of_week
+            
+
+            start_roll_date : pd.Timestamp = front_month_settlement + pd.DateOffset(days_until_tuesday_front_month)
+
+   
+            #it is going to be negative, because we are looking for the days until the preceeding tuesday
+
+            days_until_tuesday_second_month = 1-second_month_settlement.day_of_week  
+            end_roll : pd.Timestamp =  second_month_settlement + pd.DateOffset(days_until_tuesday_second_month)
+            day_before_end_roll : pd.Timestamp = end_roll+minus_one_day
+
+            yield (start_roll_date,front_month_settlement,day_before_end_roll,end_roll)
+
+    def ammend_df():
+        for (start_roll_date,front_month_settlement,day_before_end_roll,end_roll) in roll_periods():
+                    
+            this_row_period_slice=slice(start_roll_date,day_before_end_roll)
+            ic(this_row_period_slice)
+            df_foo.loc[this_row_period_slice,start_roll_col] = start_roll_date
+            df_foo.loc[this_row_period_slice,end_roll_col] = end_roll
+
+            #roll_period_trade_days is dt in https://www.spglobal.com/spdji/en/documents/methodologies/methodology-sp-vix-futures-indices.pdf page 5
+            #includes first day of the roll period, but excludes the last.
+
+            # After the close on the Tuesday, corresponding to the start of the Roll Period, all of the weight is allocated 
+            # to the shorter-term (i.e., mth month) contract. Then on each subsequent business day a fraction of the mth
+            # month VIX futures holding is sold and an equal notional amount of the longer-term (n
+            # th month) VIX futures
+            # is bought. The fraction, or quantity, is proportional to the number of mth month VIX futures contracts as of 
+            # the previous index roll day, and inversely proportional to the length of the current Roll Period. In this way 
+            # the initial position in the mth month contract is progressively moved to the n
+            # th month one over the course 
+            # of the month, until the following Roll Period starts when the old n
+            # th month VIX futures contract becomes 
+            # the new mth month VIX futures contract and gets sold every day afterward as the process begins again.
+
+            #the above is slightly weird, because the expiring future still trades on the wednesday, though it no weight.
+              
+            #for the  front month settlement day, and the start of the roll period day, we use the second and third month to compute weightings
+
+            df_foo.loc[start_roll_date:front_month_settlement,'First Component']=2
+            df_foo.loc[start_roll_date:front_month_settlement,'Second Component']=3
+
+            roll_period_trade_days = cfe_exchange_open_days(start_roll_date, day_before_end_roll) 
+            
+
+
+            ic(roll_period_trade_days)
+            #use the same methoology for roll period calendar days for choosing the start and end dates.
+            roll_period_calendar_days = int( (day_before_end_roll - start_roll_date)/np.timedelta64(1,'D') )
 
-    df_foo[start_roll_front_month] = pd.to_datetime(df_foo[start_roll_front_month])
-    df_foo[rpcd] = vix_calendar[sd][1] - df_foo[start_roll_front_month]
+
+
+            df_foo.loc[this_row_period_slice, rptd] = roll_period_trade_days
+            df_foo.loc[this_row_period_slice, rpcd] = roll_period_calendar_days
+
+    ammend_df()
+    df_foo[start_roll_col] = pd.to_datetime(df_foo[start_roll_col])
     tenor_tds = "Tenor_Trade_Days"
     ten_caldays = "Tenor_Days"
 
     fmw = "Front Month Weight"
     smw = "Next Month Weight"
     trade_days_to_settle = df_foo[tenor_tds] = vix_calendar[tenor_tds][1]
-    df_foo[fmw] = front_month_weight = trade_days_to_settle / df_foo[rptd]
-    df_foo[smw] = -1 * front_month_weight + 1
+
+    #The total number of business days within a Roll Period beginning with, and including, the 
+    #following business day and ending with, but excluding, the following Cboe VIX Futures 
+    #Settlement Date. The number of business days includes a new holiday introduced intra-month 
+    #up to the business day proceeding such a holiday
+
+
+    df_foo["Trade_Day_Plus_1"]=df_foo.index + pd.DateOffset(1)
+    df_foo["End_Roll_Minus_1"]= df_foo[end_roll_col] + minus_one_day
+    df_foo['Settle_1_Minus_1']=df_foo["Settle 1"] + minus_one_day
+
+    def remaining_roll_period_trade_days_on_row(row):
+        return cfe_exchange_open_days(row["Trade_Day_Plus_1"],row['End_Roll_Minus_1'])
+
+    remaining_roll_period_trade_days : pd.DataFrame    
+    df_foo[rrptd]=remaining_roll_period_trade_days=df_foo.apply(remaining_roll_period_trade_days_on_row,axis=1, result_type='expand')
+
+    def remaining_roll_period_calendar_days_on_row(row):
+        return int((row['End_Roll_Minus_1']-row.name)/np.timedelta64(1,'D'))
+
+
+    remaining_roll_period_trade_days : pd.DataFrame
+    df_foo[rrpcd] = remaining_roll_period_calendar_days=df_foo.apply(remaining_roll_period_calendar_days_on_row,axis=1,result_type='expand')
+
+    front_month_weights : pd.Series
+    next_month_weights : pd.Series
+
+
+    df_foo[fmw] = front_month_weights = remaining_roll_period_trade_days / df_foo[rptd]
+    df_foo[smw] = next_month_weights  = -1 * front_month_weights + 1
+
+
+
+
+    #identify problematic weights. 
+    #should never happen if the code is correct.
+    front_month_weights_too_big_sel = front_month_weights >1
+    front_month_weights_too_small_sel = front_month_weights<0
+ 
+
+    if front_month_weights_too_big_sel.any():
+        front_month_weights_too_big=front_month_weights[front_month_weights_too_big_sel]
+        ic(front_month_weights_too_big)
+
+    if front_month_weights_too_small_sel.any():
+        front_month_weights_too_small=front_month_weights[front_month_weights_too_small_sel]
+        ic(front_month_weights_too_small)
+
+    assert front_month_weights.max() <= 1
+    assert front_month_weights.min() >= 0
+    assert ((front_month_weights+next_month_weights)==1).all()          #they better add up to one
+
+    tenor_1_weight = (df_foo["First Component"]==1)*front_month_weights  
+    tenor_2_weight = (df_foo["First Component"]==2) * front_month_weights +\
+                     (df_foo["Second Component"] == 2) * next_month_weights
+    tenor_3_weight = (df_foo["Second Component"] == 3) * next_month_weights
+
+    assert ((tenor_1_weight+tenor_2_weight+tenor_3_weight)==1).all()   #better add up to one!
+
+    df_foo["T1W"]=tenor_1_weight
+    df_foo["T2W"]=tenor_2_weight
+    df_foo["T3W"]=tenor_3_weight
+
+
     ttr = "Temp Trade Date"
     df_foo[ttr] = df_foo.index.to_series()
     #    temp_tdts="Temporary Tenor_Days"
     #    df_foo[temp_tdts]=df_foo[tdts]
     ll = len(df_foo)
 
     def maturity_date(row):
         # Use the trade date X trade days later, where X is the current roll period
         # in trade days.
         trade_date = row[ttr]
         try:
             row_roll_period_trade_days = row[rptd]  # trade_days_to_settle[trade_date]
             trade_date_loc = trade_days_to_settle.index.get_loc(trade_date)
             trade_date_loc_end_of_roll = trade_date_loc + row_roll_period_trade_days
-            trade_date_loc_end_of_roll_capped = pd.nan if trade_date_loc_end_of_roll > ll else \
+            trade_date_loc_end_of_roll_capped = np.nan if trade_date_loc_end_of_roll > ll else \
                 trade_date_loc_end_of_roll
             trade_date_end_of_roll = df_foo.iloc[trade_date_loc_end_of_roll_capped].at[ttr]
             return trade_date_end_of_roll
         except Exception as e:
             pass
             #we are always going to get some of these at the end, since the dates go past the dates
             #in the data frames.  they need to be filtered out after.
@@ -219,35 +386,64 @@
     return df_foo
 
 
 @u.timeit()
 def pivot_on_contract_maturity(df):
     return df.reset_index().pivot(columns="Contract Month", index="Trade Date")
 
+def cfe_exchange_open_dates(selection_slice : slice = None)  -> pd.DatetimeIndex:
+    """
+    Return the dates, sorted, that the CFE is open, based on 
+    partial string indexing (https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#partial-string-indexing). 
+
+    Pass in a slice object that can select from a DateTimeIndex.  like slice('2024-04','2024-04') for April 2024, or slice(None,'2024-04') for
+    all dates until and including April 2024.
+    Pass in both Dates unless you want all dates before or all dates after the partial string index supplied.   
+    
+    """
+    return _valid_cfe_days.loc[selection_slice if selection_slice else slice(None)]
 
 def cfe_exchange_open_days(start_date, end_date):
     exchange_open_days = _valid_cfe_days.loc[start_date:end_date]
     return len(exchange_open_days)
 
 def remaining_cfe_exchange_open_days(start_date,end_date):
     next_day=start_date + pd.DateOffset(1)
     return cfe_exchange_open_days(next_day,end_date)
 
+
 @u.timeit()
-def vix_futures_trade_dates_and_expiry_dates(number_of_futures_maturities=9):
+def vix_futures_trade_dates_and_expiry_dates(number_of_futures_maturities:int = 9) -> pd.DataFrame:
     f"""
     :param number_of_futures_maturities:
         :return:  a data frame with an index of trade date and maturity (in months) and a value of the Expiry.  
                    We refer to a DataFrame in this format as a wide vix calendar or wide settlement calendar..
                    The dates will include all past dates which the VIX futures have traded, and future dates until
                     {_future_date}
         """
     # by trial and error, this gives us the day
     # careful to select the portion of the valid dates before _future_date
-    trade_dates = _valid_cfe_days[:_future_date]
+    trade_dates :pd.DatetimeIndex = _valid_cfe_days[:_future_date]
+    return _vix_futures_trade_dates_and_expiry_dates_for_dates(trade_dates,number_of_futures_maturities)
+
+@u.timeit()
+def _vix_futures_trade_dates_and_expiry_dates_for_dates(trade_dates : pd.DatetimeIndex,number_of_futures_maturities:int = 9) -> pd.DataFrame:
+    f"""
+    :param trade_dates:  a subset of dates from _valid_cfe_days
+    :param number_of_futures_maturities:
+        :return:  a data frame with an index of trade date and maturity (in months) and a value of the Expiry.  
+                   We refer to a DataFrame in this format as a wide vix calendar or wide settlement calendar..
+                   The dates will include all past dates which the VIX futures have traded, and future dates until
+                    {_future_date}.
+
+        Library consumers should prefer vix_futures_trade_dates_and_expiry_dates.  
+
+        """
+    # by trial and error, this gives us the day
+    # careful to select the portion of the valid dates before _future_date
     ii = pd.Index(trade_dates, name="Trade Date")
 
     @u.timeit()
     def add_columns_d(maturity):
         df = pd.DataFrame(index=ii)
         """Add the Contract Month (in months), Expiry, Tenor_Days, 
         and Tenor_Trade_Days to the dataframe"""
```

### Comparing `vix_utils-0.1.6/src/vix_utils/vixutil.py` & `vix_utils-0.1.7/src/vix_utils/vixutil.py`

 * *Files identical despite different names*

### Comparing `vix_utils-0.1.6/PKG-INFO` & `vix_utils-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vix_utils
-Version: 0.1.6
+Version: 0.1.7
 Summary: Provide VIX Cash and Futures Term Structure as Pandas dataframes
 Keywords: vix,volatility,pandas,vix term structure,cboe
 Author-email: Doug Ransom <doug@ransom.vip>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Requires-Dist: pandas
 Requires-Dist: pandas-market-calendars >= 4.4.0
 Requires-Dist: aiofiles
 Requires-Dist: aiohttp[speedups]
 Requires-Dist: openpyxl
 Requires-Dist: appdirs
 Requires-Dist: more_itertools
+Requires-Dist: icecream
 Requires-Dist: matplotlib ; extra == "examples"
 Requires-Dist: scipy ; extra == "examples"
 Requires-Dist: pytest ; extra == "test"
 Project-URL: home-page, https://github.com/dougransom/vix_utils
 Provides-Extra: examples
 Provides-Extra: test
 
@@ -101,11 +102,9 @@
 These dates appear to be missing from the CBOE Data.
 At some point they need to be patched in if they exist.
 ```
 [Timestamp('2006-11-10 00:00:00'), Timestamp('2007-01-03 00:00:00'), Timestamp('2021-04-02 00:00:00'), Timestamp('2021-12-24 00:00:00')]
 ```
 There seem to be  a few dates where spot indexes are missing, you will have to workaround by using fill feature of Pandas datafame, or skip those days, in any analysis.
 ~~~
-## Developing
-https://numpydoc.readthedocs.io/en/latest/format.html
```

