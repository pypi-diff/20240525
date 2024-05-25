# Comparing `tmp/idlea-1.2.8.tar.gz` & `tmp/idlea-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\idlea-1.2.8.tar", last modified: Sun Dec 11 01:19:43 2022, max compression
+gzip compressed data, was "dist\idlea-1.2.9.tar", last modified: Sat May 25 08:45:18 2024, max compression
```

## Comparing `idlea-1.2.8.tar` & `idlea-1.2.9.tar`

### file list

```diff
@@ -1,85 +1,73 @@
-drwxrwxrwx   0        0        0        0 2022-12-11 01:19:43.000000 idlea-1.2.8/
--rw-rw-rw-   0        0        0      142 2022-02-28 12:46:56.000000 idlea-1.2.8/.gitignore
--rw-rw-rw-   0        0        0   238895 2022-11-30 01:19:27.000000 idlea-1.2.8/IDLE-Advance.git
-drwxrwxrwx   0        0        0        0 2022-12-11 01:19:42.000000 idlea-1.2.8/idlea.egg-info/
--rw-rw-rw-   0        0        0        1 2022-12-11 01:19:40.000000 idlea-1.2.8/idlea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-12-11 01:19:40.000000 idlea-1.2.8/idlea.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0    13045 2022-12-11 01:19:40.000000 idlea-1.2.8/idlea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1733 2022-12-11 01:19:40.000000 idlea-1.2.8/idlea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2022-12-11 01:19:40.000000 idlea-1.2.8/idlea.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-11 01:19:43.000000 idlea-1.2.8/idlealib/
--rw-rw-rw-   0        0        0      991 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/About.py
--rw-rw-rw-   0        0        0      904 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/AutoComment.py
--rw-rw-rw-   0        0        0     1306 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/AutoReload.py
--rw-rw-rw-   0        0        0     2522 2022-05-13 11:42:48.000000 idlea-1.2.8/idlealib/AutoSave.py
--rw-rw-rw-   0        0        0     3896 2022-05-13 11:35:35.000000 idlea-1.2.8/idlealib/CalltipSelect.py
--rw-rw-rw-   0        0        0     1166 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/ClearShell.py
--rw-rw-rw-   0        0        0     1409 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/CompareFile.py
--rw-rw-rw-   0        0        0      530 2021-08-11 09:23:06.000000 idlea-1.2.8/idlealib/CopyNoSelect.py
--rw-rw-rw-   0        0        0     1432 2022-10-31 03:06:11.000000 idlea-1.2.8/idlealib/CursorHistory.py
--rw-rw-rw-   0        0        0      956 2021-07-12 09:50:02.000000 idlea-1.2.8/idlealib/DragOpen.py
--rw-rw-rw-   0        0        0      955 2022-10-21 06:25:35.000000 idlea-1.2.8/idlealib/DuplicateLines.py
--rw-rw-rw-   0        0        0     2782 2022-11-28 01:23:53.000000 idlea-1.2.8/idlealib/FileManager.py
--rw-rw-rw-   0        0        0     1439 2022-05-13 11:42:48.000000 idlea-1.2.8/idlealib/HelpViewer.py
-drwxrwxrwx   0        0        0        0 2022-12-11 01:19:43.000000 idlea-1.2.8/idlealib/nouse/
--rw-rw-rw-   0        0        0       80 2021-09-08 12:07:00.000000 idlea-1.2.8/idlealib/nouse/readme.md
--rw-rw-rw-   0        0        0     1386 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/nouse/RecentClosed.py
--rw-rw-rw-   0        0        0      753 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/nouse/SaveArchive.py
--rw-rw-rw-   0        0        0      938 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/PrintCr.py
--rw-rw-rw-   0        0        0     1105 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/QuickOpen.py
--rw-rw-rw-   0        0        0      808 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/QuickSearch.py
--rw-rw-rw-   0        0        0     1985 2022-05-13 11:35:35.000000 idlea-1.2.8/idlealib/readme.md
--rw-rw-rw-   0        0        0     1898 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/RecentClipboard.py
--rw-rw-rw-   0        0        0     2340 2022-05-13 11:42:48.000000 idlea-1.2.8/idlealib/RecentSaved.py
--rw-rw-rw-   0        0        0     6838 2022-11-30 01:20:28.000000 idlea-1.2.8/idlealib/ReplaceBar.py
--rw-rw-rw-   0        0        0     1032 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/RunArgs.py
--rw-rw-rw-   0        0        0     1566 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/RunMultiLine.py
--rw-rw-rw-   0        0        0     2614 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/RunSelected.py
--rw-rw-rw-   0        0        0     1248 2022-05-13 11:42:48.000000 idlea-1.2.8/idlealib/SaveUntitled.py
-drwxrwxrwx   0        0        0        0 2022-12-11 01:19:43.000000 idlea-1.2.8/idlealib/scripts/
--rw-rw-rw-   0        0        0     5677 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/scripts/context_helper.pyw
--rw-rw-rw-   0        0        0     1489 2021-08-19 07:50:30.000000 idlea-1.2.8/idlealib/scripts/Desktop.lnk
--rw-rw-rw-   0        0        0       81 2021-08-17 06:22:54.000000 idlea-1.2.8/idlealib/scripts/help.py
--rw-rw-rw-   0        0        0      330 2021-08-10 16:05:02.000000 idlea-1.2.8/idlealib/scripts/new_file.reg
--rw-rw-rw-   0        0        0     2337 2021-08-19 07:49:46.000000 idlea-1.2.8/idlealib/scripts/Programs.lnk
--rw-rw-rw-   0        0        0       30 2021-09-08 12:07:08.000000 idlea-1.2.8/idlealib/scripts/readme.md
--rw-rw-rw-   0        0        0      556 2022-05-13 11:35:35.000000 idlea-1.2.8/idlealib/scripts/right_click.reg
--rwxrwxrwx   0        0        0       20 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/scripts/run.bat
--rw-rw-rw-   0        0        0      451 2021-08-18 09:07:30.000000 idlea-1.2.8/idlealib/scripts/run.py
--rw-rw-rw-   0        0        0      451 2022-05-13 11:35:35.000000 idlea-1.2.8/idlealib/scripts/run.pyw
--rw-rw-rw-   0        0        0       51 2021-08-23 10:50:12.000000 idlea-1.2.8/idlealib/scripts/run.vbs
--rw-rw-rw-   0        0        0      333 2021-09-08 13:07:20.000000 idlea-1.2.8/idlealib/scripts/spec.py
--rw-rw-rw-   0        0        0     1777 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/scripts/test.py
--rw-rw-rw-   0        0        0      713 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/ScrollHorizontal.py
--rw-rw-rw-   0        0        0     3184 2022-10-31 02:54:48.000000 idlea-1.2.8/idlealib/SelectVertical.py
--rw-rw-rw-   0        0        0     1743 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/ShareQRCode.py
--rw-rw-rw-   0        0        0     1052 2022-11-28 01:23:53.000000 idlea-1.2.8/idlealib/ShiftLines.py
--rw-rw-rw-   0        0        0      364 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/ShiftTab.py
--rw-rw-rw-   0        0        0     1841 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/SmartCopy.py
--rw-rw-rw-   0        0        0     2306 2022-10-21 10:04:12.000000 idlea-1.2.8/idlealib/SmartPairing.py
--rw-rw-rw-   0        0        0     6120 2022-11-28 01:23:53.000000 idlea-1.2.8/idlealib/SmartSelect.py
--rw-rw-rw-   0        0        0     1431 2021-08-09 01:10:46.000000 idlea-1.2.8/idlealib/SwapCopy.py
--rw-rw-rw-   0        0        0      531 2022-10-21 10:05:32.000000 idlea-1.2.8/idlealib/TimeTag.py
--rw-rw-rw-   0        0        0      965 2022-11-28 01:23:53.000000 idlea-1.2.8/idlealib/TrimTrailing.py
--rw-rw-rw-   0        0        0      943 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/UpperCase.py
--rw-rw-rw-   0        0        0     2431 2022-10-20 07:33:17.000000 idlea-1.2.8/idlealib/WindowManager.py
--rw-rw-rw-   0        0        0      642 2022-02-28 12:46:56.000000 idlea-1.2.8/idlealib/WrapShell.py
--rw-rw-rw-   0        0        0     9730 2022-10-31 03:06:02.000000 idlea-1.2.8/idlealib/__init__.py
--rw-rw-rw-   0        0        0      352 2022-05-13 11:35:35.000000 idlea-1.2.8/idlealib/__main__.py
--rwxrwxrwx   0        0        0       32 2021-09-07 01:06:20.000000 idlea-1.2.8/install.bat
--rw-rw-rw-   0        0        0     1119 2021-09-12 08:54:18.000000 idlea-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0       51 2022-05-13 11:35:35.000000 idlea-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0    13045 2022-12-11 01:19:43.000000 idlea-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    10180 2022-11-30 01:20:28.000000 idlea-1.2.8/README.md
--rwxrwxrwx   0        0        0       20 2022-02-28 12:46:56.000000 idlea-1.2.8/run.bat
--rw-rw-rw-   0        0        0       33 2021-09-08 00:55:12.000000 idlea-1.2.8/run.py
--rw-rw-rw-   0        0        0       33 2022-05-13 11:35:35.000000 idlea-1.2.8/run.pyw
--rw-rw-rw-   0        0        0       51 2021-08-23 10:50:12.000000 idlea-1.2.8/run.vbs
--rw-rw-rw-   0        0        0       42 2022-12-11 01:19:43.000000 idlea-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1664 2022-05-13 11:35:35.000000 idlea-1.2.8/setup.py
--rw-rw-rw-   0        0        0      566 2022-05-13 11:35:35.000000 idlea-1.2.8/TODO.md
--rw-rw-rw-   0        0        0        5 2022-11-30 01:20:28.000000 idlea-1.2.8/VERSION.txt
--rwxrwxrwx   0        0        0       53 2022-02-28 12:46:56.000000 idlea-1.2.8/__pip_install.bat
--rwxrwxrwx   0        0        0       31 2022-02-28 12:46:56.000000 idlea-1.2.8/__pip_uninstall.bat
--rwxrwxrwx   0        0        0      160 2022-02-28 12:46:56.000000 idlea-1.2.8/___local_test.bat
--rwxrwxrwx   0        0        0      165 2022-02-28 12:46:56.000000 idlea-1.2.8/___pypi_upload.bat
+drwxrwxrwx   0        0        0        0 2024-05-25 08:45:18.000000 idlea-1.2.9/
+-rw-rw-rw-   0        0        0      142 2022-02-28 11:18:27.000000 idlea-1.2.9/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-25 08:45:18.000000 idlea-1.2.9/idlea.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-25 08:45:18.000000 idlea-1.2.9/idlea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-05-25 08:45:18.000000 idlea-1.2.9/idlea.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0    10969 2024-05-25 08:45:18.000000 idlea-1.2.9/idlea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2024-05-25 08:45:18.000000 idlea-1.2.9/idlea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 08:45:18.000000 idlea-1.2.9/idlea.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 08:45:18.000000 idlea-1.2.9/idlealib/
+-rw-rw-rw-   0        0        0      991 2022-07-24 01:04:40.000000 idlea-1.2.9/idlealib/About.py
+-rw-rw-rw-   0        0        0     1119 2024-05-25 07:26:05.000000 idlea-1.2.9/idlealib/AutoComment.py
+-rw-rw-rw-   0        0        0     1306 2024-05-25 00:28:15.000000 idlea-1.2.9/idlealib/AutoReload.py
+-rw-rw-rw-   0        0        0     2654 2024-05-25 07:26:05.000000 idlea-1.2.9/idlealib/AutoSave.py
+-rw-rw-rw-   0        0        0     3896 2022-07-24 01:04:37.000000 idlea-1.2.9/idlealib/CalltipSelect.py
+-rw-rw-rw-   0        0        0     1166 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/ClearShell.py
+-rw-rw-rw-   0        0        0     1409 2022-07-24 01:04:42.000000 idlea-1.2.9/idlealib/CompareFile.py
+-rw-rw-rw-   0        0        0     3339 2024-05-25 08:36:19.000000 idlea-1.2.9/idlealib/ContextManager.py
+-rw-rw-rw-   0        0        0      530 2022-06-19 04:30:02.000000 idlea-1.2.9/idlealib/CopyNoSelect.py
+-rw-rw-rw-   0        0        0     1432 2022-11-06 04:01:29.000000 idlea-1.2.9/idlealib/CursorHistory.py
+-rw-rw-rw-   0        0        0      957 2024-05-25 08:35:32.000000 idlea-1.2.9/idlealib/DragOpen.py
+-rw-rw-rw-   0        0        0      955 2022-11-06 04:01:29.000000 idlea-1.2.9/idlealib/DuplicateLines.py
+-rw-rw-rw-   0        0        0     2782 2024-05-24 13:31:47.000000 idlea-1.2.9/idlealib/FileManager.py
+-rw-rw-rw-   0        0        0     1439 2022-07-24 01:04:39.000000 idlea-1.2.9/idlealib/HelpViewer.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:45:18.000000 idlea-1.2.9/idlealib/nouse/
+-rw-rw-rw-   0        0        0       80 2022-02-26 22:34:41.000000 idlea-1.2.9/idlealib/nouse/readme.md
+-rw-rw-rw-   0        0        0     1386 2022-07-24 01:04:40.000000 idlea-1.2.9/idlealib/nouse/RecentClosed.py
+-rw-rw-rw-   0        0        0      753 2022-07-24 01:04:39.000000 idlea-1.2.9/idlealib/nouse/SaveArchive.py
+-rw-rw-rw-   0        0        0      938 2022-07-24 01:04:40.000000 idlea-1.2.9/idlealib/PrintCr.py
+-rw-rw-rw-   0        0        0     1065 2024-05-25 08:36:17.000000 idlea-1.2.9/idlealib/QuickOpen.py
+-rw-rw-rw-   0        0        0      808 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/QuickSearch.py
+-rw-rw-rw-   0        0        0     1985 2022-07-24 01:04:38.000000 idlea-1.2.9/idlealib/readme.md
+-rw-rw-rw-   0        0        0     1898 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/RecentClipboard.py
+-rw-rw-rw-   0        0        0     2340 2022-07-24 01:04:39.000000 idlea-1.2.9/idlealib/RecentSaved.py
+-rw-rw-rw-   0        0        0     6838 2024-05-24 13:31:47.000000 idlea-1.2.9/idlealib/ReplaceBar.py
+-rw-rw-rw-   0        0        0     1171 2024-05-25 07:17:43.000000 idlea-1.2.9/idlealib/RunArgs.py
+-rw-rw-rw-   0        0        0     1566 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/RunMultiLine.py
+-rw-rw-rw-   0        0        0     2614 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/RunSelected.py
+-rw-rw-rw-   0        0        0     1248 2022-07-24 01:04:39.000000 idlea-1.2.9/idlealib/SaveUntitled.py
+drwxrwxrwx   0        0        0        0 2024-05-25 08:45:18.000000 idlea-1.2.9/idlealib/scripts/
+-rw-rw-rw-   0        0        0       81 2021-08-17 06:22:54.000000 idlea-1.2.9/idlealib/scripts/help.py
+-rw-rw-rw-   0        0        0      451 2021-08-18 09:07:30.000000 idlea-1.2.9/idlealib/scripts/run.py
+-rw-rw-rw-   0        0        0      333 2022-02-26 22:34:41.000000 idlea-1.2.9/idlealib/scripts/spec.py
+-rw-rw-rw-   0        0        0     1777 2024-05-24 13:40:19.000000 idlea-1.2.9/idlealib/scripts/test.py
+-rw-rw-rw-   0        0        0      713 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/ScrollHorizontal.py
+-rw-rw-rw-   0        0        0     3184 2022-11-06 04:01:29.000000 idlea-1.2.9/idlealib/SelectVertical.py
+-rw-rw-rw-   0        0        0     1885 2024-05-25 08:35:33.000000 idlea-1.2.9/idlealib/ShareQRCode.py
+-rw-rw-rw-   0        0        0     1052 2024-05-24 13:31:47.000000 idlea-1.2.9/idlealib/ShiftLines.py
+-rw-rw-rw-   0        0        0      364 2022-07-24 01:04:41.000000 idlea-1.2.9/idlealib/ShiftTab.py
+-rw-rw-rw-   0        0        0     1841 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/SmartCopy.py
+-rw-rw-rw-   0        0        0     2306 2022-11-06 04:01:29.000000 idlea-1.2.9/idlealib/SmartPairing.py
+-rw-rw-rw-   0        0        0     6120 2024-05-24 13:31:47.000000 idlea-1.2.9/idlealib/SmartSelect.py
+-rw-rw-rw-   0        0        0     1431 2021-08-09 01:10:46.000000 idlea-1.2.9/idlealib/SwapCopy.py
+-rw-rw-rw-   0        0        0      665 2024-05-25 08:36:19.000000 idlea-1.2.9/idlealib/TimeStamp.py
+-rw-rw-rw-   0        0        0      965 2024-05-24 13:31:47.000000 idlea-1.2.9/idlealib/TrimTrailing.py
+-rw-rw-rw-   0        0        0      943 2022-07-24 01:04:40.000000 idlea-1.2.9/idlealib/UpperCase.py
+-rw-rw-rw-   0        0        0     2431 2022-07-24 01:04:40.000000 idlea-1.2.9/idlealib/WindowManager.py
+-rw-rw-rw-   0        0        0      642 2022-02-28 11:18:27.000000 idlea-1.2.9/idlealib/WrapShell.py
+-rw-rw-rw-   0        0        0     9713 2024-05-25 08:42:01.000000 idlea-1.2.9/idlealib/__init__.py
+-rw-rw-rw-   0        0        0      352 2022-07-24 01:04:38.000000 idlea-1.2.9/idlealib/__main__.py
+-rwxrwxrwx   0        0        0      255 2024-05-25 08:36:19.000000 idlea-1.2.9/initialize_on_windows.bat
+-rw-rw-rw-   0        0        0     1125 2024-05-25 08:36:20.000000 idlea-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0       51 2022-07-24 01:04:38.000000 idlea-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    10969 2024-05-25 08:45:18.000000 idlea-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10188 2024-05-25 08:36:20.000000 idlea-1.2.9/README.md
+-rw-rw-rw-   0        0        0       33 2021-09-08 00:55:12.000000 idlea-1.2.9/run.py
+-rw-rw-rw-   0        0        0       33 2022-07-24 01:04:37.000000 idlea-1.2.9/run.pyw
+-rw-rw-rw-   0        0        0       42 2024-05-25 08:45:18.000000 idlea-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1881 2024-05-25 08:36:20.000000 idlea-1.2.9/setup.py
+-rw-rw-rw-   0        0        0      566 2024-05-25 01:52:51.000000 idlea-1.2.9/TODO.md
+-rw-rw-rw-   0        0        0        5 2024-05-25 08:36:20.000000 idlea-1.2.9/VERSION.txt
+-rwxrwxrwx   0        0        0      387 2024-05-25 08:36:19.000000 idlea-1.2.9/__local_test.bat
+-rwxrwxrwx   0        0        0      161 2024-05-25 07:26:05.000000 idlea-1.2.9/__pypi_upload.bat
+-rwxrwxrwx   0        0        0      594 2024-05-25 08:36:19.000000 idlea-1.2.9/__test_install_all.bat
```

### Comparing `idlea-1.2.8/idlealib/About.py` & `idlea-1.2.9/idlealib/About.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/AutoReload.py` & `idlea-1.2.9/idlealib/AutoReload.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/AutoSave.py` & `idlea-1.2.9/idlealib/AutoSave.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,43 +3,48 @@
 
 if __name__ == '__main__':
     import __init__
     __init__.test_editor(__file__)
 
 
 import os
