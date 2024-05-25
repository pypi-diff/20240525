# Comparing `tmp/schwab-py-0.0.0a9.tar.gz` & `tmp/schwab_py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-py-0.0.0a9.tar", last modified: Sun Apr 14 18:49:14 2024, max compression
+gzip compressed data, was "schwab_py-1.0.0.tar", last modified: Sat May 25 12:26:01 2024, max compression
```

## Comparing `schwab-py-0.0.0a9.tar` & `schwab_py-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,61 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.268338 schwab-py-0.0.0a9/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-03-26 01:18:54.000000 schwab-py-0.0.0a9/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:49:14.268278 schwab-py-0.0.0a9/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     2075 2024-03-26 01:18:54.000000 schwab-py-0.0.0a9/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.265801 schwab-py-0.0.0a9/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)      211 2024-04-03 01:16:43.000000 schwab-py-0.0.0a9/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    24395 2024-04-08 21:07:33.000000 schwab-py-0.0.0a9/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.266307 schwab-py-0.0.0a9/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-04-01 12:04:09.000000 schwab-py-0.0.0a9/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2603 2024-04-03 01:45:43.000000 schwab-py-0.0.0a9/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    34237 2024-04-14 18:48:14.000000 schwab-py-0.0.0a9/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     2458 2024-04-06 13:43:58.000000 schwab-py-0.0.0a9/schwab/client/synchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5482 2024-04-03 01:18:33.000000 schwab-py-0.0.0a9/schwab/debug.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.266969 schwab-py-0.0.0a9/schwab/orders/
--rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-04-06 23:27:37.000000 schwab-py-0.0.0a9/schwab/orders/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    11013 2024-04-14 17:35:12.000000 schwab-py-0.0.0a9/schwab/orders/common.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-04-14 17:35:34.000000 schwab-py-0.0.0a9/schwab/orders/equities.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    14184 2024-04-14 17:37:24.000000 schwab-py-0.0.0a9/schwab/orders/generic.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    17394 2024-04-14 17:35:49.000000 schwab-py-0.0.0a9/schwab/orders/options.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5097 2024-04-01 12:04:09.000000 schwab-py-0.0.0a9/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       20 2024-04-14 18:48:56.000000 schwab-py-0.0.0a9/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.267805 schwab-py-0.0.0a9/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     3518 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)      532 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      129 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        7 2024-04-14 18:49:14.000000 schwab-py-0.0.0a9/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-04-14 18:49:14.268654 schwab-py-0.0.0a9/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1814 2024-04-06 13:16:58.000000 schwab-py-0.0.0a9/setup.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-04-14 18:49:14.267657 schwab-py-0.0.0a9/tests/
--rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-04-02 12:25:54.000000 schwab-py-0.0.0a9/tests/test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.532307 schwab_py-1.0.0/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-05-17 12:00:12.000000 schwab_py-1.0.0/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     7267 2024-05-25 12:26:01.532221 schwab_py-1.0.0/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5750 2024-05-17 12:00:12.000000 schwab_py-1.0.0/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.521681 schwab_py-1.0.0/bin/
+-rwxr-xr-x   0 alexgolec   (501) staff       (20)      171 2024-05-17 12:00:12.000000 schwab_py-1.0.0/bin/schwab-order-codegen.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.523699 schwab_py-1.0.0/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      229 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14218 2024-05-25 12:21:55.000000 schwab_py-1.0.0/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.524263 schwab_py-1.0.0/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1942 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    44924 2024-05-25 12:21:55.000000 schwab_py-1.0.0/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1809 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/client/synchronous.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.524821 schwab_py-1.0.0/schwab/contrib/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/contrib/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     9608 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/contrib/orders.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      885 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/contrib/util.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4919 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/debug.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.525888 schwab_py-1.0.0/schwab/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    11019 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/common.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/equities.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14407 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/generic.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17650 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/options.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.526314 schwab_py-1.0.0/schwab/scripts/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/scripts/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4155 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/scripts/orders_codegen.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    52329 2024-05-22 03:52:54.000000 schwab_py-1.0.0/schwab/streaming.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5149 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       18 2024-05-25 12:23:35.000000 schwab_py-1.0.0/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.531543 schwab_py-1.0.0/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     7267 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1129 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      152 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)       13 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-05-25 12:26:01.532569 schwab_py-1.0.0/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1904 2024-05-17 12:00:12.000000 schwab_py-1.0.0/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.529487 schwab_py-1.0.0/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17156 2024-05-25 12:21:55.000000 schwab_py-1.0.0/tests/auth_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    85571 2024-05-25 12:21:55.000000 schwab_py-1.0.0/tests/client_test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.529990 schwab_py-1.0.0/tests/contrib/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/contrib/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    30599 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/contrib/orders_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      413 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/contrib/util_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5320 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/debug_test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.531024 schwab_py-1.0.0/tests/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      989 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/common_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    41836 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/generic_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17525 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/options_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4624 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders_test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.531304 schwab_py-1.0.0/tests/scripts/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/scripts/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    16623 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/scripts/orders_codegen_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)   200493 2024-05-22 03:52:54.000000 schwab_py-1.0.0/tests/streaming_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     6591 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3300 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/utils_test.py
```

### Comparing `schwab-py-0.0.0a9/LICENSE` & `schwab_py-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a9/schwab/client/asynchronous.py` & `schwab_py-1.0.0/schwab/client/asynchronous.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,72 +10,50 @@
 
 class AsyncClient(BaseClient):
 
     async def close_async_session(self):
         await self.session.aclose()
 
     async def _get_request(self, path, params):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: GET to %s, params=%s',
                 req_num, dest, LazyLog(lambda: json.dumps(params, indent=4)))
 
         resp = await self.session.get(dest, params=params)
         self._log_response(resp, req_num)
         register_redactions_from_response(resp)
         return resp
 
     async def _post_request(self, path, data):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: POST to %s, json=%s',
                 req_num, dest, LazyLog(lambda: json.dumps(data, indent=4)))
 
         resp = await self.session.post(dest, json=data)
         self._log_response(resp, req_num)
         register_redactions_from_response(resp)
         return resp
 
     async def _put_request(self, path, data):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: PUT to %s, json=%s',
                 req_num, dest, LazyLog(lambda: json.dumps(data, indent=4)))
 
         resp = await self.session.put(dest, json=data)
         self._log_response(resp, req_num)
         register_redactions_from_response(resp)
         return resp
 
-    async def _patch_request(self, path, data):
-        self.ensure_updated_refresh_token()
-
-        dest = 'https://api.schwabapi.com' + path
-
-        req_num = self._req_num()
-        self.logger.debug('Req %s: PATCH to %s, json=%s',
-                req_num, dest, LazyLog(lambda: json.dumps(data, indent=4)))
-
-        resp = await self.session.patch(dest, json=data)
-        self._log_response(resp, req_num)
-        register_redactions_from_response(resp)
-        return resp
-
     async def _delete_request(self, path):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: DELETE to %s', req_num, dest)
 
         resp = await self.session.delete(dest)
         self._log_response(resp, req_num)
```

### Comparing `schwab-py-0.0.0a9/schwab/client/base.py` & `schwab_py-1.0.0/schwab/client/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import json
 import logging
 import pickle
 import schwab
 import time
 import warnings
 
+from schwab.orders.generic import OrderBuilder
+
 from ..utils import EnumEnforcer
 
 
 def get_logger():
     return logging.getLogger(__name__)
 
 
@@ -76,61 +78,58 @@
                 error_str = "expected type '{}' for {}, got '{}'".format(
                     exp_type_names[0], name, value_type_name)
             else:
                 error_str = "expected type in ({}) for {}, got '{}'".format(
                     ', '.join(exp_type_names), name, value_type_name)
             raise ValueError(error_str)
 
-    def _format_datetime(self, var_name, dt):
-        '''Formats datetime objects appropriately, depending on whether they are
-        naive or timezone-aware'''
-        self._assert_type(var_name, dt, [self._DATETIME])
+    def _format_date_as_iso(self, var_name, dt):
+        '''Formats datetime or date objects as yyyy-MM-dd'T'HH:mm:ss.SSSZ'''
+        self._assert_type(var_name, dt, [self._DATE, self._DATETIME])
+
+        if not isinstance(dt, self._DATETIME):
+            dt = datetime.datetime(year=dt.year, month=dt.month, day=dt.day)
 
         return dt.strftime('%Y-%m-%dT%H:%M:%SZ')
 
-    def _format_date(self, var_name, dt):
-        '''Formats datetime objects appropriately, depending on whether they are
-        naive or timezone-aware'''
-        self._assert_type(var_name, dt, [self._DATE, self._DATETIME])
+    def _format_date_as_day(self, var_name, dt):
+        '''Formats datetime or date objects as YYYY-MM-DD'''
+        self._assert_type(var_name, dt, [self._DATE])
 
