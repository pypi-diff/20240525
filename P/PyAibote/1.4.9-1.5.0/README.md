# Comparing `tmp/PyAibote-1.4.9.tar.gz` & `tmp/PyAibote-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.4.9.tar", last modified: Sat May 25 02:05:35 2024, max compression
+gzip compressed data, was "PyAibote-1.5.0.tar", last modified: Sat May 25 08:25:17 2024, max compression
```

## Comparing `PyAibote-1.4.9.tar` & `PyAibote-1.5.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:35.352908 PyAibote-1.4.9/
--rw-rw-rw-   0        0        0     1089 2024-05-25 02:05:35.332902 PyAibote-1.4.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:34.772272 PyAibote-1.4.9/PyAibote/
--rw-rw-rw-   0        0        0     2679 2024-05-25 01:54:49.000000 PyAibote-1.4.9/PyAibote/AndroidBot.py
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:34.913272 PyAibote-1.4.9/PyAibote/AndroidBotModel/
--rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
--rw-rw-rw-   0        0        0     2381 2024-04-22 13:58:45.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/AndroidLoadWait.py
--rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/ColorFindingOperation.py
--rw-rw-rw-   0        0        0     6178 2024-05-14 09:14:47.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/Control.py
--rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/CoordinateOperation.py
--rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/EquipmentOperation.py
--rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/FileTransfer.py
--rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/MapFindingOperation.py
--rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/OcrCorrelation.py
--rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
--rw-rw-rw-   0        0        0     9217 2024-04-22 14:06:16.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/ScreenshotOperation.py
--rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/UrlRequest.py
--rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/YoloService.py
--rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.4.9/PyAibote/AndroidBotModel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:34.918272 PyAibote-1.4.9/PyAibote/CommonUse/
--rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.4.9/PyAibote/CommonUse/ChatGenerative.py
--rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.4.9/PyAibote/CommonUse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:35.052908 PyAibote-1.4.9/PyAibote/Tool/
--rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.4.9/PyAibote/Tool/DatabaseFunc.py
--rw-rw-rw-   0        0        0     2188 2024-04-30 01:29:58.000000 PyAibote-1.4.9/PyAibote/Tool/DebugStartDriver.py
--rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.4.9/PyAibote/Tool/Logger.py
--rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.4.9/PyAibote/Tool/LoggerFunc.py
--rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.4.9/PyAibote/Tool/SendTcpData.py
--rw-rw-rw-   0        0        0     1090 2024-05-25 02:00:00.000000 PyAibote-1.4.9/PyAibote/Tool/SocketServer.py
--rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.4.9/PyAibote/Tool/Sqlite3DataBase.py
--rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.4.9/PyAibote/Tool/UniversalFunction.py
--rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.4.9/PyAibote/Tool/WriteReadFileFunc.py
--rw-rw-rw-   0        0        0      550 2024-05-25 01:55:35.000000 PyAibote-1.4.9/PyAibote/Tool/__init__.py
--rw-rw-rw-   0        0        0     2024 2024-05-18 03:36:32.000000 PyAibote-1.4.9/PyAibote/WebBot.py
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:35.223909 PyAibote-1.4.9/PyAibote/WebBotModel/
--rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.4.9/PyAibote/WebBotModel/CookiesOperation.py
--rw-rw-rw-   0        0        0     1356 2024-05-11 08:59:42.000000 PyAibote-1.4.9/PyAibote/WebBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.4.9/PyAibote/WebBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.4.9/PyAibote/WebBotModel/IframeOperation.py
--rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.4.9/PyAibote/WebBotModel/JSinjection.py
--rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.4.9/PyAibote/WebBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.4.9/PyAibote/WebBotModel/PagesAndNavigation.py
--rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.4.9/PyAibote/WebBotModel/PopUpWindow.py
--rw-rw-rw-   0        0        0     3421 2024-04-22 07:22:21.000000 PyAibote-1.4.9/PyAibote/WebBotModel/WebLoadWait.py
--rw-rw-rw-   0        0        0     5548 2024-04-24 07:42:11.000000 PyAibote-1.4.9/PyAibote/WebBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0      718 2024-05-18 03:36:16.000000 PyAibote-1.4.9/PyAibote/WebBotModel/__init__.py
--rw-rw-rw-   0        0        0     4186 2024-05-25 01:54:28.000000 PyAibote-1.4.9/PyAibote/WindowsBot.py
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:35.329908 PyAibote-1.4.9/PyAibote/WindowsBotModel/
--rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/ColorOperation.py
--rw-rw-rw-   0        0        0    23558 2024-05-14 08:46:42.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/DigitalHumanOperation.py
--rw-rw-rw-   0        0        0     2221 2024-05-11 08:52:11.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/ExcelOperation.py
--rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/OcrOperation.py
--rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/OtherOperations.py
--rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/SystemOperation.py
--rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/VoiceService.py
--rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/WinHidCorrelation.py
--rw-rw-rw-   0        0        0     2412 2024-04-22 07:22:40.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/WinLoadWait.py
--rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/YoloOperation.py
--rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.4.9/PyAibote/WindowsBotModel/__init__.py
--rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.4.9/PyAibote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 02:05:34.808263 PyAibote-1.4.9/PyAibote.egg-info/
--rw-rw-rw-   0        0        0     1089 2024-05-25 02:05:34.000000 PyAibote-1.4.9/PyAibote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2024-05-25 02:05:34.000000 PyAibote-1.4.9/PyAibote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 02:05:34.000000 PyAibote-1.4.9/PyAibote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-25 02:05:34.000000 PyAibote-1.4.9/PyAibote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-25 02:05:34.000000 PyAibote-1.4.9/PyAibote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10966 2024-05-11 08:33:55.000000 PyAibote-1.4.9/README.md
--rw-rw-rw-   0        0        0       42 2024-05-25 02:05:35.353901 PyAibote-1.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1425 2024-05-25 02:03:20.000000 PyAibote-1.4.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.718847 PyAibote-1.5.0/
+-rw-rw-rw-   0        0        0     1089 2024-05-25 08:25:17.706848 PyAibote-1.5.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.224640 PyAibote-1.5.0/PyAibote/
+-rw-rw-rw-   0        0        0     2679 2024-05-25 01:54:49.000000 PyAibote-1.5.0/PyAibote/AndroidBot.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.394638 PyAibote-1.5.0/PyAibote/AndroidBotModel/
+-rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
+-rw-rw-rw-   0        0        0     2381 2024-04-22 13:58:45.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/AndroidLoadWait.py
+-rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/ColorFindingOperation.py
+-rw-rw-rw-   0        0        0     6178 2024-05-14 09:14:47.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/Control.py
+-rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/CoordinateOperation.py
+-rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/EquipmentOperation.py
+-rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/FileTransfer.py
+-rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/MapFindingOperation.py
+-rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/OcrCorrelation.py
+-rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
+-rw-rw-rw-   0        0        0     9217 2024-04-22 14:06:16.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/ScreenshotOperation.py
+-rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/UrlRequest.py
+-rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/YoloService.py
+-rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.5.0/PyAibote/AndroidBotModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.400644 PyAibote-1.5.0/PyAibote/CommonUse/
+-rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.5.0/PyAibote/CommonUse/ChatGenerative.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.5.0/PyAibote/CommonUse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.470642 PyAibote-1.5.0/PyAibote/Tool/
+-rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.5.0/PyAibote/Tool/DatabaseFunc.py
+-rw-rw-rw-   0        0        0     2188 2024-04-30 01:29:58.000000 PyAibote-1.5.0/PyAibote/Tool/DebugStartDriver.py
+-rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.5.0/PyAibote/Tool/Logger.py
+-rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.5.0/PyAibote/Tool/LoggerFunc.py
+-rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.5.0/PyAibote/Tool/SendTcpData.py
+-rw-rw-rw-   0        0        0     1090 2024-05-25 02:00:00.000000 PyAibote-1.5.0/PyAibote/Tool/SocketServer.py
+-rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.5.0/PyAibote/Tool/Sqlite3DataBase.py
+-rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.5.0/PyAibote/Tool/UniversalFunction.py
+-rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.5.0/PyAibote/Tool/WriteReadFileFunc.py
+-rw-rw-rw-   0        0        0      550 2024-05-25 01:55:35.000000 PyAibote-1.5.0/PyAibote/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2024 2024-05-18 03:36:32.000000 PyAibote-1.5.0/PyAibote/WebBot.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.597332 PyAibote-1.5.0/PyAibote/WebBotModel/
+-rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.5.0/PyAibote/WebBotModel/CookiesOperation.py
+-rw-rw-rw-   0        0        0     1356 2024-05-11 08:59:42.000000 PyAibote-1.5.0/PyAibote/WebBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.5.0/PyAibote/WebBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.5.0/PyAibote/WebBotModel/IframeOperation.py
+-rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.5.0/PyAibote/WebBotModel/JSinjection.py
+-rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.5.0/PyAibote/WebBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.5.0/PyAibote/WebBotModel/PagesAndNavigation.py
+-rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.5.0/PyAibote/WebBotModel/PopUpWindow.py
+-rw-rw-rw-   0        0        0     3421 2024-04-22 07:22:21.000000 PyAibote-1.5.0/PyAibote/WebBotModel/WebLoadWait.py
+-rw-rw-rw-   0        0        0     5548 2024-04-24 07:42:11.000000 PyAibote-1.5.0/PyAibote/WebBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0      718 2024-05-18 03:36:16.000000 PyAibote-1.5.0/PyAibote/WebBotModel/__init__.py
+-rw-rw-rw-   0        0        0     4186 2024-05-25 01:54:28.000000 PyAibote-1.5.0/PyAibote/WindowsBot.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.702847 PyAibote-1.5.0/PyAibote/WindowsBotModel/
+-rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/ColorOperation.py
+-rw-rw-rw-   0        0        0    23558 2024-05-14 08:46:42.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/DigitalHumanOperation.py
+-rw-rw-rw-   0        0        0     2221 2024-05-11 08:52:11.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/ExcelOperation.py
+-rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/OcrOperation.py
+-rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/OtherOperations.py
+-rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/SystemOperation.py
+-rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/VoiceService.py
+-rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/WinHidCorrelation.py
+-rw-rw-rw-   0        0        0     2412 2024-04-22 07:22:40.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/WinLoadWait.py
+-rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/YoloOperation.py
+-rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.5.0/PyAibote/WindowsBotModel/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.5.0/PyAibote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:25:17.271639 PyAibote-1.5.0/PyAibote.egg-info/
+-rw-rw-rw-   0        0        0     1089 2024-05-25 08:25:17.000000 PyAibote-1.5.0/PyAibote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2493 2024-05-25 08:25:17.000000 PyAibote-1.5.0/PyAibote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 08:25:17.000000 PyAibote-1.5.0/PyAibote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-25 08:25:17.000000 PyAibote-1.5.0/PyAibote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 08:25:17.000000 PyAibote-1.5.0/PyAibote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10966 2024-05-11 08:33:55.000000 PyAibote-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-25 08:25:17.718847 PyAibote-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2024-05-25 08:24:57.000000 PyAibote-1.5.0/setup.py
```

### Comparing `PyAibote-1.4.9/PKG-INFO` & `PyAibote-1.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.9
+Version: 1.5.0
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.5,<4.0
 Description-Content-Type: text/markdown
 
 Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium
```

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBot.py` & `PyAibote-1.5.0/PyAibote/AndroidBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/AndroidHidCorrelation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/AndroidHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/AndroidLoadWait.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/AndroidLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/ColorFindingOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/ColorFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/Control.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/Control.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/CoordinateOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/CoordinateOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/ElementOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/EquipmentOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/EquipmentOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/FileTransfer.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/FileTransfer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/MapFindingOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/MapFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/OcrCorrelation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/OcrCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/ScreenProjectionOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/ScreenProjectionOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/ScreenshotOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/ScreenshotOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/UrlRequest.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/UrlRequest.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/VerificationCodeOperation.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/YoloService.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/YoloService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/AndroidBotModel/__init__.py` & `PyAibote-1.5.0/PyAibote/AndroidBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/CommonUse/ChatGenerative.py` & `PyAibote-1.5.0/PyAibote/CommonUse/ChatGenerative.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/DatabaseFunc.py` & `PyAibote-1.5.0/PyAibote/Tool/DatabaseFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/DebugStartDriver.py` & `PyAibote-1.5.0/PyAibote/Tool/DebugStartDriver.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/Logger.py` & `PyAibote-1.5.0/PyAibote/Tool/Logger.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/LoggerFunc.py` & `PyAibote-1.5.0/PyAibote/Tool/LoggerFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/SendTcpData.py` & `PyAibote-1.5.0/PyAibote/Tool/SendTcpData.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/SocketServer.py` & `PyAibote-1.5.0/PyAibote/Tool/SocketServer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/Sqlite3DataBase.py` & `PyAibote-1.5.0/PyAibote/Tool/Sqlite3DataBase.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/UniversalFunction.py` & `PyAibote-1.5.0/PyAibote/Tool/UniversalFunction.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/WriteReadFileFunc.py` & `PyAibote-1.5.0/PyAibote/Tool/WriteReadFileFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/Tool/__init__.py` & `PyAibote-1.5.0/PyAibote/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBot.py` & `PyAibote-1.5.0/PyAibote/WebBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/CookiesOperation.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/CookiesOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/DrivingOperation.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/ElementOperation.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/IframeOperation.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/IframeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/JSinjection.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/JSinjection.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/KeymouseOperation.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/PagesAndNavigation.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/PagesAndNavigation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/PopUpWindow.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/PopUpWindow.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/WebLoadWait.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/WebLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/WindowOperation.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WebBotModel/__init__.py` & `PyAibote-1.5.0/PyAibote/WebBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBot.py` & `PyAibote-1.5.0/PyAibote/WindowsBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/ColorOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/ColorOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/DigitalHumanOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/DigitalHumanOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/DrivingOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/ElementOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/ExcelOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/ExcelOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/KeymouseOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/OcrOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/OcrOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/OtherOperations.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/OtherOperations.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/SystemOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/SystemOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/VerificationCodeOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/VoiceService.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/VoiceService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/WinHidCorrelation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/WinHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/WinLoadWait.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/WinLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/WindowOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/YoloOperation.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/YoloOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote/WindowsBotModel/__init__.py` & `PyAibote-1.5.0/PyAibote/WindowsBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/PyAibote.egg-info/PKG-INFO` & `PyAibote-1.5.0/PyAibote.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.9
+Version: 1.5.0
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.5,<4.0
 Description-Content-Type: text/markdown
 
 Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium
```

### Comparing `PyAibote-1.4.9/PyAibote.egg-info/SOURCES.txt` & `PyAibote-1.5.0/PyAibote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/README.md` & `PyAibote-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.9/setup.py` & `PyAibote-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     "Pillow",
     "requests",
     "pymysql"
 ]
 
 setup(
     name="PyAibote", 
-    version="1.4.9", 
+    version="1.5.0", 
     author="Riven", 
     author_email="pyaibote@163.com", 
     description="A pure code RPA office automation framework, which supports Android, Browser and Windows", 
     long_description="Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium", # 加载read_me的内容
     long_description_content_type="text/markdown", 
     url="https://www.pyaibote.com",  
     packages=packages, 
     package_data={"": ['*.py']},
     install_requires = install_requires,
-    python_requires = ">=3.7,<4.0"
+    python_requires = ">=3.5,<4.0"
 )
```

