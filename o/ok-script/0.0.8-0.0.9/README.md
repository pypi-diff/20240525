# Comparing `tmp/ok-script-0.0.8.tar.gz` & `tmp/ok-script-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ok-script-0.0.8.tar", last modified: Mon Apr  8 16:53:20 2024, max compression
+gzip compressed data, was "ok-script-0.0.9.tar", last modified: Sun Apr 14 03:16:19 2024, max compression
```

## Comparing `ok-script-0.0.8.tar` & `ok-script-0.0.9.tar`

### file list

```diff
@@ -1,170 +1,173 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.822513 ok-script-0.0.8/
--rw-rw-rw-   0        0        0     2196 2024-04-08 16:53:20.821519 ok-script-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2024-02-09 15:31:41.000000 ok-script-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.324413 ok-script-0.0.8/ok/
--rw-rw-rw-   0        0        0     5055 2024-04-08 14:20:09.000000 ok-script-0.0.8/ok/OK.py
--rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.8/ok/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.333496 ok-script-0.0.8/ok/capture/
--rw-rw-rw-   0        0        0      602 2024-04-05 09:34:11.000000 ok-script-0.0.8/ok/capture/BaseCaptureMethod.py
--rw-rw-rw-   0        0        0     5347 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/HwndWindow.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:29:44.000000 ok-script-0.0.8/ok/capture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.360165 ok-script-0.0.8/ok/capture/adb/
--rw-rw-rw-   0        0        0      908 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/adb/ADBCaptureMethod.py
--rw-rw-rw-   0        0        0     8433 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/adb/DeviceManager.py
--rw-rw-rw-   0        0        0        0 2024-02-04 14:45:00.000000 ok-script-0.0.8/ok/capture/adb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.361671 ok-script-0.0.8/ok/capture/adb/bin/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/capture/adb/bin/__init__.py
--rw-rw-rw-   0        0        0     2355 2024-03-14 10:16:17.000000 ok-script-0.0.8/ok/capture/adb/targets.py
--rw-rw-rw-   0        0        0     5784 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/adb/vbox.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.399565 ok-script-0.0.8/ok/capture/windows/
--rw-rw-rw-   0        0        0     9158 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/windows/WindowsGraphicsCaptureMethod.py
--rw-rw-rw-   0        0        0        0 2024-02-03 03:10:06.000000 ok-script-0.0.8/ok/capture/windows/__init__.py
--rw-rw-rw-   0        0        0     2673 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/capture/windows/d3d11.py
--rw-rw-rw-   0        0        0     4639 2024-03-16 14:22:58.000000 ok-script-0.0.8/ok/capture/windows/utils.py
--rw-rw-rw-   0        0        0     1320 2024-04-01 01:55:20.000000 ok-script-0.0.8/ok/capture/windows/window.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.405474 ok-script-0.0.8/ok/color/
--rw-rw-rw-   0        0        0     1550 2024-03-18 15:46:15.000000 ok-script-0.0.8/ok/color/Color.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/color/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.414804 ok-script-0.0.8/ok/config/
--rw-rw-rw-   0        0        0     2195 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/config/Config.py
--rw-rw-rw-   0        0        0      386 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/config/InfoDict.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.443530 ok-script-0.0.8/ok/feature/
--rw-rw-rw-   0        0        0     7181 2024-03-24 13:07:51.000000 ok-script-0.0.8/ok/feature/Box.py
--rw-rw-rw-   0        0        0      739 2024-03-16 12:36:18.000000 ok-script-0.0.8/ok/feature/Feature.py
--rw-rw-rw-   0        0        0     9052 2024-04-08 14:19:18.000000 ok-script-0.0.8/ok/feature/FeatureSet.py
--rw-rw-rw-   0        0        0     2104 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/feature/FindFeature.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.472314 ok-script-0.0.8/ok/gui/
--rw-rw-rw-   0        0        0     4501 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/App.py
--rw-rw-rw-   0        0        0      604 2024-04-03 09:22:41.000000 ok-script-0.0.8/ok/gui/Communicate.py
--rw-rw-rw-   0        0        0     2541 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/MainWindow.py
--rw-rw-rw-   0        0        0     1849 2024-03-07 15:43:39.000000 ok-script-0.0.8/ok/gui/TabTitles.py
--rw-rw-rw-   0        0        0      132 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.502660 ok-script-0.0.8/ok/gui/debug/
--rw-rw-rw-   0        0        0     1213 2024-03-08 05:29:34.000000 ok-script-0.0.8/ok/gui/debug/AspectRatioWidget.py
--rw-rw-rw-   0        0        0     1334 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/DebugTab.py
--rw-rw-rw-   0        0        0     5095 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/FrameWidget.py
--rw-rw-rw-   0        0        0     1211 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/InfoWidget.py
--rw-rw-rw-   0        0        0     2690 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/debug/LoggerWidget.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/debug/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.507527 ok-script-0.0.8/ok/gui/i18n/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/i18n/__init__.py
--rw-rw-rw-   0        0        0       52 2024-04-01 11:14:15.000000 ok-script-0.0.8/ok/gui/i18n/path.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.511455 ok-script-0.0.8/ok/gui/icon/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/icon/__init__.py
--rw-rw-rw-   0        0        0      174 2024-03-26 17:34:24.000000 ok-script-0.0.8/ok/gui/icon/icon.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.516384 ok-script-0.0.8/ok/gui/loading/
--rw-rw-rw-   0        0        0     6156 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/loading/LoadingWindow.py
--rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.8/ok/gui/loading/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.522325 ok-script-0.0.8/ok/gui/overlay/
--rw-rw-rw-   0        0        0     1402 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/overlay/OverlayWindow.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/overlay/__init__.py
--rw-rw-rw-   0        0        0    22185 2024-04-04 16:18:48.000000 ok-script-0.0.8/ok/gui/resources.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.550306 ok-script-0.0.8/ok/gui/tasks/
--rw-rw-rw-   0        0        0      668 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/ConfigItemFactory.py
--rw-rw-rw-   0        0        0     1567 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/StartButton.py
--rw-rw-rw-   0        0        0      903 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/TaskOpButton.py
--rw-rw-rw-   0        0        0     5969 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/tasks/TaskTab.py
--rw-rw-rw-   0        0        0     1546 2024-04-03 14:53:01.000000 ok-script-0.0.8/ok/gui/tasks/TooltipTableWidget.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/tasks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.565517 ok-script-0.0.8/ok/gui/util/
--rw-rw-rw-   0        0        0      400 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/util/Alert.py
--rw-rw-rw-   0        0        0      356 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/util/InitWorker.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/util/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.585979 ok-script-0.0.8/ok/gui/widget/
--rw-rw-rw-   0        0        0      943 2024-04-08 14:19:18.000000 ok-script-0.0.8/ok/gui/widget/ListTableWidgetItem.py
--rw-rw-rw-   0        0        0     1316 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/widget/NumericTableWidgetItem.py
--rw-rw-rw-   0        0        0     2126 2024-04-02 12:32:43.000000 ok-script-0.0.8/ok/gui/widget/RoundCornerContainer.py
--rw-rw-rw-   0        0        0      830 2024-03-25 08:54:00.000000 ok-script-0.0.8/ok/gui/widget/TabWidget.py
--rw-rw-rw-   0        0        0      399 2024-03-25 14:18:22.000000 ok-script-0.0.8/ok/gui/widget/UpdateConfigWidgetItem.py
--rw-rw-rw-   0        0        0      685 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/gui/widget/YesNonWidgetItem.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/gui/widget/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.599219 ok-script-0.0.8/ok/interaction/
--rw-rw-rw-   0        0        0     1153 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/interaction/ADBInteraction.py
--rw-rw-rw-   0        0        0     1050 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/interaction/BaseInteraction.py
--rw-rw-rw-   0        0        0     1693 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/interaction/Win32Interaction.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/interaction/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.604071 ok-script-0.0.8/ok/logging/
--rw-rw-rw-   0        0        0     3618 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/logging/Logger.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.608960 ok-script-0.0.8/ok/ocr/
--rw-rw-rw-   0        0        0     2099 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/ocr/OCR.py
--rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.8/ok/ocr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.612463 ok-script-0.0.8/ok/predict/
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/predict/__init__.py
--rw-rw-rw-   0        0        0     1595 2023-12-15 17:49:57.000000 ok-script-0.0.8/ok/predict/predict.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.662316 ok-script-0.0.8/ok/rotypes/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.664508 ok-script-0.0.8/ok/rotypes/Windows/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.668402 ok-script-0.0.8/ok/rotypes/Windows/Foundation/
--rw-rw-rw-   0        0        0     2023 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Foundation/Collections.py
--rw-rw-rw-   0        0        0     5385 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Foundation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.672366 ok-script-0.0.8/ok/rotypes/Windows/Globalization/
--rw-rw-rw-   0        0        0      909 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Globalization/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.674316 ok-script-0.0.8/ok/rotypes/Windows/Graphics/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.676262 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Capture/
--rw-rw-rw-   0        0        0     4675 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Capture/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.679184 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.682674 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/
--rw-rw-rw-   0        0        0     1234 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py
--rw-rw-rw-   0        0        0     4181 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.684620 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Imaging/
--rw-rw-rw-   0        0        0     1053 2024-04-08 14:19:18.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/Imaging/__init__.py
--rw-rw-rw-   0        0        0      127 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Graphics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.687541 ok-script-0.0.8/ok/rotypes/Windows/Media/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.689487 ok-script-0.0.8/ok/rotypes/Windows/Media/Ocr/
--rw-rw-rw-   0        0        0     3039 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Media/Ocr/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Media/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.691468 ok-script-0.0.8/ok/rotypes/Windows/Security/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.694425 ok-script-0.0.8/ok/rotypes/Windows/Security/Cryptography/
--rw-rw-rw-   0        0        0      675 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Security/Cryptography/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Security/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.695397 ok-script-0.0.8/ok/rotypes/Windows/Storage/
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.697342 ok-script-0.0.8/ok/rotypes/Windows/Storage/Streams/
--rw-rw-rw-   0        0        0      837 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/rotypes/Windows/Storage/Streams/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/Storage/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/Windows/__init__.py
--rw-rw-rw-   0        0        0      145 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/__init__.py
--rw-rw-rw-   0        0        0     3532 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/delegate.py
--rw-rw-rw-   0        0        0      575 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/export.py
--rw-rw-rw-   0        0        0     9281 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/idldsl.py
--rw-rw-rw-   0        0        0     2311 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/inspectable.py
--rw-rw-rw-   0        0        0      840 2024-03-14 16:08:07.000000 ok-script-0.0.8/ok/rotypes/roapi.py
--rw-rw-rw-   0        0        0     2560 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/types.py
--rw-rw-rw-   0        0        0     1566 2024-01-26 14:10:34.000000 ok-script-0.0.8/ok/rotypes/winstring.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.715599 ok-script-0.0.8/ok/save/
--rw-rw-rw-   0        0        0      796 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/BlackBarProcessor.py
--rw-rw-rw-   0        0        0       97 2024-03-16 12:49:02.000000 ok-script-0.0.8/ok/save/PostProcessor.py
--rw-rw-rw-   0        0        0      828 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/SaveByInterval.py
--rw-rw-rw-   0        0        0     1019 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/SaveByKeyPress.py
--rw-rw-rw-   0        0        0     1455 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/save/SaveMethodBase.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/save/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.724481 ok-script-0.0.8/ok/scene/
--rw-rw-rw-   0        0        0      328 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/scene/FeatureScene.py
--rw-rw-rw-   0        0        0      576 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/scene/Scene.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/scene/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.728376 ok-script-0.0.8/ok/stats/
--rw-rw-rw-   0        0        0     1014 2024-02-26 12:12:14.000000 ok-script-0.0.8/ok/stats/StreamStats.py
--rw-rw-rw-   0        0        0        0 2024-02-06 15:39:35.000000 ok-script-0.0.8/ok/stats/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.757717 ok-script-0.0.8/ok/task/
--rw-rw-rw-   0        0        0     3096 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/BaseTask.py
--rw-rw-rw-   0        0        0     4788 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/ExecutorOperation.py
--rw-rw-rw-   0        0        0      148 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/FindFeatureTask.py
--rw-rw-rw-   0        0        0     9455 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/task/TaskExecutor.py
--rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.8/ok/task/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.779705 ok-script-0.0.8/ok/util/
--rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.8/ok/util/__init__.py
--rw-rw-rw-   0        0        0      699 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/util/json.py
--rw-rw-rw-   0        0        0      109 2024-04-02 11:28:23.000000 ok-script-0.0.8/ok/util/list.py
--rw-rw-rw-   0        0        0     1127 2024-04-04 17:00:56.000000 ok-script-0.0.8/ok/util/path.py
--rw-rw-rw-   0        0        0      246 2024-03-26 05:25:09.000000 ok-script-0.0.8/ok/util/thread.py
--rw-rw-rw-   0        0        0     2923 2024-03-14 10:21:07.000000 ok-script-0.0.8/ok/util/win32_process.py
--rw-rw-rw-   0        0        0      727 2024-04-08 14:19:17.000000 ok-script-0.0.8/ok/util/yaml.py
-drwxrwxrwx   0        0        0        0 2024-04-08 16:53:20.816592 ok-script-0.0.8/ok_script.egg-info/
--rw-rw-rw-   0        0        0     2196 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3422 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2024-04-08 16:53:20.000000 ok-script-0.0.8/ok_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 16:53:20.823486 ok-script-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-04-08 16:52:53.000000 ok-script-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.949245 ok-script-0.0.9/
+-rw-rw-rw-   0        0        0     2199 2024-04-14 03:16:19.948241 ok-script-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1516 2024-04-10 02:48:54.000000 ok-script-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.500138 ok-script-0.0.9/ok/
+-rw-rw-rw-   0        0        0     5165 2024-04-13 17:30:30.000000 ok-script-0.0.9/ok/OK.py
+-rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.9/ok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.505313 ok-script-0.0.9/ok/capture/
+-rw-rw-rw-   0        0        0      602 2024-04-05 09:34:11.000000 ok-script-0.0.9/ok/capture/BaseCaptureMethod.py
+-rw-rw-rw-   0        0        0     5347 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/capture/HwndWindow.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:29:44.000000 ok-script-0.0.9/ok/capture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.513188 ok-script-0.0.9/ok/capture/adb/
+-rw-rw-rw-   0        0        0      908 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/capture/adb/ADBCaptureMethod.py
+-rw-rw-rw-   0        0        0     8035 2024-04-10 15:45:57.000000 ok-script-0.0.9/ok/capture/adb/DeviceManager.py
+-rw-rw-rw-   0        0        0        0 2024-02-04 14:45:00.000000 ok-script-0.0.9/ok/capture/adb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.515134 ok-script-0.0.9/ok/capture/adb/bin/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/capture/adb/bin/__init__.py
+-rw-rw-rw-   0        0        0     2355 2024-03-14 10:16:17.000000 ok-script-0.0.9/ok/capture/adb/targets.py
+-rw-rw-rw-   0        0        0     5784 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/capture/adb/vbox.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.534035 ok-script-0.0.9/ok/capture/windows/
+-rw-rw-rw-   0        0        0     9158 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/capture/windows/WindowsGraphicsCaptureMethod.py
+-rw-rw-rw-   0        0        0        0 2024-02-03 03:10:06.000000 ok-script-0.0.9/ok/capture/windows/__init__.py
+-rw-rw-rw-   0        0        0     2673 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/capture/windows/d3d11.py
+-rw-rw-rw-   0        0        0     4639 2024-03-16 14:22:58.000000 ok-script-0.0.9/ok/capture/windows/utils.py
+-rw-rw-rw-   0        0        0     1320 2024-04-01 01:55:20.000000 ok-script-0.0.9/ok/capture/windows/window.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.537928 ok-script-0.0.9/ok/color/
+-rw-rw-rw-   0        0        0     1550 2024-03-18 15:46:15.000000 ok-script-0.0.9/ok/color/Color.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/color/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.543379 ok-script-0.0.9/ok/config/
+-rw-rw-rw-   0        0        0     2195 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/config/Config.py
+-rw-rw-rw-   0        0        0      386 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/config/InfoDict.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.561018 ok-script-0.0.9/ok/feature/
+-rw-rw-rw-   0        0        0     7746 2024-04-10 15:13:21.000000 ok-script-0.0.9/ok/feature/Box.py
+-rw-rw-rw-   0        0        0      739 2024-03-16 12:36:18.000000 ok-script-0.0.9/ok/feature/Feature.py
+-rw-rw-rw-   0        0        0     9052 2024-04-08 14:19:18.000000 ok-script-0.0.9/ok/feature/FeatureSet.py
+-rw-rw-rw-   0        0        0     2104 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/feature/FindFeature.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.594129 ok-script-0.0.9/ok/gui/
+-rw-rw-rw-   0        0        0     4553 2024-04-13 17:30:06.000000 ok-script-0.0.9/ok/gui/App.py
+-rw-rw-rw-   0        0        0      604 2024-04-03 09:22:41.000000 ok-script-0.0.9/ok/gui/Communicate.py
+-rw-rw-rw-   0        0        0     2711 2024-04-13 17:28:54.000000 ok-script-0.0.9/ok/gui/MainWindow.py
+-rw-rw-rw-   0        0        0     1849 2024-03-07 15:43:39.000000 ok-script-0.0.9/ok/gui/TabTitles.py
+-rw-rw-rw-   0        0        0      132 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.597049 ok-script-0.0.9/ok/gui/about/
+-rw-rw-rw-   0        0        0      442 2024-04-13 17:37:15.000000 ok-script-0.0.9/ok/gui/about/AboutTab.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/about/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.607053 ok-script-0.0.9/ok/gui/debug/
+-rw-rw-rw-   0        0        0     1213 2024-03-08 05:29:34.000000 ok-script-0.0.9/ok/gui/debug/AspectRatioWidget.py
+-rw-rw-rw-   0        0        0     1334 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/debug/DebugTab.py
+-rw-rw-rw-   0        0        0     5095 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/debug/FrameWidget.py
+-rw-rw-rw-   0        0        0     1211 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/debug/InfoWidget.py
+-rw-rw-rw-   0        0        0     2690 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/debug/LoggerWidget.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/debug/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.609030 ok-script-0.0.9/ok/gui/i18n/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/i18n/__init__.py
+-rw-rw-rw-   0        0        0       52 2024-04-01 11:14:15.000000 ok-script-0.0.9/ok/gui/i18n/path.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.617051 ok-script-0.0.9/ok/gui/icon/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/icon/__init__.py
+-rw-rw-rw-   0        0        0      174 2024-03-26 17:34:24.000000 ok-script-0.0.9/ok/gui/icon/icon.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.619027 ok-script-0.0.9/ok/gui/loading/
+-rw-rw-rw-   0        0        0     6200 2024-04-10 15:47:47.000000 ok-script-0.0.9/ok/gui/loading/LoadingWindow.py
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.9/ok/gui/loading/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.621987 ok-script-0.0.9/ok/gui/overlay/
+-rw-rw-rw-   0        0        0     1402 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/overlay/OverlayWindow.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/overlay/__init__.py
+-rw-rw-rw-   0        0        0    22185 2024-04-04 16:18:48.000000 ok-script-0.0.9/ok/gui/resources.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.630740 ok-script-0.0.9/ok/gui/tasks/
+-rw-rw-rw-   0        0        0      668 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/tasks/ConfigItemFactory.py
+-rw-rw-rw-   0        0        0     1567 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/tasks/StartButton.py
+-rw-rw-rw-   0        0        0      903 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/tasks/TaskOpButton.py
+-rw-rw-rw-   0        0        0     5969 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/tasks/TaskTab.py
+-rw-rw-rw-   0        0        0     1546 2024-04-03 14:53:01.000000 ok-script-0.0.9/ok/gui/tasks/TooltipTableWidget.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/tasks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.635609 ok-script-0.0.9/ok/gui/util/
+-rw-rw-rw-   0        0        0      400 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/util/Alert.py
+-rw-rw-rw-   0        0        0      356 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/util/InitWorker.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/util/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.663157 ok-script-0.0.9/ok/gui/widget/
+-rw-rw-rw-   0        0        0      943 2024-04-08 14:19:18.000000 ok-script-0.0.9/ok/gui/widget/ListTableWidgetItem.py
+-rw-rw-rw-   0        0        0     1316 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/widget/NumericTableWidgetItem.py
+-rw-rw-rw-   0        0        0     2126 2024-04-02 12:32:43.000000 ok-script-0.0.9/ok/gui/widget/RoundCornerContainer.py
+-rw-rw-rw-   0        0        0      830 2024-03-25 08:54:00.000000 ok-script-0.0.9/ok/gui/widget/TabWidget.py
+-rw-rw-rw-   0        0        0      399 2024-03-25 14:18:22.000000 ok-script-0.0.9/ok/gui/widget/UpdateConfigWidgetItem.py
+-rw-rw-rw-   0        0        0      685 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/gui/widget/YesNonWidgetItem.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/gui/widget/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.669149 ok-script-0.0.9/ok/interaction/
+-rw-rw-rw-   0        0        0     1153 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/interaction/ADBInteraction.py
+-rw-rw-rw-   0        0        0     1050 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/interaction/BaseInteraction.py
+-rw-rw-rw-   0        0        0     1693 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/interaction/Win32Interaction.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/interaction/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.672114 ok-script-0.0.9/ok/logging/
+-rw-rw-rw-   0        0        0     3618 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/logging/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/logging/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.675034 ok-script-0.0.9/ok/ocr/
+-rw-rw-rw-   0        0        0     2099 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/ocr/OCR.py
+-rw-rw-rw-   0        0        0        0 2024-03-17 08:31:48.000000 ok-script-0.0.9/ok/ocr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.686784 ok-script-0.0.9/ok/predict/
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/predict/__init__.py
+-rw-rw-rw-   0        0        0     1595 2023-12-15 17:49:57.000000 ok-script-0.0.9/ok/predict/predict.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.715356 ok-script-0.0.9/ok/rotypes/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.718276 ok-script-0.0.9/ok/rotypes/Windows/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.730092 ok-script-0.0.9/ok/rotypes/Windows/Foundation/
+-rw-rw-rw-   0        0        0     2023 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Foundation/Collections.py
+-rw-rw-rw-   0        0        0     5385 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Foundation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.740146 ok-script-0.0.9/ok/rotypes/Windows/Globalization/
+-rw-rw-rw-   0        0        0      909 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Globalization/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.742249 ok-script-0.0.9/ok/rotypes/Windows/Graphics/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.744195 ok-script-0.0.9/ok/rotypes/Windows/Graphics/Capture/
+-rw-rw-rw-   0        0        0     4675 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Graphics/Capture/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.746142 ok-script-0.0.9/ok/rotypes/Windows/Graphics/DirectX/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.747117 ok-script-0.0.9/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/
+-rw-rw-rw-   0        0        0     1234 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py
+-rw-rw-rw-   0        0        0     4181 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Graphics/DirectX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.760123 ok-script-0.0.9/ok/rotypes/Windows/Graphics/Imaging/
+-rw-rw-rw-   0        0        0     1053 2024-04-08 14:19:18.000000 ok-script-0.0.9/ok/rotypes/Windows/Graphics/Imaging/__init__.py
+-rw-rw-rw-   0        0        0      127 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/Windows/Graphics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.761410 ok-script-0.0.9/ok/rotypes/Windows/Media/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.773244 ok-script-0.0.9/ok/rotypes/Windows/Media/Ocr/
+-rw-rw-rw-   0        0        0     3039 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Media/Ocr/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/Windows/Media/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.774218 ok-script-0.0.9/ok/rotypes/Windows/Security/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.784008 ok-script-0.0.9/ok/rotypes/Windows/Security/Cryptography/
+-rw-rw-rw-   0        0        0      675 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Security/Cryptography/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/Windows/Security/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.785956 ok-script-0.0.9/ok/rotypes/Windows/Storage/
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.796262 ok-script-0.0.9/ok/rotypes/Windows/Storage/Streams/
+-rw-rw-rw-   0        0        0      837 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/rotypes/Windows/Storage/Streams/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/Windows/Storage/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/Windows/__init__.py
+-rw-rw-rw-   0        0        0      145 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/__init__.py
+-rw-rw-rw-   0        0        0     3532 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/delegate.py
+-rw-rw-rw-   0        0        0      575 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/export.py
+-rw-rw-rw-   0        0        0     9281 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/idldsl.py
+-rw-rw-rw-   0        0        0     2311 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/inspectable.py
+-rw-rw-rw-   0        0        0      840 2024-03-14 16:08:07.000000 ok-script-0.0.9/ok/rotypes/roapi.py
+-rw-rw-rw-   0        0        0     2560 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/types.py
+-rw-rw-rw-   0        0        0     1566 2024-01-26 14:10:34.000000 ok-script-0.0.9/ok/rotypes/winstring.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.847271 ok-script-0.0.9/ok/save/
+-rw-rw-rw-   0        0        0      796 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/save/BlackBarProcessor.py
+-rw-rw-rw-   0        0        0       97 2024-03-16 12:49:02.000000 ok-script-0.0.9/ok/save/PostProcessor.py
+-rw-rw-rw-   0        0        0      828 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/save/SaveByInterval.py
+-rw-rw-rw-   0        0        0     1019 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/save/SaveByKeyPress.py
+-rw-rw-rw-   0        0        0     1455 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/save/SaveMethodBase.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/save/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.859037 ok-script-0.0.9/ok/scene/
+-rw-rw-rw-   0        0        0      328 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/scene/FeatureScene.py
+-rw-rw-rw-   0        0        0      576 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/scene/Scene.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/scene/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.861449 ok-script-0.0.9/ok/stats/
+-rw-rw-rw-   0        0        0     1014 2024-02-26 12:12:14.000000 ok-script-0.0.9/ok/stats/StreamStats.py
+-rw-rw-rw-   0        0        0        0 2024-02-06 15:39:35.000000 ok-script-0.0.9/ok/stats/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.876204 ok-script-0.0.9/ok/task/
+-rw-rw-rw-   0        0        0     3181 2024-04-10 10:15:40.000000 ok-script-0.0.9/ok/task/BaseTask.py
+-rw-rw-rw-   0        0        0     4783 2024-04-10 03:01:03.000000 ok-script-0.0.9/ok/task/ExecutorOperation.py
+-rw-rw-rw-   0        0        0      148 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/task/FindFeatureTask.py
+-rw-rw-rw-   0        0        0     9211 2024-04-10 10:15:40.000000 ok-script-0.0.9/ok/task/TaskExecutor.py
+-rw-rw-rw-   0        0        0        0 2024-01-11 17:02:40.000000 ok-script-0.0.9/ok/task/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.918094 ok-script-0.0.9/ok/util/
+-rw-rw-rw-   0        0        0        0 2023-12-13 14:30:39.000000 ok-script-0.0.9/ok/util/__init__.py
+-rw-rw-rw-   0        0        0      699 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/util/json.py
+-rw-rw-rw-   0        0        0      109 2024-04-02 11:28:23.000000 ok-script-0.0.9/ok/util/list.py
+-rw-rw-rw-   0        0        0     1127 2024-04-04 17:00:56.000000 ok-script-0.0.9/ok/util/path.py
+-rw-rw-rw-   0        0        0      246 2024-03-26 05:25:09.000000 ok-script-0.0.9/ok/util/thread.py
+-rw-rw-rw-   0        0        0     2923 2024-03-14 10:21:07.000000 ok-script-0.0.9/ok/util/win32_process.py
+-rw-rw-rw-   0        0        0      727 2024-04-08 14:19:17.000000 ok-script-0.0.9/ok/util/yaml.py
+drwxrwxrwx   0        0        0        0 2024-04-14 03:16:19.947268 ok-script-0.0.9/ok_script.egg-info/
+-rw-rw-rw-   0        0        0     2199 2024-04-14 03:16:19.000000 ok-script-0.0.9/ok_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-04-14 03:16:19.000000 ok-script-0.0.9/ok_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 03:16:19.000000 ok-script-0.0.9/ok_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-04-14 03:16:19.000000 ok-script-0.0.9/ok_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2024-04-14 03:16:19.000000 ok-script-0.0.9/ok_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 03:16:19.950240 ok-script-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-04-14 03:15:53.000000 ok-script-0.0.9/setup.py
```

### Comparing `ok-script-0.0.8/PKG-INFO` & `ok-script-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ok-script
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automation with Computer Vision for Python
 Home-page: https://github.com/ok-oldking/ok-script
 Author: ok-oldking
 Author-email: firedcto@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Requires-Dist: adbutils==2.2.1
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: PyDirectInput~=1.0.4
 Requires-Dist: pywin32==306
 Requires-Dist: typing-extensions~=4.10.0
 Requires-Dist: PySide6~=6.6.2
 
