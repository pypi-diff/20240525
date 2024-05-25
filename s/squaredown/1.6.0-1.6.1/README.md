# Comparing `tmp/squaredown-1.6.0.tar.gz` & `tmp/squaredown-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squaredown-1.6.0.tar", max compression
+gzip compressed data, was "squaredown-1.6.1.tar", max compression
```

## Comparing `squaredown-1.6.0.tar` & `squaredown-1.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1079 2024-05-25 15:35:26.345613 squaredown-1.6.0/LICENSE
--rw-r--r--   0        0        0     1405 2024-05-25 15:35:26.345613 squaredown-1.6.0/README.md
--rw-r--r--   0        0        0      911 2024-05-25 15:35:26.345613 squaredown-1.6.0/pyproject.toml
--rw-r--r--   0        0        0      259 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/__init__.py
--rw-r--r--   0        0        0     5629 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/catalog.py
--rw-r--r--   0        0        0     3128 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/connector.py
--rw-r--r--   0        0        0    13792 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/i_square.py
--rw-r--r--   0        0        0     4088 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/itemizations.py
--rw-r--r--   0        0        0     2244 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/locations.py
--rw-r--r--   0        0        0      987 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/logging_config.json
--rw-r--r--   0        0        0    16660 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/orders.py
--rw-r--r--   0        0        0     9373 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/payouts.py
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 squaredown-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-25 17:25:23.197545 squaredown-1.6.1/LICENSE
+-rw-r--r--   0        0        0     1405 2024-05-25 17:25:23.197545 squaredown-1.6.1/README.md
+-rw-r--r--   0        0        0      911 2024-05-25 17:25:23.197545 squaredown-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/__init__.py
+-rw-r--r--   0        0        0     5629 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/catalog.py
+-rw-r--r--   0        0        0     3128 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/connector.py
+-rw-r--r--   0        0        0    13792 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/i_square.py
+-rw-r--r--   0        0        0     4088 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/itemizations.py
+-rw-r--r--   0        0        0     2244 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/locations.py
+-rw-r--r--   0        0        0      987 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/logging_config.json
+-rw-r--r--   0        0        0    16660 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/orders.py
+-rw-r--r--   0        0        0     9373 2024-05-25 17:25:23.197545 squaredown-1.6.1/squaredown/payouts.py
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 squaredown-1.6.1/PKG-INFO
```

### Comparing `squaredown-1.6.0/LICENSE` & `squaredown-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/README.md` & `squaredown-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/pyproject.toml` & `squaredown-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squaredown"
-version = "1.6.0"
+version = "1.6.1"
 description = "Customized Square interface"
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/squaredown"
 keywords = ["python", "square", "mongodb"]
 packages = [{include = "squaredown"}]
```

### Comparing `squaredown-1.6.0/squaredown/catalog.py` & `squaredown-1.6.1/squaredown/catalog.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/squaredown/connector.py` & `squaredown-1.6.1/squaredown/connector.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/squaredown/i_square.py` & `squaredown-1.6.1/squaredown/i_square.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/squaredown/itemizations.py` & `squaredown-1.6.1/squaredown/itemizations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/squaredown/locations.py` & `squaredown-1.6.1/squaredown/locations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/squaredown/logging_config.json` & `squaredown-1.6.1/squaredown/logging_config.json`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/squaredown/orders.py` & `squaredown-1.6.1/squaredown/orders.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/squaredown/payouts.py` & `squaredown-1.6.1/squaredown/payouts.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.0/PKG-INFO` & `squaredown-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squaredown
-Version: 1.6.0
+Version: 1.6.1
 Summary: Customized Square interface
 Home-page: https://github.com/aracnid/squaredown
 License: MIT
 Keywords: python,square,mongodb
 Author: Jason Romano
 Author-email: aracnid@gmail.com
 Requires-Python: >=3.10,<4.0
```

