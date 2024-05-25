# Comparing `tmp/xju-3.2.0.tar.gz` & `tmp/xju-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xju-3.2.0.tar", last modified: Fri May  3 10:40:21 2024, max compression
+gzip compressed data, was "xju-3.2.1.tar", last modified: Sat May 25 02:26:06 2024, max compression
```

## Comparing `xju-3.2.0.tar` & `xju-3.2.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-03 10:40:21.473490 xju-3.2.0/
--rw-r--r--   0 xju       (1001) xju       (1001)     1064 2024-05-03 10:40:20.000000 xju-3.2.0/MIT-LICENCE
--rw-r--r--   0 xju       (1001) xju       (1001)    10476 2024-05-03 10:40:21.473490 xju-3.2.0/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     8940 2024-05-03 10:40:20.000000 xju-3.2.0/README.rst
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2024-05-03 10:40:20.000000 xju-3.2.0/pyproject.toml
--rw-r--r--   0 xju       (1001) xju       (1001)       38 2024-05-03 10:40:21.473490 xju-3.2.0/setup.cfg
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-03 10:40:21.465489 xju-3.2.0/src/
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-03 10:40:21.469490 xju-3.2.0/src/xju/
--rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-3.2.0/src/xju/assert_.py
--rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-3.2.0/src/xju/assert_.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-03 10:40:21.469490 xju-3.2.0/src/xju/cmc/
--rwxr-xr-x   0 xju       (1001) xju       (1001)     9796 2023-11-19 01:52:13.000000 xju-3.2.0/src/xju/cmc/AsyncDict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-3.2.0/src/xju/cmc/AsyncOpt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-3.2.0/src/xju/cmc/AsyncServiceQueue.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-11-26 07:06:55.000000 xju-3.2.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-3.2.0/src/xju/cmc/Dict.py.test
--rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-3.2.0/src/xju/cmc/Opt.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1459 2024-03-19 10:15:57.000000 xju-3.2.0/src/xju/cmc/Process.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-3.2.0/src/xju/cmc/ThreadMutexLockCondition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    45419 2024-03-09 04:40:58.000000 xju-3.2.0/src/xju/cmc/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)     8548 2024-03-09 07:44:30.000000 xju-3.2.0/src/xju/cmc/async_cmclass.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-3.2.0/src/xju/cmc/cmc.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    14897 2024-03-09 07:13:47.000000 xju-3.2.0/src/xju/cmc/cmclass.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4475 2024-03-01 12:12:32.000000 xju-3.2.0/src/xju/cmc/delay_cancellation.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-03 10:40:21.473490 xju-3.2.0/src/xju/cmc/io/
--rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-3.2.0/src/xju/cmc/io/FileLock.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-3.2.0/src/xju/cmc/io/FileMode.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-3.2.0/src/xju/cmc/io/FilePosition.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-3.2.0/src/xju/cmc/io/FileReader.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-3.2.0/src/xju/cmc/io/FileWriter.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-3.2.0/src/xju/cmc/io/Pipe.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-3.2.0/src/xju/cmc/io/UnixStreamSocket.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18361 2024-03-19 08:42:32.000000 xju-3.2.0/src/xju/cmc/io/__init__.py
--rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-3.2.0/src/xju/cmc/perflog.py
--rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-3.2.0/src/xju/cmc/perflog.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-3.2.0/src/xju/cmc/signal.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-3.2.0/src/xju/cmc/signal.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-3.2.0/src/xju/cmc/tstore.py
--rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-3.2.0/src/xju/cmc/tstore.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7377 2024-05-03 10:40:20.000000 xju-3.2.0/src/xju/cmc_mypy_plugin.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2193 2024-02-04 01:38:20.000000 xju-3.2.0/src/xju/cmd.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-3.2.0/src/xju/cmd.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    85204 2024-05-03 10:25:37.000000 xju-3.2.0/src/xju/json_codec.py
--rwxr-xr-x   0 xju       (1001) xju       (1001)    47610 2024-05-03 10:25:06.000000 xju-3.2.0/src/xju/json_codec.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     9347 2024-05-03 10:40:20.000000 xju-3.2.0/src/xju/json_codec_mypy_plugin.py
--rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-3.2.0/src/xju/jsonschema.py
--rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-3.2.0/src/xju/jsonschema.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1352 2024-03-01 12:17:56.000000 xju-3.2.0/src/xju/misc.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-3.2.0/src/xju/misc.py.test
--r--r--r--   0 xju       (1001) xju       (1001)    26466 2024-04-28 03:38:30.000000 xju-3.2.0/src/xju/newtype.py
--rw-r--r--   0 xju       (1001) xju       (1001)    13529 2024-04-28 03:38:21.000000 xju-3.2.0/src/xju/newtype.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-3.2.0/src/xju/patch.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-3.2.0/src/xju/patch.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)    18970 2024-04-28 00:35:48.000000 xju-3.2.0/src/xju/pq.py
--rw-r--r--   0 xju       (1001) xju       (1001)    11182 2024-04-28 00:35:48.000000 xju-3.2.0/src/xju/pq.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)        0 2024-05-03 10:40:20.000000 xju-3.2.0/src/xju/py.typed
--rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-3.2.0/src/xju/rfc2616.py
--rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-3.2.0/src/xju/rfc2616.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     3403 2023-10-03 21:35:57.000000 xju-3.2.0/src/xju/time.py
--rw-r--r--   0 xju       (1001) xju       (1001)     2762 2023-10-03 21:39:56.000000 xju-3.2.0/src/xju/time.py.test
--rw-r--r--   0 xju       (1001) xju       (1001)     7647 2024-03-19 08:36:54.000000 xju-3.2.0/src/xju/xn.py
--rw-r--r--   0 xju       (1001) xju       (1001)     6010 2024-03-19 08:44:56.000000 xju-3.2.0/src/xju/xn.py.test
-drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-03 10:40:21.473490 xju-3.2.0/src/xju.egg-info/
--rw-r--r--   0 xju       (1001) xju       (1001)    10476 2024-05-03 10:40:21.000000 xju-3.2.0/src/xju.egg-info/PKG-INFO
--rw-r--r--   0 xju       (1001) xju       (1001)     1508 2024-05-03 10:40:21.000000 xju-3.2.0/src/xju.egg-info/SOURCES.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        1 2024-05-03 10:40:21.000000 xju-3.2.0/src/xju.egg-info/dependency_links.txt
--rw-r--r--   0 xju       (1001) xju       (1001)        4 2024-05-03 10:40:21.000000 xju-3.2.0/src/xju.egg-info/top_level.txt
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-25 02:26:06.662345 xju-3.2.1/
+-rw-r--r--   0 xju       (1001) xju       (1001)     1064 2024-05-25 02:26:05.000000 xju-3.2.1/MIT-LICENCE
+-rw-r--r--   0 xju       (1001) xju       (1001)    10843 2024-05-25 02:26:06.662345 xju-3.2.1/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     9307 2024-05-25 02:26:05.000000 xju-3.2.1/README.rst
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2024-05-25 02:26:05.000000 xju-3.2.1/pyproject.toml
+-rw-r--r--   0 xju       (1001) xju       (1001)       38 2024-05-25 02:26:06.662345 xju-3.2.1/setup.cfg
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-25 02:26:06.654345 xju-3.2.1/src/
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-25 02:26:06.658345 xju-3.2.1/src/xju/
+-rw-r--r--   0 xju       (1001) xju       (1001)     6193 2023-06-11 10:22:00.000000 xju-3.2.1/src/xju/assert_.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6256 2023-06-11 10:46:04.000000 xju-3.2.1/src/xju/assert_.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-25 02:26:06.662345 xju-3.2.1/src/xju/cmc/
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     9796 2023-11-19 01:52:13.000000 xju-3.2.1/src/xju/cmc/AsyncDict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     4077 2023-06-20 10:35:13.000000 xju-3.2.1/src/xju/cmc/AsyncOpt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3356 2023-03-18 10:41:04.000000 xju-3.2.1/src/xju/cmc/AsyncServiceQueue.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2716 2023-11-26 07:06:55.000000 xju-3.2.1/src/xju/cmc/AsyncTaskMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     8726 2023-03-18 10:40:34.000000 xju-3.2.1/src/xju/cmc/Dict.py.test
+-rwxr-xr-x   0 xju       (1001) xju       (1001)     3827 2023-06-21 01:32:08.000000 xju-3.2.1/src/xju/cmc/Opt.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1459 2024-03-19 10:15:57.000000 xju-3.2.1/src/xju/cmc/Process.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2295 2023-03-18 10:40:59.000000 xju-3.2.1/src/xju/cmc/ThreadMutexLockCondition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    45419 2024-03-09 04:40:58.000000 xju-3.2.1/src/xju/cmc/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     8548 2024-03-09 07:44:30.000000 xju-3.2.1/src/xju/cmc/async_cmclass.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2239 2023-06-17 10:59:33.000000 xju-3.2.1/src/xju/cmc/cmc.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    14897 2024-03-09 07:13:47.000000 xju-3.2.1/src/xju/cmc/cmclass.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4475 2024-03-01 12:12:32.000000 xju-3.2.1/src/xju/cmc/delay_cancellation.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-25 02:26:06.662345 xju-3.2.1/src/xju/cmc/io/
+-rw-r--r--   0 xju       (1001) xju       (1001)     2279 2023-03-18 10:40:06.000000 xju-3.2.1/src/xju/cmc/io/FileLock.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1598 2023-03-18 10:39:38.000000 xju-3.2.1/src/xju/cmc/io/FileMode.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1801 2023-03-18 10:39:45.000000 xju-3.2.1/src/xju/cmc/io/FilePosition.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3935 2023-03-18 10:39:53.000000 xju-3.2.1/src/xju/cmc/io/FileReader.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     4407 2023-03-18 10:39:59.000000 xju-3.2.1/src/xju/cmc/io/FileWriter.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3806 2023-03-29 20:33:11.000000 xju-3.2.1/src/xju/cmc/io/Pipe.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     5008 2023-03-18 10:40:18.000000 xju-3.2.1/src/xju/cmc/io/UnixStreamSocket.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18361 2024-03-19 08:42:32.000000 xju-3.2.1/src/xju/cmc/io/__init__.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    23724 2022-10-22 03:21:18.000000 xju-3.2.1/src/xju/cmc/perflog.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    16348 2023-03-18 10:40:54.000000 xju-3.2.1/src/xju/cmc/perflog.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     2042 2023-03-11 11:25:32.000000 xju-3.2.1/src/xju/cmc/signal.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1460 2023-03-18 10:40:41.000000 xju-3.2.1/src/xju/cmc/signal.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    26119 2022-10-28 11:58:37.000000 xju-3.2.1/src/xju/cmc/tstore.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    12879 2023-03-18 10:40:48.000000 xju-3.2.1/src/xju/cmc/tstore.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7377 2024-05-25 02:26:05.000000 xju-3.2.1/src/xju/cmc_mypy_plugin.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2193 2024-02-04 01:38:20.000000 xju-3.2.1/src/xju/cmd.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2132 2023-03-18 11:29:29.000000 xju-3.2.1/src/xju/cmd.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    85530 2024-05-25 00:35:44.000000 xju-3.2.1/src/xju/json_codec.py
+-rwxr-xr-x   0 xju       (1001) xju       (1001)    47600 2024-05-25 00:28:05.000000 xju-3.2.1/src/xju/json_codec.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     9347 2024-05-25 02:26:05.000000 xju-3.2.1/src/xju/json_codec_mypy_plugin.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     8199 2023-03-11 10:40:25.000000 xju-3.2.1/src/xju/jsonschema.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     9298 2023-03-18 10:37:26.000000 xju-3.2.1/src/xju/jsonschema.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1352 2024-03-01 12:17:56.000000 xju-3.2.1/src/xju/misc.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1170 2023-03-18 10:38:39.000000 xju-3.2.1/src/xju/misc.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    26466 2024-05-24 23:53:23.000000 xju-3.2.1/src/xju/newtype.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    13529 2024-05-24 23:53:23.000000 xju-3.2.1/src/xju/newtype.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     1340 2022-10-22 04:27:19.000000 xju-3.2.1/src/xju/patch.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1121 2023-03-18 10:38:49.000000 xju-3.2.1/src/xju/patch.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)    18970 2024-05-24 23:53:23.000000 xju-3.2.1/src/xju/pq.py
+-rw-r--r--   0 xju       (1001) xju       (1001)    11182 2024-05-24 23:53:23.000000 xju-3.2.1/src/xju/pq.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)        0 2024-05-25 02:26:05.000000 xju-3.2.1/src/xju/py.typed
+-rw-r--r--   0 xju       (1001) xju       (1001)     1744 2022-10-19 21:07:30.000000 xju-3.2.1/src/xju/rfc2616.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     1937 2023-03-18 10:39:11.000000 xju-3.2.1/src/xju/rfc2616.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     3403 2023-10-03 21:35:57.000000 xju-3.2.1/src/xju/time.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     2762 2023-10-03 21:39:56.000000 xju-3.2.1/src/xju/time.py.test
+-rw-r--r--   0 xju       (1001) xju       (1001)     7647 2024-03-19 08:36:54.000000 xju-3.2.1/src/xju/xn.py
+-rw-r--r--   0 xju       (1001) xju       (1001)     6010 2024-03-19 08:44:56.000000 xju-3.2.1/src/xju/xn.py.test
+drwxr-xr-x   0 xju       (1001) xju       (1001)        0 2024-05-25 02:26:06.658345 xju-3.2.1/src/xju.egg-info/
+-rw-r--r--   0 xju       (1001) xju       (1001)    10843 2024-05-25 02:26:06.000000 xju-3.2.1/src/xju.egg-info/PKG-INFO
+-rw-r--r--   0 xju       (1001) xju       (1001)     1508 2024-05-25 02:26:06.000000 xju-3.2.1/src/xju.egg-info/SOURCES.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        1 2024-05-25 02:26:06.000000 xju-3.2.1/src/xju.egg-info/dependency_links.txt
+-rw-r--r--   0 xju       (1001) xju       (1001)        4 2024-05-25 02:26:06.000000 xju-3.2.1/src/xju.egg-info/top_level.txt
```

### Comparing `xju-3.2.0/MIT-LICENCE` & `xju-3.2.1/MIT-LICENCE`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/PKG-INFO` & `xju-3.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 3.2.0
+Version: 3.2.1
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -195,14 +195,19 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 3.2.1 keep Array as typescript type for json_codec encoding of pythong set
+        - json_codec typescript side has no transforming decode/encode step -
+          it assumes the json objects *are* the typescript objects
+        - someday perhaps json_codec will generate full typescript codecs,
+          which will then allow non-json types on the typescript side
 - 3.2.0 add set support to xju.json_codec
 - 3.1.0 add validity pattern support to xju.newtype.Str
 - 3.1.0 fix xju.json_codec encode of subclass value
 - 3.0.1 fix json_codec_mypy_plugin issues 2, 3
 - 3.0.0 actually switch xju.xn.in_function_context to use first_para_of not first_line_of
         - see *breaking change* below, this time actually did that change
 - 2.0.3 improve xju.json_codec typescript object key generation v xju.NewStr
```

