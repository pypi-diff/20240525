# Comparing `tmp/talipp-2.2.1.tar.gz` & `tmp/talipp-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talipp-2.2.1.tar", last modified: Fri Apr 19 19:55:22 2024, max compression
+gzip compressed data, was "talipp-2.3.0.tar", last modified: Sat May 25 04:49:43 2024, max compression
```

## Comparing `talipp-2.2.1.tar` & `talipp-2.3.0.tar`

### file list

```diff
@@ -1,138 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.209199 talipp-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-19 19:55:11.000000 talipp-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 19:55:11.000000 talipp-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-19 19:55:22.209199 talipp-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8786 2024-04-19 19:55:11.000000 talipp-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:11.000000 talipp-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:55:22.209199 talipp-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-19 19:55:11.000000 talipp-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.193199 talipp-2.2.1/talipp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicator_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.201199 talipp-2.2.1/talipp/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ADX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ALMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/AO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ATR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/AccuDist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Aroon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/BB.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/BOP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/CCI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/CHOP.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ChaikinOsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ChandeKrollStop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/CoppockCurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/DEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/DPO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/DonchianChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/EMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/EMV.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/FibRetracement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ForceIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/HMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/IBS.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Ichimoku.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KAMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KST.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KVO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/KeltnerChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/MACD.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/MassIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/McGinleyDynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/MeanDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/OBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ParabolicSAR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/PivotsHL.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ROC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/RSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SFX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SMMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SOBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/STC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/StdDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/Stoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/StochRSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/SuperTrend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/T3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TRIX.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/TTM.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/UO.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/VTX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/VWAP.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/VWMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/WMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/ZLEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/indicators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/ma.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-19 19:55:11.000000 talipp-2.2.1/talipp/ohlcv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.193199 talipp-2.2.1/talipp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-19 19:55:21.000000 talipp-2.2.1/talipp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-19 19:55:22.000000 talipp-2.2.1/talipp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:55:21.000000 talipp-2.2.1/talipp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 19:55:21.000000 talipp-2.2.1/talipp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:55:22.209199 talipp-2.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ADX.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ALMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_AO.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ATR.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_AccuDist.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_Aroon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_BB.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_BOP.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_CCI.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_CHOP.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ChaikinOsc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ChandeKrollStop.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_CoppockCurve.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_DEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_DPO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_DonchianChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_EMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_EMV.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ForceIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_HMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_IBS.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KAMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KST.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KVO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_KeltnerChannels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_MACD.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_MassIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_McGinleyDynamic.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_MeanDev.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_OBV.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_OHLCV.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ParabolicSAR.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ROC.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_RSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SFX.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SMMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SOBV.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_STC.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_StdDev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_Stoch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_StochRSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_SuperTrend.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_T3.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TRIX.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TSI.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_TTM.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_UO.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_VTX.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_VWAP.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_VWMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_WMA.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_ZLEMA.py
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_indicator_chaining.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_indicator_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_indicator_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-19 19:55:11.000000 talipp-2.2.1/test/test_input.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:49:43.922631 talipp-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-25 04:49:33.000000 talipp-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-25 04:49:33.000000 talipp-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-05-25 04:49:43.922631 talipp-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-05-25 04:49:33.000000 talipp-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 04:49:33.000000 talipp-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 04:49:43.922631 talipp-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-25 04:49:33.000000 talipp-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:49:43.906630 talipp-2.3.0/talipp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicator_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:49:43.914631 talipp-2.3.0/talipp/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ADX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ALMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/AO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ATR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/AccuDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/Aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/BB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/BOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/CCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/CHOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ChaikinOsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ChandeKrollStop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/CoppockCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/DEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/DPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/DonchianChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/EMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/EMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/FibonacciRetracement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ForceIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/HMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/IBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/Ichimoku.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/Indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/KAMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/KST.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/KVO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/KeltnerChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/MACD.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/MassIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/McGinleyDynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/MeanDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/OBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ParabolicSAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/PivotsHL.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ROC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/RSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/SFX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/SMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/SMMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/SOBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/STC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/StdDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/Stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/StochRSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/SuperTrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/T3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/TEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/TRIX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/TSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/TTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/UO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/VTX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/VWAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/VWMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/WMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ZLEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/ZigZag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/indicators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/ma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-25 04:49:33.000000 talipp-2.3.0/talipp/ohlcv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:49:43.906630 talipp-2.3.0/talipp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-05-25 04:49:43.000000 talipp-2.3.0/talipp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-25 04:49:43.000000 talipp-2.3.0/talipp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 04:49:43.000000 talipp-2.3.0/talipp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 04:49:43.000000 talipp-2.3.0/talipp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 04:49:43.922631 talipp-2.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ADX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ALMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_AO.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ATR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_AccuDist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_Aroon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_BB.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_BOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_CCI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_CHOP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ChaikinOsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ChandeKrollStop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_CoppockCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_DEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_DPO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_DonchianChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_EMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_EMV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ForceIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_HMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_IBS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_KAMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_KST.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_KVO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_KeltnerChannels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_MACD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_MassIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_McGinleyDynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_MeanDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_OBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_OHLCV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ParabolicSAR.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ROC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_RSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_SFX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_SMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_SMMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_SOBV.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_STC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_StdDev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_Stoch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_StochRSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_SuperTrend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_T3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_TEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_TRIX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_TSI.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_TTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_UO.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_VTX.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_VWAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_VWMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_WMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ZLEMA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_ZigZag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_indicator_chaining.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_indicator_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_indicator_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-05-25 04:49:33.000000 talipp-2.3.0/test/test_input.py
```

### Comparing `talipp-2.2.1/LICENSE` & `talipp-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/PKG-INFO` & `talipp-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talipp
-Version: 2.2.1
+Version: 2.3.0
 Summary: talipp - Incremental Technical Analysis Library
 Home-page: https://github.com/nardew/talipp
 Author: nardew
 Author-email: talipp.pyth@gmail.com
 License: UNKNOWN
 Description: # talipp - Incremental Technical Analysis Library
         