+import sys
 
 TICK = 7000
 
 
 class AutoSave:
     def __init__(self, parent):
         if hasattr(parent, 'write'): # is shell?
             return
 
         self.text = parent.text
         self.root = parent.root
         self.io = parent.io
         self.get_saved = parent.get_saved # function
 
-        self.fixfixlastline()
+        self.HotFix()
 
         self.root.after(TICK, self.Backup)
 
         self.AfterOpen()
         parent.after_save.append(self.AfterSave)
         parent.before_close.append(self.BeforeClose)
 
-    def fixfixlastline(self): # append '\n' at last line **after** cursor
-        def fixlastline2():
+    def HotFix(self): # append '\n' at last line **after** cursor
+        def new_api():
             self.text.mark_gravity('insert', 'left')
-            fixlastline()
+            ret = old_api()
             self.text.mark_gravity('insert', 'right')
-        fixlastline = self.io.fixlastline
-        self.io.fixlastline = fixlastline2
+            return ret
+
+        if sys.version_info < (3, 7):
+            old_api, self.io.fixlastline = self.io.fixlastline, new_api
+        else:
+            old_api, self.io.fixnewlines = self.io.fixnewlines, new_api
 
     def Backup(self, loop=True):
         filename = self.io.filename
         if not self.io.text: # will set as None in io.close()
             return # break loop only editor closed
         if filename:
             filename_bak = os.path.splitext(filename)[0] + '.pybak'