-        d = datetime.date(year=dt.year, month=dt.month, day=dt.day)
+        return dt.strftime('%Y-%m-%d')
 
-        return d.isoformat()
 
-    def _datetime_as_millis(self, var_name, dt):
+    def _format_date_as_millis(self, var_name, dt):
         'Converts datetime objects to compatible millisecond values'
         self._assert_type(var_name, dt, [self._DATETIME])
 
         return int(dt.timestamp() * 1000)
 
-    def ensure_updated_refresh_token(self, update_interval_seconds=None):
-        '''
-        The client automatically performs a token refresh
-        '''
-        if not self.token_metadata:
-            return None
-
-        new_session = self.token_metadata.ensure_refresh_token_update(
-            self.api_key, self.session, update_interval_seconds)
-        if new_session:
-            self.session = new_session
-
-        return new_session is not None
 
     def set_timeout(self, timeout):
         '''Sets the timeout configuration for this client. Applies to all HTTP 
         calls.
 
         :param timeout: ``httpx`` timeout configuration. Passed directly to 
                         underlying ``httpx`` library. See
                         `here <https://www.python-httpx.org/advanced/
                         #setting-a-default-timeout-on-a-client>`__ for
                         examples.'''
         self.session.timeout = timeout
 
+    def token_age(self):
+        '''Get the age of the token used to create this client, in seconds. For 
+        users who prefer to proactively delete their token files before the 
+        become expired, this method can offer a hint for when to do so.
+
+        Note that the actual expiration is governed by Schwab's internal 
+        implementation, and the token might become expired sooner *or* later 
+        than the documented seven day term.'''
+        return self.token_metadata.token_age()
+
 
     ##########################################################################
     # Accounts
 
     class Account:
         class Fields(Enum):
             '''Account fields passed to :meth:`get_account` and
@@ -176,329 +175,26 @@
             params['fields'] = ','.join(fields)
 
         path = '/trader/v1/accounts'
         return self._get_request(path, params)
 
 
     ##########################################################################
-    # Price History
-
-    class PriceHistory:
-        class PeriodType(Enum):
-            DAY = 'day'
-            MONTH = 'month'
-            YEAR = 'year'
-            YEAR_TO_DATE = 'ytd'
-
-        class Period(Enum):
-            # Daily
-            ONE_DAY = 1
-            TWO_DAYS = 2
-            THREE_DAYS = 3
-            FOUR_DAYS = 4
-            FIVE_DAYS = 5
-            TEN_DAYS = 10
-
-            # Monthly
-            ONE_MONTH = 1
-            TWO_MONTHS = 2
-            THREE_MONTHS = 3
-            SIX_MONTHS = 6
-
-            # Year
-            ONE_YEAR = 1
-            TWO_YEARS = 2
-            THREE_YEARS = 3
-            FIVE_YEARS = 5
-            TEN_YEARS = 10
-            FIFTEEN_YEARS = 15
-            TWENTY_YEARS = 20
-
-            # Year to date
-            YEAR_TO_DATE = 1
-
-        class FrequencyType(Enum):
-            MINUTE = 'minute'
-            DAILY = 'daily'
-            WEEKLY = 'weekly'
-            MONTHLY = 'monthly'
-
-        class Frequency(Enum):
-            # Minute
-            EVERY_MINUTE = 1
-            EVERY_FIVE_MINUTES = 5
-            EVERY_TEN_MINUTES = 10
-            EVERY_FIFTEEN_MINUTES = 15
-            EVERY_THIRTY_MINUTES = 30
-
-            # Other frequencies
-            DAILY = 1
-            WEEKLY = 1
-            MONTHLY = 1
-
-    def get_price_history(
-            self,
-            symbol,
-            *,
-            period_type=None,
-            period=None,
-            frequency_type=None,
-            frequency=None,
-            start_datetime=None,
-            end_datetime=None,
-            need_extended_hours_data=None,
-            need_previous_close=None):
-        '''Get price history for a symbol.
-
-        :param period_type: The type of period to show.
-        :param period: The number of periods to show. Should not be provided if
-                       ``start_datetime`` and ``end_datetime``.
-        :param frequency_type: The type of frequency with which a new candle
-                               is formed.
-        :param frequency: The number of the frequencyType to be included in each
-                          candle.
-        :param start_datetime: Start date.
-        :param end_datetime: End date. Default is previous trading day.
-        :param need_extended_hours_data: If true, return extended hours data.
-                                         Default is true.
-        :param need_previous_close: If true, return the previous close price and 
-                                    date.
-        '''
-        period_type = self.convert_enum(
-            period_type, self.PriceHistory.PeriodType)
-        period = self.convert_enum(period, self.PriceHistory.Period)
-        frequency_type = self.convert_enum(
-            frequency_type, self.PriceHistory.FrequencyType)
-        frequency = self.convert_enum(
-            frequency, self.PriceHistory.Frequency)
-
-        params = {
-                'symbol': symbol,
-        }
-
-        if period_type is not None:
-            params['periodType'] = period_type
-        if period is not None:
-            params['period'] = period
-        if frequency_type is not None:
-            params['frequencyType'] = frequency_type
-        if frequency is not None:
-            params['frequency'] = frequency
-        if start_datetime is not None:
-            params['startDate'] = self._datetime_as_millis(
-                'start_datetime', start_datetime)
-        if end_datetime is not None:
-            params['endDate'] = self._datetime_as_millis(
-                'end_datetime', end_datetime)
-        if need_extended_hours_data is not None:
-            params['needExtendedHoursData'] = need_extended_hours_data
-        if need_previous_close is not None:
-            params['needPreviousClose'] = need_previous_close
-
-        path = '/marketdata/v1/pricehistory'.format(symbol)
-        return self._get_request(path, params)
-
-
-    ##########################################################################
-    # Price history utilities
-
-
-    def __normalize_start_and_end_datetimes(self, start_datetime, end_datetime):
-        if start_datetime is None:
-            start_datetime = datetime.datetime(year=1971, month=1, day=1)
-        if end_datetime is None:
-            end_datetime = (datetime.datetime.utcnow() +
-                    datetime.timedelta(days=7))
-
-        return start_datetime, end_datetime
-
-
-    def get_price_history_every_minute(
-            self, symbol, *, start_datetime=None, end_datetime=None, 
-            need_extended_hours_data=None, need_previous_close=None):
-        '''
-        Fetch price history for a stock or ETF symbol at a per-minute
-        granularity. This endpoint currently appears to return up to 48 days of
-        data.
-        '''
-
-        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
-                start_datetime, end_datetime)
-
-        return self.get_price_history(
-                symbol,
-                period_type=self.PriceHistory.PeriodType.DAY,
-                period=self.PriceHistory.Period.ONE_DAY,
-                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
-                frequency=self.PriceHistory.Frequency.EVERY_MINUTE,
-                start_datetime=start_datetime,
-                end_datetime=end_datetime,
-                need_extended_hours_data=need_extended_hours_data, 
-                need_previous_close=need_previous_close)
-
-
-    def get_price_history_every_five_minutes(
-            self, symbol, *, start_datetime=None, end_datetime=None, 
-            need_extended_hours_data=None, need_previous_close=None):
-        '''
-        Fetch price history for a stock or ETF symbol at a per-five-minutes
-        granularity. This endpoint currently appears to return approximately
-        nine months of data.
-        '''
-
-        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
-                start_datetime, end_datetime)
-
-        return self.get_price_history(
-                symbol,
-                period_type=self.PriceHistory.PeriodType.DAY,
-                period=self.PriceHistory.Period.ONE_DAY,
-                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
-                frequency=self.PriceHistory.Frequency.EVERY_FIVE_MINUTES,
-                start_datetime=start_datetime,
-                end_datetime=end_datetime,
-                need_extended_hours_data=need_extended_hours_data, 
-                need_previous_close=need_previous_close)
-
-
-    def get_price_history_every_ten_minutes(
-            self, symbol, *, start_datetime=None, end_datetime=None, 
-            need_extended_hours_data=None, need_previous_close=None):
-        '''
-        Fetch price history for a stock or ETF symbol at a per-ten-minutes
-        granularity. This endpoint currently appears to return approximately
-        nine months of data.
-        '''
-
-        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
-                start_datetime, end_datetime)
-
-        return self.get_price_history(
-                symbol,
-                period_type=self.PriceHistory.PeriodType.DAY,
-                period=self.PriceHistory.Period.ONE_DAY,
-                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
-                frequency=self.PriceHistory.Frequency.EVERY_TEN_MINUTES,
-                start_datetime=start_datetime,
-                end_datetime=end_datetime,
-                need_extended_hours_data=need_extended_hours_data, 
-                need_previous_close=need_previous_close)
-
-
-    def get_price_history_every_fifteen_minutes(
-            self, symbol, *, start_datetime=None, end_datetime=None, 
-            need_extended_hours_data=None, need_previous_close=None):
-        '''
-        Fetch price history for a stock or ETF symbol at a per-fifteen-minutes
-        granularity. This endpoint currently appears to return approximately
-        nine months of data.
-        '''
-
-        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
-                start_datetime, end_datetime)
-
-        return self.get_price_history(
-                symbol,
-                period_type=self.PriceHistory.PeriodType.DAY,
-                period=self.PriceHistory.Period.ONE_DAY,
-                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
-                frequency=self.PriceHistory.Frequency.EVERY_FIFTEEN_MINUTES,
-                start_datetime=start_datetime,
-                end_datetime=end_datetime,
-                need_extended_hours_data=need_extended_hours_data, 
-                need_previous_close=need_previous_close)
-
-
-    def get_price_history_every_thirty_minutes(
-            self, symbol, *, start_datetime=None, end_datetime=None, 
-            need_extended_hours_data=None, need_previous_close=None):
-        '''
-        Fetch price history for a stock or ETF symbol at a per-thirty-minutes
-        granularity. This endpoint currently appears to return approximately
-        nine months of data.
-        '''
-
-        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
-                start_datetime, end_datetime)
-
-        return self.get_price_history(
-                symbol,
-                period_type=self.PriceHistory.PeriodType.DAY,
-                period=self.PriceHistory.Period.ONE_DAY,
-                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
-                frequency=self.PriceHistory.Frequency.EVERY_THIRTY_MINUTES,
-                start_datetime=start_datetime,
-                end_datetime=end_datetime,
-                need_extended_hours_data=need_extended_hours_data, 
-                need_previous_close=need_previous_close)
-
-
-    def get_price_history_every_day(
-            self, symbol, *, start_datetime=None, end_datetime=None, 
-            need_extended_hours_data=None, need_previous_close=None):
-        '''
-        Fetch price history for a stock or ETF symbol at a daily granularity. 
-        The exact period of time over which this endpoint returns data is 
-        unclear, although it has been observed returning data as far back as 
-        1985 (for ``AAPL``).
-        '''
-
-        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
-                start_datetime, end_datetime)
-
-        return self.get_price_history(
-                symbol,
-                period_type=self.PriceHistory.PeriodType.YEAR,
-                period=self.PriceHistory.Period.TWENTY_YEARS,
-                frequency_type=self.PriceHistory.FrequencyType.DAILY,
-                frequency=self.PriceHistory.Frequency.EVERY_MINUTE,
-                start_datetime=start_datetime,
-                end_datetime=end_datetime,
-                need_extended_hours_data=need_extended_hours_data, 
-                need_previous_close=need_previous_close)
-
-
-    def get_price_history_every_week(
-            self, symbol, *, start_datetime=None, end_datetime=None, 
-            need_extended_hours_data=None, need_previous_close=None):
-        '''
-        Fetch price history for a stock or ETF symbol at a weekly granularity.
-        The exact period of time over which this endpoint returns data is 
-        unclear, although it has been observed returning data as far back as 
-        1985 (for ``AAPL``).
-        '''
-
-        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
-                start_datetime, end_datetime)
-
-        return self.get_price_history(
-                symbol,
-                period_type=self.PriceHistory.PeriodType.YEAR,
-                period=self.PriceHistory.Period.TWENTY_YEARS,
-                frequency_type=self.PriceHistory.FrequencyType.WEEKLY,
-                frequency=self.PriceHistory.Frequency.EVERY_MINUTE,
-                start_datetime=start_datetime,
-                end_datetime=end_datetime,
-                need_extended_hours_data=need_extended_hours_data, 
-                need_previous_close=need_previous_close)
-
-
-    ##########################################################################
     # Orders
 
-    def cancel_order(self, order_id, account_hash):
-        '''Cancel a specific order for a specific account'''
-        path = '/trader/v1/accounts/{}/orders/{}'.format(account_hash, order_id)
-        return self._delete_request(path)
-
     def get_order(self, order_id, account_hash):
         '''Get a specific order for a specific account by its order ID'''
         path = '/trader/v1/accounts/{}/orders/{}'.format(account_hash, order_id)
         return self._get_request(path, {})
 
+    def cancel_order(self, order_id, account_hash):
+        '''Cancel a specific order for a specific account'''
+        path = '/trader/v1/accounts/{}/orders/{}'.format(account_hash, order_id)
+        return self._delete_request(path)
+
     class Order:
         class Status(Enum):
             '''Order statuses passed to :meth:`get_orders_for_account` and
             :meth:`get_orders_for_all_linked_accounts`'''
             AWAITING_PARENT_ORDER = 'AWAITING_PARENT_ORDER'
             AWAITING_CONDITION = 'AWAITING_CONDITION'
             AWAITING_MANUAL_REVIEW = 'AWAITING_MANUAL_REVIEW'
@@ -520,23 +216,24 @@
                           max_results=None,
                           from_entered_datetime=None,
                           to_entered_datetime=None,
                           status=None):
         status = self.convert_enum(status, self.Order.Status)
 
         if from_entered_datetime is None:
-            from_entered_datetime = datetime.datetime(
-                year=2024, month=4, day=1)
+            from_entered_datetime = (
+                    datetime.datetime.now(datetime.timezone.utc) -
+                    datetime.timedelta(days=60))
         if to_entered_datetime is None:
-            to_entered_datetime = datetime.datetime.utcnow()
+            to_entered_datetime = datetime.datetime.now(datetime.timezone.utc)
 
         params = {
-            'fromEnteredTime': self._format_datetime(
+            'fromEnteredTime': self._format_date_as_iso(
                 'from_entered_datetime', from_entered_datetime),
-            'toEnteredTime': self._format_datetime(
+            'toEnteredTime': self._format_date_as_iso(
                 'to_entered_datetime', to_entered_datetime),
         }
 
         if max_results:
             params['maxResults'] = max_results
 
         if status:
@@ -575,16 +272,15 @@
             status=status))
 
     def get_orders_for_all_linked_accounts(self,
                                            *,
                                            max_results=None,
                                            from_entered_datetime=None,
                                            to_entered_datetime=None,
-                                           status=None,
-                                           statuses=None):
+                                           status=None):
         '''Orders for all linked accounts. Optionally specify a single status on 
         which to filter.
 
         :param max_results: The maximum number of orders to retrieve.
         :param from_entered_datetime: Specifies that no orders entered before
                                       this time should be returned. Date must
                                       be within 60 days from today's date.
