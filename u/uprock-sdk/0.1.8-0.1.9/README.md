# Comparing `tmp/uprock_sdk-0.1.8.tar.gz` & `tmp/uprock_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uprock_sdk-0.1.8.tar", max compression
+gzip compressed data, was "uprock_sdk-0.1.9.tar", max compression
```

## Comparing `uprock_sdk-0.1.8.tar` & `uprock_sdk-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       12 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/README.md
--rw-r--r--   0        0        0      468 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      337 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/uprock_sdk/__init__.py
--rw-r--r--   0        0        0     3176 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/uprock_sdk/customers.py
--rw-r--r--   0        0        0      566 2024-04-02 10:27:21.426401 uprock_sdk-0.1.8/uprock_sdk/settings.py
--rw-r--r--   0        0        0     2931 2024-04-02 10:27:21.426401 uprock_sdk-0.1.8/uprock_sdk/terms.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 uprock_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-04-02 18:10:00.075145 uprock_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0      468 2024-04-02 18:10:00.075145 uprock_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      337 2024-04-02 18:10:00.075145 uprock_sdk-0.1.9/uprock_sdk/__init__.py
+-rw-r--r--   0        0        0     3176 2024-04-02 18:10:00.075145 uprock_sdk-0.1.9/uprock_sdk/customers.py
+-rw-r--r--   0        0        0      566 2024-04-02 18:10:00.075145 uprock_sdk-0.1.9/uprock_sdk/settings.py
+-rw-r--r--   0        0        0      546 2024-04-02 18:10:00.075145 uprock_sdk-0.1.9/uprock_sdk/telegram_bots.py
+-rw-r--r--   0        0        0     2931 2024-04-02 18:10:00.076145 uprock_sdk-0.1.9/uprock_sdk/terms.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 uprock_sdk-0.1.9/PKG-INFO
```

### Comparing `uprock_sdk-0.1.8/uprock_sdk/customers.py` & `uprock_sdk-0.1.9/uprock_sdk/customers.py`

 * *Files identical despite different names*

### Comparing `uprock_sdk-0.1.8/uprock_sdk/settings.py` & `uprock_sdk-0.1.9/uprock_sdk/settings.py`

 * *Files identical despite different names*

### Comparing `uprock_sdk-0.1.8/uprock_sdk/terms.py` & `uprock_sdk-0.1.9/uprock_sdk/terms.py`

 * *Files identical despite different names*

### Comparing `uprock_sdk-0.1.8/PKG-INFO` & `uprock_sdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uprock-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Aleksey Dalekin
 Author-email: adalekin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