```

### Comparing `idlea-1.2.8/idlealib/CalltipSelect.py` & `idlea-1.2.9/idlealib/CalltipSelect.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/ClearShell.py` & `idlea-1.2.9/idlealib/ClearShell.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/CompareFile.py` & `idlea-1.2.9/idlealib/CompareFile.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/CopyNoSelect.py` & `idlea-1.2.9/idlealib/CopyNoSelect.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/CursorHistory.py` & `idlea-1.2.9/idlealib/CursorHistory.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/DragOpen.py` & `idlea-1.2.9/idlealib/DragOpen.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 class DragOpen:
     def __init__(self, parent):
         self.flist = parent.flist
         try:
             import windnd
             windnd.hook_dropfiles(parent.text, func=self.DragOpen)
-        except Exception as e:
-            print('import windnd error:', e)
+        except ImportError as e:
+            print('%s: %s' % (__name__, e))
 
     def DragOpen(self, files): # TODO 恢复记忆位置
         for file_b in files:
             file = file_b.decode('gbk')
             if file.endswith('.py'): # TODO 非py文件是否打开
                 edit = self.flist.open(file)
                 # TODO 由于滚动条存在导致有时候拖拽加载会闪退，增加下面两行可以避免
```

### Comparing `idlea-1.2.8/idlealib/DuplicateLines.py` & `idlea-1.2.9/idlealib/DuplicateLines.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/FileManager.py` & `idlea-1.2.9/idlealib/FileManager.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/HelpViewer.py` & `idlea-1.2.9/idlealib/HelpViewer.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/nouse/RecentClosed.py` & `idlea-1.2.9/idlealib/nouse/RecentClosed.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/nouse/SaveArchive.py` & `idlea-1.2.9/idlealib/nouse/SaveArchive.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/PrintCr.py` & `idlea-1.2.9/idlealib/PrintCr.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/QuickOpen.py` & `idlea-1.2.9/idlealib/QuickOpen.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,30 +15,28 @@
         parent.rmenu.add_separator()
         # parent.rmenu.add_command(label='Open', command=self.Open)
         parent.rmenu.add_command(label='Start', command=self.Start)
 
         # parent.add_adv_menu('Quick Open', self.Open)
         parent.add_adv_menu('Quick Start', self.Start)
 