@@ -608,15 +304,15 @@
         :meth:`schwab.utils.Utils.extract_order_id` for more details. Note unlike
         most methods in this library, responses for successful calls to this
         method typically do not contain ``json()`` data, and attempting to
         extract it will likely result in an exception.'''
         if isinstance(order_spec, OrderBuilder):
             order_spec = order_spec.build()
 
-        path = '/v1/trader/accounts/{}/orders'.format(account_hash)
+        path = '/trader/v1/accounts/{}/orders'.format(account_hash)
         return self._post_request(path, order_spec)
 
     def replace_order(self, account_hash, order_id, order_spec):
         '''Replace an existing order for an account. The existing order will be
         replaced by the new order. Once replaced, the old order will be canceled
         and a new order will be created.'''
         if isinstance(order_spec, OrderBuilder):
@@ -627,22 +323,128 @@
 
     def preview_order(self, account_hash, order_spec):
         '''Preview an order, i.e. test whether an order would be accepted by the 
         API and see the structure it would result in.'''
         if isinstance(order_spec, OrderBuilder):
             order_spec = order_spec.build()
 
-        path = '/v1/trader/accounts/{}/previewOrder'.format(account_hash)
+        path = '/trader/v1/accounts/{}/previewOrder'.format(account_hash)
         return self._post_request(path, order_spec)
 
 
     ##########################################################################
+    # Transaction History
+
+    class Transactions:
+        class TransactionType(Enum):
+            TRADE = 'TRADE'
+            RECEIVE_AND_DELIVER = 'RECEIVE_AND_DELIVER'
+            DIVIDEND_OR_INTEREST = 'DIVIDEND_OR_INTEREST'
+            ACH_RECEIPT = 'ACH_RECEIPT'
+            ACH_DISBURSEMENT = 'ACH_DISBURSEMENT'
+            CASH_RECEIPT = 'CASH_RECEIPT'
+            CASH_DISBURSEMENT = 'CASH_DISBURSEMENT'
+            ELECTRONIC_FUND = 'ELECTRONIC_FUND'
+            WIRE_OUT = 'WIRE_OUT'
+            WIRE_IN = 'WIRE_IN'
+            JOURNAL = 'JOURNAL'
+            MEMORANDUM = 'MEMORANDUM'
+            MARGIN_CALL = 'MARGIN_CALL'
+            MONEY_MARKET = 'MONEY_MARKET'
+            SMA_ADJUSTMENT = 'SMA_ADJUSTMENT'
+
+    def get_transactions(
+            self,
+            account_hash,
+            *,
+            start_date=None,
+            end_date=None,
+            transaction_types=None,
+            symbol=None):
+        '''Transaction for a specific account.
+
+        :param account_hash: Account hash corresponding to the account whose 
+                             transactions should be returned.
+        :param start_date: Only transactions after this date will be returned.
+                           Date must be within 60 days of the current date. If 
+                           this parameter is not set, it will be set to 60 days 
+                           prior to now.
+                           Accepts ``datetime.date`` and ``datetime.datetime``.
+        :param end_date: Only transactions before this date will be returned. If 
+                         this parameter is not set, it will be set to the 
+                         current time.
+                         Accepts ``datetime.date`` and ``datetime.datetime``.
+        :param transaction_types: Only transactions with one of the specified 
+                                  types will be returned.
+        :param symbol: Only transactions with the specified symbol will be
+                        returned.
+        '''
+        # Transaction types
+        if transaction_types is None:
+            transaction_types = [
+                    t.value for t in self.Transactions.TransactionType]
+        else:
+            transaction_types = self.convert_enum_iterable(
+                transaction_types, self.Transactions.TransactionType)
+
+        # Start date
+        if start_date is None:
+            start_date = self._format_date_as_iso(
+                    'start_date',
+                    datetime.datetime.now(datetime.timezone.utc)
+                    - datetime.timedelta(days=60))
+        else:
+            start_date = self._format_date_as_iso('start_date', start_date)
+
+        # End date
+        if end_date is None:
+            end_date = self._format_date_as_iso(
+                    'end_date', datetime.datetime.now(datetime.timezone.utc))
+        else:
+            end_date = self._format_date_as_iso('end_date', end_date)
+
+        params = {
+                'types':  ','.join(transaction_types),
+                'startDate': start_date,
+                'endDate': end_date,
+        }
+
+        if symbol is not None:
+            params['symbol'] = symbol
+
+        path = '/trader/v1/accounts/{}/transactions'.format(account_hash)
+        return self._get_request(path, params)
+
+    def get_transaction(self, account_hash, transaction_id):
+        '''Transaction for a specific account.
+
+        :param account_hash: Account hash corresponding to the account whose 
+                             transactions should be returned.
+        :param transaction_id: ID of the transaction for which to return to 
+                               return data.
+        '''
+        path = '/trader/v1/accounts/{}/transactions/{}'.format(
+            account_hash, transaction_id)
+        return self._get_request(path, {})
+
+
+    ##########################################################################
+    # User Info and Preferences
+
+    def get_user_preferences(self):
+        '''Preferences for the logged in account, including all linked
+        accounts.'''
+        path = '/trader/v1/userPreference'
+        return self._get_request(path, {})
+
+
+    ##########################################################################
     # Quotes
 
-    class GetQuote:
+    class Quote:
         class Fields(Enum):
             QUOTE = 'quote'
             FUNDAMENTAL = 'fundamental'
 
     def get_quote(self, symbol, *, fields=None):
         '''
         Get quote for a symbol. Note due to limitations in URL encoding, this
