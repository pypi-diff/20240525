# Comparing `tmp/pyiso20022-0.0.1.tar.gz` & `tmp/pyiso20022-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiso20022-0.0.1.tar", last modified: Wed May 22 19:53:38 2024, max compression
+gzip compressed data, was "pyiso20022-0.1.1.tar", last modified: Sat May 25 19:13:23 2024, max compression
```

## Comparing `pyiso20022-0.0.1.tar` & `pyiso20022-0.1.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-22 19:53:04.000000 pyiso20022-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 19:53:04.000000 pyiso20022-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/myproj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:04.000000 pyiso20022-0.0.1/myproj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 19:53:04.000000 pyiso20022-0.0.1/myproj/myclass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 19:53:17.000000 pyiso20022-0.0.1/pyiso20022/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022/head/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/head/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022/head/head_001_001_02/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/head/head_001_001_02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/head/head_001_001_02/head_001_001_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022/head/head_001_001_04/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/head/head_001_001_04/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/head/head_001_001_04/head_001_001_04.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022/pacs/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 19:53:17.000000 pyiso20022-0.0.1/pyiso20022/pacs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-22 19:53:24.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91247 2024-05-22 19:53:24.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-22 19:53:25.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92601 2024-05-22 19:53:25.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-22 19:53:23.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105538 2024-05-22 19:53:23.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_12/
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-22 19:53:25.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   106664 2024-05-22 19:53:25.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_13/
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-22 19:53:24.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   108350 2024-05-22 19:53:24.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_14/
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-22 19:53:23.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_14/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   106172 2024-05-22 19:53:23.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_003_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-22 19:53:26.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_003_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   101568 2024-05-22 19:53:26.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-22 19:53:27.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93875 2024-05-22 19:53:27.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-22 19:53:26.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   108639 2024-05-22 19:53:26.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-22 19:53:27.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   130882 2024-05-22 19:53:27.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_13/
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-22 19:53:28.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   127463 2024-05-22 19:53:28.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.159206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_007_001_13/
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-05-22 19:53:22.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_007_001_13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   108036 2024-05-22 19:53:22.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-22 19:53:17.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91471 2024-05-22 19:53:17.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-22 19:53:18.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92665 2024-05-22 19:53:18.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-22 19:53:18.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100613 2024-05-22 19:53:18.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-22 19:53:19.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   107712 2024-05-22 19:53:20.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_10/
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-22 19:53:19.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   107685 2024-05-22 19:53:19.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_12/
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-22 19:53:19.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104266 2024-05-22 19:53:19.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-22 19:53:20.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    92079 2024-05-22 19:53:20.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-22 19:53:21.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100868 2024-05-22 19:53:21.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-22 19:53:21.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100166 2024-05-22 19:53:21.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-22 19:53:22.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100319 2024-05-22 19:53:22.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.163206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_010_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-22 19:53:17.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_010_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41010 2024-05-22 19:53:17.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_028_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-22 19:53:28.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_028_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    98096 2024-05-22 19:53:28.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pacs/pacs_029_001_02/
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-22 19:53:20.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_029_001_02/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35965 2024-05-22 19:53:20.000000 pyiso20022-0.0.1/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/pain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-22 19:53:31.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90820 2024-05-22 19:53:31.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-22 19:53:32.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91335 2024-05-22 19:53:32.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-22 19:53:33.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99320 2024-05-22 19:53:33.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-22 19:53:32.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109547 2024-05-22 19:53:32.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-22 19:53:35.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91765 2024-05-22 19:53:35.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-22 19:53:33.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93119 2024-05-22 19:53:33.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-22 19:53:34.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109842 2024-05-22 19:53:34.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.167206 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_12/
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-22 19:53:34.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   109813 2024-05-22 19:53:34.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-22 19:53:30.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    90494 2024-05-22 19:53:30.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_08/
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-22 19:53:30.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_08/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91844 2024-05-22 19:53:30.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_10/
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-22 19:53:31.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104507 2024-05-22 19:53:31.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_11/
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   104478 2024-05-22 19:53:29.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_06/
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-22 19:53:37.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_06/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89884 2024-05-22 19:53:37.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_07/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-22 19:53:35.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_07/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91285 2024-05-22 19:53:35.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_09/
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-22 19:53:36.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_09/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100667 2024-05-22 19:53:36.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_10/
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-22 19:53:36.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_10/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   100638 2024-05-22 19:53:36.000000 pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:53:38.155206 pyiso20022-0.0.1/pyiso20022.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-22 19:53:38.000000 pyiso20022-0.0.1/pyiso20022.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-22 19:53:38.000000 pyiso20022-0.0.1/pyiso20022.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:53:38.000000 pyiso20022-0.0.1/pyiso20022.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 19:53:38.000000 pyiso20022-0.0.1/pyiso20022.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:53:38.171206 pyiso20022-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-22 19:53:04.000000 pyiso20022-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.811134 pyiso20022-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-25 19:12:56.000000 pyiso20022-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-25 19:13:23.811134 pyiso20022-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-25 19:12:56.000000 pyiso20022-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/myproj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 19:12:56.000000 pyiso20022-0.1.1/myproj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-25 19:12:56.000000 pyiso20022-0.1.1/myproj/myclass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 19:13:01.000000 pyiso20022-0.1.1/pyiso20022/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/head/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 19:13:14.000000 pyiso20022-0.1.1/pyiso20022/head/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/head/head_001_001_02/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-25 19:13:15.000000 pyiso20022-0.1.1/pyiso20022/head/head_001_001_02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32949 2024-05-25 19:13:15.000000 pyiso20022-0.1.1/pyiso20022/head/head_001_001_02/head_001_001_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/head/head_001_001_04/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-25 19:13:14.000000 pyiso20022-0.1.1/pyiso20022/head/head_001_001_04/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34348 2024-05-25 19:13:14.000000 pyiso20022-0.1.1/pyiso20022/head/head_001_001_04/head_001_001_04.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/pacs/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 19:13:01.000000 pyiso20022-0.1.1/pyiso20022/pacs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-25 19:13:09.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91247 2024-05-25 19:13:09.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-25 19:13:10.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92601 2024-05-25 19:13:11.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-05-25 19:13:08.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105538 2024-05-25 19:13:08.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-05-25 19:13:10.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106664 2024-05-25 19:13:10.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_13/
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-25 19:13:09.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108350 2024-05-25 19:13:09.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_14/
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-25 19:13:08.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_14/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106172 2024-05-25 19:13:08.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_003_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-25 19:13:11.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_003_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101568 2024-05-25 19:13:11.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-05-25 19:13:12.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93875 2024-05-25 19:13:12.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-25 19:13:11.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108639 2024-05-25 19:13:12.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-25 19:13:13.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130882 2024-05-25 19:13:13.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.795134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_13/
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-25 19:13:13.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127463 2024-05-25 19:13:13.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_007_001_13/
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-05-25 19:13:07.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_007_001_13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108036 2024-05-25 19:13:07.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-25 19:13:02.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91471 2024-05-25 19:13:02.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-25 19:13:02.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92665 2024-05-25 19:13:02.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-25 19:13:03.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100613 2024-05-25 19:13:03.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-25 19:13:04.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107712 2024-05-25 19:13:04.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-25 19:13:04.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107685 2024-05-25 19:13:04.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-25 19:13:03.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104266 2024-05-25 19:13:03.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-25 19:13:05.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92079 2024-05-25 19:13:05.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.799134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-25 19:13:06.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100868 2024-05-25 19:13:06.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-25 19:13:06.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100166 2024-05-25 19:13:06.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-25 19:13:07.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100319 2024-05-25 19:13:07.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_010_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-25 19:13:01.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_010_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41010 2024-05-25 19:13:01.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_028_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-25 19:13:14.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_028_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98096 2024-05-25 19:13:14.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pacs/pacs_029_001_02/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-25 19:13:05.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_029_001_02/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35965 2024-05-25 19:13:05.000000 pyiso20022-0.1.1/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pain/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 19:13:15.000000 pyiso20022-0.1.1/pyiso20022/pain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-05-25 19:13:17.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90820 2024-05-25 19:13:17.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-25 19:13:18.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91335 2024-05-25 19:13:18.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-25 19:13:19.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99320 2024-05-25 19:13:19.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.803134 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-05-25 19:13:18.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109547 2024-05-25 19:13:18.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-05-25 19:13:21.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91765 2024-05-25 19:13:21.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-25 19:13:19.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93119 2024-05-25 19:13:19.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-05-25 19:13:20.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109842 2024-05-25 19:13:20.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_12/
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-25 19:13:20.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109813 2024-05-25 19:13:20.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-05-25 19:13:16.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90494 2024-05-25 19:13:16.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_08/
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-25 19:13:16.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_08/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91844 2024-05-25 19:13:16.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-25 19:13:17.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104507 2024-05-25 19:13:17.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.807134 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_11/
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-25 19:13:15.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104478 2024-05-25 19:13:15.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.811134 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_06/
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-25 19:13:23.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_06/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89884 2024-05-25 19:13:23.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.811134 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_07/
+-rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-25 19:13:21.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_07/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91285 2024-05-25 19:13:21.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.811134 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_09/
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-25 19:13:22.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_09/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100667 2024-05-25 19:13:22.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.811134 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_10/
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-05-25 19:13:22.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_10/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100638 2024-05-25 19:13:22.000000 pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 19:13:23.791134 pyiso20022-0.1.1/pyiso20022.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-25 19:13:23.000000 pyiso20022-0.1.1/pyiso20022.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-25 19:13:23.000000 pyiso20022-0.1.1/pyiso20022.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 19:13:23.000000 pyiso20022-0.1.1/pyiso20022.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 19:13:23.000000 pyiso20022-0.1.1/pyiso20022.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 19:13:23.811134 pyiso20022-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-25 19:12:56.000000 pyiso20022-0.1.1/setup.py
```

### Comparing `pyiso20022-0.0.1/LICENSE` & `pyiso20022-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/head/head_001_001_02/__init__.py` & `pyiso20022-0.1.1/pyiso20022/head/head_001_001_02/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/head/head_001_001_02/head_001_001_02.py` & `pyiso20022-0.1.1/pyiso20022/head/head_001_001_02/head_001_001_02.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/head/head_001_001_04/__init__.py` & `pyiso20022-0.1.1/pyiso20022/head/head_001_001_04/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/head/head_001_001_04/head_001_001_04.py` & `pyiso20022-0.1.1/pyiso20022/head/head_001_001_04/head_001_001_04.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_08/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_08/pacs_002_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_09/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_09/pacs_002_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_11/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_11/pacs_002_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_12/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_12/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_12/pacs_002_001_12.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_13/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_13/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_13/pacs_002_001_13.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_14/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_14/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_002_001_14/pacs_002_001_14.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_003_001_11/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_003_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_003_001_11/pacs_003_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_07/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_07/pacs_004_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_09/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_09/pacs_004_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_11/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_11/pacs_004_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_13/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_13/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_004_001_13/pacs_004_001_13.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_007_001_13/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_007_001_13/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_007_001_13/pacs_007_001_13.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_06/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_06/pacs_008_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_07/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_07/pacs_008_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_08/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_08/pacs_008_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_09/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_09/pacs_008_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_10/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_10/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_10/pacs_008_001_10.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_12/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_12/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_008_001_12/pacs_008_001_12.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_07/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_07/pacs_009_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_08/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_08/pacs_009_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_09/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_09/pacs_009_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_11/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_009_001_11/pacs_009_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_010_001_06/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_010_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_010_001_06/pacs_010_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_028_001_06/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_028_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_028_001_06/pacs_028_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_029_001_02/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_029_001_02/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py` & `pyiso20022-0.1.1/pyiso20022/pacs/pacs_029_001_02/pacs_029_001_02.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_07/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_07/pain_001_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_08/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_08/pain_001_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_09/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_09/pain_001_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_11/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_001_001_11/pain_001_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_08/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_08/pain_002_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_09/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_09/pain_002_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_11/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_11/pain_002_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_12/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_12/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_002_001_12/pain_002_001_12.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_07/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_07/pain_007_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_08/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_08/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_08/pain_007_001_08.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_10/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_10/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_10/pain_007_001_10.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_11/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_11/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_007_001_11/pain_007_001_11.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_06/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_06/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_06/pain_008_001_06.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_07/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_07/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_07/pain_008_001_07.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_09/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_09/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_09/pain_008_001_09.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_10/__init__.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_10/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py` & `pyiso20022-0.1.1/pyiso20022/pain/pain_008_001_10/pain_008_001_10.py`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/pyiso20022.egg-info/SOURCES.txt` & `pyiso20022-0.1.1/pyiso20022.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiso20022-0.0.1/setup.py` & `pyiso20022-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyiso20022",
-    version="0.0.1",
+    version="0.1.1",
     author="Peter Houghton",
     author_email="pete@investigatingsoftware.co.uk",
     description="pyiso20022 is a library for generating ISO20022 messages in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoughton/pyiso20022",
     packages=setuptools.find_packages(),
```