### Comparing `xju-3.2.0/README.rst` & `xju-3.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,19 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 3.2.1 keep Array as typescript type for json_codec encoding of pythong set
+        - json_codec typescript side has no transforming decode/encode step -
+          it assumes the json objects *are* the typescript objects
+        - someday perhaps json_codec will generate full typescript codecs,
+          which will then allow non-json types on the typescript side
 - 3.2.0 add set support to xju.json_codec
 - 3.1.0 add validity pattern support to xju.newtype.Str
 - 3.1.0 fix xju.json_codec encode of subclass value
 - 3.0.1 fix json_codec_mypy_plugin issues 2, 3
 - 3.0.0 actually switch xju.xn.in_function_context to use first_para_of not first_line_of
         - see *breaking change* below, this time actually did that change
 - 2.0.3 improve xju.json_codec typescript object key generation v xju.NewStr
```

### Comparing `xju-3.2.0/pyproject.toml` & `xju-3.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "xju"
-version = "3.2.0"
+version = "3.2.1"
 description = "xju library"
 readme = "README.rst"
 authors = [{ name = "Trevor Taylor"}]
 license = { file = "MIT-LICENCE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `xju-3.2.0/src/xju/assert_.py` & `xju-3.2.1/src/xju/assert_.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/assert_.py.test` & `xju-3.2.1/src/xju/assert_.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/AsyncDict.py.test` & `xju-3.2.1/src/xju/cmc/AsyncDict.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/AsyncOpt.py.test` & `xju-3.2.1/src/xju/cmc/AsyncOpt.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/AsyncServiceQueue.py.test` & `xju-3.2.1/src/xju/cmc/AsyncServiceQueue.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/AsyncTaskMutexLockCondition.py.test` & `xju-3.2.1/src/xju/cmc/AsyncTaskMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/Dict.py.test` & `xju-3.2.1/src/xju/cmc/Dict.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/Opt.py.test` & `xju-3.2.1/src/xju/cmc/Opt.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/Process.py.test` & `xju-3.2.1/src/xju/cmc/Process.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/ThreadMutexLockCondition.py.test` & `xju-3.2.1/src/xju/cmc/ThreadMutexLockCondition.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/__init__.py` & `xju-3.2.1/src/xju/cmc/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/async_cmclass.py.test` & `xju-3.2.1/src/xju/cmc/async_cmclass.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/cmc.py.test` & `xju-3.2.1/src/xju/cmc/cmc.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/cmclass.py.test` & `xju-3.2.1/src/xju/cmc/cmclass.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/delay_cancellation.py.test` & `xju-3.2.1/src/xju/cmc/delay_cancellation.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/FileLock.py.test` & `xju-3.2.1/src/xju/cmc/io/FileLock.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/FileMode.py.test` & `xju-3.2.1/src/xju/cmc/io/FileMode.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/FilePosition.py.test` & `xju-3.2.1/src/xju/cmc/io/FilePosition.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/FileReader.py.test` & `xju-3.2.1/src/xju/cmc/io/FileReader.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/FileWriter.py.test` & `xju-3.2.1/src/xju/cmc/io/FileWriter.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/Pipe.py.test` & `xju-3.2.1/src/xju/cmc/io/Pipe.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/UnixStreamSocket.py.test` & `xju-3.2.1/src/xju/cmc/io/UnixStreamSocket.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/io/__init__.py` & `xju-3.2.1/src/xju/cmc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/perflog.py` & `xju-3.2.1/src/xju/cmc/perflog.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/perflog.py.test` & `xju-3.2.1/src/xju/cmc/perflog.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/signal.py` & `xju-3.2.1/src/xju/cmc/signal.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/signal.py.test` & `xju-3.2.1/src/xju/cmc/signal.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/tstore.py` & `xju-3.2.1/src/xju/cmc/tstore.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc/tstore.py.test` & `xju-3.2.1/src/xju/cmc/tstore.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmc_mypy_plugin.py` & `xju-3.2.1/src/xju/cmc_mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmd.py` & `xju-3.2.1/src/xju/cmd.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/cmd.py.test` & `xju-3.2.1/src/xju/cmd.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/json_codec.py` & `xju-3.2.1/src/xju/json_codec.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,86 +422,95 @@
     def encode(self,x,back_ref:None|Callable[[Any],JsonType]):
         if type(x) is not set:
             raise Exception(f'{x!r} is not a set')
         return [self.value_codec.encode(_,back_ref) for _ in x]
     def decode(self,x,back_ref:None|Callable[[JsonType],Any]):
         if type(x) is not list:
             raise Exception(f'{x!r} is not a set')
-        return set([self.value_codec.decode(_,back_ref) for _ in x])
+        result = set([self.value_codec.decode(_,back_ref) for _ in x])
+        if len(result) < len(x):
+            raise Exception(f'{x!r} contains at least one duplicate element')
+        return result
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             "type": "array",
             "uniqueItems": True,
             "items": self.value_codec.get_json_schema(definitions, self_ref)
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None)->str:
-        return f"Set<{self.value_codec.typescript_type(back_refs)}>"
+        return f"Array<{self.value_codec.typescript_type(back_refs)}> /* with unique elements */"
     def typescript_as_object_key_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         raise Exception(f"{self.typescript_type(back_refs)} is not allowed as a typescript object key type")
     def ensure_typescript_defs(self, namespace) -> None:
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
-        raise Exception(f"get_typescript_isa is not available for Set")
+        tt=self.typescript_type(back_refs)
+        return TypeScriptSourceCode(
+            f"(((v:any):v is {tt}=>(\n"
+            "     Array.isArray(v) && \n"
+            f"    v.filter((x)=>(\n"
+            f"        !{indent(8,self.value_codec.get_typescript_isa(TypeScriptSourceCode('x'),namespace,back_refs))})).length==0))({expression}))")
     def get_typescript_asa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         tt=self.typescript_type(back_refs)
         return TypeScriptSourceCode(
             f"((v: any): {tt} => {{try{{\n"
             f"    if (!Array.isArray(v)) throw new Error(`${{v}} is not an array it is a ${{typeof v}}`);\n"
-            f"    const result = new {self.typescript_type(back_refs)};\n"
-            f"    v.forEach((x)=>result.add({indent(4,self.value_codec.get_typescript_asa(TypeScriptSourceCode('x'),namespace,back_refs))}));\n"
-            f"    return result;\n"
+            f"    v.forEach((x)=>{indent(4,self.value_codec.get_typescript_asa(TypeScriptSourceCode('x'),namespace,back_refs))});\n"
+            f"    return v as {tt};\n"
             f"}}catch(e:any){{throw new Error(`${{v}} is not a {tt} because ${{e}}`);}}}})({expression})")
     pass
 
 class AnySetCodecImpl:
     def __init__(self):
         self.value_codec=AnyJsonCodecImpl()
         pass
     def encode(self,x,back_ref:None|Callable[[Any],JsonType]):
         if type(x) is not set:
             raise Exception(f'{x!r} is not a set')
         return [self.value_codec.encode(_,back_ref) for _ in x]
     def decode(self,x,back_ref:None|Callable[[JsonType],Any]):
         if type(x) is not list:
             raise Exception(f'{x!r} is not a list')
