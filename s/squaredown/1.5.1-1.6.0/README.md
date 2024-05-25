# Comparing `tmp/squaredown-1.5.1.tar.gz` & `tmp/squaredown-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squaredown-1.5.1.tar", max compression
+gzip compressed data, was "squaredown-1.6.0.tar", max compression
```

## Comparing `squaredown-1.5.1.tar` & `squaredown-1.6.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1079 2024-04-01 04:26:49.305738 squaredown-1.5.1/LICENSE
--rw-r--r--   0        0        0     1405 2024-04-01 04:26:49.305738 squaredown-1.5.1/README.md
--rw-r--r--   0        0        0      912 2024-04-01 04:26:49.305738 squaredown-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      259 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/__init__.py
--rw-r--r--   0        0        0     5629 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/catalog.py
--rw-r--r--   0        0        0     3128 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/connector.py
--rw-r--r--   0        0        0    12628 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/i_square.py
--rw-r--r--   0        0        0     4088 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/itemizations.py
--rw-r--r--   0        0        0     2244 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/locations.py
--rw-r--r--   0        0        0      987 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/logging_config.json
--rw-r--r--   0        0        0    16660 2024-04-01 04:26:49.305738 squaredown-1.5.1/squaredown/orders.py
--rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 squaredown-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-25 15:35:26.345613 squaredown-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1405 2024-05-25 15:35:26.345613 squaredown-1.6.0/README.md
+-rw-r--r--   0        0        0      911 2024-05-25 15:35:26.345613 squaredown-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/__init__.py
+-rw-r--r--   0        0        0     5629 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/catalog.py
+-rw-r--r--   0        0        0     3128 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/connector.py
+-rw-r--r--   0        0        0    13792 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/i_square.py
+-rw-r--r--   0        0        0     4088 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/itemizations.py
+-rw-r--r--   0        0        0     2244 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/locations.py
+-rw-r--r--   0        0        0      987 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/logging_config.json
+-rw-r--r--   0        0        0    16660 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/orders.py
+-rw-r--r--   0        0        0     9373 2024-05-25 15:35:26.345613 squaredown-1.6.0/squaredown/payouts.py
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 squaredown-1.6.0/PKG-INFO
```

### Comparing `squaredown-1.5.1/LICENSE` & `squaredown-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/README.md` & `squaredown-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/pyproject.toml` & `squaredown-1.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squaredown"
-version = "1.5.1"
+version = "1.6.0"
 description = "Customized Square interface"
 authors = ["Jason Romano <aracnid@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/aracnid/squaredown"
 keywords = ["python", "square", "mongodb"]
 packages = [{include = "squaredown"}]
@@ -15,15 +15,15 @@
 aracnid-logger = "^1.0"
 aracnid-utils = "^1.0"
 i-mongodb = "^2.0"
 squareup = "^19.1"
 tqdm = "^4.64"
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^2.15"
+pylint = "^3.0"
 pytest = "^7.2"
 pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `squaredown-1.5.1/squaredown/catalog.py` & `squaredown-1.6.0/squaredown/catalog.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/squaredown/connector.py` & `squaredown-1.6.0/squaredown/connector.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/squaredown/i_square.py` & `squaredown-1.6.0/squaredown/i_square.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,42 +39,120 @@
         )
 
         self.api_orders = self.square_client.orders
         self.api_payments = self.square_client.payments
         self.api_refunds = self.square_client.refunds
         self.api_catalog = self.square_client.catalog
         self.api_locations = self.square_client.locations
+        self.api_payouts = self.square_client.payouts
 
-    def decode_order(self, order):
-        """Decodes a Square Order into a python dictionary.
+    # region METHODS
+
+    @staticmethod
+    def decode_datetime(dt_str):
+        """Decodes a Square datetime string into a datetime object
+
+        The datetime.fromisoformat() class method does not handle "Z" timezone
+        notation, so the default_tzinfo() method is used instead.
+
+        Args:
+            dt_str: Datetime string to decode.
+        """
+        return utils.default_tzinfo(parse(dt_str), tz.tzlocal())
+
+    def search(self, obj_type, search_filter):
+        """Retrieves a list of filtered Square objects.
+
+        Args:
+            obj_type: Type of Square object to search, e.g., 'orders', 'items', etc.
+            search_filter: Search filter
+
+        Returns:
+            List of Square objects that meet the filter criteria.
+        """
+        obj_list = []
+
+        # get the api for the object
+        api_type = None
+        if obj_type == 'orders':
+            api_type = self.api_orders
+        elif obj_type == 'objects':
+            api_type = self.api_catalog
+
+        if not api_type:
+            return obj_list
+
+        loop_count = 0
+        result = self.search_fn(obj_type, search_filter)
+        if result.is_success():
+            loop_count += 1
+            obj_list = result.body.get(obj_type)
+
+            # process remaining pages
+            cursor = result.body['cursor'] if 'cursor' in result.body else None
+            while cursor:
+                search_filter['cursor'] = cursor
+                result = self.search_fn(obj_type, search_filter)
+
+                if result.is_success():
+                    loop_count += 1
+                    obj_list.extend(result.body[obj_type])
+                    cursor = result.body['cursor'] if 'cursor' in result.body else None
+                elif result.is_error():
+                    logger.error(f'Error calling Square Api ({obj_type}): {loop_count}')
+                    logger.error(result.errors)
+
+        elif result.is_error():
+            logger.error(f'Error calling Square Api ({obj_type}): loop {loop_count}')
+            logger.error(result.errors)
+
+        return obj_list
+
+    def search_fn(self, obj_type, search_filter):
+        """Executes the search function for the specified "obj_type".
+
+        Args:
+            obj_type: Type of Square object to search, e.g., 'orders', 'items', etc.
+            search_filter: Search filter
+
+        Returns:
+            Result of the search function.
+        """
+        if obj_type == 'orders':
+            return self.api_orders.search_orders(search_filter)
+        if obj_type == 'objects':
+            return self.api_catalog.search_catalog_objects(search_filter)
+
+        return None
+
+    # endregion
+
+    # region DECODE-FNS
+
+    def decode_catalog_obj(self, obj, collection):
+        """Decodes a Square Catalog object into a python dictionary.
 
         Square represents timestamps as RFC 3339 strings. This method decodes
         these strings into localized datetime objects.
 
         Args:
-            order: The Square Order object.
+            obj: The Square Catalog object.
+            collection: one of the following catalog names
+                'square_categories', 'square_items', 'square_variations',
+                'square_modifiers'
         """
-        if 'created_at' in order:
-            order['created_at'] = self.decode_datetime(
-                order['created_at'])
-        if 'updated_at' in order:
-            order['updated_at'] = self.decode_datetime(
-                order['updated_at'])
-        if 'closed_at' in order:
-            order['closed_at'] = self.decode_datetime(
-                order['closed_at'])
-        if 'fulfillments' in order:
-            for fulfillment in order['fulfillments']:
-                self.decode_fulfillment(fulfillment)
-        if 'tenders' in order:
-            for tender in order['tenders']:
-                self.decode_tender(tender)
-        if 'refunds' in order:
-            for refund in order['refunds']:
-                self.decode_refund(refund)
+        if 'updated_at' in obj:
+            obj['updated_at'] = self.decode_datetime(
+                obj['updated_at'])
+
+        if collection == 'square_items':
+            variations = obj['item_data']['variations']
+            for variation in variations:
+                variation['updated_at'] = self.decode_datetime(
+                    variation['updated_at'])
 
     def decode_fulfillment(self, fulfillment):
         """Decodes a Square OrderFulfillment into a python dictionary.
 
         Square represents timestamps as RFC 3339 strings. This method decodes
         these strings into localized datetime objects.
 
@@ -154,26 +232,54 @@
         if 'placed_at' in shipment_details:
             shipment_details['placed_at'] = self.decode_datetime(
                 shipment_details['placed_at'])
         if 'shipped_at' in shipment_details:
             shipment_details['shipped_at'] = self.decode_datetime(
                 shipment_details['shipped_at'])
 
-    def decode_tender(self, tender):
-        """Decodes a Square Tender into a python dictionary.
+    def decode_location(self, location):
+        """Decodes a Square Location into a python dictionary.
 
         Square represents timestamps as RFC 3339 strings. This method decodes
         these strings into localized datetime objects.
 
         Args:
-            tender: The Square Tender object.
+            location: The Square Location object.
         """
-        if 'created_at' in tender:
-            tender['created_at'] = self.decode_datetime(
-                tender['created_at'])
+        if 'created_at' in location:
+            location['created_at'] = self.decode_datetime(
+                location['created_at'])
+
+    def decode_order(self, order):
+        """Decodes a Square Order into a python dictionary.
+
+        Square represents timestamps as RFC 3339 strings. This method decodes
+        these strings into localized datetime objects.
+
+        Args:
+            order: The Square Order object.
+        """
+        if 'created_at' in order:
+            order['created_at'] = self.decode_datetime(
+                order['created_at'])
+        if 'updated_at' in order:
+            order['updated_at'] = self.decode_datetime(
+                order['updated_at'])
+        if 'closed_at' in order:
+            order['closed_at'] = self.decode_datetime(
+                order['closed_at'])
+        if 'fulfillments' in order:
+            for fulfillment in order['fulfillments']:
+                self.decode_fulfillment(fulfillment)
+        if 'tenders' in order:
+            for tender in order['tenders']:
+                self.decode_tender(tender)
+        if 'refunds' in order:
+            for refund in order['refunds']:
+                self.decode_refund(refund)
 
     def decode_payment(self, payment):
         """Decodes a Square Payment into a python dictionary.
 
         Square represents timestamps as RFC 3339 strings. This method decodes
         these strings into localized datetime objects.
 
@@ -191,14 +297,42 @@
                 if 'effective_at' in fee:
                     fee['effective_at'] = self.decode_datetime(
                         fee['effective_at'])
         if 'delayed_until' in payment:
             payment['delayed_until'] = self.decode_datetime(
                 payment['delayed_until'])
 
+    def decode_payout(self, payout):
+        """Decodes a Square Payout into a python dictionary.
+
+        Square represents timestamps as RFC 3339 strings. This method decodes
+        these strings into localized datetime objects.
+
+        Args:
+            payout: The Square payout object.
+        """
+        if 'created_at' in payout:
+            payout['created_at'] = self.decode_datetime(payout['created_at'])
+        if 'updated_at' in payout:
+            payout['updated_at'] = self.decode_datetime(payout['updated_at'])
+
+    def decode_payout_entry(self, payout_entry):
+        """Decodes a Square Payout into a python dictionary.
+
+        Square represents timestamps as RFC 3339 strings. This method decodes
+        these strings into localized datetime objects.
+
+        Args:
+            payout_entry: The Square payout_entry object.
+        """
+        if 'effective_at' in payout_entry:
+            payout_entry['effective_at'] = self.decode_datetime(
+                payout_entry['effective_at']
+            )
+
     def decode_refund(self, refund):
         """Decodes a Square PaymentRefund into a python dictionary.
 
         Square represents timestamps as RFC 3339 strings. This method decodes
         these strings into localized datetime objects.
 
         Args:
@@ -212,118 +346,21 @@
                 refund['updated_at'])
         if 'processing_fee' in refund:
             for fee in refund['processing_fee']:
                 if 'effective_at' in fee:
                     fee['effective_at'] = self.decode_datetime(
                         fee['effective_at'])
 
-    def decode_catalog_obj(self, obj, collection):
-        """Decodes a Square Catalog object into a python dictionary.
-
-        Square represents timestamps as RFC 3339 strings. This method decodes
-        these strings into localized datetime objects.
-
-        Args:
-            obj: The Square Catalog object.
-            collection: one of the following catalog names
-                'square_categories', 'square_items', 'square_variations',
-                'square_modifiers'
-        """
-        if 'updated_at' in obj:
-            obj['updated_at'] = self.decode_datetime(
-                obj['updated_at'])
-
-        if collection == 'square_items':
-            variations = obj['item_data']['variations']
-            for variation in variations:
-                variation['updated_at'] = self.decode_datetime(
-                    variation['updated_at'])
-
-    def decode_location(self, location):
-        """Decodes a Square Location into a python dictionary.
+    def decode_tender(self, tender):
+        """Decodes a Square Tender into a python dictionary.
 
         Square represents timestamps as RFC 3339 strings. This method decodes
         these strings into localized datetime objects.
 
         Args:
-            location: The Square Location object.
-        """
-        if 'created_at' in location:
-            location['created_at'] = self.decode_datetime(
-                location['created_at'])
-
-    @staticmethod
-    def decode_datetime(dt_str):
-        """Decodes a Square datetime string into a datetime object
-
-        The datetime.fromisoformat() class method does not handle "Z" timezone
-        notation, so the default_tzinfo() method is used instead.
-
-        Args:
-            dt_str: Datetime string to decode.
-        """
-        return utils.default_tzinfo(parse(dt_str), tz.tzlocal())
-
-    def search(self, obj_type, search_filter):
-        """Retrieves a list of filtered Square objects.
-
-        Args:
-            obj_type: Type of Square object to search, e.g., 'orders', 'items', etc.
-            search_filter: Search filter
-
-        Returns:
-            List of Square objects that meet the filter criteria.
-        """
-        obj_list = []
-
-        # get the api for the object
-        api_type = None
-        if obj_type == 'orders':
-            api_type = self.api_orders
-        elif obj_type == 'objects':
-            api_type = self.api_catalog
-
-        if not api_type:
-            return obj_list
-
-        loop_count = 0
-        result = self.search_fn(obj_type, search_filter)
-        if result.is_success():
-            loop_count += 1
-            obj_list = result.body.get(obj_type)
-
-            # process remaining pages
-            cursor = result.body['cursor'] if 'cursor' in result.body else None
-            while cursor:
-                search_filter['cursor'] = cursor
-                result = self.search_fn(obj_type, search_filter)
-
-                if result.is_success():
-                    loop_count += 1
-                    obj_list.extend(result.body[obj_type])
-                    cursor = result.body['cursor'] if 'cursor' in result.body else None
-                elif result.is_error():
-                    logger.error(f'Error calling Square Api ({obj_type}): {loop_count}')
-                    logger.error(result.errors)
-
-        elif result.is_error():
-            logger.error(f'Error calling Square Api ({obj_type}): loop {loop_count}')
-            logger.error(result.errors)
-
-        return obj_list
-
-    def search_fn(self, obj_type, search_filter):
-        """Executes the search function for the specified "obj_type".
-
-        Args:
-            obj_type: Type of Square object to search, e.g., 'orders', 'items', etc.
-            search_filter: Search filter
-
-        Returns:
-            Result of the search function.
+            tender: The Square Tender object.
         """
-        if obj_type == 'orders':
-            return self.api_orders.search_orders(search_filter)
-        if obj_type == 'objects':
-            return self.api_catalog.search_catalog_objects(search_filter)
+        if 'created_at' in tender:
+            tender['created_at'] = self.decode_datetime(
+                tender['created_at'])
 
-        return None
+    # endregion
```

### Comparing `squaredown-1.5.1/squaredown/itemizations.py` & `squaredown-1.6.0/squaredown/itemizations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/squaredown/locations.py` & `squaredown-1.6.0/squaredown/locations.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/squaredown/logging_config.json` & `squaredown-1.6.0/squaredown/logging_config.json`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/squaredown/orders.py` & `squaredown-1.6.0/squaredown/orders.py`

 * *Files identical despite different names*

### Comparing `squaredown-1.5.1/PKG-INFO` & `squaredown-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squaredown
-Version: 1.5.1
+Version: 1.6.0
 Summary: Customized Square interface
 Home-page: https://github.com/aracnid/squaredown
 License: MIT
 Keywords: python,square,mongodb
 Author: Jason Romano
 Author-email: aracnid@gmail.com
 Requires-Python: >=3.10,<4.0
```