-        print(os.getcwd())
-
     # def Open(self):
     #     if not self.text.tag_ranges('sel'):
     #         return
     #     s = self.text.get('sel.first', 'sel.last')
     #     os.popen('explorer ' + s)
 
     def Start(self):
         if not self.text.tag_ranges('sel'):
             return
         s = self.text.get('sel.first', 'sel.last')
         os.popen('start ' + s)
 
 
-'F:\lsx\coding\idle\idlealib\scripts'
-'scripts\readme.md'
-"F:\lsx\代码说明.docx"
-"notepad 1.txt"
-"C:\\"
-"cmd /k ipconfig"
-
-# todo 相对文件夹打不开
+TEST = r"""
+    C:\Windows\System32\calc.exe
+    C:\Windows\System32\
+    .\docs\LICENSE.txt
+    .\docs\
+    notepad new.txt
+    cmd /k ipconfig
+"""
```

### Comparing `idlea-1.2.8/idlealib/QuickSearch.py` & `idlea-1.2.9/idlealib/QuickSearch.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/readme.md` & `idlea-1.2.9/idlealib/readme.md`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/RecentClipboard.py` & `idlea-1.2.9/idlealib/RecentClipboard.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/RecentSaved.py` & `idlea-1.2.9/idlealib/RecentSaved.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/ReplaceBar.py` & `idlea-1.2.9/idlealib/ReplaceBar.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/RunArgs.py` & `idlea-1.2.9/idlealib/RunArgs.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,24 +14,30 @@
         if hasattr(parent, 'write'): # is shell?
             return
 
         self.text = parent.text
         self.root = parent.root
         self.flist = parent.flist
 
+        self.args = None
+
         parent.add_adv_menu('Run with args', self.Run, sp=True)
 
+    def AppendArgs(self, interp):
+        if self.args is not None:
+            code = "__import__('sys').argv.extend(%r.split())" % self.args
+            interp.runcommand(code)
+            self.args = None
+
     def Run(self):
         args = askstring('Run with args', 'args:', parent=self.root)
         if args is not None:
-            cmd = "__import__('sys').argv.extend(%r.split())" % args
+            self.args = args
             shell = self.flist.open_shell()
-            interp = shell.interp
-            interp.runcommand(cmd)
-            interp._runcode = interp.runcode
-            interp.runcode = lambda evt: [interp.runcommand(cmd), interp._runcode(evt)]
+            _runcode = shell.interp.runcode
+            shell.interp.runcode = lambda code: [self.AppendArgs(shell.interp), _runcode(code)]
             self.text.event_generate('<<run-module>>')
 
 
 if __name__ == '__main__': # for test
     import sys
     print(sys.argv)
```