@@ -34,20 +34,21 @@
         
         Last but not least, `talipp` is a community project and therefore open to any suggestions how to make it better. You are encouraged to come up with proposals.
         
         ---
         
         ### What's new in the latest version
         
+        - ZigZag indicator
         - IBS indicator
         - auto-sampling of input values
         
         - [v2.0.0 scope](https://github.com/nardew/talipp/issues/111)
         
-        For the full history of changes see [CHANGELOG](https://github.com/nardew/talipp/blob/main/CHANGELOG.md).
+        For the full history of changes see [CHANGELOG](https://github.com/nardew/talipp/releases).
         
         ---
         
         ### List of incremental indicators
         
         `talipp` currently provides below set of indicators. If your favourite indicator is missing, then create a ticket via GitHub Issues and there is a good chance that it will be included in the future version of the library.
         
@@ -90,14 +91,15 @@
         - SuperTrend
         - TRIX
         - TTM Squeeze
         - True Strength Index (TSI)
         - Ultimate Oscillator (UO)
         - Vortex Indicator (VTX)
         - Volume Weighted Average Price (VWAP)
+        - ZigZag
         
         ### Installation
         ```bash
         pip install talipp
         ```
         In case you want to install the latest version from the repo, use
         ```bash
```

### Comparing `talipp-2.2.1/README.md` & `talipp-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,21 @@
 
 Last but not least, `talipp` is a community project and therefore open to any suggestions how to make it better. You are encouraged to come up with proposals.
 
 ---
 
 ### What's new in the latest version
 
+- ZigZag indicator
 - IBS indicator
 - auto-sampling of input values
 
 - [v2.0.0 scope](https://github.com/nardew/talipp/issues/111)
 
-For the full history of changes see [CHANGELOG](https://github.com/nardew/talipp/blob/main/CHANGELOG.md).
+For the full history of changes see [CHANGELOG](https://github.com/nardew/talipp/releases).
 
 ---
 
 ### List of incremental indicators
 
 `talipp` currently provides below set of indicators. If your favourite indicator is missing, then create a ticket via GitHub Issues and there is a good chance that it will be included in the future version of the library.
 
@@ -82,14 +83,15 @@
 - SuperTrend
 - TRIX
 - TTM Squeeze
 - True Strength Index (TSI)
 - Ultimate Oscillator (UO)
 - Vortex Indicator (VTX)
 - Volume Weighted Average Price (VWAP)
+- ZigZag
 
 ### Installation
 ```bash
 pip install talipp
 ```
 In case you want to install the latest version from the repo, use
 ```bash
```

### Comparing `talipp-2.2.1/setup.py` & `talipp-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicator_util.py` & `talipp-2.3.0/talipp/indicator_util.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ADX.py` & `talipp-2.3.0/talipp/indicators/ADX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ALMA.py` & `talipp-2.3.0/talipp/indicators/ALMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/AO.py` & `talipp-2.3.0/talipp/indicators/AO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ATR.py` & `talipp-2.3.0/talipp/indicators/ATR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/AccuDist.py` & `talipp-2.3.0/talipp/indicators/AccuDist.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/Aroon.py` & `talipp-2.3.0/talipp/indicators/Aroon.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/BB.py` & `talipp-2.3.0/talipp/indicators/BB.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/BOP.py` & `talipp-2.3.0/talipp/indicators/BOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/CCI.py` & `talipp-2.3.0/talipp/indicators/CCI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/CHOP.py` & `talipp-2.3.0/talipp/indicators/CHOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ChaikinOsc.py` & `talipp-2.3.0/talipp/indicators/ChaikinOsc.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ChandeKrollStop.py` & `talipp-2.3.0/talipp/indicators/ChandeKrollStop.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/CoppockCurve.py` & `talipp-2.3.0/talipp/indicators/CoppockCurve.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/DEMA.py` & `talipp-2.3.0/talipp/indicators/DEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/DPO.py` & `talipp-2.3.0/talipp/indicators/DPO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/DonchianChannels.py` & `talipp-2.3.0/talipp/indicators/DonchianChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/EMA.py` & `talipp-2.3.0/talipp/indicators/EMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/EMV.py` & `talipp-2.3.0/talipp/indicators/EMV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ForceIndex.py` & `talipp-2.3.0/talipp/indicators/ForceIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/HMA.py` & `talipp-2.3.0/talipp/indicators/HMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/IBS.py` & `talipp-2.3.0/talipp/indicators/IBS.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/Ichimoku.py` & `talipp-2.3.0/talipp/indicators/Ichimoku.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/Indicator.py` & `talipp-2.3.0/talipp/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/KAMA.py` & `talipp-2.3.0/talipp/indicators/KAMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/KST.py` & `talipp-2.3.0/talipp/indicators/KST.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/KVO.py` & `talipp-2.3.0/talipp/indicators/KVO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/KeltnerChannels.py` & `talipp-2.3.0/talipp/indicators/KeltnerChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/MACD.py` & `talipp-2.3.0/talipp/indicators/MACD.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/MassIndex.py` & `talipp-2.3.0/talipp/indicators/MassIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/McGinleyDynamic.py` & `talipp-2.3.0/talipp/indicators/McGinleyDynamic.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/MeanDev.py` & `talipp-2.3.0/talipp/indicators/MeanDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/OBV.py` & `talipp-2.3.0/talipp/indicators/OBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ParabolicSAR.py` & `talipp-2.3.0/talipp/indicators/ParabolicSAR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/PivotsHL.py` & `talipp-2.3.0/talipp/indicators/PivotsHL.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     HIGH = enum.auto()
     """High pivot."""
 
 
 @dataclass
 class PivotsHLVal:
-    """`ParabolicSAR` output type.
+    """`PivotsHL` output type.
 
     Args:
         ohlcv: Pivot.
         type: Pivot type.
     """
 
     ohlcv: OHLCV = None
```

### Comparing `talipp-2.2.1/talipp/indicators/ROC.py` & `talipp-2.3.0/talipp/indicators/ROC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/RSI.py` & `talipp-2.3.0/talipp/indicators/RSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/SFX.py` & `talipp-2.3.0/talipp/indicators/SFX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/SMA.py` & `talipp-2.3.0/talipp/indicators/SMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/SMMA.py` & `talipp-2.3.0/talipp/indicators/SMMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/SOBV.py` & `talipp-2.3.0/talipp/indicators/SOBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/STC.py` & `talipp-2.3.0/talipp/indicators/STC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/StdDev.py` & `talipp-2.3.0/talipp/indicators/StdDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/Stoch.py` & `talipp-2.3.0/talipp/indicators/Stoch.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/StochRSI.py` & `talipp-2.3.0/talipp/indicators/StochRSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/SuperTrend.py` & `talipp-2.3.0/talipp/indicators/SuperTrend.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/T3.py` & `talipp-2.3.0/talipp/indicators/T3.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/TEMA.py` & `talipp-2.3.0/talipp/indicators/TEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/TRIX.py` & `talipp-2.3.0/talipp/indicators/TRIX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/TSI.py` & `talipp-2.3.0/talipp/indicators/TSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/TTM.py` & `talipp-2.3.0/talipp/indicators/TTM.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/UO.py` & `talipp-2.3.0/talipp/indicators/UO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/VTX.py` & `talipp-2.3.0/talipp/indicators/VTX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/VWAP.py` & `talipp-2.3.0/talipp/indicators/VWAP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/VWMA.py` & `talipp-2.3.0/talipp/indicators/VWMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/WMA.py` & `talipp-2.3.0/talipp/indicators/WMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/ZLEMA.py` & `talipp-2.3.0/talipp/indicators/ZLEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/indicators/__init__.py` & `talipp-2.3.0/talipp/indicators/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from .CHOP import CHOP as CHOP
 from .CoppockCurve import CoppockCurve as CoppockCurve
 from .DEMA import DEMA as DEMA
 from .DonchianChannels import DonchianChannels as DonchianChannels
 from .DPO import DPO as DPO
 from .EMA import EMA as EMA
 from .EMV import EMV as EMV
-from .FibRetracement import FibRetracement as FibRetracement
+from .FibonacciRetracement import FibonacciRetracement as FibonacciRetracement
 from .ForceIndex import ForceIndex as ForceIndex
 from .HMA import HMA as HMA
 from .IBS import IBS as IBS
 from .Ichimoku import Ichimoku as Ichimoku
 from .KAMA import KAMA as KAMA
 from .KeltnerChannels import KeltnerChannels as KeltnerChannels
 from .KST import KST as KST
@@ -49,14 +49,15 @@
 from .TSI import TSI as TSI
 from .TTM import TTM as TTM
 from .UO import UO as UO
 from .VTX import VTX as VTX
 from .VWAP import VWAP as VWAP
 from .VWMA import VWMA as VWMA
 from .WMA import WMA as WMA
+from .ZigZag import ZigZag as ZigZag
 from .ZLEMA import ZLEMA as ZLEMA
 
 __all__ = (
     "AccuDist",
     "ADX",
     "ALMA",
     "AO",
@@ -70,15 +71,15 @@
     "CHOP",
     "CoppockCurve",
     "DEMA",
     "DonchianChannels",
     "DPO",
     "EMA",
     "EMV",
-    "FibRetracement",
+    "FibonacciRetracement",
     "ForceIndex",
     "HMA",
     "IBS",
     "Ichimoku",
     "KAMA",
     "KeltnerChannels",
     "KST",
@@ -107,9 +108,10 @@
     "TSI",
     "TTM",
     "UO",
     "VTX",
     "VWAP",
     "VWMA",
     "WMA",
+    "ZigZag",
     "ZLEMA"
 )
```

### Comparing `talipp-2.2.1/talipp/input.py` & `talipp-2.3.0/talipp/input.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/ma.py` & `talipp-2.3.0/talipp/ma.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp/ohlcv.py` & `talipp-2.3.0/talipp/ohlcv.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/talipp.egg-info/PKG-INFO` & `talipp-2.3.0/talipp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talipp
-Version: 2.2.1
+Version: 2.3.0
 Summary: talipp - Incremental Technical Analysis Library
 Home-page: https://github.com/nardew/talipp
 Author: nardew
 Author-email: talipp.pyth@gmail.com
 License: UNKNOWN
 Description: # talipp - Incremental Technical Analysis Library
         
@@ -34,20 +34,21 @@
         
         Last but not least, `talipp` is a community project and therefore open to any suggestions how to make it better. You are encouraged to come up with proposals.
         
         ---
         
         ### What's new in the latest version
         
+        - ZigZag indicator
         - IBS indicator
         - auto-sampling of input values
         
         - [v2.0.0 scope](https://github.com/nardew/talipp/issues/111)
         
-        For the full history of changes see [CHANGELOG](https://github.com/nardew/talipp/blob/main/CHANGELOG.md).
+        For the full history of changes see [CHANGELOG](https://github.com/nardew/talipp/releases).
         
         ---
         
         ### List of incremental indicators
         
         `talipp` currently provides below set of indicators. If your favourite indicator is missing, then create a ticket via GitHub Issues and there is a good chance that it will be included in the future version of the library.
         
@@ -90,14 +91,15 @@
         - SuperTrend
         - TRIX
         - TTM Squeeze
         - True Strength Index (TSI)
         - Ultimate Oscillator (UO)
         - Vortex Indicator (VTX)
         - Volume Weighted Average Price (VWAP)
+        - ZigZag
         
         ### Installation
         ```bash
         pip install talipp
         ```
         In case you want to install the latest version from the repo, use
         ```bash
```

### Comparing `talipp-2.2.1/talipp.egg-info/SOURCES.txt` & `talipp-2.3.0/talipp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 talipp/indicators/ChandeKrollStop.py
 talipp/indicators/CoppockCurve.py
 talipp/indicators/DEMA.py
 talipp/indicators/DPO.py
 talipp/indicators/DonchianChannels.py
 talipp/indicators/EMA.py
 talipp/indicators/EMV.py
-talipp/indicators/FibRetracement.py
+talipp/indicators/FibonacciRetracement.py
 talipp/indicators/ForceIndex.py
 talipp/indicators/HMA.py
 talipp/indicators/IBS.py
 talipp/indicators/Ichimoku.py
 talipp/indicators/Indicator.py
 talipp/indicators/KAMA.py
 talipp/indicators/KST.py
@@ -66,14 +66,15 @@
 talipp/indicators/TTM.py
 talipp/indicators/UO.py
 talipp/indicators/VTX.py
 talipp/indicators/VWAP.py
 talipp/indicators/VWMA.py
 talipp/indicators/WMA.py
 talipp/indicators/ZLEMA.py
+talipp/indicators/ZigZag.py
 talipp/indicators/__init__.py
 test/test_ADX.py
 test/test_ALMA.py
 test/test_AO.py
 test/test_ATR.py
 test/test_AccuDist.py
 test/test_Aroon.py
@@ -121,11 +122,12 @@
 test/test_TTM.py
 test/test_UO.py
 test/test_VTX.py
 test/test_VWAP.py
 test/test_VWMA.py
 test/test_WMA.py
 test/test_ZLEMA.py
+test/test_ZigZag.py
 test/test_indicator_chaining.py
 test/test_indicator_sampling.py
 test/test_indicator_util.py
 test/test_input.py
```

### Comparing `talipp-2.2.1/test/test_ADX.py` & `talipp-2.3.0/test/test_ADX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ALMA.py` & `talipp-2.3.0/test/test_ALMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_AO.py` & `talipp-2.3.0/test/test_AO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ATR.py` & `talipp-2.3.0/test/test_ATR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_AccuDist.py` & `talipp-2.3.0/test/test_AccuDist.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_Aroon.py` & `talipp-2.3.0/test/test_Aroon.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_BB.py` & `talipp-2.3.0/test/test_BB.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_BOP.py` & `talipp-2.3.0/test/test_BOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_CCI.py` & `talipp-2.3.0/test/test_CCI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_CHOP.py` & `talipp-2.3.0/test/test_CHOP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ChaikinOsc.py` & `talipp-2.3.0/test/test_ChaikinOsc.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ChandeKrollStop.py` & `talipp-2.3.0/test/test_ChandeKrollStop.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_CoppockCurve.py` & `talipp-2.3.0/test/test_CoppockCurve.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_DEMA.py` & `talipp-2.3.0/test/test_DEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_DPO.py` & `talipp-2.3.0/test/test_DPO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_DonchianChannels.py` & `talipp-2.3.0/test/test_DonchianChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_EMA.py` & `talipp-2.3.0/test/test_EMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_EMV.py` & `talipp-2.3.0/test/test_EMV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ForceIndex.py` & `talipp-2.3.0/test/test_ForceIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_HMA.py` & `talipp-2.3.0/test/test_HMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_IBS.py` & `talipp-2.3.0/test/test_IBS.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_KAMA.py` & `talipp-2.3.0/test/test_KAMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_KST.py` & `talipp-2.3.0/test/test_KST.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_KVO.py` & `talipp-2.3.0/test/test_KVO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_KeltnerChannels.py` & `talipp-2.3.0/test/test_KeltnerChannels.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_MACD.py` & `talipp-2.3.0/test/test_MACD.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_MassIndex.py` & `talipp-2.3.0/test/test_MassIndex.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_McGinleyDynamic.py` & `talipp-2.3.0/test/test_McGinleyDynamic.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_MeanDev.py` & `talipp-2.3.0/test/test_MeanDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_OBV.py` & `talipp-2.3.0/test/test_OBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_OHLCV.py` & `talipp-2.3.0/test/test_OHLCV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ParabolicSAR.py` & `talipp-2.3.0/test/test_ParabolicSAR.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ROC.py` & `talipp-2.3.0/test/test_ROC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_RSI.py` & `talipp-2.3.0/test/test_RSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_SFX.py` & `talipp-2.3.0/test/test_SFX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_SMA.py` & `talipp-2.3.0/test/test_SMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_SMMA.py` & `talipp-2.3.0/test/test_SMMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_SOBV.py` & `talipp-2.3.0/test/test_SOBV.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_STC.py` & `talipp-2.3.0/test/test_STC.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_StdDev.py` & `talipp-2.3.0/test/test_StdDev.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_Stoch.py` & `talipp-2.3.0/test/test_Stoch.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_StochRSI.py` & `talipp-2.3.0/test/test_StochRSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_SuperTrend.py` & `talipp-2.3.0/test/test_SuperTrend.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_T3.py` & `talipp-2.3.0/test/test_T3.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_TEMA.py` & `talipp-2.3.0/test/test_TEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_TRIX.py` & `talipp-2.3.0/test/test_TRIX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_TSI.py` & `talipp-2.3.0/test/test_TSI.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_TTM.py` & `talipp-2.3.0/test/test_TTM.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_UO.py` & `talipp-2.3.0/test/test_UO.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_VTX.py` & `talipp-2.3.0/test/test_VTX.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_VWAP.py` & `talipp-2.3.0/test/test_VWAP.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_VWMA.py` & `talipp-2.3.0/test/test_VWMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_WMA.py` & `talipp-2.3.0/test/test_WMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_ZLEMA.py` & `talipp-2.3.0/test/test_ZLEMA.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_indicator_chaining.py` & `talipp-2.3.0/test/test_indicator_chaining.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_indicator_sampling.py` & `talipp-2.3.0/test/test_indicator_sampling.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_indicator_util.py` & `talipp-2.3.0/test/test_indicator_util.py`

 * *Files identical despite different names*

### Comparing `talipp-2.2.1/test/test_input.py` & `talipp-2.3.0/test/test_input.py`

 * *Files identical despite different names*

