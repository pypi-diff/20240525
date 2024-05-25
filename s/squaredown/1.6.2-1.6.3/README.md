# Comparing `tmp/squaredown-1.6.2.tar.gz` & `tmp/squaredown-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squaredown-1.6.2.tar", max compression
+gzip compressed data, was "squaredown-1.6.3.tar", max compression
```

## Comparing `squaredown-1.6.2.tar` & `squaredown-1.6.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1079 2024-05-25 17:35:11.660426 squaredown-1.6.2/LICENSE
--rw-r--r--   0        0        0     1405 2024-05-25 17:35:11.660426 squaredown-1.6.2/README.md
--rw-r--r--   0        0        0      911 2024-05-25 17:35:11.660426 squaredown-1.6.2/pyproject.toml
--rw-r--r--   0        0        0      259 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/__init__.py
--rw-r--r--   0        0        0     5629 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/catalog.py
--rw-r--r--   0        0        0     3128 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/connector.py
--rw-r--r--   0        0        0    13792 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/i_square.py
--rw-r--r--   0        0        0     4088 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/itemizations.py
--rw-r--r--   0        0        0     2244 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/locations.py
--rw-r--r--   0        0        0      987 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/logging_config.json
--rw-r--r--   0        0        0    16660 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/orders.py
--rw-r--r--   0        0        0     9373 2024-05-25 17:35:11.660426 squaredown-1.6.2/squaredown/payouts.py
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 squaredown-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-25 18:12:19.142140 squaredown-1.6.3/LICENSE
+-rw-r--r--   0        0        0     1405 2024-05-25 18:12:19.142140 squaredown-1.6.3/README.md
+-rw-r--r--   0        0        0      911 2024-05-25 18:12:19.142140 squaredown-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/__init__.py
+-rw-r--r--   0        0        0     5629 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/catalog.py
+-rw-r--r--   0        0        0     3128 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/connector.py
+-rw-r--r--   0        0        0    13792 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/i_square.py
+-rw-r--r--   0        0        0     4088 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/itemizations.py
+-rw-r--r--   0        0        0     2244 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/locations.py
+-rw-r--r--   0        0        0      987 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/logging_config.json
+-rw-r--r--   0        0        0    16660 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/orders.py
+-rw-r--r--   0        0        0     9563 2024-05-25 18:12:19.142140 squaredown-1.6.3/squaredown/payouts.py
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 squaredown-1.6.3/PKG-INFO
```

### Comparing `squaredown-1.6.2/LICENSE` & `squaredown-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/README.md` & `squaredown-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/pyproject.toml` & `squaredown-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squaredown"
-version = "1.6.2"
+version = "1.6.3"
 description = "Customized Square interface"
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/squaredown"
 keywords = ["python", "square", "mongodb"]
 packages = [{include = "squaredown"}]
```

### Comparing `squaredown-1.6.2/squaredown/catalog.py` & `squaredown-1.6.3/squaredown/catalog.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/squaredown/connector.py` & `squaredown-1.6.3/squaredown/connector.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/squaredown/i_square.py` & `squaredown-1.6.3/squaredown/i_square.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/squaredown/itemizations.py` & `squaredown-1.6.3/squaredown/itemizations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/squaredown/locations.py` & `squaredown-1.6.3/squaredown/locations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/squaredown/logging_config.json` & `squaredown-1.6.3/squaredown/logging_config.json`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/squaredown/orders.py` & `squaredown-1.6.3/squaredown/orders.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.6.2/squaredown/payouts.py` & `squaredown-1.6.3/squaredown/payouts.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,25 +88,28 @@
         """
         payouts = []
         start, end = self.timespan(collection='square_payouts', **kwargs)
         logger.debug('timespan: %s, %s', start, end)
 
         result = self.api_payouts.list_payouts(
             begin_time=start.isoformat(),
-            end_time=end.isoformat()
+            end_time=end.isoformat(),
+            sort_order='ASC'
         )
 
         if result.is_success():
             while result.body != {}:
                 payouts.extend(result.body['payouts'])
 
                 if result.cursor:
                     result = self.api_payouts.list_payouts(
                         begin_time=start.isoformat(),
-                        end_time=end.isoformat()
+                        end_time=end.isoformat(),
+                        sort_order='ASC',
+                        cursor=result.cursor
                     )
                 else:
                     break
 
         elif result.is_error():
             for error in result.errors:
                 logger.error(
@@ -223,24 +226,26 @@
 
         Returns:
             list: List of Square Payout Entries.
         """
         payout_entries = []
 
         result = self.api_payouts.list_payout_entries(
-            payout_id=payout_id
+            payout_id=payout_id,
+            sort_order='ASC'
         )
 
         if result.is_success():
             while result.body != {}:
                 payout_entries.extend(result.body['payout_entries'])
 
                 if result.cursor:
                     result = self.api_payouts.list_payout_entries(
                         payout_id=payout_id,
+                        sort_order='ASC',
                         cursor=result.cursor
                     )
                 else:
                     break
 
         elif result.is_error():
             for error in result.errors:
```

### Comparing `squaredown-1.6.2/PKG-INFO` & `squaredown-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squaredown
-Version: 1.6.2
+Version: 1.6.3
 Summary: Customized Square interface
 Home-page: https://github.com/aracnid/squaredown
 License: MIT
 Keywords: python,square,mongodb
 Author: Jason Romano
 Author-email: aracnid@gmail.com
 Requires-Python: >=3.10,<4.0
```