### Comparing `idlea-1.2.8/idlealib/RunMultiLine.py` & `idlea-1.2.9/idlealib/RunMultiLine.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/RunSelected.py` & `idlea-1.2.9/idlealib/RunSelected.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/SaveUntitled.py` & `idlea-1.2.9/idlealib/SaveUntitled.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/scripts/test.py` & `idlea-1.2.9/idlealib/scripts/test.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/ScrollHorizontal.py` & `idlea-1.2.9/idlealib/ScrollHorizontal.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/SelectVertical.py` & `idlea-1.2.9/idlealib/SelectVertical.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/ShareQRCode.py` & `idlea-1.2.9/idlealib/ShareQRCode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 '''将选中代码转化为二维码'''
 
 
 if __name__ == '__main__':
     import __init__
     __init__.test_editor(__file__)
 
-
 import tkinter as tk
-from PIL import ImageTk
-
-import qrcode
+try:
+    import qrcode
+    from PIL import ImageTk
+except ImportError as e:
+    print('%s: %s' % (__name__, e))
+    qrcode = None
 
 # TODO 过长文本保护（Unicode长度）/翻页显示
 # TODO 调整弹出位置
 
 
 def qrmake(qrstr): # max about 2340 chars
     qr = qrcode.QRCode(box_size=2, border=2)