-# autoui
+# ok-script
 
 This project aims to provide a universal framework for developing automation tool for PC/Android games, running in
 windows,
 emulator, or physical Android Phone. Currently still working in progress, there is a working
 
 ## Showcase
```

### Comparing `ok-script-0.0.8/README.md` & `ok-script-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# autoui
+# ok-script
 
 This project aims to provide a universal framework for developing automation tool for PC/Android games, running in
 windows,
 emulator, or physical Android Phone. Currently still working in progress, there is a working
 
 ## Showcase
```

### Comparing `ok-script-0.0.8/ok/OK.py` & `ok-script-0.0.9/ok/OK.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,26 +32,30 @@
         print(f"AutoHelper init, config: {config}")
         self.debug = config.get("debug", False)
         self.exit_event = threading.Event()
         self.config = config
         self.init_device_manager()
         if config.get("use_gui"):
             self.app = App(self.config.get('gui_icon'), self.debug, self.config.get('gui_title'),
-                           self.config['tasks'], self.exit_event)
+                           self.config['tasks'], self.config.get('about'), self.exit_event)
             ok.gui.app = self.app
+        else:
+            self.device_manager.set_preferred_device()
+            self.device_manager.start()
+            self.do_init()
+
+    def start(self):
+        if self.config.get("use_gui"):
             self.app.show_loading()
             self.worker = InitWorker(self.do_init)
             self.worker.start()
             self.app.exec()
         else:
