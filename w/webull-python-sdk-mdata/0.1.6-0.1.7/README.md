# Comparing `tmp/webull_python_sdk_mdata-0.1.6.tar.gz` & `tmp/webull_python_sdk_mdata-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull_python_sdk_mdata-0.1.6.tar", last modified: Sat May 11 03:37:06 2024, max compression
+gzip compressed data, was "webull_python_sdk_mdata-0.1.7.tar", last modified: Sat May 25 02:18:50 2024, max compression
```

## Comparing `webull_python_sdk_mdata-0.1.6.tar` & `webull_python_sdk_mdata-0.1.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.207157 webull_python_sdk_mdata-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-11 03:37:06.207157 webull_python_sdk_mdata-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:37:06.207157 webull_python_sdk_mdata-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.207157 webull_python_sdk_mdata-0.1.6/webull_python_sdk_mdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-11 03:37:06.000000 webull_python_sdk_mdata-0.1.6/webull_python_sdk_mdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-11 03:37:06.000000 webull_python_sdk_mdata-0.1.6/webull_python_sdk_mdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:37:06.000000 webull_python_sdk_mdata-0.1.6/webull_python_sdk_mdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-11 03:37:06.000000 webull_python_sdk_mdata-0.1.6/webull_python_sdk_mdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 03:37:06.000000 webull_python_sdk_mdata-0.1.6/webull_python_sdk_mdata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.199156 webull_python_sdk_mdata-0.1.6/webullsdkmdata/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.199156 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/category.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/exchange_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/exercise_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/expiration_cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/instrument_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/option_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/subscribe_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/timespan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.199156 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.203156 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/market_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.203156 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/pb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/pb/quote_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.203156 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/response_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/market_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.203156 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/ask_bid_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/basic_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/broker_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/default_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/order_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/payload_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/quote_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/quote_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/snapshot_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/snapshot_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/tick_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/tick_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.207157 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/get_historical_bars_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/get_instruments_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/get_snapshot_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:06.207157 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/base_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_historical_bars_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_instruments_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_quote_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_snapshot_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_streaming_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_tick_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/quotes_subscribe_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-11 03:37:00.000000 webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/quotes_unsubscribe_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.140912 webull_python_sdk_mdata-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-25 02:18:50.140912 webull_python_sdk_mdata-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:18:50.140912 webull_python_sdk_mdata-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.140912 webull_python_sdk_mdata-0.1.7/webull_python_sdk_mdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-25 02:18:50.000000 webull_python_sdk_mdata-0.1.7/webull_python_sdk_mdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-25 02:18:50.000000 webull_python_sdk_mdata-0.1.7/webull_python_sdk_mdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:18:50.000000 webull_python_sdk_mdata-0.1.7/webull_python_sdk_mdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-25 02:18:50.000000 webull_python_sdk_mdata-0.1.7/webull_python_sdk_mdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 02:18:50.000000 webull_python_sdk_mdata-0.1.7/webull_python_sdk_mdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.128912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.132912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/exchange_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/exercise_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/expiration_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/instrument_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/option_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/subscribe_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/timespan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.132912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.132912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/market_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.132912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/pb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/pb/quote_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.132912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/response_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/market_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.136912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/ask_bid_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/basic_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/broker_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/default_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/order_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/payload_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/quote_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/quote_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/snapshot_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/snapshot_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/tick_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/tick_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.136912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/get_historical_bars_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/get_instruments_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/get_snapshot_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:50.136912 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/base_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_historical_bars_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_instruments_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_quote_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_snapshot_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_streaming_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_tick_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/quotes_subscribe_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-25 02:18:46.000000 webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/quotes_unsubscribe_request.py
```

### Comparing `webull_python_sdk_mdata-0.1.6/setup.py` & `webull_python_sdk_mdata-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 RD_CONTENT_TYPE = "text/markdown"
 LICENSE = "Apache License 2.0"
 
 with open("README.rst") as fp:
     LONG_DESCRIPTION = fp.read()
 
 requires = [
-    "webull-python-sdk-core==0.1.6",
-    "webull-python-sdk-quotes-core==0.1.6"
+    "webull-python-sdk-core==0.1.7",
+    "webull-python-sdk-quotes-core==0.1.7"
 ]
 
 setup_args = {
     'version': VERSION,
     'author': AUTHOR,
     'author_email': AUTHOR_EMAIL,
     'description': DESCRIPTION,
```

### Comparing `webull_python_sdk_mdata-0.1.6/webull_python_sdk_mdata.egg-info/SOURCES.txt` & `webull_python_sdk_mdata-0.1.7/webull_python_sdk_mdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/category.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/category.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/direction.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/direction.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/exchange_code.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/exchange_code.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/exercise_style.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/exercise_style.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/expiration_cycle.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/expiration_cycle.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/instrument_status.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/instrument_status.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/option_type.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/option_type.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/subscribe_type.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/subscribe_type.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/common/timespan.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/common/timespan.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/instrument.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/instrument.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/market_data.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/market_data.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/pb/quote_pb2.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/pb/quote_pb2.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/response.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/response.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/grpc/response_code.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/grpc/response_code.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/instrument.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/instrument.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/market_data.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/market_data.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/ask_bid_result.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/ask_bid_result.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/basic_result.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/basic_result.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/broker_result.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/broker_result.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/default_client.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/default_client.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/message_pb2.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/message_pb2.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/order_result.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/order_result.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/payload_type.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/payload_type.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/quote_decoder.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/quote_decoder.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/quote_result.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/quote_result.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/snapshot_decoder.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/snapshot_decoder.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/snapshot_result.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/snapshot_result.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/tick_decoder.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/tick_decoder.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/quotes/subscribe/tick_result.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/quotes/subscribe/tick_result.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/get_historical_bars_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/get_historical_bars_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/get_instruments_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/get_instruments_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/get_snapshot_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/get_snapshot_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/base_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/base_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_historical_bars_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_historical_bars_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_instruments_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_instruments_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_quote_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_quote_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_snapshot_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_snapshot_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_streaming_token_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_streaming_token_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/get_tick_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/get_tick_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/quotes_subscribe_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/quotes_subscribe_request.py`

 * *Files identical despite different names*

### Comparing `webull_python_sdk_mdata-0.1.6/webullsdkmdata/request/grpc/quotes_unsubscribe_request.py` & `webull_python_sdk_mdata-0.1.7/webullsdkmdata/request/grpc/quotes_unsubscribe_request.py`

 * *Files identical despite different names*