@@ -39,14 +41,17 @@
         self.focus()
         self.bind('<Return>', lambda e: self.destroy())
         self.bind('<Escape>', lambda e: self.destroy())
 
 
 class ShareQRCode:
     def __init__(self, parent):
+        if qrcode is None:
+            return
+
         self.text = parent.text
         self.top = parent.top
 
         self.text.bind('<<share-qrcode>>', self.Post)
 
         parent.rmenu.add_separator()
         parent.rmenu.add_command(label='Share Code', command=self.Post)
```

### Comparing `idlea-1.2.8/idlealib/ShiftLines.py` & `idlea-1.2.9/idlealib/ShiftLines.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/SmartCopy.py` & `idlea-1.2.9/idlealib/SmartCopy.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/SmartPairing.py` & `idlea-1.2.9/idlealib/SmartPairing.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/SmartSelect.py` & `idlea-1.2.9/idlealib/SmartSelect.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/SwapCopy.py` & `idlea-1.2.9/idlealib/SwapCopy.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/TimeTag.py` & `idlea-1.2.9/idlealib/TimeStamp.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 
 if __name__ == '__main__':
     import __init__
     __init__.test_editor(__file__)
 
 
+import re
 import time
 
 
-class TimeTag:
+class TimeStamp:
     def __init__(self, parent):
         self.text = parent.text
 
         parent.text.bind('<F4>', self.Insert)
 
     def Insert(self, evt):
