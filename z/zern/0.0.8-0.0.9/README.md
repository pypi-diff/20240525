# Comparing `tmp/zern-0.0.8.tar.gz` & `tmp/zern-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zern-0.0.8.tar", last modified: Mon May  6 07:58:27 2024, max compression
+gzip compressed data, was "zern-0.0.9.tar", last modified: Mon May  6 08:02:58 2024, max compression
```

## Comparing `zern-0.0.8.tar` & `zern-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.600166 zern-0.0.8/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.8/LICENSE
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 07:58:27.596166 zern-0.0.8/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     5788 2024-05-06 04:59:34.000000 zern-0.0.8/README.md
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      702 2024-05-06 07:54:46.000000 zern-0.0.8/pyproject.toml
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-06 07:58:27.600166 zern-0.0.8/setup.cfg
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/Core/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-06 07:56:14.000000 zern-0.0.8/src/zern/Core/session.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.8/src/zern/Core/trader.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/Core/websocket_connection/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3604 2024-05-06 07:57:44.000000 zern-0.0.8/src/zern/Core/websocket_connection/ticker.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.8/src/zern/__init__.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern/utils/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.8/src/zern/utils/OrderedList.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.8/src/zern/utils/Types.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.8/src/zern/utils/parsing.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 07:58:27.596166 zern-0.0.8/src/zern.egg-info/
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      386 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/SOURCES.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/dependency_links.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       40 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/requires.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-06 07:58:27.000000 zern-0.0.8/src/zern.egg-info/top_level.txt
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 08:02:58.279508 zern-0.0.9/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.9/LICENSE
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 08:02:58.279508 zern-0.0.9/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     5788 2024-05-06 08:01:13.000000 zern-0.0.9/README.md
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      702 2024-05-06 08:02:29.000000 zern-0.0.9/pyproject.toml
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-06 08:02:58.279508 zern-0.0.9/setup.cfg
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 08:02:58.279508 zern-0.0.9/src/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 08:02:58.279508 zern-0.0.9/src/zern/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 08:02:58.279508 zern-0.0.9/src/zern/Core/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-06 07:56:14.000000 zern-0.0.9/src/zern/Core/session.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.9/src/zern/Core/trader.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 08:02:58.279508 zern-0.0.9/src/zern/Core/websocket_connection/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3604 2024-05-06 07:57:44.000000 zern-0.0.9/src/zern/Core/websocket_connection/ticker.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.9/src/zern/__init__.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 08:02:58.279508 zern-0.0.9/src/zern/utils/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.9/src/zern/utils/OrderedList.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.9/src/zern/utils/Types.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.9/src/zern/utils/parsing.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-06 08:02:58.279508 zern-0.0.9/src/zern.egg-info/
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6442 2024-05-06 08:02:58.000000 zern-0.0.9/src/zern.egg-info/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      386 2024-05-06 08:02:58.000000 zern-0.0.9/src/zern.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-06 08:02:58.000000 zern-0.0.9/src/zern.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       40 2024-05-06 08:02:58.000000 zern-0.0.9/src/zern.egg-info/requires.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-06 08:02:58.000000 zern-0.0.9/src/zern.egg-info/top_level.txt
```

### Comparing `zern-0.0.8/LICENSE` & `zern-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zern-0.0.8/PKG-INFO` & `zern-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.8
+Version: 0.0.9
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 ```python
 from zern import Trader
 trader = Trader(user_name=YOUR_USERNAME,password=YOUR_PASSWORD,totp_key=YOUR_TOTP_KEY)
 ```
 
 The `Trader` class is used to initiate the trading process and interact with the trading platform. It provides various methods to retrieve data, manage orders, and access trading information.
 
-Check above in requirements if you need to get the totp key.
+Check below in TOTP section if you need to get the totp key.
 
 #### → GET YOUR INSTRUMENTS TOKENS HERE (If Required)
 ```python
 trader.instruments #this will contain all the instrument tokens and symbols. feel free to search it as per your requirements. the helper functions also use this variable.
 ```
```

### Comparing `zern-0.0.8/README.md` & `zern-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```python
 from zern import Trader
 trader = Trader(user_name=YOUR_USERNAME,password=YOUR_PASSWORD,totp_key=YOUR_TOTP_KEY)
 ```
 
 The `Trader` class is used to initiate the trading process and interact with the trading platform. It provides various methods to retrieve data, manage orders, and access trading information.
 
-Check above in requirements if you need to get the totp key.
+Check below in TOTP section if you need to get the totp key.
 
 #### → GET YOUR INSTRUMENTS TOKENS HERE (If Required)
 ```python
 trader.instruments #this will contain all the instrument tokens and symbols. feel free to search it as per your requirements. the helper functions also use this variable.
 ```
```

### Comparing `zern-0.0.8/pyproject.toml` & `zern-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zern"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Harsha Avapati", email="harshaavapati@gmail.com" },
 ]
 description = "An unofficial client library using Zerodha web api for live data and historical data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `zern-0.0.8/src/zern/Core/session.py` & `zern-0.0.9/src/zern/Core/session.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.8/src/zern/Core/trader.py` & `zern-0.0.9/src/zern/Core/trader.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.8/src/zern/Core/websocket_connection/ticker.py` & `zern-0.0.9/src/zern/Core/websocket_connection/ticker.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.8/src/zern/utils/OrderedList.py` & `zern-0.0.9/src/zern/utils/OrderedList.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.8/src/zern/utils/Types.py` & `zern-0.0.9/src/zern/utils/Types.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.8/src/zern/utils/parsing.py` & `zern-0.0.9/src/zern/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.8/src/zern.egg-info/PKG-INFO` & `zern-0.0.9/src/zern.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.8
+Version: 0.0.9
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,15 +25,15 @@
 ```python
 from zern import Trader
 trader = Trader(user_name=YOUR_USERNAME,password=YOUR_PASSWORD,totp_key=YOUR_TOTP_KEY)
 ```
 
 The `Trader` class is used to initiate the trading process and interact with the trading platform. It provides various methods to retrieve data, manage orders, and access trading information.
 
-Check above in requirements if you need to get the totp key.
+Check below in TOTP section if you need to get the totp key.
 
 #### → GET YOUR INSTRUMENTS TOKENS HERE (If Required)
 ```python
 trader.instruments #this will contain all the instrument tokens and symbols. feel free to search it as per your requirements. the helper functions also use this variable.
 ```
```

