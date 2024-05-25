# Comparing `tmp/MobileInventoryCLI-0.4.98.tar.gz` & `tmp/MobileInventoryCLI-0.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.98.tar", last modified: Tue May  7 14:56:25 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.99.tar", last modified: Tue May  7 15:27:16 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.98.tar` & `MobileInventoryCLI-0.4.99.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.094138 MobileInventoryCLI-0.4.98/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.080804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.080804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.084138 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.084138 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.084138 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.084138 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2690 2024-05-07 14:56:05.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/SMLabelImporter.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   117305 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
--rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     7211 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.087471 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    22046 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    84220 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    29832 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-07 14:56:21.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5953 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        6 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/version.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.090804 MobileInventoryCLI-0.4.98/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-07 14:51:07.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:25.094138 MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-07 14:56:25.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5568 2024-05-07 14:56:25.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-07 14:56:25.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-05-07 14:56:25.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-07 14:56:25.000000 MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-05-07 14:56:25.094138 MobileInventoryCLI-0.4.98/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-07 14:56:25.094138 MobileInventoryCLI-0.4.98/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-05-07 14:56:24.000000 MobileInventoryCLI-0.4.98/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.037550 MobileInventoryCLI-0.4.99/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.024217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.024217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.027550 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.027550 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    38216 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.027550 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.027550 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)    10261 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3146 2024-05-07 15:16:18.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/SMLabelImporter.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   117305 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      310 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/testClass.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     7211 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6122 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.030883 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4349 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    18881 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    22046 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    84220 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    29832 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1191 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-05-07 15:26:23.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2781 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5953 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        6 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/version.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-05-07 14:56:32.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-07 15:27:16.034217 MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      884 2024-05-07 15:27:15.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5568 2024-05-07 15:27:15.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-07 15:27:15.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      140 2024-05-07 15:27:15.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-05-07 15:27:15.000000 MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      884 2024-05-07 15:27:16.037550 MobileInventoryCLI-0.4.99/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-07 15:27:16.037550 MobileInventoryCLI-0.4.99/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      973 2024-05-07 15:27:14.000000 MobileInventoryCLI-0.4.99/setup.py
```

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/SMLabelImporter.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/SMLabelImporter.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,38 +32,47 @@
         tables=soup.find_all('table')
         csvd=[]
         csvd.append(['Barcode','Code','Name','ALT_Barcode'])
         for r in tables:
             links=r.find_all('a')
             for link in links:
                 name,upc=link.text,str(link['href'].split('/')[-1])[2:]
+                print(str(link['href']))
                 if name != '':
                     if upc != '':
                         try:
+                            print(upc)
                             if len(upc) > 8:
                                 upca=UPCA(upc)
                                 upce=convert.convert_barcode_from_upca_to_upce(upc)
                             else:
+                                if len(upc) < 8:
+                                    print(f"invalid barcode '{upc}'")
+                                    continue
                                 upce=upc
                                 upca=convert.convert_barcode_from_upce_to_upca(upc)
                             if upce == False:
                                 upce=''
                             csvd.append([upca,'',name.replace('\n','$newline$').replace(';','$semicolon$'),upce])
-                            print(name,upca,upce)
+                            print(name,upca,upce,'added',sep=';')
                         except Exception as e:
-                            print(name,upc,e)
+                            print(name,upc,e,'Exception')
         if engine != None:
             with Session(engine) as session:
                 for num,(upc,code,name,alt) in enumerate(csvd):
-                    check=session.query(Entry).filter(Barcode==str(upc)).first()
+                    print((upc,code,name,alt))
+                    check=session.query(Entry).filter(Entry.Barcode==str(upc)).first()
                     if not check:
+                        print(f"adding {upc} -> {name}")
                         ne=Entry(Barcode=str(upc),Code=str(code),Name=name,ALT_Barcode=str(alt),Price=0,CaseCount=1)
                         session.add(ne)
                         if num % 30 == 0:
                             session.commit()
+                    else:
+                        print(check.seeShort())
                 session.commit()
                 session.flush()
 
 
         writer.writerows(csvd)
         #print(links)
 if __name__ == "__main__":
```

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.98
+Version: 0.4.99
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
@@ -22,7 +22,8 @@
 Requires-Dist: Pillow
 Requires-Dist: python-barcode
 Requires-Dist: qrcode
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
 Requires-Dist: argparse
 Requires-Dist: geocoder
+Requires-Dist: beautifulsoup4
```

### Comparing `MobileInventoryCLI-0.4.98/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.99/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.98/PKG-INFO` & `MobileInventoryCLI-0.4.99/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.98
+Version: 0.4.99
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
@@ -22,7 +22,8 @@
 Requires-Dist: Pillow
 Requires-Dist: python-barcode
 Requires-Dist: qrcode
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
 Requires-Dist: argparse
 Requires-Dist: geocoder
+Requires-Dist: beautifulsoup4
```

### Comparing `MobileInventoryCLI-0.4.98/setup.py` & `MobileInventoryCLI-0.4.99/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.98'
+version='0.4.99'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
@@ -13,13 +13,13 @@
         'Operating System :: OS Independent',
         'Operating System :: Android',
         'Environment :: Console',
         'Programming Language :: SQL',
           ],
       packages=find_packages(),
       python_requires='>=3.6',
-      install_requires=['cython','pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow','python-barcode','qrcode','requests','sqlalchemy','argparse','geocoder'],
+      install_requires=['cython','pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow','python-barcode','qrcode','requests','sqlalchemy','argparse','geocoder','beautifulsoup4'],
       package_data={
         '':["*.config","*.txt","*.README","*.TTF"],
         }
       )
```