-            self.device_manager.set_preferred_device()
-            self.device_manager.start()
-            self.do_init()
             self.task_executor.start()
-            if config.get("debug"):
+            if self.config.get("debug"):
                 self.app = QApplication(sys.argv)
                 self.overlay_window = OverlayWindow(ok.gui.device_manager.hwnd)
                 self.app.exec()
             else:
                 try:
                     # Starting the task in a separate thread (optional)
                     # This allows the main thread to remain responsive to keyboard interrupts
```

### Comparing `ok-script-0.0.8/ok/capture/BaseCaptureMethod.py` & `ok-script-0.0.9/ok/capture/BaseCaptureMethod.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/HwndWindow.py` & `ok-script-0.0.9/ok/capture/HwndWindow.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/adb/ADBCaptureMethod.py` & `ok-script-0.0.9/ok/capture/adb/ADBCaptureMethod.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/adb/DeviceManager.py` & `ok-script-0.0.9/ok/capture/adb/DeviceManager.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,36 +98,28 @@
             if self.hwnd:
                 nick = self.hwnd.title_text()
                 width = self.hwnd.width
                 height = self.hwnd.height
             self.device_dict[self.hwnd_title] = {"address": "", "imei": self.hwnd_title, "method": "windows",
                                                  "model": "", "nick": nick or self.hwnd_title,
                                                  "connected": self.hwnd is not None and self.hwnd.exists,
-                                                 "preferred": False,
                                                  "resolution": f"{width}x{height}"}
         communicate.adb_devices.emit()
         self.config.save_file()
         logger.debug(f'refresh {self.device_dict}')
 
     def set_preferred_device(self, imei=None):
         logger.debug(f"set_preferred_device {imei}")