-        return set([self.value_codec.decode(_,back_ref) for _ in x])
+        result = set([self.value_codec.decode(_,back_ref) for _ in x])
+        if len(result) < len(x):
+            raise Exception(f'{x!r} contains at least one duplicate element')
+        return result
     def get_json_schema(self, definitions:dict[str,dict], self_ref:None|str) -> dict:
         return {
             "type": "array",
             "uniqueItems": True
         }
     def typescript_type(self,back_refs:TypeScriptBackRefs|None)->str:
-        return f"Set<any>"
+        return f"Array<any> /* with unique elements */"
     def typescript_as_object_key_type(self,back_refs:TypeScriptBackRefs|None) -> str:
         raise Exception(f"{self.typescript_type(back_refs)} is not allowed as a typescript object key type")
     def ensure_typescript_defs(self, namespace) -> None:
         pass
     def get_typescript_isa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
-        raise Exception(f"get_typescript_isa is not available for Set")
+        return TypeScriptSourceCode(
+            f"(Array.isArray({expression}))")
     def get_typescript_asa(self,
                            expression:TypeScriptSourceCode,
                            namespace: TypeScriptNamespace,
                            back_refs:TypeScriptBackRefs|None) -> TypeScriptSourceCode:
         tt=self.typescript_type(back_refs)
         return TypeScriptSourceCode(
-            f"((v: any): {tt} => {{try{{\n\n"
-            f"    if (!Array.isArray(v)) throw new Error(`${{v}} is not an Array it is a ${{typeof v}}`);\n"
-            f"    const result = new {self.typescript_type(back_refs)};\n"
-            f"    v.forEach((x)=>result.add(x));\n"
-            f"    return result;\n"
-            f"}}catch(e:any){{throw new Error(`${{v}} is not a {tt} because ${{e}}`);}}}})({expression})")
+            f"((v: any): {tt} => {{\n"
+            f"    if (!Array.isArray(v)) throw new Error(`${{v}} is not an {tt} it is a ${{typeof v}}`);\n"
+            f"    return v as {tt};\n"
+            f"}})({expression})")
     pass
 
 class TupleCodec:
     def __init__(self,value_codecs):
         self.value_codecs=value_codecs
         self.number_of_codecs=len(value_codecs)
         pass
