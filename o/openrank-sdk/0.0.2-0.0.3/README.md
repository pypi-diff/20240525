# Comparing `tmp/openrank_sdk-0.0.2.tar.gz` & `tmp/openrank_sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openrank_sdk-0.0.2.tar", max compression
+gzip compressed data, was "openrank_sdk-0.0.3.tar", max compression
```

## Comparing `openrank_sdk-0.0.2.tar` & `openrank_sdk-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3060 2024-05-23 07:21:38.123069 openrank_sdk-0.0.2/README.md
--rw-r--r--   0        0        0       42 2024-05-23 05:23:19.504354 openrank_sdk-0.0.2/openrank_sdk/__init__.py
--rw-r--r--   0        0        0     5476 2024-05-23 07:13:53.223669 openrank_sdk-0.0.2/openrank_sdk/eigentrust_client.py
--rw-r--r--   0        0        0      304 2024-05-25 05:48:00.098147 openrank_sdk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 openrank_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3086 2024-05-25 05:55:22.919334 openrank_sdk-0.0.3/README.md
+-rw-r--r--   0        0        0       42 2024-05-23 05:23:19.504354 openrank_sdk-0.0.3/openrank_sdk/__init__.py
+-rw-r--r--   0        0        0     5476 2024-05-23 07:13:53.223669 openrank_sdk-0.0.3/openrank_sdk/eigentrust_client.py
+-rw-r--r--   0        0        0      304 2024-05-25 05:55:42.941171 openrank_sdk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 openrank_sdk-0.0.3/PKG-INFO
```

### Comparing `openrank_sdk-0.0.2/README.md` & `openrank_sdk-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Py-EigenTrust
+# OpenRank SDK
 
-Py-EigenTrust is a python wrapper for https://github.com/Karma3Labs/go-eigentrust
+## EigenTrust by OpenRank
+EigenTrust SDk is a python wrapper for https://github.com/Karma3Labs/go-eigentrust
 
 ### Input
 
 You will need *local trust* and optionally *pre-trust.*  If pre-trust is not specified, each peer will have an equal weight. Both can be specified
 using a CSV or an array of a dict with `i`, `j`, and `v`.
 
 Sample local trust dict variable
```

### Comparing `openrank_sdk-0.0.2/openrank_sdk/eigentrust_client.py` & `openrank_sdk-0.0.3/openrank_sdk/eigentrust_client.py`

 * *Files identical despite different names*

### Comparing `openrank_sdk-0.0.2/PKG-INFO` & `openrank_sdk-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: openrank-sdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: SeungJu Lee
 Author-email: sj@karma3labs.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: urllib3 (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
-# Py-EigenTrust
+# OpenRank SDK
 
-Py-EigenTrust is a python wrapper for https://github.com/Karma3Labs/go-eigentrust
+## EigenTrust by OpenRank
+EigenTrust SDk is a python wrapper for https://github.com/Karma3Labs/go-eigentrust
 
 ### Input
 
 You will need *local trust* and optionally *pre-trust.*  If pre-trust is not specified, each peer will have an equal weight. Both can be specified
 using a CSV or an array of a dict with `i`, `j`, and `v`.
 
 Sample local trust dict variable
```