-        preferred = None
         if imei is None:
-            for device in self.device_dict.values():
-                if device.get('preferred'):
-                    preferred = device
-                    imei = preferred['imei']
-        else:
-            preferred = self.device_dict.get(imei)
-        for key in self.device_dict.keys():
-            if imei == key:
-                self.device_dict[imei]["preferred"] = False
+            imei = self.config.get("preferred")
+        preferred = self.device_dict.get(imei)
         if preferred is None and len(self.device_dict) > 0:
             preferred = next(iter(self.device_dict.values()))
         if preferred is not None:
+            imei = preferred['imei']
             preferred['preferred'] = True
             if preferred['method'] == 'windows':
                 if not isinstance(self.capture_method, WindowsGraphicsCaptureMethod):
                     if self.capture_method is not None:
                         self.capture_method.close()
                     self.capture_method = WindowsGraphicsCaptureMethod(self.hwnd)
                     self.interaction = Win32Interaction(self.capture_method)
@@ -137,34 +129,33 @@
                     if adb_device.serial == preferred.get('address'):
                         self._device = adb_device
                 if not isinstance(self.capture_method, ADBCaptureMethod):
                     if self.capture_method is not None:
                         self.capture_method.close()
                     self.capture_method = ADBCaptureMethod(self)
                     self.interaction = ADBBaseInteraction(self, self.capture_method)