```

### Comparing `xju-3.2.0/src/xju/json_codec.py.test` & `xju-3.2.1/src/xju/json_codec.py.test`

 * *Files 1% similar despite different names*

```diff
@@ -123,28 +123,38 @@
 except Exception as e:
     Assert("'fred' (of type <class 'str'>) is not a <class 'int'>").isIn(str(e))
 else:
     assert False, x
     pass
 
 
-# set maps to list...
+# un-typed set maps to list...
 Assert(codec(set).decode([5, 'fred']))==set([5, 'fred'])
 set_result=codec(set).encode(set([5, 'fred']))
 assert isinstance(set_result,list)
 Assert(set(set_result))==set([5, 'fred'])
 
 # ... but must be given a set
 try:
     x=codec(set).decode(8)
 except Exception as e:
     Assert("8 is not a list").isIn(str(e))
 else:
     assert False, x
     pass
+
+# ... and elements must be unique
+try:
+    x=codec(set).decode([1,2,3,2])
+except Exception as e:
+    Assert('[1, 2, 3, 2] contains at least one duplicate element').isIn(str(e))
+else:
+    assert False, x
+    pass
+
 # ... note element types are not checked (it is assumed
 # result will be given to json.dumps, which will fail), e.g.
 # we can happily put print, which has no mapping to a json type,
 # into a non-type-adorned list and encode that list:
 Assert(codec(set).encode(set([print])))==[print]
 
 