-        tag = time.strftime(' # %Y-%m-%d %H:%M:%S')
-        header = self.text.get('insert linestart', 'insert')
-        if not header.strip():
-            tag = tag[1:] + '\n' + header
-        self.text.insert('insert', tag)
+        if evt.state != 8:  # if not press any modifier keys
+            return
+
+        line = self.text.get('insert linestart', 'insert lineend')
+        indent = re.match(r'^\s*', line).group()
+
+        stamp = time.strftime('# %Y-%m-%d %H:%M:%S')
+        line2 = indent + stamp + '\n'
+
+        self.text.insert('insert linestart', line2)
```

### Comparing `idlea-1.2.8/idlealib/TrimTrailing.py` & `idlea-1.2.9/idlealib/TrimTrailing.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/UpperCase.py` & `idlea-1.2.9/idlealib/UpperCase.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/WindowManager.py` & `idlea-1.2.9/idlealib/WindowManager.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/WrapShell.py` & `idlea-1.2.9/idlealib/WrapShell.py`

 * *Files identical despite different names*

### Comparing `idlea-1.2.8/idlealib/__init__.py` & `idlea-1.2.9/idlealib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-"""IDLE-Advance: IDLE Useful Extensions
+"""IDLE Advance Extensions
 
 运行__main__.py获得一个加载所有插件的IDLE-Advance的示例文件。
 运行__init__.py获得一个打开自身脚本并加载所有插件的editor的例子。
 分别运行idlealib目录下的扩展文件，可以得到一个打开自身的editor或shell的例子。
 如果需要停用部分扩展，将对应的脚本移出目录后重启IDLE即可。
 
 See also: https://github.com/znsoooo/IDLE-Advance
 