@@ -650,17 +452,17 @@
         containing non-alphanumeric characters, for example as futures like
         ``/ES``. To get quotes for those symbols, use :meth:`Client.get_quotes`.
 
         :param symbol: Single symbol to fetch
         :param fields: Fields to request. If unset, return all available data. 
                        i.e. all fields. See :class:`GetQuote.Field` for options.
         '''
-        fields = self.convert_enum_iterable(fields, self.GetQuote.Fields)
+        fields = self.convert_enum_iterable(fields, self.Quote.Fields)
         if fields:
-            params = {'fields': fields}
+            params = {'fields': ','.join(fields)}
         else:
             params = {}
 
         path = '/marketdata/v1/{}/quotes'.format(symbol)
         return self._get_request(path, params)
 
     def get_quotes(self, symbols, *, fields=None, indicative=None):
@@ -674,17 +476,17 @@
         if isinstance(symbols, str):
             symbols = [symbols]
 
         params = {
             'symbols': ','.join(symbols)
         }
 
-        fields = self.convert_enum_iterable(fields, self.GetQuote.Fields)
+        fields = self.convert_enum_iterable(fields, self.Quote.Fields)
         if fields:
-            params['fields'] = fields
+            params['fields'] = ','.join(fields)
 
         if indicative is not None:
             if type(indicative) is not bool:
                 raise ValueError(
                         'value of \'indicative\' must be either True or False')
             params['indicative'] = 'true' if indicative else 'false'
 
@@ -781,20 +583,18 @@
         :param interval: Strike interval for spread strategy chains (see
                          ``strategy`` param).
         :param strike: Return options only at this strike price.
         :param strike_range: Return options for the given range. See
                              :class:`Options.StrikeRange` for choices.
         :param from_date: Only return expirations after this date. For
                           strategies, expiration refers to the nearest term
-                          expiration in the strategy. Accepts ``datetime.date``
-                          and ``datetime.datetime``.
+                          expiration in the strategy. Accepts ``datetime.date``.
         :param to_date: Only return expirations before this date. For
                         strategies, expiration refers to the nearest term
-                        expiration in the strategy. Accepts ``datetime.date``
-                        and ``datetime.datetime``.
+                        expiration in the strategy. Accepts ``datetime.date``.
         :param volatility: Volatility to use in calculations. Applies only to
                            ``ANALYTICAL`` strategy chains.
         :param underlying_price: Underlying price to use in calculations.
                                  Applies only to ``ANALYTICAL`` strategy chains.
         :param interest_rate: Interest rate to use in calculations. Applies only
                               to ``ANALYTICAL`` strategy chains.
         :param days_to_expiration: Days to expiration to use in calculations.
@@ -809,17 +609,17 @@
         contract_type = self.convert_enum(
             contract_type, self.Options.ContractType)
         strategy = self.convert_enum(strategy, self.Options.Strategy)
         strike_range = self.convert_enum(
             strike_range, self.Options.StrikeRange)
         option_type = self.convert_enum(option_type, self.Options.Type)
         exp_month = self.convert_enum(exp_month, self.Options.ExpirationMonth)
+        entitlement = self.convert_enum(entitlement, self.Options.Entitlement)
 
         params = {
-            'apikey': self.api_key,
             'symbol': symbol,
         }
 
         if contract_type is not None:
             params['contractType'] = contract_type
         if strike_count is not None:
             params['strikeCount'] = strike_count
@@ -830,27 +630,503 @@
         if interval is not None:
             params['interval'] = interval
         if strike is not None:
             params['strike'] = strike
         if strike_range is not None:
             params['range'] = strike_range
         if from_date is not None:
-            params['fromDate'] = self._format_date('from_date', from_date)
+            params['fromDate'] = self._format_date_as_day('from_date', from_date)
         if to_date is not None:
-            params['toDate'] = self._format_date('to_date', to_date)
+            params['toDate'] = self._format_date_as_day('to_date', to_date)
         if volatility is not None:
             params['volatility'] = volatility
         if underlying_price is not None:
             params['underlyingPrice'] = underlying_price
         if interest_rate is not None:
             params['interestRate'] = interest_rate
         if days_to_expiration is not None:
             params['daysToExpiration'] = days_to_expiration
         if exp_month is not None:
             params['expMonth'] = exp_month
         if option_type is not None:
             params['optionType'] = option_type
+        if entitlement is not None:
+            params['entitlement'] = entitlement
 
         path = '/marketdata/v1/chains'
         return self._get_request(path, params)
 
 
+    ##########################################################################
+    # Option Expiration Chain
+
+    def get_option_expiration_chain(self, symbol):
+        '''Preferences for the logged in account, including all linked
+        accounts.'''
+        path = '/marketdata/v1/expirationchain'
+        return self._get_request(path, {'symbol': symbol})
+
+    ##########################################################################
+    # Price History
+
+    class PriceHistory:
+        class PeriodType(Enum):
+            DAY = 'day'
+            MONTH = 'month'
+            YEAR = 'year'
+            YEAR_TO_DATE = 'ytd'
+
+        class Period(Enum):
+            # Daily
+            ONE_DAY = 1
+            TWO_DAYS = 2
+            THREE_DAYS = 3
+            FOUR_DAYS = 4
+            FIVE_DAYS = 5
+            TEN_DAYS = 10
+
+            # Monthly
+            ONE_MONTH = 1
+            TWO_MONTHS = 2
+            THREE_MONTHS = 3
+            SIX_MONTHS = 6
+
+            # Year
+            ONE_YEAR = 1
+            TWO_YEARS = 2
+            THREE_YEARS = 3
+            FIVE_YEARS = 5
+            TEN_YEARS = 10
+            FIFTEEN_YEARS = 15
+            TWENTY_YEARS = 20
+
+            # Year to date
+            YEAR_TO_DATE = 1
+
+        class FrequencyType(Enum):
+            MINUTE = 'minute'
+            DAILY = 'daily'
+            WEEKLY = 'weekly'
+            MONTHLY = 'monthly'
+
+        class Frequency(Enum):
+            # Minute
+            EVERY_MINUTE = 1
+            EVERY_FIVE_MINUTES = 5
+            EVERY_TEN_MINUTES = 10
+            EVERY_FIFTEEN_MINUTES = 15
+            EVERY_THIRTY_MINUTES = 30
+
+            # Other frequencies
+            DAILY = 1
+            WEEKLY = 1
+            MONTHLY = 1
+
+    def get_price_history(
+            self,
+            symbol,
+            *,
+            period_type=None,
+            period=None,
+            frequency_type=None,
+            frequency=None,
+            start_datetime=None,
+            end_datetime=None,
+            need_extended_hours_data=None,
+            need_previous_close=None):
+        '''Get price history for a symbol.
+
+        :param period_type: The type of period to show.
+        :param period: The number of periods to show. Should not be provided if
+                       ``start_datetime`` and ``end_datetime``.
+        :param frequency_type: The type of frequency with which a new candle
+                               is formed.
+        :param frequency: The number of the frequencyType to be included in each
+                          candle.
+        :param start_datetime: Start date.
+        :param end_datetime: End date. Default is previous trading day.
+        :param need_extended_hours_data: If true, return extended hours data.
+                                         Default is true.
+        :param need_previous_close: If true, return the previous close price and 
+                                    date.
+        '''
+        period_type = self.convert_enum(
+            period_type, self.PriceHistory.PeriodType)
+        period = self.convert_enum(period, self.PriceHistory.Period)
+        frequency_type = self.convert_enum(
+            frequency_type, self.PriceHistory.FrequencyType)
+        frequency = self.convert_enum(
+            frequency, self.PriceHistory.Frequency)
+
+        params = {
+                'symbol': symbol,
+        }
+
+        if period_type is not None:
+            params['periodType'] = period_type
+        if period is not None:
+            params['period'] = period
+        if frequency_type is not None:
+            params['frequencyType'] = frequency_type
+        if frequency is not None:
+            params['frequency'] = frequency
+        if start_datetime is not None:
+            params['startDate'] = self._format_date_as_millis(
+                'start_datetime', start_datetime)
+        if end_datetime is not None:
+            params['endDate'] = self._format_date_as_millis(
+                'end_datetime', end_datetime)
+        if need_extended_hours_data is not None:
+            params['needExtendedHoursData'] = need_extended_hours_data
+        if need_previous_close is not None:
+            params['needPreviousClose'] = need_previous_close
+
+        path = '/marketdata/v1/pricehistory'.format(symbol)
+        return self._get_request(path, params)
+
+
+    ##########################################################################
+    # Price history utilities
+
+    def __normalize_start_and_end_datetimes(self, start_datetime, end_datetime):
+        if start_datetime is None:
+            start_datetime = datetime.datetime(year=1971, month=1, day=1)
+        if end_datetime is None:
+            end_datetime = (datetime.datetime.utcnow() +
+                    datetime.timedelta(days=7))
+
+        return start_datetime, end_datetime
+
+
+    def get_price_history_every_minute(
+            self, symbol, *, start_datetime=None, end_datetime=None, 
+            need_extended_hours_data=None, need_previous_close=None):
+        '''
+        Fetch price history for a stock or ETF symbol at a per-minute
+        granularity. This endpoint currently appears to return up to 48 days of
+        data.
+        '''
+
+        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
+                start_datetime, end_datetime)
+
+        return self.get_price_history(
+                symbol,
+                period_type=self.PriceHistory.PeriodType.DAY,
+                period=self.PriceHistory.Period.ONE_DAY,
+                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
+                frequency=self.PriceHistory.Frequency.EVERY_MINUTE,
+                start_datetime=start_datetime,
+                end_datetime=end_datetime,
+                need_extended_hours_data=need_extended_hours_data, 
+                need_previous_close=need_previous_close)
+
+
+    def get_price_history_every_five_minutes(
+            self, symbol, *, start_datetime=None, end_datetime=None, 
+            need_extended_hours_data=None, need_previous_close=None):
+        '''
+        Fetch price history for a stock or ETF symbol at a per-five-minutes
+        granularity. This endpoint currently appears to return approximately
+        nine months of data.
+        '''
+
+        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
+                start_datetime, end_datetime)
+
+        return self.get_price_history(
+                symbol,
+                period_type=self.PriceHistory.PeriodType.DAY,
+                period=self.PriceHistory.Period.ONE_DAY,
+                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
+                frequency=self.PriceHistory.Frequency.EVERY_FIVE_MINUTES,
+                start_datetime=start_datetime,
+                end_datetime=end_datetime,
+                need_extended_hours_data=need_extended_hours_data, 
+                need_previous_close=need_previous_close)
+
+
+    def get_price_history_every_ten_minutes(
+            self, symbol, *, start_datetime=None, end_datetime=None, 
+            need_extended_hours_data=None, need_previous_close=None):
+        '''
+        Fetch price history for a stock or ETF symbol at a per-ten-minutes
+        granularity. This endpoint currently appears to return approximately
+        nine months of data.
+        '''
+
+        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
+                start_datetime, end_datetime)
+
+        return self.get_price_history(
+                symbol,
+                period_type=self.PriceHistory.PeriodType.DAY,
+                period=self.PriceHistory.Period.ONE_DAY,
+                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
+                frequency=self.PriceHistory.Frequency.EVERY_TEN_MINUTES,
+                start_datetime=start_datetime,
+                end_datetime=end_datetime,
+                need_extended_hours_data=need_extended_hours_data, 
+                need_previous_close=need_previous_close)
+
+
+    def get_price_history_every_fifteen_minutes(
+            self, symbol, *, start_datetime=None, end_datetime=None, 
+            need_extended_hours_data=None, need_previous_close=None):
+        '''
+        Fetch price history for a stock or ETF symbol at a per-fifteen-minutes
+        granularity. This endpoint currently appears to return approximately
+        nine months of data.
+        '''
+
+        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
+                start_datetime, end_datetime)
+
+        return self.get_price_history(
+                symbol,
+                period_type=self.PriceHistory.PeriodType.DAY,
+                period=self.PriceHistory.Period.ONE_DAY,
+                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
+                frequency=self.PriceHistory.Frequency.EVERY_FIFTEEN_MINUTES,
+                start_datetime=start_datetime,
+                end_datetime=end_datetime,
+                need_extended_hours_data=need_extended_hours_data, 
+                need_previous_close=need_previous_close)
+
+
+    def get_price_history_every_thirty_minutes(
+            self, symbol, *, start_datetime=None, end_datetime=None, 
+            need_extended_hours_data=None, need_previous_close=None):
+        '''
+        Fetch price history for a stock or ETF symbol at a per-thirty-minutes
+        granularity. This endpoint currently appears to return approximately
+        nine months of data.
+        '''
+
+        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
+                start_datetime, end_datetime)
+
+        return self.get_price_history(
+                symbol,
+                period_type=self.PriceHistory.PeriodType.DAY,
+                period=self.PriceHistory.Period.ONE_DAY,
+                frequency_type=self.PriceHistory.FrequencyType.MINUTE,
+                frequency=self.PriceHistory.Frequency.EVERY_THIRTY_MINUTES,
+                start_datetime=start_datetime,
+                end_datetime=end_datetime,
+                need_extended_hours_data=need_extended_hours_data, 
+                need_previous_close=need_previous_close)
+
+
+    def get_price_history_every_day(
+            self, symbol, *, start_datetime=None, end_datetime=None, 
+            need_extended_hours_data=None, need_previous_close=None):
+        '''
+        Fetch price history for a stock or ETF symbol at a daily granularity. 
+        The exact period of time over which this endpoint returns data is 
+        unclear, although it has been observed returning data as far back as 
+        1985 (for ``AAPL``).
+        '''
+
+        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
+                start_datetime, end_datetime)
+
+        return self.get_price_history(
+                symbol,
+                period_type=self.PriceHistory.PeriodType.YEAR,
+                period=self.PriceHistory.Period.TWENTY_YEARS,
+                frequency_type=self.PriceHistory.FrequencyType.DAILY,
+                frequency=self.PriceHistory.Frequency.EVERY_MINUTE,
+                start_datetime=start_datetime,
+                end_datetime=end_datetime,
+                need_extended_hours_data=need_extended_hours_data, 
+                need_previous_close=need_previous_close)
+
+
+    def get_price_history_every_week(
+            self, symbol, *, start_datetime=None, end_datetime=None, 
+            need_extended_hours_data=None, need_previous_close=None):
+        '''
+        Fetch price history for a stock or ETF symbol at a weekly granularity.
+        The exact period of time over which this endpoint returns data is 
+        unclear, although it has been observed returning data as far back as 
+        1985 (for ``AAPL``).
+        '''
+
+        start_datetime, end_datetime = self.__normalize_start_and_end_datetimes(
+                start_datetime, end_datetime)
+
+        return self.get_price_history(
+                symbol,
+                period_type=self.PriceHistory.PeriodType.YEAR,
+                period=self.PriceHistory.Period.TWENTY_YEARS,
+                frequency_type=self.PriceHistory.FrequencyType.WEEKLY,
+                frequency=self.PriceHistory.Frequency.EVERY_MINUTE,
+                start_datetime=start_datetime,
+                end_datetime=end_datetime,
+                need_extended_hours_data=need_extended_hours_data, 
+                need_previous_close=need_previous_close)
+
+
+    ##########################################################################
+    # Movers
+
+    class Movers:
+        class Index(Enum):
+            DJI = '$DJI'
+            COMPX = '$COMPX'
+            SPX = '$SPX'
+            NYSE = 'NYSE'
+            NASDAQ = 'NASDAQ'
+            OTCBB = 'OTCBB'
+            INDEX_ALL = 'INDEX_ALL'
+            EQUITY_ALL = 'EQUITY_ALL'
+            OPTION_ALL = 'OPTION_ALL'
+            OPTION_PUT = 'OPTION_PUT'
+            OPTION_CALL = 'OPTION_CALL'
+
+        class SortOrder(Enum):
+            '''Sort by a particular attribute'''
+            VOLUME = 'VOLUME'
+            TRADES = 'TRADES'
+            PERCENT_CHANGE_UP = 'PERCENT_CHANGE_UP'
+            PERCENT_CHANGE_DOWN = 'PERCENT_CHANGE_DOWN'
+
+        class Frequency(Enum):
+            '''To return movers with the specified directions of up or down'''
+            ZERO = 0
+            ONE = 1
+            FIVE = 5
+            TEN = 10
+            THIRTY = 30
+            SIXTY = 60
+        
+
+    def get_movers(self, index, *, sort_order=None, frequency=None):
+        '''Get a list of the top ten movers for a given index.
+
+        :param index: Category of mover. See :class:`Movers.Index` for valid 
+                      values.
+        :param sort_order: Order in which to return values. See 
+                           :class:`Movers.SortOrder for valid values`
+        :param frequency: Only return movers that saw this magnitude or greater. 
+                          See :class:`Movers.Frequency` for valid values.
+        '''
+        index = self.convert_enum(index, self.Movers.Index)
+        sort_order = self.convert_enum(sort_order, self.Movers.SortOrder)
+        frequency = self.convert_enum(frequency, self.Movers.Frequency)
+
+        path = '/marketdata/v1/movers/{}'.format(index)
+
+        params = {}
+        if sort_order is not None:
+            params['sort'] = sort_order
+        if frequency is not None:
+            params['frequency'] = str(frequency)
+
+        return self._get_request(path, params)
+
+
+    ##########################################################################
+    # Market Hours
+
+    class MarketHours:
+        class Market(Enum):
+            EQUITY = 'equity'
+            OPTION = 'option'
+            BOND = 'bond'
+            FUTURE = 'future'
+            FOREX = 'forex'
+
+    def get_market_hours(self, markets, *, date=None):
+        '''Retrieve market hours for specified markets
+
+        :param markets: Markets for which to return trading hours.
+        :param date: Date for which to return market hours. Accepts values up to 
+                     one year from today. Accepts ``datetime.date``.
+        '''
+        markets = self.convert_enum_iterable(markets, self.MarketHours.Market)
+
+        params = {
+                'markets': ','.join(markets)
+        }
+        if date is not None:
+            params['date'] = self._format_date_as_day('date', date)
+
+        return self._get_request('/marketdata/v1/markets', params)
+
+
+    ##########################################################################
+    # Instrument
+
+    class Instrument:
+        class Projection(Enum):
+            SYMBOL_SEARCH = 'symbol-search'
+            SYMBOL_REGEX = 'symbol-regex'
+            DESCRIPTION_SEARCH = 'desc-search'
+            DESCRIPTION_REGEX = 'desc-regex'
+            SEARCH = 'search'
+            FUNDAMENTAL = 'fundamental'
+
+    def get_instruments(self, symbols, projection):
+        '''Get instrument details by using different search methods. Also used 
+        to get fundamental instrument data by use of the ``FUNDAMENTAL`` 
+        projection.
+
+        :param symbol: For ``FUNDAMENTAL`` projection, the symbol for which to 
+                       get fundamentals. For other projections, a search term. 
+                       See below for details.
+        :param projection: Search mode, or ``FUNDAMENTAL`` for instrument 
+                           fundamentals. See :class:`Instrument.Projection`.
+
+        This method is a bit of a chimera because it supports both symbol 
+        search and fundamentals lookup. The format and interpretation of the 
+        ``symbol`` parameter differs according ot the value of the 
+        ``projection`` parameter:
+
+        .. list-table::
+           :widths: 25 25 50
+           :header-rows: 1
+
+           * - ``projection`` value
+             - Accepted values of ``symbol``
+             - ``symbol`` interpretation
+           * - ``SYMBOL_SEARCH``
+             - String, or array of strings
+             - Symbols for which to search results
+           * - ``SYMBOL_REGEX``
+             - Single string
+             - Regular expression to match against symbols
+           * - ``DESCRIPTION_SEARCH``
+             - Single string
+             - String to search for in symbol description
+           * - ``DESCRIPTION_REGEX``
+             - Single string
+             - Regex to search for in symbol description
+           * - ``SEARCH``
+             - Single string
+             - Regular expression to match against symbols
+           * - ``FUNDAMENTAL``
+             - String, or array of strings
+             - Symbols for which to return fundamentals. Exact match.
+        '''
+        projection = self.convert_enum(projection, self.Instrument.Projection)
+
+        params = {
+                'symbol': ','.join(symbols),
+                'projection': projection,
+        }
+
+        return self._get_request('/marketdata/v1/instruments', params)
+
+
+    def get_instrument_by_cusip(self, cusip):
+        '''Get instrument information for a single instrument by CUSIP.
+
+        :param cusip: String representing CUSIP of instrument for which to fetch 
+                      data. Note leading zeroes must be preserved.
+        '''
+        if not isinstance(cusip, str):
+            raise ValueError('cusip must be passed as str')
+
+        return self._get_request(
+                '/marketdata/v1/instruments/{}'.format(cusip), {})
```

### Comparing `schwab-py-0.0.0a9/schwab/client/synchronous.py` & `schwab_py-1.0.0/schwab/client/synchronous.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,72 +6,50 @@
     pass
 
 import json
 
 
 class Client(BaseClient):
     def _get_request(self, path, params):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: GET to %s, params=%s',
                 req_num, dest, LazyLog(lambda: json.dumps(params, indent=4)))
 
         resp = self.session.get(dest, params=params)
         self._log_response(resp, req_num)
         register_redactions_from_response(resp)
         return resp
 
     def _post_request(self, path, data):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: POST to %s, json=%s',
             req_num, dest, LazyLog(lambda: json.dumps(data, indent=4)))
 
         resp = self.session.post(dest, json=data)
         self._log_response(resp, req_num)
         register_redactions_from_response(resp)
         return resp
 
     def _put_request(self, path, data):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: PUT to %s, json=%s',
             req_num, dest, LazyLog(lambda: json.dumps(data, indent=4)))
 
         resp = self.session.put(dest, json=data)
         self._log_response(resp, req_num)
         register_redactions_from_response(resp)
         return resp
 
-    def _patch_request(self, path, data):
-        self.ensure_updated_refresh_token()
-
-        dest = 'https://api.schwabapi.com' + path
-
-        req_num = self._req_num()
-        self.logger.debug('Req %s: PATCH to %s, json=%s',
-                req_num, dest, LazyLog(lambda: json.dumps(data, indent=4)))
-
-        resp = self.session.patch(dest, json=data)
-        self._log_response(resp, req_num)
-        register_redactions_from_response(resp)
-        return resp
-
     def _delete_request(self, path):
-        self.ensure_updated_refresh_token()
-
         dest = 'https://api.schwabapi.com' + path
 
         req_num = self._req_num()
         self.logger.debug('Req %s: DELETE to %s'.format(req_num, dest))
 
         resp = self.session.delete(dest)
         self._log_response(resp, req_num)
```

### Comparing `schwab-py-0.0.0a9/schwab/debug.py` & `schwab_py-1.0.0/schwab/debug.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 import atexit
 import httpx
+import json
 import logging
 import sys
 import schwab
 
-# This creates a tuple of JSONDecodeError types as a mechanism to catch multiple
-# errors. This is needed because currently the `requests` library either uses
-# the `simplejson` library or the builtin `json` library. This tuple-based
-# approach makes it somewhat future-proof.
-# Note: the `requests` is migrating to always use the builtin `json` library.
-import json.decoder
-try:
-    import simplejson.errors
-    __json_errors = (json.decoder.JSONDecodeError,
-                     simplejson.errors.JSONDecodeError)
-except ImportError:
-    __json_errors = (json.decoder.JSONDecodeError,)
-
 
 def get_logger():
     return logging.getLogger(__name__)
 
 
 class LogRedactor:
     '''
