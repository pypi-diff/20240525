# Comparing `tmp/smartmoneyconcepts-0.0.8.tar.gz` & `tmp/smartmoneyconcepts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartmoneyconcepts-0.0.8.tar", last modified: Wed Oct  4 18:31:08 2023, max compression
+gzip compressed data, was "smartmoneyconcepts-0.0.9.tar", last modified: Wed Oct  4 19:14:35 2023, max compression
```

## Comparing `smartmoneyconcepts-0.0.8.tar` & `smartmoneyconcepts-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joshyattridge   (501) staff       (20)        0 2023-10-04 18:31:08.854407 smartmoneyconcepts-0.0.8/
--rw-r--r--   0 joshyattridge   (501) staff       (20)     1067 2021-03-30 12:46:26.000000 smartmoneyconcepts-0.0.8/LICENSE
--rw-r--r--   0 joshyattridge   (501) staff       (20)     2340 2023-10-04 18:31:08.853905 smartmoneyconcepts-0.0.8/PKG-INFO
--rw-r--r--   0 joshyattridge   (501) staff       (20)     1651 2023-09-30 18:59:23.000000 smartmoneyconcepts-0.0.8/README.md
--rw-r--r--   0 joshyattridge   (501) staff       (20)       38 2023-10-04 18:31:08.854548 smartmoneyconcepts-0.0.8/setup.cfg
--rw-r--r--   0 joshyattridge   (501) staff       (20)     1080 2023-10-04 18:30:52.000000 smartmoneyconcepts-0.0.8/setup.py
-drwxr-xr-x   0 joshyattridge   (501) staff       (20)        0 2023-10-04 18:31:08.849946 smartmoneyconcepts-0.0.8/smartmoneyconcepts/
--rw-r--r--   0 joshyattridge   (501) staff       (20)       38 2023-09-23 12:35:57.000000 smartmoneyconcepts-0.0.8/smartmoneyconcepts/__init__.py
--rw-r--r--   0 joshyattridge   (501) staff       (20)    10094 2023-10-04 18:28:32.000000 smartmoneyconcepts-0.0.8/smartmoneyconcepts/smc.py
-drwxr-xr-x   0 joshyattridge   (501) staff       (20)        0 2023-10-04 18:31:08.852650 smartmoneyconcepts-0.0.8/smartmoneyconcepts.egg-info/
--rw-r--r--   0 joshyattridge   (501) staff       (20)     2340 2023-10-04 18:31:08.000000 smartmoneyconcepts-0.0.8/smartmoneyconcepts.egg-info/PKG-INFO
--rw-r--r--   0 joshyattridge   (501) staff       (20)      292 2023-10-04 18:31:08.000000 smartmoneyconcepts-0.0.8/smartmoneyconcepts.egg-info/SOURCES.txt
--rw-r--r--   0 joshyattridge   (501) staff       (20)        1 2023-10-04 18:31:08.000000 smartmoneyconcepts-0.0.8/smartmoneyconcepts.egg-info/dependency_links.txt
--rw-r--r--   0 joshyattridge   (501) staff       (20)       20 2023-10-04 18:31:08.000000 smartmoneyconcepts-0.0.8/smartmoneyconcepts.egg-info/requires.txt
--rw-r--r--   0 joshyattridge   (501) staff       (20)       19 2023-10-04 18:31:08.000000 smartmoneyconcepts-0.0.8/smartmoneyconcepts.egg-info/top_level.txt
+drwxr-xr-x   0 joshyattridge   (501) staff       (20)        0 2023-10-04 19:14:35.226147 smartmoneyconcepts-0.0.9/
+-rw-r--r--   0 joshyattridge   (501) staff       (20)     1067 2021-03-30 12:46:26.000000 smartmoneyconcepts-0.0.9/LICENSE
+-rw-r--r--   0 joshyattridge   (501) staff       (20)     2340 2023-10-04 19:14:35.225751 smartmoneyconcepts-0.0.9/PKG-INFO
+-rw-r--r--   0 joshyattridge   (501) staff       (20)     1651 2023-09-30 18:59:23.000000 smartmoneyconcepts-0.0.9/README.md
+-rw-r--r--   0 joshyattridge   (501) staff       (20)       38 2023-10-04 19:14:35.226285 smartmoneyconcepts-0.0.9/setup.cfg
+-rw-r--r--   0 joshyattridge   (501) staff       (20)     1080 2023-10-04 19:13:29.000000 smartmoneyconcepts-0.0.9/setup.py
+drwxr-xr-x   0 joshyattridge   (501) staff       (20)        0 2023-10-04 19:14:35.220640 smartmoneyconcepts-0.0.9/smartmoneyconcepts/
+-rw-r--r--   0 joshyattridge   (501) staff       (20)       38 2023-09-23 12:35:57.000000 smartmoneyconcepts-0.0.9/smartmoneyconcepts/__init__.py
+-rw-r--r--   0 joshyattridge   (501) staff       (20)    10613 2023-10-04 19:12:49.000000 smartmoneyconcepts-0.0.9/smartmoneyconcepts/smc.py
+drwxr-xr-x   0 joshyattridge   (501) staff       (20)        0 2023-10-04 19:14:35.224894 smartmoneyconcepts-0.0.9/smartmoneyconcepts.egg-info/
+-rw-r--r--   0 joshyattridge   (501) staff       (20)     2340 2023-10-04 19:14:35.000000 smartmoneyconcepts-0.0.9/smartmoneyconcepts.egg-info/PKG-INFO
+-rw-r--r--   0 joshyattridge   (501) staff       (20)      292 2023-10-04 19:14:35.000000 smartmoneyconcepts-0.0.9/smartmoneyconcepts.egg-info/SOURCES.txt
+-rw-r--r--   0 joshyattridge   (501) staff       (20)        1 2023-10-04 19:14:35.000000 smartmoneyconcepts-0.0.9/smartmoneyconcepts.egg-info/dependency_links.txt
+-rw-r--r--   0 joshyattridge   (501) staff       (20)       20 2023-10-04 19:14:35.000000 smartmoneyconcepts-0.0.9/smartmoneyconcepts.egg-info/requires.txt
+-rw-r--r--   0 joshyattridge   (501) staff       (20)       19 2023-10-04 19:14:35.000000 smartmoneyconcepts-0.0.9/smartmoneyconcepts.egg-info/top_level.txt
```

### Comparing `smartmoneyconcepts-0.0.8/LICENSE` & `smartmoneyconcepts-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `smartmoneyconcepts-0.0.8/PKG-INFO` & `smartmoneyconcepts-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartmoneyconcepts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Getting indicators based on smart money concepts or ICT
 Home-page: https://github.com/joshyattridge/smartmoneyconcepts
 Author: Joshua Attridge
 License: UNKNOWN
 Keywords: smart,money,concepts,ict,indicators,trading,forex,stocks,crypto,order,blocks,liquidity
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `smartmoneyconcepts-0.0.8/README.md` & `smartmoneyconcepts-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `smartmoneyconcepts-0.0.8/setup.py` & `smartmoneyconcepts-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 import codecs
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Getting indicators based on smart money concepts or ICT'
 
 # read the contents of the README file
 with codecs.open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 # Setting up
```