+        self.config["preferred"] = imei
         self.config.save_file()
         logger.debug(f'preferred device: {preferred}')
 
     def start(self):
         if isinstance(self.capture_method, ADBCaptureMethod):
             if self.debug:
                 if self.hwnd is not None:
-                    self.hwnd.update_title_re("autohelper_debug")
+                    self.hwnd.update_title_re("ok_debug")
                     self.hwnd.update_frame_size(self.capture_method.width, self.capture_method.height)
                 else:
-                    self.hwnd = HwndWindow("autohelper_debug", self.exit_event, self.capture_method.width,
+                    self.hwnd = HwndWindow("ok_debug", self.exit_event, self.capture_method.width,
                                            self.capture_method.height)
             else:
                 self.hwnd.stop()
                 self.hwnd = None
 
     @property
     def device(self):
-        if self._device is None:
-            self.set_preferred_device()
         return self._device
 
     @property
     def width(self):
         if self._size[0] == 0:
             self.screencap()
         return self._size[0]
```

### Comparing `ok-script-0.0.8/ok/capture/adb/targets.py` & `ok-script-0.0.9/ok/capture/adb/targets.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/adb/vbox.py` & `ok-script-0.0.9/ok/capture/adb/vbox.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/windows/WindowsGraphicsCaptureMethod.py` & `ok-script-0.0.9/ok/capture/windows/WindowsGraphicsCaptureMethod.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/windows/d3d11.py` & `ok-script-0.0.9/ok/capture/windows/d3d11.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/windows/utils.py` & `ok-script-0.0.9/ok/capture/windows/utils.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/capture/windows/window.py` & `ok-script-0.0.9/ok/capture/windows/window.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/color/Color.py` & `ok-script-0.0.9/ok/color/Color.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/config/Config.py` & `ok-script-0.0.9/ok/config/Config.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/feature/Box.py` & `ok-script-0.0.9/ok/feature/Box.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,22 @@
         return (self.x == other.x and
                 self.y == other.y and
                 self.width == other.width and
                 self.height == other.height and
                 self.confidence == other.confidence and
                 self.name == other.name)
 
+    def in_boundary(self, boxes):
+        in_boundary_boxes = []
+        for box in boxes:
+            if (self.x <= box.x and self.x + self.width >= box.x + box.width and
+                    self.y <= box.y and self.y + self.height >= box.y + box.height):
+                in_boundary_boxes.append(box)
+        return in_boundary_boxes
+
     def __repr__(self):
         return self.name
 
     def __str__(self) -> str:
         if self.name is not None:
             return f"Box(name='{self.name}', x={self.x}, y={self.y}, width={self.width}, height={self.height}, confidence={round(self.confidence * 100)})"
         return f"Box(x={self.x}, y={self.y}, width={self.width}, height={self.height}, confidence={round(self.confidence * 100)})"
@@ -76,33 +84,40 @@
     def copy(self, x_offset=0, y_offset=0, width_offset=0, height_offset=0, name=None):
         return Box(self.x + x_offset, self.y + y_offset, self.width + width_offset, self.height + height_offset,
                    self.confidence, name or self.name)
 
     def center(self):
         return self.x + self.width / 2, self.y + self.height / 2
 
-    def find_closest_box(self, direction: str, boxes: list):
+    def find_closest_box(self, direction: str, boxes: list, condition=None):
         orig_center_x, orig_center_y = self.center()
 
         def distance_criteria(box):
             # Calculate center points for comparison
             box_center_x, box_center_y = box.center()
 
             dx = box_center_x - orig_center_x
             dy = box_center_y - orig_center_y
             distance = math.sqrt(dx ** 2 + dy ** 2)
             if box == self:
-                return float('inf')
+                distance = float('inf')
             elif direction == 'up' and self.y - (box.y + box.height / 2) >= 0:
-                return distance
+                pass
             elif direction == 'down' and box.y - (self.y + self.height / 2) >= 0:
-                return distance
+                pass
             elif direction == 'left' and self.x - (box.x + box.width / 2) >= 0:
-                return distance
+                pass
             elif direction == 'right' and box.x - (self.x + self.width / 2) >= 0:
+                pass
+            else:
+                distance = float('inf')
+            return check_condition(box, distance)
+
+        def check_condition(box, distance):
+            if condition is None or condition(box):
                 return distance
             else:
                 return float('inf')
 
         filtered_boxes = sorted(boxes, key=distance_criteria)
         # Removed debug print statement for cleanliness
```

### Comparing `ok-script-0.0.8/ok/feature/Feature.py` & `ok-script-0.0.9/ok/feature/Feature.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/feature/FeatureSet.py` & `ok-script-0.0.9/ok/feature/FeatureSet.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/feature/FindFeature.py` & `ok-script-0.0.9/ok/feature/FindFeature.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/App.py` & `ok-script-0.0.9/ok/gui/App.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 from ok.gui.overlay.OverlayWindow import OverlayWindow
 from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class App:
-    def __init__(self, icon=None, overlay=False, title="AutoUI", tasks=None,
+    def __init__(self, icon=None, overlay=False, title="AutoUI", tasks=None, about=None,
                  exit_event=None):
         super().__init__()
         self.app = QApplication(sys.argv)
         self.app.setStyle(QStyleFactory.create("Fusion"))
         self.tasks = tasks
+        self.about = about
         self.title = title
         self.overlay = overlay
         self.loading_window = None
         self.overlay_window = None
         self.main_window = None
         self.exit_event = exit_event
         self.icon = QIcon(icon or ":/icon/icon.ico")
@@ -82,15 +83,15 @@
         if done:
             self.loading_window.loading_done()
         else:
             self.loading_window.update_progress(message)
 
     def show_main_window(self):
         self.loading_window.close()
-        self.main_window = MainWindow(self.tasks, self.overlay, exit_event=self.exit_event)
+        self.main_window = MainWindow(self.tasks, self.overlay, self.about, exit_event=self.exit_event)
         self.main_window.setWindowTitle(self.title)  # Set the window title here
         self.main_window.setWindowIcon(self.icon)
         if self.overlay and ok.gui.device_manager.hwnd is not None:
             self.overlay_window = OverlayWindow(ok.gui.device_manager.hwnd)
 
         size = self.size_relative_to_screen(width=0.5, height=0.6)
         self.main_window.resize(size)
```

### Comparing `ok-script-0.0.8/ok/gui/Communicate.py` & `ok-script-0.0.9/ok/gui/Communicate.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/MainWindow.py` & `ok-script-0.0.9/ok/gui/MainWindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from PySide6.QtCore import QObject, Signal, Slot
 from PySide6.QtWidgets import QMessageBox, QTabWidget
 
+from ok.gui.about.AboutTab import AboutTab
 from ok.gui.debug.DebugTab import DebugTab
 from ok.gui.tasks.TaskTab import TaskTab
 from ok.logging.Logger import get_logger
 
 logger = get_logger(__name__)
 
 
 class Communicate(QObject):
     speak = Signal(str)
 
 
 class MainWindow(QTabWidget):
-    def __init__(self, tasks, debug=False, exit_event=None):
+    def __init__(self, tasks, debug=False, about=None, exit_event=None):
         super().__init__()
         self.exit_event = exit_event
         task_tab = TaskTab(tasks)
         self.addTab(task_tab, self.tr("Task"))
         if debug:
             debug_tab = DebugTab()
             self.addTab(debug_tab, self.tr("Debug"))
         # ... Add other tabs similarly
+        if about:
+            about_tab = AboutTab(about)
+            self.addTab(about_tab, self.tr("About"))
 
         # Styling the tabs and content if needed, for example:
         self.setStyleSheet("""
                             QTabWidget::tab-bar {
                                 alignment: center;
                             }
                             QTabBar::tab {
```

### Comparing `ok-script-0.0.8/ok/gui/TabTitles.py` & `ok-script-0.0.9/ok/gui/TabTitles.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/debug/AspectRatioWidget.py` & `ok-script-0.0.9/ok/gui/debug/AspectRatioWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/debug/DebugTab.py` & `ok-script-0.0.9/ok/gui/debug/DebugTab.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/debug/FrameWidget.py` & `ok-script-0.0.9/ok/gui/debug/FrameWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/debug/InfoWidget.py` & `ok-script-0.0.9/ok/gui/debug/InfoWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/debug/LoggerWidget.py` & `ok-script-0.0.9/ok/gui/debug/LoggerWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/loading/LoadingWindow.py` & `ok-script-0.0.9/ok/gui/loading/LoadingWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     def update_capture(self):
         devices = ok.gui.device_manager.get_devices()
         selected = self.capture_list.currentRow()
         self.capture_list.clear()
         self.capture_list_data.clear()
         if len(devices) > 0:
             for row, device in enumerate(devices):
-                if device["preferred"]:
+                if device["imei"] == ok.gui.device_manager.config.get("preferred"):
                     selected = row
                 method = self.tr("PC") if device['method'] == "windows" else self.tr("Android")
                 connected = self.tr("Connected") if device['connected'] else self.tr("Disconnected")
                 self.capture_list.addItem(
                     f"{method} {connected}: {device['nick']} {device['address']} {device.get('resolution') or ''}")
                 item = self.capture_list.item(row)
                 if not device['connected']:
```

### Comparing `ok-script-0.0.8/ok/gui/overlay/OverlayWindow.py` & `ok-script-0.0.9/ok/gui/overlay/OverlayWindow.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/resources.py` & `ok-script-0.0.9/ok/gui/resources.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/tasks/ConfigItemFactory.py` & `ok-script-0.0.9/ok/gui/tasks/ConfigItemFactory.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/tasks/StartButton.py` & `ok-script-0.0.9/ok/gui/tasks/StartButton.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/tasks/TaskOpButton.py` & `ok-script-0.0.9/ok/gui/tasks/TaskOpButton.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/tasks/TaskTab.py` & `ok-script-0.0.9/ok/gui/tasks/TaskTab.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/tasks/TooltipTableWidget.py` & `ok-script-0.0.9/ok/gui/tasks/TooltipTableWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/widget/ListTableWidgetItem.py` & `ok-script-0.0.9/ok/gui/widget/ListTableWidgetItem.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/widget/NumericTableWidgetItem.py` & `ok-script-0.0.9/ok/gui/widget/NumericTableWidgetItem.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/widget/RoundCornerContainer.py` & `ok-script-0.0.9/ok/gui/widget/RoundCornerContainer.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/widget/TabWidget.py` & `ok-script-0.0.9/ok/gui/widget/TabWidget.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/gui/widget/YesNonWidgetItem.py` & `ok-script-0.0.9/ok/gui/widget/YesNonWidgetItem.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/interaction/ADBInteraction.py` & `ok-script-0.0.9/ok/interaction/ADBInteraction.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/interaction/BaseInteraction.py` & `ok-script-0.0.9/ok/interaction/BaseInteraction.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/interaction/Win32Interaction.py` & `ok-script-0.0.9/ok/interaction/Win32Interaction.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/logging/Logger.py` & `ok-script-0.0.9/ok/logging/Logger.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/ocr/OCR.py` & `ok-script-0.0.9/ok/ocr/OCR.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/predict/predict.py` & `ok-script-0.0.9/ok/predict/predict.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Foundation/Collections.py` & `ok-script-0.0.9/ok/rotypes/Windows/Foundation/Collections.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Foundation/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Foundation/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Globalization/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Globalization/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Graphics/Capture/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Graphics/Capture/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Graphics/DirectX/Direct3D11/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Graphics/DirectX/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Graphics/DirectX/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Graphics/Imaging/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Graphics/Imaging/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Media/Ocr/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Media/Ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Security/Cryptography/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Security/Cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/Windows/Storage/Streams/__init__.py` & `ok-script-0.0.9/ok/rotypes/Windows/Storage/Streams/__init__.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/delegate.py` & `ok-script-0.0.9/ok/rotypes/delegate.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/export.py` & `ok-script-0.0.9/ok/rotypes/export.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/idldsl.py` & `ok-script-0.0.9/ok/rotypes/idldsl.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/inspectable.py` & `ok-script-0.0.9/ok/rotypes/inspectable.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/roapi.py` & `ok-script-0.0.9/ok/rotypes/roapi.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/types.py` & `ok-script-0.0.9/ok/rotypes/types.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/rotypes/winstring.py` & `ok-script-0.0.9/ok/rotypes/winstring.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/save/BlackBarProcessor.py` & `ok-script-0.0.9/ok/save/BlackBarProcessor.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/save/SaveByInterval.py` & `ok-script-0.0.9/ok/save/SaveByInterval.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/save/SaveByKeyPress.py` & `ok-script-0.0.9/ok/save/SaveByKeyPress.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/save/SaveMethodBase.py` & `ok-script-0.0.9/ok/save/SaveMethodBase.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/scene/Scene.py` & `ok-script-0.0.9/ok/scene/Scene.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/stats/StreamStats.py` & `ok-script-0.0.9/ok/stats/StreamStats.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/task/BaseTask.py` & `ok-script-0.0.9/ok/task/BaseTask.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,33 @@
 
 class BaseTask(ExecutorOperation):
     _done = False
 
     def __init__(self):
         self.logger = get_logger(self.__class__.__name__)
         self.name = self.__class__.__name__
-        self.success_count = 0
-        self.error_count = 0
         self.enabled = True
         self.running = False
         self.config = None
         self.info = InfoDict()
         self.default_config = {}
         self.last_execute_time = 0
 
     def log_info(self, message, notify=False):
         self.logger.info(message)
         self.info_set("Log", message)
         if notify:
             self.notification(message)
         communicate.task_info.emit()
 
+    def log_debug(self, message, notify=False):
+        self.logger.debug(message)
+        if notify:
+            self.notification(message)
+
     def log_error(self, message, exception=None, notify=False):
         self.logger.error(message, exception)
         if exception is not None:
             message += exception.args[0]
         self.info_set("Error", message)
         if notify:
             self.notification(message)
```

### Comparing `ok-script-0.0.8/ok/task/ExecutorOperation.py` & `ok-script-0.0.9/ok/task/ExecutorOperation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from ok.feature.Box import Box, find_box_by_name
 from ok.gui.Communicate import communicate
-from ok.logging.Logger import get_logger
-
-logger = get_logger(__name__)
 
 
 class ExecutorOperation:
     executor = None
 
     def box_in_horizontal_center(self, box, off_percent=0.02):
         center = self.executor.method.width / 2
         left = center - box.x
         right = box.x + box.width - center
         if left > 0 and right > 0 and abs(left - right) / box.width < off_percent:
             return True
         else:
             return False
 
+    def pause(self):
+        self.executor.pause()
+
     def is_scene(self, the_scene):
         return isinstance(self.executor.current_scene, the_scene)
 
     def click(self, x, y):
         self.executor.reset_scene()
         self.executor.interaction.click(x, y)
 
@@ -42,15 +42,15 @@
         - box: the matched box
 
         The method attempts to find and click on the highest-priority matching box. If no matches are found,
         or if there are no boxes, the method returns False. This operation is case-sensitive.
         """
         to_click = find_box_by_name(boxes, names)
         if to_click is not None:
-            logger.info(f"click_box_if_name_match found {to_click}")
+            self.logger.info(f"click_box_if_name_match found {to_click}")
             self.click_box(to_click, relative_x, relative_y)
             return to_click
 
     def box_of_screen(self, x, y, width, height, name=None):
         if name is None:
             name = f"{x} {y} {width} {height}"
         return Box(int(x * self.executor.method.width), int(y * self.executor.method.height),
@@ -75,17 +75,17 @@
 
     def click_box(self, box, relative_x=0.5, relative_y=0.5, raise_if_not_found=True):
         self.executor.reset_scene()
         if isinstance(box, list):
             if len(box) > 0:
                 box = box[0]
             else:
-                logger.error(f"No box")
+                self.logger.error(f"No box")
         if box is None:
-            logger.error(f"click_box box is None")
+            self.logger.error(f"click_box box is None")
             if raise_if_not_found:
                 raise Exception(f"click_box box is None")
             return
         self.executor.interaction.click_box(box, relative_x, relative_y)
 
     def wait_scene(self, scene_type=None, time_out=0, pre_action=None, post_action=None):
         return self.executor.wait_scene(scene_type, time_out, pre_action, post_action)
```

### Comparing `ok-script-0.0.8/ok/task/TaskExecutor.py` & `ok-script-0.0.9/ok/task/TaskExecutor.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,20 +166,15 @@
                 for index, task in enumerate(self.tasks):
                     if task.done or not task.enabled:
                         continue
                     self.current_task = task
                     task.running = True
                     task.last_execute_time = start
                     try:
-                        result = task.run_frame()
-                        if result is not None:
-                            if result:
-                                task.success_count += 1
-                            else:
-                                task.error_count += 1
+                        task.run_frame()
                     except TaskDisabledException:
                         logger.info(f"{task.name} is disabled, breaking")
                     except Exception as e:
                         traceback.print_exc()
                         stack_trace_str = traceback.format_exc()
                         logger.error(f"{task.name} exception: {e}, traceback: {stack_trace_str}")
                         task.error_count += 1
```

### Comparing `ok-script-0.0.8/ok/util/json.py` & `ok-script-0.0.9/ok/util/json.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/util/path.py` & `ok-script-0.0.9/ok/util/path.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/util/win32_process.py` & `ok-script-0.0.9/ok/util/win32_process.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok/util/yaml.py` & `ok-script-0.0.9/ok/util/yaml.py`

 * *Files identical despite different names*

### Comparing `ok-script-0.0.8/ok_script.egg-info/PKG-INFO` & `ok-script-0.0.9/ok_script.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ok-script
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automation with Computer Vision for Python
 Home-page: https://github.com/ok-oldking/ok-script
 Author: ok-oldking
 Author-email: firedcto@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Requires-Dist: adbutils==2.2.1
 Requires-Dist: numpy~=1.26.4
 Requires-Dist: PyDirectInput~=1.0.4
 Requires-Dist: pywin32==306
 Requires-Dist: typing-extensions~=4.10.0
 Requires-Dist: PySide6~=6.6.2
 
-# autoui
+# ok-script
 
 This project aims to provide a universal framework for developing automation tool for PC/Android games, running in
 windows,
 emulator, or physical Android Phone. Currently still working in progress, there is a working
 
 ## Showcase
```

### Comparing `ok-script-0.0.8/ok_script.egg-info/SOURCES.txt` & `ok-script-0.0.9/ok_script.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 ok/feature/__init__.py
 ok/gui/App.py
 ok/gui/Communicate.py
 ok/gui/MainWindow.py
 ok/gui/TabTitles.py
 ok/gui/__init__.py
 ok/gui/resources.py
+ok/gui/about/AboutTab.py
+ok/gui/about/__init__.py
 ok/gui/debug/AspectRatioWidget.py
 ok/gui/debug/DebugTab.py
 ok/gui/debug/FrameWidget.py
 ok/gui/debug/InfoWidget.py
 ok/gui/debug/LoggerWidget.py
 ok/gui/debug/__init__.py
 ok/gui/i18n/__init__.py
```

### Comparing `ok-script-0.0.8/setup.py` & `ok-script-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ok-script",
-    version="0.0.8",
+    version="0.0.9",
     author="ok-oldking",
     author_email="firedcto@gmail.com",
     description="Automation with Computer Vision for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ok-oldking/ok-script",
     packages=setuptools.find_packages(),
```