@@ -61,15 +49,15 @@
     '''
     Convenience method that calls ``register_redactions`` if resp represents a
     successful response. Note this method assumes that resp has a JSON contents.
     '''
     if resp.status_code == httpx.codes.OK:
         try:
             register_redactions(resp.json())
-        except __json_errors:
+        except json.decoder.JSONDecodeError:
             pass
 
 
 def register_redactions(obj, key_path=None,
                         bad_patterns=[
                             'auth', 'acl', 'displayname', 'id', 'key', 'token'],
                         whitelisted=set([
@@ -127,15 +115,15 @@
     Module-internal version of :func:`enable_bug_report_logging`, intended for
     use in tests.
     '''
     if loggers is None:
         loggers = (
             schwab.auth.get_logger(),
             schwab.client.base.get_logger(),
-            #schwab.streaming.get_logger(),
+            schwab.streaming.get_logger(),
             get_logger())
 
     class RecordingHandler(logging.Handler):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
             self.messages = []
```

### Comparing `schwab-py-0.0.0a9/schwab/orders/__init__.py` & `schwab_py-1.0.0/schwab/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a9/schwab/orders/common.py` & `schwab_py-1.0.0/schwab/orders/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,24 +360,24 @@
     TRIGGER = 'TRIGGER'
 
 
 def one_cancels_other(order1, order2):
     '''
     If one of the orders is executed, immediately cancel the other.
     '''
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.generic import OrderBuilder
 
     return (OrderBuilder()
             .set_order_strategy_type(OrderStrategyType.OCO)
             .add_child_order_strategy(order1)
             .add_child_order_strategy(order2))
 
 
 def first_triggers_second(first_order, second_order):
     '''
     If ``first_order`` is executed, immediately place ``second_order``.
     '''
-    from tda.orders.generic import OrderBuilder
+    from schwab.orders.generic import OrderBuilder
 
     return (first_order
             .set_order_strategy_type(OrderStrategyType.TRIGGER)
             .add_child_order_strategy(second_order))
```

### Comparing `schwab-py-0.0.0a9/schwab/orders/equities.py` & `schwab_py-1.0.0/schwab/orders/equities.py`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a9/schwab/orders/generic.py` & `schwab_py-1.0.0/schwab/orders/generic.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 from enum import Enum
 
 from schwab.orders import common
 from schwab.utils import EnumEnforcer
 
 import httpx
 
@@ -29,14 +31,17 @@
 
             name = name[1:]
             ret[name] = _build_object(value)
         return ret
 
 
 def truncate_float(flt):
+    warnings.warn('passing floats to set_price and set_stop_price is '+
+                  'deprecated and will be removed soon. Please update your '+
+                  'code to pass prices as strings instead.')
     if abs(flt) < 1 and flt != 0.0:
         return '{:.4f}'.format(float(int(flt * 10000)) / 10000.0)
     else:
         return '{:.2f}'.format(float(int(flt * 100)) / 100.0)
 
 
 class OrderBuilder(EnumEnforcer):
@@ -53,15 +58,15 @@
         super().__init__(enforce_enums)
 
         self._session = None
         self._duration = None
         self._orderType = None
         self._complexOrderStrategyType = None
         self._quantity = None
-        self._requestedDestination = None
+        self._destinationLinkName = None
         self._stopPrice = None
         self._stopPriceLinkBasis = None
         self._stopPriceLinkType = None
         self._stopPriceOffset = None
         self._stopType = None
         self._priceLinkBasis = None
         self._priceLinkType = None
@@ -155,30 +160,30 @@
     def clear_quantity(self):
         '''
         Clear the order-level quantity. Note this does not affect order legs.
         '''
         self._quantity = None
         return self
 
-    # RequestedDestination
-    def set_requested_destination(self, requested_destination):
+    # DestinationLinkName
+    def set_destination_link_name(self, destination_link_name):
         '''
-        Set the requested destination. See
+        Set the destination link name. See
         :class:`~schwab.orders.common.Destination` for details.
         '''
-        requested_destination = self.convert_enum(
-            requested_destination, common.Destination)
-        self._requestedDestination = requested_destination
+        destination_link_name = self.convert_enum(
+            destination_link_name, common.Destination)
+        self._destinationLinkName = destination_link_name
         return self
 
-    def clear_requested_destination(self):
+    def clear_destination_link_name(self):
         '''
-        Clear the requested destination.
+        Clear the destination link name
         '''
-        self._requestedDestination = None
+        self._destinationLinkName = None
         return self
 
     # StopPrice
     def set_stop_price(self, stop_price):
         '''
         Set the stop price. Note price can be passed as either a `float` or an
         `str`. See :ref:`number_truncation`.
```

### Comparing `schwab-py-0.0.0a9/schwab/orders/options.py` & `schwab_py-1.0.0/schwab/orders/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,55 +2,63 @@
 
 from schwab.orders.generic import OrderBuilder
 
 
 def _parse_expiration_date(expiration_date):
     date = None
     try:
-        date = datetime.datetime.strptime(expiration_date, '%m%d%y')
+        date = datetime.datetime.strptime(expiration_date, '%y%m%d')
         return datetime.date(year=date.year, month=date.month, day=date.day)
     except ValueError:
         pass
 
     raise ValueError(
         'expiration date must follow format ' +
-        '[Month with leading zero][Day with leading zero]' +
-        '[two digit year]')
+        '[two digit year][Month with leading zero]' +
+        '[Day with leading zero]')
 
 
 class OptionSymbol:
-    '''
-    Construct an option symbol from its constituent parts. Options symbols
-    have the following format: ``[Underlying]_[Two digit month][Two digit
-    day][Two digit year]['P' or 'C'][Strike price]``. Examples include:
-
-     * ``GOOG_012122P620``: GOOG Jan 21 2022 620 Put
-     * ``TSLA_112020C1360``: TSLA Nov 20 2020 1360 Call
-     * ``SPY_121622C335``: SPY Dec 16 2022 335 Call
+    '''Construct an option symbol from its constituent parts.
+
+    :param underlying_symbol: Symbol of the underlying. Not validated.
+    :param expiration_date: Expiration date. Accepts ``datetime.date``,
+                            ``datetime.datetime``, or strings with the
+                            format ``[Two digit year][Two digit month][Two
+                            digit day]``.
+    :param contract_type: ``P`` or ``PUT`` for put and ``C`` or ``CALL`` for 
+                          call.
+    :param strike_price_as_string: Strike price represented as a decimal string.
 
     Note while each of the individual parts is validated by itself, the
     option symbol itself may not represent a traded option:
 
      * Some underlyings do not support options.
      * Not all dates have valid option expiration dates.
      * Not all strike prices are valid options strikes.
 
     You can use :meth:`~schwab.client.Client.get_option_chain` to obtain real
     option symbols for an underlying, as well as extensive data in pricing,
     bid/ask spread, volume, etc.
 
-    :param underlying_symbol: Symbol of the underlying. Not validated.
-    :param expiration_date: Expiration date. Accepts ``datetime.date``,
-                            ``datetime.datetime``, or strings with the
-                            format ``[Two digit month][Two digit day][Two
-                            digit year]``.
-    :param contract_type: ``P` or `PUT`` for put and ``C` or `CALL`` for call.
-    :param strike_price_as_string: Strike price, represented by a string as
-                                   you would see at the end of a real option
-                                   symbol.
+    For those interested in the details, options symbols have the following 
+    format: ``[Underlying left justified with spaces to 6 positions] [Two digit 
+    year][Two digit month][Two digit day]['P' or 'C'][Strike price]``
+
+    The format of the strike price is modified based on its amount:
+     * If less than 1000, Strike Price is multiple by 1000 and pre-pended with
+       two zeroes
+     * If greater than 1000, it's prepended with one zero.
+
+    Examples include:
+     * ``QQQ   240420P00500000``: QQQ Apr 20, 2024 500 Put (note the two zeroes
+       in front because strike is less than 1000)
+     * ``SPXW  240420C05040000``: SPX Weekly Apr 20, 2024 5040 Call (note the
+       one zero in front because strike is greater than 1000)
+
     '''
 
     def __init__(self, underlying_symbol, expiration_date, contract_type,
                  strike_price_as_string):
         self.underlying_symbol = underlying_symbol
 
         if contract_type in ('C', 'CALL'):
@@ -68,58 +76,53 @@
                 year=expiration_date.year,
                 month=expiration_date.month,
                 day=expiration_date.day)
         elif isinstance(expiration_date, datetime.date):
             self.expiration_date = expiration_date
         else:
             raise ValueError(
-                'expiration_date must be a string with format %m%d%y ' +
-                '(e.g. 01092020) or one of datetime.date or ' +
+                'expiration_date must be a string with format %y%m%d ' +
+                '(e.g. 240614) or one of datetime.date or ' +
                 'datetime.datetime')
 
         assert(isinstance(self.expiration_date, datetime.date))
 
         strike = None
         try:
             strike = float(strike_price_as_string)
         except ValueError:
             pass
         if (strike is None or not isinstance(strike_price_as_string, str)
                 or strike <= 0):
             raise ValueError(
-                'Strike price must be a string representing a positive ' +
+                'strike price must be a string representing a positive ' +
                 'float')
 
         # Remove extraneous zeroes at the end
         strike_copy = strike_price_as_string
         while strike_copy[-1] == '0':
             strike_copy = strike_copy[:-1]
         if strike_copy[-1] == '.':
             strike_price_as_string = strike_copy[:-1]
 
         self.strike_price = strike_price_as_string
 
     @classmethod
     def parse_symbol(cls, symbol):
         '''
-        Parse a string option symbol of the for ``[Underlying]_[Two digit month]
-        [Two digit day][Two digit year]['P' or 'C'][Strike price]``.
+        Parse a string option symbol of the for ``[Underlying left justified to 6 positions][Two digit year]
+        [Two digit month][Two digit day]['P' or 'C'][Strike price]``.
         '''
         format_error_str = (
             'option symbol must have format ' +
-            '[Underlying]_[Expiration][P/C][Strike]')
+            '[Underlying left justified with spaces to 6 positions][Expiration][P/C][Strike]')
 
         # Underlying
-        try:
-            underlying, rest = symbol.split('_')
-        except ValueError:
-            underlying, rest = None, None
-        if underlying is None:
-            raise ValueError('option symbol missing underscore \'_\', ' +
-                             format_error_str)
+        underlying = symbol[:6].rstrip()
+        rest = symbol[6:]
 
         # Expiration
         type_split = rest.split('P')
         if len(type_split) == 2:
             expiration_date, strike = type_split
             contract_type = 'P'
         else:
@@ -128,27 +131,29 @@
                 expiration_date, strike = type_split
                 contract_type = 'C'
             else:
                 raise ValueError(
                     r'option must have contract type \'C\' r \'\P\', ' +
                     format_error_str)
 
+        strike = str(int(strike) / 1000.0)
+
         expiration_date = _parse_expiration_date(expiration_date)
 
         return OptionSymbol(underlying, expiration_date, contract_type, strike)
 
     def build(self):
         '''
         Returns the option symbol represented by this builder.
         '''
-        return '{}_{}{}{}'.format(
+        return '{:<6}{}{}{:08d}'.format(
             self.underlying_symbol,
-            self.expiration_date.strftime('%m%d%y'),
+            self.expiration_date.strftime('%y%m%d'),
             self.contract_type,
-            self.strike_price
+            int(float(self.strike_price) * 1000)
         )
 
 
 def __base_builder():
     from schwab.orders.common import Duration, Session
 
     return (OrderBuilder()
```

### Comparing `schwab-py-0.0.0a9/schwab/utils.py` & `schwab_py-1.0.0/schwab/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,19 +75,19 @@
 class UnsuccessfulOrderException(ValueError):
     '''
     Raised by :meth:`Utils.extract_order_id` when attempting to extract an
     order ID from a :meth:`Client.place_order` response that was not successful.
     '''
 
 
-class AccountIdMismatchException(ValueError):
+class AccountHashMismatchException(ValueError):
     '''
     Raised by :meth:`Utils.extract_order_id` when attempting to extract an
-    order ID from a :meth:`Client.place_order` with a different account ID than
-    the one with which the :class:`Utils` was initialized.
+    order ID from a :meth:`Client.place_order` with a different account hash
+    than the one with which the :class:`Utils` was initialized.
     '''
 
 
 class LazyLog:
     'Helper to defer evaluation of expensive variables in log messages'
     def __init__(self, func):
         self.func = func
@@ -95,57 +95,56 @@
         return self.func()
 
 
 class Utils(EnumEnforcer):
     '''Helper for placing orders on equities. Provides easy-to-use
     implementations for common tasks such as market and limit orders.'''
 
-    def __init__(self, client, account_id):
+    def __init__(self, client, account_hash):
         '''Creates a new ``Utils`` instance. For convenience, this object
-        assumes the user wants to work with a single account ID at a time.'''
+        assumes the user wants to work with a single account hash at a time.'''
         super().__init__(True)
 
         self.client = client
-        self.account_id = account_id
+        self.account_hash = account_hash
 
-    def set_account_id(self, account_id):
-        '''Set the account ID used by this ``Utils`` instance.'''
-        self.account_id = account_id
+    def set_account_hash(self, account_hash):
+        '''Set the account hash used by this ``Utils`` instance.'''
+        self.account_hash = account_hash
 
     def extract_order_id(self, place_order_response):
-        '''Attempts to extract the order ID from a response object returned by
-        :meth:`Client.place_order() <tda.client.Client.place_order>`. Return
+        '''Attempts to extract the order hash from a response object returned by
+        :meth:`Client.place_order() <schwab.client.Client.place_order>`. Return
         ``None`` if the order location is not contained in the response.
 
         :param place_order_response: Order response as returned by
                                      :meth:`Client.place_order()
-                                     <tda.client.Client.place_order>`. Note this
+                                     <schwab.client.Client.place_order>`. Note this
                                      method requires that the order was
                                      successful.
 
         :raise ValueError: if the order was not succesful or if the order's
-                           account ID is not equal to the account ID set in this
+                           account hash is not equal to the account hash set in this
                            ``Utils`` object.
-
         '''
         if place_order_response.is_error:
             raise UnsuccessfulOrderException(
                 'order not successful: status {}'.format(place_order_response.status_code))
 
         try:
             location = place_order_response.headers['Location']
         except KeyError:
             return None
 
         m = re.match(
-            r'https://api.tdameritrade.com/v1/accounts/(\d+)/orders/(\d+)',
-            location)
+                r'https://api.schwabapi.com/trader/v1/accounts/(\w+)/orders/(\d+)',
+                location)
 
         if m is None:
             return None
-        account_id, order_id = int(m.group(1)), int(m.group(2))
+        account_hash, order_id = m.group(1), int(m.group(2))
 
-        if str(account_id) != str(self.account_id):
-            raise AccountIdMismatchException(
-                'order request account ID != Utils.account_id')
+        if str(account_hash) != str(self.account_hash):
+            raise AccountHashMismatchException(
+                'order request account hash != Utils.account_hash')
 
         return order_id
```

### Comparing `schwab-py-0.0.0a9/setup.cfg` & `schwab_py-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab-py-0.0.0a9/setup.py` & `schwab_py-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,53 +9,57 @@
     version = version[1:-1]
 
 setuptools.setup(
     name='schwab-py',
     version=version,
     author='Alex Golec',
     author_email='bottomless.septic.tank@gmail.com',
-    description='Unofficial API wrapper for the upcoming Schwab HTTP API',
+    description='Unofficial API wrapper for the Schwab HTTP API',
     long_description=long_description,
     long_description_content_type='text/x-rst',
-    url='https://github.com/alexgolec/schwab',
+    url='https://github.com/alexgolec/schwab-py',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'Development Status :: 1 - Planning',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Topic :: Office/Business :: Financial :: Investment',
     ],
-    python_requires='>=3.8',
+    python_requires='>=3.10',
     install_requires=[
+        'autopep8',
         'authlib',
         'httpx',
         'prompt_toolkit',
         'python-dateutil',
         'selenium',
+        'websockets'
     ],
     extras_require={
         'dev': [
-            'asynctest',
+            'callee',
             'colorama',
             'coverage',
             'nose',
             'pytest',
             'pytz',
             'sphinx_rtd_theme',
             'twine',
+            'wheel',
         ]
     },
     keywords='finance trading equities bonds options research',
     project_urls={
-        'Documentation': 'https://schwab-api.readthedocs.io/en/latest/',
-        'Source': 'https://github.com/alexgolec/schwab-api',
-        'Tracker': 'https://github.com/alexgolec/schwab-api/issues',
+        'Documentation': 'https://schwab-py.readthedocs.io/en/latest/',
+        'Source': 'https://github.com/alexgolec/schwab-py',
+        'Tracker': 'https://github.com/alexgolec/schwab-py/issues',
     },
     license='MIT',
     scripts=[
+        'bin/schwab-order-codegen.py',
     ],
 )
```