### Comparing `smartmoneyconcepts-0.0.8/smartmoneyconcepts/smc.py` & `smartmoneyconcepts-0.0.9/smartmoneyconcepts/smc.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,14 +80,15 @@
         )
         bottom = np.where(
             ohlc["close"] > ohlc["open"], ohlc["high"].shift(1), ohlc["high"].shift(-1)
         )
 
         mitigated_index = np.zeros(len(ohlc), dtype=np.int32)
         for i in np.where(fvg != 0)[0]:
+            mask = np.zeros(len(ohlc), dtype=np.bool)
             if fvg[i] == 1:
                 mask = ohlc["low"][i + 2 :] <= top[i]
             elif fvg[i] == -1:
                 mask = ohlc["high"][i + 2 :] >= bottom[i]
             if np.any(mask):
                 j = np.argmax(mask) + i + 2
                 mitigated_index[i] = j
@@ -146,20 +147,27 @@
         This is the last candle before a FVG
         """
 
         # get the FVG
         fvg = cls.fvg(ohlc)
 
         ob = np.where((fvg["FVG"].shift(-1) != 0) & (fvg["FVG"] == 0), fvg["FVG"].shift(-1), 0)
-        top = np.where((fvg["FVG"].shift(-1) == -1) & (ohlc["high"] < ohlc["high"].shift(-1)), ohlc["high"].shift(-1), ohlc["high"])
-        bottom = np.where((fvg["FVG"].shift(-1) == 1) & (ohlc["low"] > ohlc["low"].shift(-1)), ohlc["low"].shift(-1), ohlc["low"])
+        # top is equal to the current candles high unless the ob is -1 and the next candles high is higher than the current candles high then top is equal to the next candles high
+        top = np.where(
+            (ob == -1) & (ohlc["high"].shift(-1) > ohlc["high"]), ohlc["high"].shift(-1), ohlc["high"]
+        )
+        # bottom is equal to the current candles low unless the ob is 1 and the next candles low is lower than the current candles low then bottom is equal to the next candles low
+        bottom = np.where(
+            (ob == 1) & (ohlc["low"].shift(-1) < ohlc["low"]), ohlc["low"].shift(-1), ohlc["low"]
+        )
 
         # set mitigated to np.nan
         mitigated_index = np.zeros(len(ohlc), dtype=np.int32)
         for i in np.where(ob != 0)[0]:
+            mask = np.zeros(len(ohlc), dtype=np.bool)
             if ob[i] == 1:
                 mask = ohlc["low"][i + 2 :] <= top[i]
             elif ob[i] == -1:
                 mask = ohlc["high"][i + 2 :] >= bottom[i]
             if np.any(mask):
                 j = np.argmax(mask) + i + 2
                 mitigated_index[i] = j
@@ -257,7 +265,10 @@
         level = pd.Series(liquidity_level, name="Level")
         liquidity_end = pd.Series(liquidity_end, name="End")
         liquidity_swept = pd.Series(liquidity_swept, name="Swept")
 
         return pd.concat(
             [liquidity, buy_sell_side, level, liquidity_end, liquidity_swept], axis=1
         )
+
+
+# TODO: correct mask error for ob and fvg
```

### Comparing `smartmoneyconcepts-0.0.8/smartmoneyconcepts.egg-info/PKG-INFO` & `smartmoneyconcepts-0.0.9/smartmoneyconcepts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartmoneyconcepts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Getting indicators based on smart money concepts or ICT
 Home-page: https://github.com/joshyattridge/smartmoneyconcepts
 Author: Joshua Attridge
 License: UNKNOWN
 Keywords: smart,money,concepts,ict,indicators,trading,forex,stocks,crypto,order,blocks,liquidity
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