-MIT license. Copyright (c) 2021-2022 Lishixian (znsoooo). All Rights Reserved.
+MIT license. Copyright (c) 2021-2024 Shixian Li (znsoooo). All Rights Reserved.
 
 """
 
 
 import os
 import sys
 
 PY36 = sys.version_info > (3, 6)
 # `abspath` for open in cmd like `python __init__.py` to open script.
 EXTENSIONS = os.listdir(os.path.dirname(os.path.abspath(__file__)))
 
-__author__  = 'Lishixian <lsx7@sina.com>'
+__author__  = 'Shixian Li <lsx7@sina.com>'
 __credits__ = 'See at: https://github.com/znsoooo/IDLE-Advance'
-__date__    = '2022'
-__version__ = '1.2'
+__date__    = '20240525'
+__version__ = '1.2.9'
 
 __all__ = ['run', 'test_editor', 'test_shell', 'PY36']
 
 
 # - Functions ----------------------------------------
 
 
@@ -216,15 +216,15 @@
         if name == 'ZzDummy':
             return
         return super().load_extension(name)
 
     def load_adv_extensions(self):
         for file in EXTENSIONS:
             name, ext = os.path.splitext(os.path.basename(file))
-            if ext == '.py' and name not in ('__init__', '__main__'):
+            if name[:2] != '__' and ext.lower() == '.py':
                 try:
                     self.load_extension(name) # TODO 支持任意位置文件导入
                 except Exception as e:
                     print("Fail to load extension 'idlealib.%s':\n  %s" % (name, e), file=sys.stderr)
                     # import traceback
                     # traceback.print_exc()
```

### Comparing `idlea-1.2.8/LICENSE.txt` & `idlea-1.2.9/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Lishixian (znsoooo). All Rights Reserved.
+Copyright (c) 2021-2024 Shixian Li (znsoooo). All rights reserved.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `idlea-1.2.8/README.md` & `idlea-1.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # IDLE-Advance
 
 ## About
 - __Platform:__ >= Windows or Linux/macOS (untested)
 - __Python:__ >= Python 3.4
-- __Author:__ Lishixian (znsoooo)
+- __Author:__ Shixian Li (znsoooo)
 - __Github:__ https://github.com/znsoooo/IDLE-Advance
-- __License:__ MIT License. Copyright (c) 2022 Lishixian (znsoooo). All Rights Reserved.
+- __License:__ MIT License. Copyright (c) 2021-2024 Shixian Li (znsoooo). All rights reserved.
 
 
 ## What is it?
 - `IDLE-Advance`  add some useful extensions base on `idlelib`. It can be work on any platform where `IDLE` can be work.
 - See `~/idlealib/readme.md` to get spec of each extension. It is same as open each script and watch \_\_doc__.
 - Stop extension(s) by moveing script(s) to `nouse` folder.
 - It will generate `.pybak` file in script folder, and `recent-saved.lst` in `userdir`. So make sure no important files will be overwritten.
@@ -87,15 +87,15 @@
 and set `value` as:
 ```
 "~\pythonw.exe" "~\idlealib\__main__.py" "%L" %*
 ```
 
 
 # IDLE增强计划（Advance）
-- __Author:__ Lishixian
+- __Author:__ Shixian Li
 - __QQ:__ 11313213
 - __Email:__ lsx7@sina.com
 - __Website:__ https://github.com/znsoooo/IDLE-Advance
 
 
 ## 运行方法
 - __平台：__ Windows/Python3.4 （Python3.4.4是Windows XP支持的最后一个版本，所以低于此版本的不再测试。Linux/macOS平台未做测试）
```

### Comparing `idlea-1.2.8/setup.py` & `idlea-1.2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import shutil
 import setuptools
 
 keys = ['readme', 'license', 'todo', 'version']
 os.makedirs('idlealib/docs', exist_ok=True)
 for file in os.listdir():
     if any(file.lower().startswith(k) for k in keys):
@@ -13,15 +14,15 @@
 
 with open('README.md', encoding='u8') as f:
     long_description = f.read().replace('[x]', chr(9989)).replace('[ ]', chr(10062)) # ✅❎
 
 setuptools.setup(
     name='idlea',
     version=version,
-    author='Lishixian(znsoooo)',
+    author='Shixian Li (znsoooo)',
     author_email='lsx7@sina.com',
     description='IDLE-Advance',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/znsoooo/IDLE-Advance',
     project_urls={
         'Bug Tracker': 'https://github.com/znsoooo/IDLE-Advance/issues',
@@ -36,11 +37,17 @@
     ],
     packages=['idlealib', 'idlealib.docs', 'idlealib.nouse', 'idlealib.scripts'],
     python_requires='>=3.4',
 
     # install_requires=['windnd'], # for drag-open file feature
     # extras_requires={'windnd': ['windnd']},
     license='MIT License',
-    entry_points={'console_scripts': ['idlea=idlealib:run']},
+    entry_points={
+        'console_scripts': [
+            'idlea=idlealib:run',
+            'idlea%d%d=idlealib:run' % sys.version_info[:2],
+            'idlea%d%d%d=idlealib:run' % (sys.version_info[:2] + (sys.maxsize.bit_length() + 1,)),
+        ]
+    },
     package_data={'': ['*.*']},
     keywords='IDLE-Advance IDLE IDLEA IDLEX extension idlelib idlexlib idlealib',
 )
```

### Comparing `idlea-1.2.8/TODO.md` & `idlea-1.2.9/TODO.md`

 * *Files identical despite different names*