@@ -167,14 +177,23 @@
 except Exception as e:
     Assert("'fred' (of type <class 'str'>) is not a <class 'int'>").isIn(str(e))
 else:
     assert False, x
     pass
 
 
+# ... and elements must be unique
+try:
+    x=codec(set[int]).decode([1,2,3,2])
+except Exception as e:
+    Assert('[1, 2, 3, 2] contains at least one duplicate element').isIn(str(e))
+else:
+    assert False, x
+    pass
+
 # bytes maps to list of number...
 Assert(codec(bytes).encode(b'\x1b\x17'))==[27,23]
 Assert(codec(bytes).decode([27,23]))==b'\x1b\x17'
 
 # ... but must be given bytes to encode...
 try:
     x=codec(bytes).encode(8)  # type: ignore
@@ -843,30 +862,14 @@
     x=codec(int|None).encode('fred')  # type: ignore
 except Exception as e:
     Assert(str(e)).contains("'fred' is not None")
 else:
     assert False, x
     pass
 
-try:
-    x=codec(set[int]).typescript_as_object_key_type()
-except Exception as e:
-    Assert(str(e)).contains("Set<number> is not allowed as a typescript object key type")
-else:
-    assert False, x
-    pass
-
-try:
-    x=codec(set).typescript_as_object_key_type()
-except Exception as e:
-    Assert(str(e)).contains("Set<any> is not allowed as a typescript object key type")
-else:
-    assert False, x
-    pass
-
 
 # Codec can generate corresponding json schema (http://json-schema.org)
 # "null", "boolean", "object", "array", "number", "string", or "integer"
 Assert(codec(NoneType).get_json_schema())=={'type': 'null', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 Assert(codec(int).get_json_schema())=={'type': 'integer', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 Assert(codec(bool).get_json_schema())=={'type': 'boolean', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
 Assert(codec(str).get_json_schema())=={'type': 'string', 'definitions': {}, '$id': 'https://example.com/address.schema.json', '$schema': 'https://json-schema.org/draft/2020-12/schema'}
@@ -1249,29 +1252,17 @@
     if (typeof v !== 'string') throw new Error(`${v} is not a string it is a ${typeof v}`);
     return v as string;
 })(7)""")
 
 codec(O).ensure_typescript_defs(typescript_namespace)
 
 
-try:
-    x=codec(set[int]).get_typescript_isa(TypeScriptSourceCode("v"),typescript_namespace)
-except Exception as e:
-    Assert(str(e)).contains("get_typescript_isa is not available for Set")
-else:
-    assert False, x
-    pass
+Assert(codec(set[int]).get_typescript_isa(TypeScriptSourceCode("v"),typescript_namespace))==TypeScriptSourceCode("(((v:any):v is Array<number> /* with unique elements */=>(\n     Array.isArray(v) && \n    v.filter((x)=>(\n        !(typeof (x) == 'number'))).length==0))(v))")
 
-try:
-    x=codec(set).get_typescript_isa(TypeScriptSourceCode("v"),typescript_namespace)
-except Exception as e:
-    Assert(str(e)).contains("get_typescript_isa is not available for Set")
-else:
-    assert False, x
-    pass
+Assert(codec(set).get_typescript_isa(TypeScriptSourceCode("v"),typescript_namespace))==TypeScriptSourceCode("(Array.isArray(v))")
 
 # ... get_formatted_defs() generates the typescript source code:
 Assert(typescript_namespace.get_formatted_defs())==TypeScriptSourceCode(
     '''\
 namespace xju {
     export namespace time {
         export type Timestamp = {
```

### Comparing `xju-3.2.0/src/xju/json_codec_mypy_plugin.py` & `xju-3.2.1/src/xju/json_codec_mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/jsonschema.py` & `xju-3.2.1/src/xju/jsonschema.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/jsonschema.py.test` & `xju-3.2.1/src/xju/jsonschema.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/misc.py` & `xju-3.2.1/src/xju/misc.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/misc.py.test` & `xju-3.2.1/src/xju/misc.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/newtype.py` & `xju-3.2.1/src/xju/newtype.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/newtype.py.test` & `xju-3.2.1/src/xju/newtype.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/patch.py` & `xju-3.2.1/src/xju/patch.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/patch.py.test` & `xju-3.2.1/src/xju/patch.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/pq.py` & `xju-3.2.1/src/xju/pq.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/pq.py.test` & `xju-3.2.1/src/xju/pq.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/rfc2616.py` & `xju-3.2.1/src/xju/rfc2616.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/rfc2616.py.test` & `xju-3.2.1/src/xju/rfc2616.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/time.py` & `xju-3.2.1/src/xju/time.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/time.py.test` & `xju-3.2.1/src/xju/time.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/xn.py` & `xju-3.2.1/src/xju/xn.py`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju/xn.py.test` & `xju-3.2.1/src/xju/xn.py.test`

 * *Files identical despite different names*

### Comparing `xju-3.2.0/src/xju.egg-info/PKG-INFO` & `xju-3.2.1/src/xju.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xju
-Version: 3.2.0
+Version: 3.2.1
 Summary: xju library
 Author: Trevor Taylor
 License: Copyright © 2022 Trevor Taylor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -195,14 +195,19 @@
 
 * Exception wrapping to provide human readable context gathering
 
 * see `xju/xn.py.test <xju/xn.py.test>`_ for sample code
 
 Release History
 
+- 3.2.1 keep Array as typescript type for json_codec encoding of pythong set
+        - json_codec typescript side has no transforming decode/encode step -
+          it assumes the json objects *are* the typescript objects
+        - someday perhaps json_codec will generate full typescript codecs,
+          which will then allow non-json types on the typescript side
 - 3.2.0 add set support to xju.json_codec
 - 3.1.0 add validity pattern support to xju.newtype.Str
 - 3.1.0 fix xju.json_codec encode of subclass value
 - 3.0.1 fix json_codec_mypy_plugin issues 2, 3
 - 3.0.0 actually switch xju.xn.in_function_context to use first_para_of not first_line_of
         - see *breaking change* below, this time actually did that change
 - 2.0.3 improve xju.json_codec typescript object key generation v xju.NewStr
```

### Comparing `xju-3.2.0/src/xju.egg-info/SOURCES.txt` & `xju-3.2.1/src/xju.egg-info/SOURCES.txt`

 * *Files identical despite different names*

