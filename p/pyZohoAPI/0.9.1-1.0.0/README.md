# Comparing `tmp/pyZohoAPI-0.9.1.tar.gz` & `tmp/pyzohoapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyZohoAPI-0.9.1.tar", last modified: Thu Sep 30 21:09:52 2021, max compression
+gzip compressed data, was "pyzohoapi-1.0.0.tar", max compression
```

## Comparing `pyZohoAPI-0.9.1.tar` & `pyzohoapi-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0     1094 2021-02-22 17:36:44.048988 pyZohoAPI-0.9.1/LICENSE
--rw-r--r--   0        0        0     1094 2021-02-22 17:36:44.048988 pyZohoAPI-0.9.1/LICENSE
--rw-r--r--   0        0        0     1187 2021-09-30 21:09:12.576063 pyZohoAPI-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      303 2021-09-30 21:09:12.577068 pyZohoAPI-0.9.1/pyzohoapi/__init__.py
--rw-r--r--   0        0        0     1677 2021-04-12 16:45:18.251606 pyZohoAPI-0.9.1/pyzohoapi/books.py
--rw-r--r--   0        0        0    17171 2021-09-30 16:10:42.622618 pyZohoAPI-0.9.1/pyzohoapi/core/__init__.py
--rw-r--r--   0        0        0    12536 2021-05-12 15:47:32.496055 pyZohoAPI-0.9.1/pyzohoapi/core/collection.py
--rw-r--r--   0        0        0     1600 2021-03-13 20:16:47.883264 pyZohoAPI-0.9.1/pyzohoapi/core/utils.py
--rw-r--r--   0        0        0     2352 2021-05-28 17:09:57.021803 pyZohoAPI-0.9.1/pyzohoapi/exceptions/__init__.py
--rw-r--r--   0        0        0     3288 2021-06-16 17:21:08.137254 pyZohoAPI-0.9.1/pyzohoapi/inventory.py
--rw-r--r--   0        0        0     5054 2021-09-30 21:06:45.014687 pyZohoAPI-0.9.1/pyzohoapi/objecttypes/__init__.py
--rw-r--r--   0        0        0     3751 2021-09-30 14:47:04.365927 pyZohoAPI-0.9.1/pyzohoapi/objecttypes/mixins/__init__.py
--rw-r--r--   0        0        0     2004 2021-05-26 20:22:44.442023 pyZohoAPI-0.9.1/pyzohoapi/objecttypes/mixins/CompositeItemOps.py
--rw-r--r--   0        0        0     1862 2021-05-26 20:32:59.533825 pyZohoAPI-0.9.1/pyzohoapi/objecttypes/mixins/CustomFields.py
--rw-r--r--   0        0        0     1868 2021-09-30 21:09:12.578061 pyZohoAPI-0.9.1/README.md
--rw-r--r--   0        0        0     2657 2021-09-30 21:09:52.172626 pyZohoAPI-0.9.1/setup.py
--rw-r--r--   0        0        0     2808 2021-09-30 21:09:52.172626 pyZohoAPI-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-25 14:12:23.999748 pyzohoapi-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2109 2024-05-25 14:12:23.999748 pyzohoapi-1.0.0/README.md
+-rw-r--r--   0        0        0     1167 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      292 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/__init__.py
+-rw-r--r--   0        0        0     1617 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/books.py
+-rw-r--r--   0        0        0    17242 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/core/__init__.py
+-rw-r--r--   0        0        0    12157 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/core/collection.py
+-rw-r--r--   0        0        0     1559 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/core/utils.py
+-rw-r--r--   0        0        0     2285 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/exceptions/__init__.py
+-rw-r--r--   0        0        0     3250 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/inventory.py
+-rw-r--r--   0        0        0     5119 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/objecttypes/__init__.py
+-rw-r--r--   0        0        0     1960 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/objecttypes/mixins/CompositeItemOps.py
+-rw-r--r--   0        0        0     1820 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/objecttypes/mixins/CustomFields.py
+-rw-r--r--   0        0        0     3665 2024-05-25 14:12:24.003748 pyzohoapi-1.0.0/pyzohoapi/objecttypes/mixins/__init__.py
+-rw-r--r--   0        0        0     3308 1970-01-01 00:00:00.000000 pyzohoapi-1.0.0/PKG-INFO
```

### Comparing `pyZohoAPI-0.9.1/LICENSE` & `pyzohoapi-1.0.0/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Todd D. Esposito
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021-2024 Todd D. Esposito
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyZohoAPI-0.9.1/pyproject.toml` & `pyzohoapi-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-[tool.poetry]
-name = "pyZohoAPI"
-version = "0.9.1"
-description = "Pythonic access to Zoho APIs in the Finance Plus suite."
-authors = ["Todd Esposito <todd@toddesposito.com>"]
-license = "MIT"
-readme = "README.md"
-include = ["LICENSE"]
-homepage = "https://github.com/tdesposito/pyZohoAPI"
-repository = "https://github.com/tdesposito/pyZohoAPI"
-documentation = "https://pyzohoapi.readthedocs.io/en/latest/"
-keywords = [
-  "api",
-  "zoho api",
-  "zoho books",
-  "zoho inventory",
-  "zoho",
-]
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Intended Audience :: Developers",
-  "Topic :: Software Development :: Libraries :: Python Modules",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-]
-
-[tool.poetry.dependencies]
-python = "^3.6"
-requests = "^2.25.1"
-
-[tool.poetry.dev-dependencies]
-furo = "^2020.12.30-beta.24"
-sphinx = "^3.4.3"
-myst-parser = "^0.13.3"
-sphinx-autobuild = "^2020.9.1"
-sphinx-copybutton = "^0.3.1"
-pytest = "^6.2.4"
-
-[build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+[tool.poetry]
+name = "pyZohoAPI"
+version = "1.0.0"
+description = "Pythonic access to Zoho APIs in the Finance Plus suite."
+authors = ["Todd Esposito <todd@toddesposito.com>"]
+license = "MIT"
+readme = "README.md"
+include = ["LICENSE"]
+homepage = "https://github.com/tdesposito/pyZohoAPI"
+repository = "https://github.com/tdesposito/pyZohoAPI"
+documentation = "https://pyzohoapi.readthedocs.io/en/latest/"
+keywords = [
+  "api",
+  "zoho api",
+  "zoho books",
+  "zoho inventory",
+  "zoho",
+]
+classifiers = [
+  "Development Status :: 4 - Beta",
+  "Intended Audience :: Developers",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Programming Language :: Python :: 3.6",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+]
+
+[tool.poetry.dependencies]
+python = "^3.6"
+requests = "^2.25.1"
+simplejson = "^3.17.5"
+
+[tool.poetry.dev-dependencies]
+furo = "^2020.12.30-beta.24"
+sphinx = "^3.4.3"
+myst-parser = "^0.13.3"
+sphinx-autobuild = "^2020.9.1"
+sphinx-copybutton = "^0.3.1"
+pytest = "^6.2.4"
+
+[build-system]
+requires = ["poetry>=0.12"]
+build-backend = "poetry.masonry.api"
```

### Comparing `pyZohoAPI-0.9.1/pyzohoapi/books.py` & `pyzohoapi-1.0.0/pyzohoapi/books.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
-# Distributed under the MIT License (see http://opensource.org/licenses/MIT).
-
-from .core import ZohoAPIBase
-from .exceptions import ZohoException
-from . import objecttypes
-
-class ZohoBooks(ZohoAPIBase):
-    _scope = "ZohoBooks.FullAccess.all"
-
-    def get_endpoint(self, region):
-        return f"https://books.zoho.{self._regionmap[region]}/api/v3"
-
-    def Account(self, *args, **kwargs): return objecttypes.Account(self, *args, **kwargs)
-    def CompositeItem(self, *args, **kwargs): return objecttypes.CompositeItem(self, *args, **kwargs)
-    def Contact(self, *args, **kwargs): return objecttypes.Contact(self, *args, **kwargs)
-    def CustomerPayment(self, *args, **kwargs): return objecttypes.CustomerPayment(self, *args, **kwargs)
-    def Document(self, *args, **kwargs): return objecttypes.Document(self, *args, **kwargs)
-    def Invoice(self, *args, **kwargs): return objecttypes.Invoice(self, *args, **kwargs)
-    def Item(self, *args, **kwargs): return objecttypes.Item(self, *args, **kwargs)
-    def ItemGroup(self, *args, **kwargs): return objecttypes.ItemGroup(self, *args, **kwargs)
-    def Organization(self, *args, **kwargs): return objecttypes.Organization(self, *args, **kwargs)
-    def PurchaseOrder(self, *args, **kwargs): return objecttypes.PurchaseOrder(self, *args, **kwargs)
-    def SalesOrder(self, *args, **kwargs): return objecttypes.SalesOrder(self, *args, **kwargs)
-    def SalesPerson(self, *args, **kwargs): return objecttypes.SalesPerson(self, *args, **kwargs)
-    def User(self, *args, **kwargs): return objecttypes.User(self, *args, **kwargs)
+# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
+# Distributed under the MIT License (see http://opensource.org/licenses/MIT).
+
+from .core import ZohoAPIBase
+from . import objecttypes
+
+class ZohoBooks(ZohoAPIBase):
+    _scope = "ZohoBooks.FullAccess.all"
+
+    def get_endpoint(self, region):
+        return f"https://www.zohoapis.{self._regionmap[region]}/books/v3"
+
+    def Account(self, *args, **kwargs): return objecttypes.Account(self, *args, **kwargs)
+    def CompositeItem(self, *args, **kwargs): return objecttypes.CompositeItem(self, *args, **kwargs)
+    def Contact(self, *args, **kwargs): return objecttypes.Contact(self, *args, **kwargs)
+    def CustomerPayment(self, *args, **kwargs): return objecttypes.CustomerPayment(self, *args, **kwargs)
+    def Document(self, *args, **kwargs): return objecttypes.Document(self, *args, **kwargs)
+    def Invoice(self, *args, **kwargs): return objecttypes.Invoice(self, *args, **kwargs)
+    def Item(self, *args, **kwargs): return objecttypes.Item(self, *args, **kwargs)
+    def ItemGroup(self, *args, **kwargs): return objecttypes.ItemGroup(self, *args, **kwargs)
+    def Organization(self, *args, **kwargs): return objecttypes.Organization(self, *args, **kwargs)
+    def PurchaseOrder(self, *args, **kwargs): return objecttypes.PurchaseOrder(self, *args, **kwargs)
+    def SalesOrder(self, *args, **kwargs): return objecttypes.SalesOrder(self, *args, **kwargs)
+    def SalesPerson(self, *args, **kwargs): return objecttypes.SalesPerson(self, *args, **kwargs)
+    def User(self, *args, **kwargs): return objecttypes.User(self, *args, **kwargs)
```

### Comparing `pyZohoAPI-0.9.1/pyzohoapi/core/__init__.py` & `pyzohoapi-1.0.0/pyzohoapi/core/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,423 +1,433 @@
-# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
-# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
-
-import datetime
-import logging
-from time import sleep
-
-import requests
-
-from .collection import DottedDict, DottedList
-from .utils import diff
-from ..exceptions import *
-
-logging.getLogger('pyzohoapi').addHandler(logging.NullHandler())
-
-class ZohoAPIBase:
-    _regionmap = {
-        'australia': "com.au",
-        'com.au': "com.au",
-        'com': "com",
-        'eu': "eu",
-        'europe': "eu",
-        'in': "in",
-        'india': "in",
-        'us': "com",
-    }
-    def __init__(self, organization_id, region="us", **apiArgs):
-        """ Constructor
-
-        :param organization_id: Zoho Organization ID to which to connect
-        :type organization_id: str
-        :param region: Zoho Data Center Region. Defaults to "us".
-        :type region: str
-        :param **apiArgs: additional parameters for API operation.
-        :raises ZohoUnknownRegionException: if the region is unknown or invalid.
-
-        """
-        region = region.lower()
-        if region not in self._regionmap:
-            raise ZohoUnknownRegionException(region)
-        self._org = organization_id
-        self._endpoint = self.get_endpoint(region)
-        self._oauth = f"https://accounts.zoho.{self._regionmap[region]}/oauth/v2"
-        self._ratelimit = {
-            'limit': None,
-            'NextCall': datetime.datetime.now().timestamp(),
-            'remaining': 99999999,
-            'reset': None,
-        }
-        self._api_keys = {
-            'access_token': None,
-            'client_id': None,
-            'client_secret': None,
-            'intercall_delay': 0,
-            'max_retries': 10,
-            'max_retry_after': 180,
-            'min_calls_remaining': 1,
-            'redirect_url': None,
-            'refresh_token': None,
-            'retry_backoff_seconds': 0.5,
-        }
-        self.update_tokens(apiArgs)
-        self._logger = logging.getLogger('pyzohoapi')
-
-    def auth_header(self):
-        """ Returns the authorization header, refreshing the access_token as needed.
-
-        :return: {'Authorization': '... access token ...'}
-        :raises ZohoAuthRefreshFailure: if a refresh attemp fails.
-        :raises ZohoInsufficentAuthKeys: if we don't have enough info to refresh.
-        """
-        if self._api_keys.get('access_token') and self._api_keys['AccessExpiresAt'] > datetime.datetime.now().timestamp():
-            return {'Authorization': f"Zoho-oauthtoken {self._api_keys['access_token']}"}
-        if self._api_keys.get('refresh_token'):
-            self.log("requesting new access token")
-            rsp = requests.post(f"{self._oauth}/token", params={
-                'refresh_token': self._api_keys['refresh_token'],
-                'client_id': self._api_keys['client_id'],
-                'client_secret': self._api_keys['client_secret'],
-                'redirect_url': self._api_keys['redirect_url'],
-                'grant_type': "refresh_token"
-            })
-            if rsp.ok:
-                self.update_tokens(rsp.json())
-                return {'Authorization': f"Zoho-oauthtoken {self._api_keys['access_token']}"}
-            raise ZohoAuthRefreshFailure()
-        raise ZohoInsufficentAuthKeys()
-
-    def do_request(self, requestFunc, url, body=None, files=None):
-        if self._api_keys['min_calls_remaining'] >= int(self._ratelimit['remaining']):
-            if self._ratelimit['ResetAt'] > datetime.datetime.now():
-                self.log("API call limit exceeded")
-                raise ZohoAPICallsExceeded()
-
-        now = datetime.datetime.now().timestamp()
-        if now < self._ratelimit['NextCall']:
-            self.log("pausing for internal API rate limit")
-            sleep(self._ratelimit['NextCall'] - now)
-
-        retries = self._api_keys['max_retries']
-        while True:
-            reqparams = {
-                'headers': self.auth_header(),
-                'files': files,
-                'json': body,
-            }
-            rsp = requestFunc(url, **reqparams)
-            self._ratelimit['NextCall'] = datetime.datetime.now().timestamp() + self._api_keys['intercall_delay']
-            if rsp.status_code == 429 and retries:  # Too Many Requests
-                retries -= 1
-                sleeptime = int(rsp.headers.get('retry-after', self._api_keys['retry_backoff_seconds']))
-                if sleeptime <= self._api_keys['max_retry_after']:
-                    self.log("pausing before retry")
-                    sleep(sleeptime)
-                else:
-                    raise ZohoAPIThrottled()
-            elif not rsp.ok:
-                err_params = {
-                    'code': rsp.status_code,
-                    'url': url,
-                    'msg': f"Encountered #{rsp.status_code} error calling Zoho API",
-                }
-                if rsp.headers.get('content-type',"").startswith("application/json"):
-                    d = rsp.json()
-                    err_params.update({'zoho_code': d.get('code'), 'zoho_msg': d.get('message',"")})
-                if rsp.status_code == 401:
-                    self._api_keys['access_token'] = None
-                    retries -= 1
-                    if retries:
-                        continue
-                raise {
-                    '400': ZohoBadRequest,
-                    '401': ZohoUnauthorized,
-                    '404': ZohoNotFound,
-                    '405': ZohoMethodNotAllowed,
-                }.get(str(rsp.status_code), ZohoException)(**err_params)
-            else:
-                if rsp.headers['content-type'].startswith("application/json"):
-                    d = rsp.json()
-                    if d.get('code') == 0:
-                        self.update_rate_limit(rsp.headers)
-                        return rsp
-                    elif d.get('code') == "43" and retries:    # Throttled
-                        retries -= 1
-                        sleeptime = int(rsp.headers.get('retry-after', self._api_keys['retry_backoff_seconds']))
-                        if sleeptime <= self._api_keys['max_retry_after']:
-                            self.log("pausing before retry")
-                            sleep(sleeptime)
-                        else:
-                            raise ZohoAPIThrottled()
-                else:
-                    return rsp
-
-    def delete(self, urlFragment):
-        url = f"{self._endpoint}/{urlFragment}?organization={self._org}"
-        self.log(f"DELETE {url}")
-        rsp = self.do_request(requests.delete, url)
-        return rsp.ok
-
-    def get(self, urlFragment, queryString):
-        url = f"{self._endpoint}/{urlFragment}?organization={self._org}&{queryString}"
-        self.log(f"GET {url}")
-        rsp = self.do_request(requests.get, url)
-        if rsp.headers['content-type'].startswith("application/json"):
-            data = rsp.json()
-            if data['code'] == 0:
-                return data
-            raise ZohoException(f"zoho returned {data['code']}: {data['message']}")
-        return DottedDict({
-            'content': rsp.content,
-            'content_type': rsp.headers['content-type'],
-        })
-
-    def get_endpoint(self, region):
-        # This MUST be overridden in subclasses for the APIs to work.
-        # It's only here in the base class for testing
-        return False
-
-    def log(self, message, level=logging.DEBUG):
-        self._logger.log(level, f"{self.__class__.__name__} (Org# {self._org}): {message}")
-
-    def post(self, urlFragment, data=None, queryString="", files=None):
-        url = f"{self._endpoint}/{urlFragment}?organization={self._org}&{queryString}"
-        self.log(f"POST {url}")
-        rsp = self.do_request(requests.post, url, data, files)
-        if rsp.headers['content-type'].startswith("application/json"):
-            data = rsp.json()
-            if data['code'] == 0:
-                return data
-            raise ZohoException(f"zoho returned {data['code']}: {data['message']}")
-        return {
-            'content': rsp.content,
-            'content_type': rsp.headers['content-type'],
-        }
-
-    def put(self, urlFragment, data, queryString):
-        url = f"{self._endpoint}/{urlFragment}?organization={self._org}&{queryString}"
-        self.log(f"PUT {url}")
-        rsp = self.do_request(requests.put, url, data)
-        if rsp.headers['content-type'].startswith("application/json"):
-            data = rsp.json()
-            if data['code'] == 0:
-                return data
-            raise ZohoException(f"zoho returned {data['code']}: {data['message']}")
-        return {
-            'content': rsp.content,
-            'content_type': rsp.headers['content-type'],
-        }
-
-    def update_rate_limit(self, headers):
-        for key in ['limit', 'reset', 'remaining']:
-            if headers.get(f'x-rate-limit-{key}'):
-                self._ratelimit[key] = headers[f'x-rate-limit-{key}']
-        self._ratelimit['ResetAt'] = datetime.datetime.now() + datetime.timedelta(seconds=int(self._ratelimit.get('reset', 0)))
-
-    def update_tokens(self, apiArgs):
-        self._api_keys.update(apiArgs)
-        self._api_keys['AccessExpiresAt'] = datetime.datetime.now().timestamp() + int(apiArgs.get('expires_in', 0)) - 10
-
-
-class ZohoObjectBase:
-    ID = property(lambda self: self._id)
-    IsDeleted = property(lambda self: self._id is False)
-    IsList = property(lambda self: isinstance(self._data, DottedList))
-    IsLoaded = property(lambda self: self._data is not None)
-    Number = property(lambda self: self._data[self._number_field] if isinstance(self._data, DottedDict) else None)
-
-    def __init__(self, api, id=None, **searchParams):
-        self._id = id
-        self._api = api
-        self._data = None
-        self._nextpage = None
-        if id or {k:v for k,v in searchParams.items() if isinstance(v, str)}:
-            try:
-                self._load(id=id, **searchParams)
-            except ZohoNotFound as e:
-                pass    # not found, but no need to raise this error.
-
-    def __iter__(self):
-        return self.Iter()
-
-    def __getattr__(self, key):
-        if self._data:
-            return self._data[key]
-        return None
-
-    def __repr__(self):
-        if self._id:
-            return f"{self.__class__.__name__} #{self._id}"
-        if isinstance(self._data, DottedList):
-            return f"List of {self.__class__.__name__} objects"
-        return f"New {self.__class__.__name__}"
-
-    def __setattr__(self, key, value):
-        if key.startswith('_'):
-            super().__setattr__(key, value)
-        else:
-            if not self._data:
-                self._data = DottedDict()
-            self._data[key] = value
-
-    def _load(self, page=None, **searchParams):
-        data = self._api.get(self._url_fragment(), self._query_string(**searchParams))
-        if data is None:
-            self._data = None
-        elif self._id and self._is_raw:
-            self._data = DottedDict(data)
-        else:
-            if self._id:
-                self._reload(data)
-            else:
-                if page:
-                    self._data.extend(DottedList(data.get(self._plural)))
-                else:
-                    self._data = DottedList(data.get(self._plural))
-                if data.get('page_context',{}).get('has_more_page'):
-                    self._searchParams = searchParams
-                    self._nextpage = data['page_context']['page'] + 1
-                else:
-                    self._nextpage = None
-
-    @staticmethod
-    def _passes_filter(obj, filterFunc=None, **filters):
-        """ Utility function for filtering object lists
-        """
-        if filterFunc and not filterFunc(obj):
-            return False
-        for k,v in filters.items():
-            if k in obj and obj[k] != v:
-                return False
-        return True
-
-    def _query_string(self, **queryArgs):
-        qs = "&".join([f"{k}={v}" for (k,v) in queryArgs.items() if v])
-        if self._nextpage:
-            qs += f"&page={self._nextpage}"
-        return qs
-
-    def _reload(self, data):
-        self._orig = data.get(self._singular)
-        self._data = DottedDict(self._orig)
-        self._id = self._data.get(self._id_field)
-
-    def _url_fragment(self, id=None, extraPath=[]):
-        if self._id or id:
-            return f"{self._type}/{id if id else self._id}/{'/'.join(extraPath)}"
-        else:
-            return self._type
-
-    def get(self, key, default=None):
-        if self._id:
-            return self._data.get(key, default)
-        return default
-
-    def Create(self, **qParams):
-        """ Create this object in Zoho
-
-        :return: `self` as created by Zoho
-        :raises ZohoInvalidOpError: if `self` isn't "new"
-        """
-        if not self._id:
-            newData = self._api.post(self._url_fragment(), self._data.to_python(), self._query_string(**qParams))
-            if newData:
-                self._reload(newData)
-            return self
-        raise ZohoInvalidOpError("Create", self)
-
-    def Delete(self):
-        """ Delete this object from Zoho
-
-        :return: `self`
-        :raises ZohoInvalidOpError: if `self` isn't "single-object"
-        """
-        if self._id:
-            if self._api.delete(self._url_fragment()):
-                self._id = False
-                self._data[self._id_field] = None
-            return self
-        raise ZohoInvalidOpError("Delete", self)
-
-    def First(self, **kwargs):
-        """ Get the first ZohoObject from the list.
-
-        If kwargs are provided, they are used to filter what counts as "first."
-
-        :return: a ZohoObject
-        """
-        if self._data == None:
-            # We were a "new" object, but need to become a list-of
-            self._load()
-        if isinstance(self._data, DottedList) and len(self._data):
-            if kwargs:
-                rval = None
-                for _ in self.Iter(raw=True, **kwargs): rval = _; break;
-                if rval:
-                    return self.__class__(self._api, rval[self._id_field])
-            else:
-                return self.__class__(self._api, self._data[0][self._id_field])
-        return self.__class__(self._api)
-
-    def GetRelated(self, targetType, key):
-        if self._id and self._data:
-            if isinstance(self._data.get(key), str):
-                return targetType(self._data[key])
-        raise ZohoInvalidOpError("GetRelated", self)
-
-    def Iter(self, filterFunc=None, raw=False, **filter):
-        """ Iterate over the list of ZohoObjects
-
-        If called on a non-connected ("new") object, we get the list of ALL objects
-
-        :param filterFunc: function which takes the item to test, returning True or False
-        :param raw: return the raw list data?
-        :param filter: fields/values to filter the list by
-        :return: iterable of ZohoObjects (technically, a generator)
-        """
-        if self._id:
-            return [self]
-        if not self.IsLoaded:
-            self._load()
-
-        if self.IsLoaded:
-            start = 0
-            while start < len(self._data) or self._nextpage:
-                if start >= len(self._data):
-                    self._load(page=self._nextpage, **self._searchParams)
-
-                item = self._data[start]
-                if self._passes_filter(item, filterFunc=filterFunc, **filter):
-                    if raw:
-                        yield item
-                    else:
-                        yield self.__class__(self._api, id=item[self._id_field])
-                start += 1
-        else:
-            return []
-
-    def IterRelatedList(self, targetType, listKey, idField):
-        if self._id and self._data:
-            for item in self._data.get(listKey, []):
-                yield targetType(item.get(idField))
-        else:
-            raise ZohoInvalidOpError("IterRelatedList", self)
-
-    def MapRelatedList(self, targetType, listKey, idField):
-        if self._id and self._data:
-            for item in self._data.get(listKey, []):
-                yield DottedDict({'meta': item.to_python(), 'object': targetType(item.get(idField))})
-        else:
-            raise ZohoInvalidOpError("MapRelatedList", self)
-
-    def Update(self):
-        if self._id and self._data:
-            updated = diff(self._orig, self._data.to_python())
-            if updated:
-                # Maybe we don't need this; testing must ensue
-                # for k in self._req_fields:
-                #     if self._data.get(k):
-                #         updated[k] = self._data[k]
-                data = self._api.put(self._url_fragment(), updated, "")
-                self._reload(data)
-            return self
-        raise ZohoInvalidOpError("Update", self)
+# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
+# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
+
+import datetime
+import logging
+from time import sleep
+
+import requests
+import simplejson
+
+from .collection import DottedDict, DottedList
+from .utils import diff
+from ..exceptions import ZohoAPICallsExceeded, ZohoAPIThrottled, ZohoAuthRefreshFailure, ZohoBadRequest, ZohoException, ZohoInsufficientAuthKeys, ZohoInvalidOpError, ZohoMethodNotAllowed, ZohoNotFound, ZohoUnauthorized, ZohoUnknownRegionException
+
+logging.getLogger('pyzohoapi').addHandler(logging.NullHandler())
+
+class ZohoAPIBase:
+    _regionmap = {
+        # US
+        'us': "com",
+        'com': "com",
+        # India
+        'in': "in",
+        'india': "in",
+        # Europe
+        'eu': "eu",
+        'europe': "eu",
+        # Japan
+        "jp": "jp",
+        "japan": "jp",
+        # Canada
+        "cn": "com.cn",
+        "canada": "com.cn",
+        # Australia
+        'australia': "com.au",
+        'com.au': "com.au",
+    }
+    def __init__(self, organization_id, region="us", **apiArgs):
+        """ Constructor
+
+        :param organization_id: Zoho Organization ID to which to connect
+        :type organization_id: str
+        :param region: Zoho Data Center Region. Defaults to "us".
+        :type region: str
+        :param **apiArgs: additional parameters for API operation.
+        :raises ZohoUnknownRegionException: if the region is unknown or invalid.
+
+        """
+        region = region.lower()
+        if region not in self._regionmap:
+            raise ZohoUnknownRegionException(region)
+        self._org = organization_id
+        self._endpoint = self.get_endpoint(region)
+        self._oauth = f"https://accounts.zoho.{self._regionmap[region]}/oauth/v2"
+        self._ratelimit = {
+            'limit': None,
+            'NextCall': datetime.datetime.now().timestamp(),
+            'remaining': 99999999,
+            'reset': None,
+        }
+        self._api_keys = {
+            'access_token': None,
+            'client_id': None,
+            'client_secret': None,
+            'intercall_delay': 0,
+            'max_retries': 10,
+            'max_retry_after': 180,
+            'min_calls_remaining': 1,
+            'redirect_url': None,
+            'refresh_token': None,
+            'retry_backoff_seconds': 0.5,
+        }
+        self.update_tokens(apiArgs)
+        self._logger = logging.getLogger('pyzohoapi')
+
+    def auth_header(self):
+        """ Returns the authorization header, refreshing the access_token as needed.
+
+        :return: {'Authorization': '... access token ...'}
+        :raises ZohoAuthRefreshFailure: if a refresh attempt fails.
+        :raises ZohoInsufficientAuthKeys: if we don't have enough info to refresh.
+        """
+        if self._api_keys.get('access_token') and self._api_keys['AccessExpiresAt'] > datetime.datetime.now().timestamp():
+            return {'Authorization': f"Zoho-oauthtoken {self._api_keys['access_token']}"}
+        if self._api_keys.get('refresh_token'):
+            self.log("requesting new access token")
+            rsp = requests.post(f"{self._oauth}/token", params={
+                'refresh_token': self._api_keys['refresh_token'],
+                'client_id': self._api_keys['client_id'],
+                'client_secret': self._api_keys['client_secret'],
+                'redirect_url': self._api_keys['redirect_url'],
+                'grant_type': "refresh_token"
+            })
+            if rsp.ok:
+                self.update_tokens(rsp.json())
+                return {'Authorization': f"Zoho-oauthtoken {self._api_keys['access_token']}"}
+            raise ZohoAuthRefreshFailure()
+        raise ZohoInsufficientAuthKeys()
+
+    def do_request(self, requestFunc, url, body=None, files=None):
+        if self._api_keys['min_calls_remaining'] >= int(self._ratelimit['remaining']):
+            if self._ratelimit['ResetAt'] > datetime.datetime.now():
+                self.log("API call limit exceeded")
+                raise ZohoAPICallsExceeded()
+
+        now = datetime.datetime.now().timestamp()
+        if now < self._ratelimit['NextCall']:
+            self.log("pausing for internal API rate limit")
+            sleep(self._ratelimit['NextCall'] - now)
+
+        retries = self._api_keys['max_retries']
+        while True:
+            reqparams = {
+                'headers': self.auth_header(),
+                'files': files,
+                'data': simplejson.dumps(body) if body else None,
+            }
+            rsp = requestFunc(url, **reqparams)
+            self._ratelimit['NextCall'] = datetime.datetime.now().timestamp() + self._api_keys['intercall_delay']
+            if rsp.status_code == 429 and retries:  # Too Many Requests
+                retries -= 1
+                sleeptime = int(rsp.headers.get('retry-after', self._api_keys['retry_backoff_seconds']))
+                if sleeptime <= self._api_keys['max_retry_after']:
+                    self.log("pausing before retry")
+                    sleep(sleeptime)
+                else:
+                    raise ZohoAPIThrottled()
+            elif not rsp.ok:
+                err_params = {
+                    'code': rsp.status_code,
+                    'url': url,
+                    'msg': f"Encountered #{rsp.status_code} error calling Zoho API",
+                }
+                if rsp.headers.get('content-type',"").startswith("application/json"):
+                    d = rsp.json()
+                    err_params.update({'zoho_code': d.get('code'), 'zoho_msg': d.get('message',"")})
+                if rsp.status_code == 401:
+                    self._api_keys['access_token'] = None
+                    retries -= 1
+                    if retries:
+                        continue
+                raise {
+                    '400': ZohoBadRequest,
+                    '401': ZohoUnauthorized,
+                    '404': ZohoNotFound,
+                    '405': ZohoMethodNotAllowed,
+                }.get(str(rsp.status_code), ZohoException)(**err_params)
+            else:
+                if rsp.headers['content-type'].startswith("application/json"):
+                    d = rsp.json()
+                    if d.get('code') == 0:
+                        self.update_rate_limit(rsp.headers)
+                        return rsp
+                    elif d.get('code') == "43" and retries:    # Throttled
+                        retries -= 1
+                        sleeptime = int(rsp.headers.get('retry-after', self._api_keys['retry_backoff_seconds']))
+                        if sleeptime <= self._api_keys['max_retry_after']:
+                            self.log("pausing before retry")
+                            sleep(sleeptime)
+                        else:
+                            raise ZohoAPIThrottled()
+                else:
+                    return rsp
+
+    def delete(self, urlFragment):
+        url = f"{self._endpoint}/{urlFragment}?organization_id={self._org}"
+        self.log(f"DELETE {url}")
+        rsp = self.do_request(requests.delete, url)
+        return rsp.ok
+
+    def get(self, urlFragment, queryString):
+        url = f"{self._endpoint}/{urlFragment}?organization_id={self._org}&{queryString}"
+        self.log(f"GET {url}")
+        rsp = self.do_request(requests.get, url)
+        if rsp.headers['content-type'].startswith("application/json"):
+            data = simplejson.loads(rsp.text, use_decimal=True)
+            if data['code'] == 0:
+                return data
+            raise ZohoException(f"zoho returned {data['code']}: {data['message']}")
+        return DottedDict({
+            'content': rsp.content,
+            'content_type': rsp.headers['content-type'],
+        })
+
+    def get_endpoint(self, region):
+        # This MUST be overridden in subclasses for the APIs to work.
+        # It's only here in the base class for testing
+        return False
+
+    def log(self, message, level=logging.DEBUG):
+        self._logger.log(level, f"{self.__class__.__name__} (Org# {self._org}): {message}")
+
+    def post(self, urlFragment, data=None, queryString="", files=None):
+        url = f"{self._endpoint}/{urlFragment}?organization_id={self._org}&{queryString}"
+        self.log(f"POST {url}")
+        rsp = self.do_request(requests.post, url, data, files)
+        if rsp.headers['content-type'].startswith("application/json"):
+            data = simplejson.loads(rsp.text, use_decimal=True)
+            if data['code'] == 0:
+                return data
+            raise ZohoException(f"zoho returned {data['code']}: {data['message']}")
+        return {
+            'content': rsp.content,
+            'content_type': rsp.headers['content-type'],
+        }
+
+    def put(self, urlFragment, data, queryString):
+        url = f"{self._endpoint}/{urlFragment}?organization_id={self._org}&{queryString}"
+        self.log(f"PUT {url}")
+        rsp = self.do_request(requests.put, url, data)
+        if rsp.headers['content-type'].startswith("application/json"):
+            data = simplejson.loads(rsp.text, use_decimal=True)
+            if data['code'] == 0:
+                return data
+            raise ZohoException(f"zoho returned {data['code']}: {data['message']}")
+        return {
+            'content': rsp.content,
+            'content_type': rsp.headers['content-type'],
+        }
+
+    def update_rate_limit(self, headers):
+        for key in ['limit', 'reset', 'remaining']:
+            if headers.get(f'x-rate-limit-{key}'):
+                self._ratelimit[key] = headers[f'x-rate-limit-{key}']
+        self._ratelimit['ResetAt'] = datetime.datetime.now() + datetime.timedelta(seconds=int(self._ratelimit.get('reset', 0)))
+
+    def update_tokens(self, apiArgs):
+        self._api_keys.update(apiArgs)
+        # we subtract a few ticks from our expiry time, to cushion against drift
+        self._api_keys['AccessExpiresAt'] = datetime.datetime.now().timestamp() + int(apiArgs.get('expires_in', 0)) - 10
+
+
+class ZohoObjectBase:
+    ID = property(lambda self: self._id)
+    IsDeleted = property(lambda self: self._id is False)
+    IsList = property(lambda self: isinstance(self._data, DottedList))
+    IsLoaded = property(lambda self: self._data is not None)
+    Number = property(lambda self: self._data[self._number_field] if isinstance(self._data, DottedDict) else None)
+
+    def __init__(self, api, id=None, **searchParams):
+        self._id = id
+        self._api = api
+        self._data = None
+        self._nextpage = None
+        if id or {k:v for k,v in searchParams.items() if isinstance(v, str)}:
+            try:
+                self._load(id=id, **searchParams)
+            except ZohoNotFound:
+                pass    # not found, but no need to raise this error.
+
+    def __iter__(self):
+        return self.Iter()
+
+    def __getattr__(self, key):
+        if self._data:
+            return self._data[key]
+        return None
+
+    def __repr__(self):
+        if self._id:
+            return f"{self.__class__.__name__} #{self._id}"
+        if isinstance(self._data, DottedList):
+            return f"List of {self.__class__.__name__} objects"
+        return f"New {self.__class__.__name__}"
+
+    def __setattr__(self, key, value):
+        if key.startswith('_'):
+            super().__setattr__(key, value)
+        else:
+            if not self._data:
+                self._data = DottedDict()
+            self._data[key] = value
+
+    def _load(self, page=None, **searchParams):
+        data = self._api.get(self._url_fragment(), self._query_string(**searchParams))
+        if data is None:
+            self._data = None
+        elif self._id and self._is_raw:
+            self._data = DottedDict(data)
+        else:
+            if self._id:
+                self._reload(data)
+            else:
+                if page:
+                    self._data.extend(DottedList(data.get(self._plural)))
+                else:
+                    self._data = DottedList(data.get(self._plural))
+                if data.get('page_context',{}).get('has_more_page'):
+                    self._searchParams = searchParams
+                    self._nextpage = data['page_context']['page'] + 1
+                else:
+                    self._nextpage = None
+
+    @staticmethod
+    def _passes_filter(obj, filterFunc=None, **filters):
+        """ Utility function for filtering object lists
+        """
+        if filterFunc and not filterFunc(obj):
+            return False
+        for k,v in filters.items():
+            if k in obj and obj[k] != v:
+                return False
+        return True
+
+    def _query_string(self, **queryArgs):
+        qs = "&".join([f"{k}={v}" for (k,v) in queryArgs.items() if v])
+        if self._nextpage:
+            qs += f"&page={self._nextpage}"
+        return qs
+
+    def _reload(self, data):
+        self._orig = data.get(self._singular)
+        self._data = DottedDict(self._orig)
+        self._id = self._data.get(self._id_field)
+
+    def _url_fragment(self, id=None, extraPath=[]):
+        if self._id or id:
+            return f"{self._type}/{id if id else self._id}/{'/'.join(extraPath)}"
+        else:
+            return self._type
+
+    def get(self, key, default=None):
+        if self._id:
+            return self._data.get(key, default)
+        return default
+
+    def Create(self, **qParams):
+        """ Create this object in Zoho
+
+        :return: `self` as created by Zoho
+        :raises ZohoInvalidOpError: if `self` isn't "new"
+        """
+        if not self._id:
+            newData = self._api.post(self._url_fragment(), self._data.to_python(), self._query_string(**qParams))
+            if newData:
+                self._reload(newData)
+            return self
+        raise ZohoInvalidOpError("Create", self)
+
+    def Delete(self):
+        """ Delete this object from Zoho
+
+        :return: `self`
+        :raises ZohoInvalidOpError: if `self` isn't "single-object"
+        """
+        if self._id:
+            if self._api.delete(self._url_fragment()):
+                self._id = False
+                self._data[self._id_field] = None
+            return self
+        raise ZohoInvalidOpError("Delete", self)
+
+    def First(self, **kwargs):
+        """ Get the first ZohoObject from the list.
+
+        If kwargs are provided, they are used to filter what counts as "first."
+
+        :return: a ZohoObject
+        """
+        if self._data is None:
+            # We were a "new" object, but need to become a list-of
+            self._load()
+        if isinstance(self._data, DottedList) and len(self._data):
+            if kwargs:
+                rval = None
+                for _ in self.Iter(raw=True, **kwargs):
+                    rval = _
+                    break
+                if rval:
+                    return self.__class__(self._api, rval[self._id_field])
+            else:
+                return self.__class__(self._api, self._data[0][self._id_field])
+        return self.__class__(self._api)
+
+    def GetRelated(self, targetType, key):
+        if self._id and self._data:
+            if isinstance(self._data.get(key), str):
+                return targetType(self._data[key])
+        raise ZohoInvalidOpError("GetRelated", self)
+
+    def Iter(self, filterFunc=None, raw=False, **filter):
+        """ Iterate over the list of ZohoObjects
+
+        If called on a non-connected ("new") object, we get the list of ALL objects
+
+        :param filterFunc: function which takes the item to test, returning True or False
+        :param raw: return the raw list data?
+        :param filter: fields/values to filter the list by
+        :return: iterable of ZohoObjects (technically, a generator)
+        """
+        if self._id:
+            return [self]
+        if not self.IsLoaded:
+            self._load()
+
+        if self.IsLoaded:
+            start = 0
+            while start < len(self._data) or self._nextpage:
+                if start >= len(self._data):
+                    self._load(page=self._nextpage, **self._searchParams)
+
+                item = self._data[start]
+                if self._passes_filter(item, filterFunc=filterFunc, **filter):
+                    if raw:
+                        yield item
+                    else:
+                        yield self.__class__(self._api, id=item[self._id_field])
+                start += 1
+        else:
+            return []
+
+    def IterRelatedList(self, targetType, listKey, idField):
+        if self._id and self._data:
+            for item in self._data.get(listKey, []):
+                yield targetType(item.get(idField))
+        else:
+            raise ZohoInvalidOpError("IterRelatedList", self)
+
+    def MapRelatedList(self, targetType, listKey, idField):
+        if self._id and self._data:
+            for item in self._data.get(listKey, []):
+                yield DottedDict({'meta': item.to_python(), 'object': targetType(item.get(idField))})
+        else:
+            raise ZohoInvalidOpError("MapRelatedList", self)
+
+    def Update(self):
+        if self._id and self._data:
+            updated = diff(self._orig, self._data.to_python())
+            if updated:
+                data = self._api.put(self._url_fragment(), updated, "")
+                self._reload(data)
+            return self
+        raise ZohoInvalidOpError("Update", self)
```

### Comparing `pyZohoAPI-0.9.1/pyzohoapi/core/collection.py` & `pyzohoapi-1.0.0/pyzohoapi/core/collection.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,379 +1,379 @@
-# -*- coding: utf-8 -*-
-
-# The MIT License (MIT)
-#
-# Copyright (c) 2014 Carlos Escribano Rey
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-
-#==============================================================================#
-# Modified slighly to include in pyZohoAPI
-# We've removed py2 support, and added upstream-but-unmerged pullreq #14
-
-import collections
-import json
-import re
-
-from abc import ABCMeta, abstractmethod
-
-class KeyOrAttributeError(KeyError, AttributeError): pass
-
-
-SPLIT_REGEX = r"(?<!\\)(\.)"
-
-
-def is_dotted_key(key):
-    """Returns True if the key has any not-escaped dot inside"""
-    return len(re.findall(SPLIT_REGEX, key)) > 0
-
-
-def split_key(key, max_keys=0):
-    parts = [x for x in re.split(SPLIT_REGEX, key) if x != "."]
-    result = []
-    while len(parts) > 0:
-        if max_keys > 0 and len(result) == max_keys:
-            break
-        result.append(parts.pop(0))
-
-    if len(parts) > 0:
-        result.append(".".join(parts))
-    return result
-
-
-class DottedCollection(object, metaclass=ABCMeta):
-    """Abstract Base Class for DottedDict and DottedDict"""
-
-    @classmethod
-    def factory(cls, initial=None):
-        """Returns a DottedDict or a DottedList based on the type of the
-        initial value, that must be a dict or a list. In other case the same
-        original value will be returned.
-        """
-        if isinstance(initial, list):
-            return DottedList(initial)
-        elif isinstance(initial, dict):
-            return DottedDict(initial)
-        else:
-            return initial
-
-    @classmethod
-    def load_json(cls, json_value):
-        """Returns a DottedCollection from a JSON string"""
-        return cls.factory(json.loads(json_value))
-
-    @classmethod
-    def _factory_by_index(cls, dotted_key):
-        """Returns the proper DottedCollection that best suits the next key in
-        the dotted_key string. First guesses the next key and then analyzes it.
-        If the next key is numeric then returns a DottedList. In other case a
-        DottedDict is returned.
-        """
-        if not isinstance(dotted_key, str):
-            next_key = str(dotted_key)
-        elif not is_dotted_key(dotted_key):
-            next_key = dotted_key
-        else:
-            next_key, tmp = split_key(dotted_key, 1)
-
-        return DottedCollection.factory([] if next_key.isdigit() else {})
-
-    def __init__(self, initial):
-        """Base constructor. If there are nested dicts or lists they are
-        transformed into DottedCollection instances.
-        """
-        if not isinstance(initial, list) and not isinstance(initial, dict):
-            raise ValueError('initial value must be a list or a dict')
-
-        self._validate_initial(initial)
-
-        self.store = initial
-
-        if isinstance(self.store, list):
-            data = enumerate(self.store)
-        else:
-            data = self.store.items()
-
-        for key, value in data:
-            try:
-                self.store[key] = DottedCollection.factory(value)
-            except ValueError:
-                pass
-
-    def _validate_initial(self, initial):
-        """Validates data so no unescaped dotted key is present."""
-        if isinstance(initial, list):
-            for item in initial:
-                self._validate_initial(item)
-        elif isinstance(initial, dict):
-            for key, item in initial.items():
-                if is_dotted_key(key):
-                    raise ValueError("{0} is not a valid key inside a "
-                                     "DottedCollection!".format(key))
-                self._validate_initial(item)
-
-    def __len__(self):
-        return len(self.store)
-
-    def __iter__(self):
-        return iter(self.store)
-
-    def __repr__(self):
-        return repr(self.store)
-
-    def to_json(self):
-        return json.dumps(self, cls=DottedJSONEncoder)
-
-    @abstractmethod
-    def __getitem__(self, name):
-        pass
-
-    @abstractmethod
-    def __setitem__(self, name, value):
-        pass
-
-    @abstractmethod
-    def __delitem__(self, name):
-        pass
-
-    @abstractmethod
-    def to_python(self):
-        pass
-
-
-class DottedList(DottedCollection, collections.abc.MutableSequence):
-    """A list with support for the dotted path syntax"""
-
-    def __init__(self, initial=None):
-        DottedCollection.__init__(
-            self,
-            [] if initial is None else list(initial)
-        )
-
-    def __getitem__(self, index):
-        if isinstance(index, slice):
-            return self.store[index]
-
-        if isinstance(index, int) \
-                or (isinstance(index, str) and index.isdigit()):
-            return self.store[int(index)]
-
-        elif isinstance(index, str) and is_dotted_key(index):
-            my_index, alt_index = split_key(index, 1)
-            target = self.store[int(my_index)]
-
-            # required by the dotted path
-            if not isinstance(target, DottedCollection):
-                raise IndexError('cannot get "{0}" in "{1}" ({2})'.format(
-                    alt_index,
-                    my_index,
-                    repr(target)
-                ))
-
-            return target[alt_index]
-
-        else:
-            raise IndexError('cannot get %s in %s' % (index, repr(self.store)))
-
-    def __setitem__(self, index, value):
-        if isinstance(index, int) \
-                or (isinstance(index, str) and index.isdigit()):
-            # If the index does not exist in the list but it's the same index
-            # we would obtain by appending the value to the list we actually
-            # append the value. (***)
-            if int(index) not in self.store and int(index) == len(self.store):
-                self.store.append(DottedCollection.factory(value))
-            else:
-                self.store[int(index)] = DottedCollection.factory(value)
-
-        elif isinstance(index, str) and is_dotted_key(index):
-            my_index, alt_index = split_key(index, 1)
-
-            # (***)
-            if int(my_index) not in self.store \
-                    and int(my_index) == len(self.store):
-                self.store.append(
-                    DottedCollection._factory_by_index(alt_index))
-
-            if not isinstance(self[int(my_index)], DottedCollection):
-                raise IndexError('cannot set "%s" in "%s" (%s)' % (
-                    alt_index, my_index, repr(self[int(my_index)])))
-
-            self[int(my_index)][alt_index] = DottedCollection.factory(value)
-
-        else:
-            raise IndexError('cannot use %s as index in %s' % (
-                index, repr(self.store)))
-
-    def __delitem__(self, index):
-        if isinstance(index, int) \
-                or (isinstance(index, str) and index.isdigit()):
-            del self.store[int(index)]
-
-        elif isinstance(index, str) and is_dotted_key(index):
-            my_index, alt_index = split_key(index, 1)
-            target = self.store[int(my_index)]
-
-            # required by the dotted path
-            if not isinstance(target, DottedCollection):
-                raise IndexError('cannot delete "%s" in "%s" (%s)' % (
-                    alt_index, my_index, repr(target)))
-
-            del target[alt_index]
-
-        else:
-            raise IndexError('cannot delete %s in %s' % (
-                index, repr(self.store)))
-
-    def to_python(self):
-        """Returns a plain python list and converts to plain python objects all
-        this object's descendants.
-        """
-        result = list(self)
-
-        for index, value in enumerate(result):
-            if isinstance(value, DottedCollection):
-                result[index] = value.to_python()
-
-        return result
-
-    def insert(self, index, value):
-        self.store.insert(index, value)
-
-
-class DottedDict(DottedCollection, collections.abc.MutableMapping):
-    """A dict with support for the dotted path syntax"""
-    def __init__(self, initial=None):
-        DottedCollection.__init__(
-            self,
-            {} if initial is None else dict(initial)
-        )
-
-    def __getitem__(self, k):
-        key = self.__keytransform__(k)
-
-        if not isinstance(k, str) or not is_dotted_key(key):
-            try:
-                return self.store[key]
-            except KeyError as e:
-                raise KeyOrAttributeError(e)
-
-        my_key, alt_key = split_key(key, 1)
-        target = self.store[my_key]
-
-        # required by the dotted path
-        if not isinstance(target, DottedCollection):
-            raise KeyError('cannot get "{0}" in "{1}" ({2})'.format(
-                alt_key,
-                my_key,
-                repr(target)
-            ))
-
-        return target[alt_key]
-
-    def __setitem__(self, k, value):
-        key = self.__keytransform__(k)
-
-        if not isinstance(k, str):
-            raise KeyError('DottedDict keys must be str or unicode')
-        elif not is_dotted_key(key):
-            self.store[key] = DottedCollection.factory(value)
-        else:
-            my_key, alt_key = split_key(key, 1)
-
-            if my_key not in self.store:
-                self.store[my_key] = DottedCollection._factory_by_index(alt_key)
-
-            self.store[my_key][alt_key] = value
-
-    def __delitem__(self, k):
-        key = self.__keytransform__(k)
-
-        if not isinstance(k, str) or not is_dotted_key(key):
-            del self.store[key]
-
-        else:
-            my_key, alt_key = split_key(key, 1)
-            target = self.store[my_key]
-
-            if not isinstance(target, DottedCollection):
-                raise KeyError('cannot delete "{0}" in "{1}" ({2})'.format(
-                    alt_key,
-                    my_key,
-                    repr(target)
-                ))
-
-            del target[alt_key]
-
-    def to_python(self):
-        """Returns a plain python dict and converts to plain python objects all
-        this object's descendants.
-        """
-        result = dict(self)
-
-        for key, value in result.items():
-            if isinstance(value, DottedCollection):
-                result[key] = value.to_python()
-
-        return result
-
-    __getattr__ = __getitem__
-
-    # self.store does not exist before __init__() initializes it
-
-    def __setattr__(self, key, value):
-        if key in self.__dict__ or key == 'store':
-            object.__setattr__(self, key, value)
-        else:
-            self.__setitem__(key, value)
-
-    def __delattr__(self, key):
-        if key in self.__dict__ or key == 'store':
-            object.__delattr__(self, key)
-        else:
-            self.__delitem__(key)
-
-    def __contains__(self, k):
-        key = self.__keytransform__(k)
-
-        if not isinstance(k, str) or not is_dotted_key(key):
-            return self.store.__contains__(key)
-
-        my_key, alt_key = split_key(key, 1)
-        target = self.store[my_key]
-
-        if not isinstance(target, DottedCollection):
-            return False
-
-        return alt_key in target
-
-    def __keytransform__(self, key):
-        return key
-
-
-#
-# JSON stuff
-#
-
-
-class DottedJSONEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, DottedCollection):
-            return obj.store
-        else:
-            return json.JSONEncoder.default(obj)
+# -*- coding: utf-8 -*-
+
+# The MIT License (MIT)
+#
+# Copyright (c) 2014 Carlos Escribano Rey
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+
+#==============================================================================#
+# Modified slighly to include in pyZohoAPI
+# We've removed py2 support, and added upstream-but-unmerged pullreq #14
+
+import collections
+import json
+import re
+
+from abc import ABCMeta, abstractmethod
+
+class KeyOrAttributeError(KeyError, AttributeError): pass
+
+
+SPLIT_REGEX = r"(?<!\\)(\.)"
+
+
+def is_dotted_key(key):
+    """Returns True if the key has any not-escaped dot inside"""
+    return len(re.findall(SPLIT_REGEX, key)) > 0
+
+
+def split_key(key, max_keys=0):
+    parts = [x for x in re.split(SPLIT_REGEX, key) if x != "."]
+    result = []
+    while len(parts) > 0:
+        if max_keys > 0 and len(result) == max_keys:
+            break
+        result.append(parts.pop(0))
+
+    if len(parts) > 0:
+        result.append(".".join(parts))
+    return result
+
+
+class DottedCollection(object, metaclass=ABCMeta):
+    """Abstract Base Class for DottedDict and DottedDict"""
+
+    @classmethod
+    def factory(cls, initial=None):
+        """Returns a DottedDict or a DottedList based on the type of the
+        initial value, that must be a dict or a list. In other case the same
+        original value will be returned.
+        """
+        if isinstance(initial, list):
+            return DottedList(initial)
+        elif isinstance(initial, dict):
+            return DottedDict(initial)
+        else:
+            return initial
+
+    @classmethod
+    def load_json(cls, json_value):
+        """Returns a DottedCollection from a JSON string"""
+        return cls.factory(json.loads(json_value))
+
+    @classmethod
+    def _factory_by_index(cls, dotted_key):
+        """Returns the proper DottedCollection that best suits the next key in
+        the dotted_key string. First guesses the next key and then analyzes it.
+        If the next key is numeric then returns a DottedList. In other case a
+        DottedDict is returned.
+        """
+        if not isinstance(dotted_key, str):
+            next_key = str(dotted_key)
+        elif not is_dotted_key(dotted_key):
+            next_key = dotted_key
+        else:
+            next_key, tmp = split_key(dotted_key, 1)
+
+        return DottedCollection.factory([] if next_key.isdigit() else {})
+
+    def __init__(self, initial):
+        """Base constructor. If there are nested dicts or lists they are
+        transformed into DottedCollection instances.
+        """
+        if not isinstance(initial, list) and not isinstance(initial, dict):
+            raise ValueError('initial value must be a list or a dict')
+
+        self._validate_initial(initial)
+
+        self.store = initial
+
+        if isinstance(self.store, list):
+            data = enumerate(self.store)
+        else:
+            data = self.store.items()
+
+        for key, value in data:
+            try:
+                self.store[key] = DottedCollection.factory(value)
+            except ValueError:
+                pass
+
+    def _validate_initial(self, initial):
+        """Validates data so no unescaped dotted key is present."""
+        if isinstance(initial, list):
+            for item in initial:
+                self._validate_initial(item)
+        elif isinstance(initial, dict):
+            for key, item in initial.items():
+                if is_dotted_key(key):
+                    raise ValueError("{0} is not a valid key inside a "
+                                     "DottedCollection!".format(key))
+                self._validate_initial(item)
+
+    def __len__(self):
+        return len(self.store)
+
+    def __iter__(self):
+        return iter(self.store)
+
+    def __repr__(self):
+        return repr(self.store)
+
+    def to_json(self):
+        return json.dumps(self, cls=DottedJSONEncoder)
+
+    @abstractmethod
+    def __getitem__(self, name):
+        pass
+
+    @abstractmethod
+    def __setitem__(self, name, value):
+        pass
+
+    @abstractmethod
+    def __delitem__(self, name):
+        pass
+
+    @abstractmethod
+    def to_python(self):
+        pass
+
+
+class DottedList(DottedCollection, collections.abc.MutableSequence):
+    """A list with support for the dotted path syntax"""
+
+    def __init__(self, initial=None):
+        DottedCollection.__init__(
+            self,
+            [] if initial is None else list(initial)
+        )
+
+    def __getitem__(self, index):
+        if isinstance(index, slice):
+            return self.store[index]
+
+        if isinstance(index, int) \
+                or (isinstance(index, str) and index.isdigit()):
+            return self.store[int(index)]
+
+        elif isinstance(index, str) and is_dotted_key(index):
+            my_index, alt_index = split_key(index, 1)
+            target = self.store[int(my_index)]
+
+            # required by the dotted path
+            if not isinstance(target, DottedCollection):
+                raise IndexError('cannot get "{0}" in "{1}" ({2})'.format(
+                    alt_index,
+                    my_index,
+                    repr(target)
+                ))
+
+            return target[alt_index]
+
+        else:
+            raise IndexError('cannot get %s in %s' % (index, repr(self.store)))
+
+    def __setitem__(self, index, value):
+        if isinstance(index, int) \
+                or (isinstance(index, str) and index.isdigit()):
+            # If the index does not exist in the list but it's the same index
+            # we would obtain by appending the value to the list we actually
+            # append the value. (***)
+            if int(index) not in self.store and int(index) == len(self.store):
+                self.store.append(DottedCollection.factory(value))
+            else:
+                self.store[int(index)] = DottedCollection.factory(value)
+
+        elif isinstance(index, str) and is_dotted_key(index):
+            my_index, alt_index = split_key(index, 1)
+
+            # (***)
+            if int(my_index) not in self.store \
+                    and int(my_index) == len(self.store):
+                self.store.append(
+                    DottedCollection._factory_by_index(alt_index))
+
+            if not isinstance(self[int(my_index)], DottedCollection):
+                raise IndexError('cannot set "%s" in "%s" (%s)' % (
+                    alt_index, my_index, repr(self[int(my_index)])))
+
+            self[int(my_index)][alt_index] = DottedCollection.factory(value)
+
+        else:
+            raise IndexError('cannot use %s as index in %s' % (
+                index, repr(self.store)))
+
+    def __delitem__(self, index):
+        if isinstance(index, int) \
+                or (isinstance(index, str) and index.isdigit()):
+            del self.store[int(index)]
+
+        elif isinstance(index, str) and is_dotted_key(index):
+            my_index, alt_index = split_key(index, 1)
+            target = self.store[int(my_index)]
+
+            # required by the dotted path
+            if not isinstance(target, DottedCollection):
+                raise IndexError('cannot delete "%s" in "%s" (%s)' % (
+                    alt_index, my_index, repr(target)))
+
+            del target[alt_index]
+
+        else:
+            raise IndexError('cannot delete %s in %s' % (
+                index, repr(self.store)))
+
+    def to_python(self):
+        """Returns a plain python list and converts to plain python objects all
+        this object's descendants.
+        """
+        result = list(self)
+
+        for index, value in enumerate(result):
+            if isinstance(value, DottedCollection):
+                result[index] = value.to_python()
+
+        return result
+
+    def insert(self, index, value):
+        self.store.insert(index, value)
+
+
+class DottedDict(DottedCollection, collections.abc.MutableMapping):
+    """A dict with support for the dotted path syntax"""
+    def __init__(self, initial=None):
+        DottedCollection.__init__(
+            self,
+            {} if initial is None else dict(initial)
+        )
+
+    def __getitem__(self, k):
+        key = self.__keytransform__(k)
+
+        if not isinstance(k, str) or not is_dotted_key(key):
+            try:
+                return self.store[key]
+            except KeyError as e:
+                raise KeyOrAttributeError(e)
+
+        my_key, alt_key = split_key(key, 1)
+        target = self.store[my_key]
+
+        # required by the dotted path
+        if not isinstance(target, DottedCollection):
+            raise KeyError('cannot get "{0}" in "{1}" ({2})'.format(
+                alt_key,
+                my_key,
+                repr(target)
+            ))
+
+        return target[alt_key]
+
+    def __setitem__(self, k, value):
+        key = self.__keytransform__(k)
+
+        if not isinstance(k, str):
+            raise KeyError('DottedDict keys must be str or unicode')
+        elif not is_dotted_key(key):
+            self.store[key] = DottedCollection.factory(value)
+        else:
+            my_key, alt_key = split_key(key, 1)
+
+            if my_key not in self.store:
+                self.store[my_key] = DottedCollection._factory_by_index(alt_key)
+
+            self.store[my_key][alt_key] = value
+
+    def __delitem__(self, k):
+        key = self.__keytransform__(k)
+
+        if not isinstance(k, str) or not is_dotted_key(key):
+            del self.store[key]
+
+        else:
+            my_key, alt_key = split_key(key, 1)
+            target = self.store[my_key]
+
+            if not isinstance(target, DottedCollection):
+                raise KeyError('cannot delete "{0}" in "{1}" ({2})'.format(
+                    alt_key,
+                    my_key,
+                    repr(target)
+                ))
+
+            del target[alt_key]
+
+    def to_python(self):
+        """Returns a plain python dict and converts to plain python objects all
+        this object's descendants.
+        """
+        result = dict(self)
+
+        for key, value in result.items():
+            if isinstance(value, DottedCollection):
+                result[key] = value.to_python()
+
+        return result
+
+    __getattr__ = __getitem__
+
+    # self.store does not exist before __init__() initializes it
+
+    def __setattr__(self, key, value):
+        if key in self.__dict__ or key == 'store':
+            object.__setattr__(self, key, value)
+        else:
+            self.__setitem__(key, value)
+
+    def __delattr__(self, key):
+        if key in self.__dict__ or key == 'store':
+            object.__delattr__(self, key)
+        else:
+            self.__delitem__(key)
+
+    def __contains__(self, k):
+        key = self.__keytransform__(k)
+
+        if not isinstance(k, str) or not is_dotted_key(key):
+            return self.store.__contains__(key)
+
+        my_key, alt_key = split_key(key, 1)
+        target = self.store[my_key]
+
+        if not isinstance(target, DottedCollection):
+            return False
+
+        return alt_key in target
+
+    def __keytransform__(self, key):
+        return key
+
+
+#
+# JSON stuff
+#
+
+
+class DottedJSONEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, DottedCollection):
+            return obj.store
+        else:
+            return json.JSONEncoder.default(obj)
```

### Comparing `pyZohoAPI-0.9.1/pyzohoapi/exceptions/__init__.py` & `pyzohoapi-1.0.0/pyzohoapi/exceptions/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
-# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
-
-class ZohoException(Exception):
-    def __init__(self, msg="Unspecified Error", **kwargs):
-        super().__init__(msg)
-
-#---------------------------------------------------------------------------
-# Exceptions raised by API objects
-
-class ZohoAuthRefreshFailure(ZohoException):
-    def __init__(self):
-        super().__init__("Unable to refresh access token")
-
-
-class ZohoInsufficentAuthKeys(ZohoException):
-    def __init__(self):
-        super().__init__("Unable to generate Authorization header")
-
-
-class ZohoUnknownRegionException(ZohoException):
-    def __init__(self, region):
-        super().__init__(f'Unknown Region "{region}"')
-
-
-#---------------------------------------------------------------------------
-# Exceptions raised by Zoho objects
-
-class ZohoAPICallsExceeded(ZohoException):
-    def __init__(self):
-        super().__init__("No API Calls remaining")
-
-
-class ZohoAPIThrottled(ZohoException):
-    def __init__(self):
-        super().__init__("API Throttled")
-
-
-
-class ZohoBadRequest(ZohoException):
-    def __init__(self, url, zoho_code="-no code-", zoho_msg="-no message-", **kwargs):
-        super().__init__(f"Bad Request (HTTP-400)\n{zoho_msg} (Zoho-{zoho_code})")
-
-
-class ZohoUnauthorized(ZohoException):
-    def __init__(self, **kwargs):
-        super().__init__(f"Unauthorized - Invalid Access Token (HTTP=401)")
-
-
-class ZohoNotFound(ZohoException):
-    def __init__(self, url, **kwargs):
-        super().__init__(f"Not Found: '{url}' (HTTP-404)")
-
-
-class ZohoMethodNotAllowed(ZohoException):
-    def __init__(self, url, **kwargs):
-        super().__init__(f"Method not allowed on '{url}' (HTTP-405)")
-
-
-class ZohoInvalidOpError(ZohoException):
-    def __init__(self, op, target):
-        if target.ID is False:
-            super().__init__(f"Can't call {op} on a deleted {target.__class__.__name__}")
-        elif target.IsList:
-            super().__init__(f"Can't call {op} on a list-of {target.__class__.__name__}")
-        else:
-            # TODO: revise this message, provided we find a use for it
-            super().__init__(f"Can't call {op} on an object of type {target.__class__.__name__}")
+# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
+# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
+
+class ZohoException(Exception):
+    def __init__(self, msg="Unspecified Error", **kwargs):
+        super().__init__(msg)
+
+#---------------------------------------------------------------------------
+# Exceptions raised by API objects
+
+class ZohoAuthRefreshFailure(ZohoException):
+    def __init__(self):
+        super().__init__("Unable to refresh access token")
+
+
+class ZohoInsufficientAuthKeys(ZohoException):
+    def __init__(self):
+        super().__init__("Unable to generate Authorization header")
+
+
+class ZohoUnknownRegionException(ZohoException):
+    def __init__(self, region):
+        super().__init__(f'Unknown Region "{region}"')
+
+
+#---------------------------------------------------------------------------
+# Exceptions raised by Zoho objects
+
+class ZohoAPICallsExceeded(ZohoException):
+    def __init__(self):
+        super().__init__("No API Calls remaining")
+
+
+class ZohoAPIThrottled(ZohoException):
+    def __init__(self):
+        super().__init__("API Throttled")
+
+
+
+class ZohoBadRequest(ZohoException):
+    def __init__(self, url, zoho_code="-no code-", zoho_msg="-no message-", **kwargs):
+        super().__init__(f"Bad Request (HTTP-400)\n{zoho_msg} (Zoho-{zoho_code})")
+
+
+class ZohoUnauthorized(ZohoException):
+    def __init__(self, **kwargs):
+        super().__init__(f"Unauthorized - Invalid Access Token (HTTP=401)")
+
+
+class ZohoNotFound(ZohoException):
+    def __init__(self, url, **kwargs):
+        super().__init__(f"Not Found: '{url}' (HTTP-404)")
+
+
+class ZohoMethodNotAllowed(ZohoException):
+    def __init__(self, url, **kwargs):
+        super().__init__(f"Method not allowed on '{url}' (HTTP-405)")
+
+
+class ZohoInvalidOpError(ZohoException):
+    def __init__(self, op, target):
+        if target.ID is False:
+            super().__init__(f"Can't call {op} on a deleted {target.__class__.__name__}")
+        elif target.IsList:
+            super().__init__(f"Can't call {op} on a list-of {target.__class__.__name__}")
+        else:
+            # TODO: revise this message, provided we find a use for it
+            super().__init__(f"Can't call {op} on an object of type {target.__class__.__name__}")
```

### Comparing `pyZohoAPI-0.9.1/pyzohoapi/inventory.py` & `pyzohoapi-1.0.0/pyzohoapi/inventory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
-# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
-
-from .core import ZohoAPIBase
-from . import objecttypes
-
-class ZohoInventory(ZohoAPIBase):
-    _scope = "ZohoInventory.FullAccess.all"
-
-    def get_endpoint(self, region):
-        return f"https://inventory.zoho.{self._regionmap[region]}/api/v1"
-
-    def Account(self, *args, **kwargs): return objecttypes.Account(self, *args, **kwargs)
-    def Bill(self, *args, **kwargs): return objecttypes.Bill(self, *args, **kwargs)
-    def Brand(self, *args, **kwargs): return objecttypes.Brand(self, *args, **kwargs)
-    def Bundle(self, *args, **kwargs): return objecttypes.Bundle(self, *args, **kwargs)
-    def CompositeItem(self, *args, **kwargs): return objecttypes.CompositeItem(self, *args, **kwargs)
-    def Contact(self, *args, **kwargs): return objecttypes.Contact(self, *args, **kwargs)
-    def CustomerPayment(self, *args, **kwargs): return objecttypes.CustomerPayment(self, *args, **kwargs)
-    def Currency(self, *args, **kwargs): return objecttypes.Currency(self, *args, **kwargs)
-    def Document(self, *args, **kwargs): return objecttypes.Document(self, *args, **kwargs)
-    def Invoice(self, *args, **kwargs): return objecttypes.Invoice(self, *args, **kwargs)
-    def Item(self, *args, **kwargs): return objecttypes.Item(self, *args, **kwargs)
-    def ItemAdjustment(self, *args, **kwargs): return objecttypes.ItemAdjustment(self, *args, **kwargs)
-    def ItemGroup(self, *args, **kwargs): return objecttypes.ItemGroup(self, *args, **kwargs)
-    def Organization(self, *args, **kwargs): return objecttypes.Organization(self, *args, **kwargs)
-    def Package(self, *args, **kwargs): return objecttypes.Package(self, *args, **kwargs)
-    def PriceList(self, *args, **kwargs): return objecttypes.PriceList(self, *args, **kwargs)
-    def PurchaseOrder(self, *args, **kwargs): return objecttypes.PurchaseOrder(self, *args, **kwargs)
-    def PurchaseReceive(self, *args, **kwargs): return objecttypes.PurchaseReceive(self, *args, **kwargs)
-    def RetainerInvoice(self, *args, **kwargs): return objecttypes.RetainerInvoice(self, *args, **kwargs)
-    def SalesOrder(self, *args, **kwargs): return objecttypes.SalesOrder(self, *args, **kwargs)
-    def SalesPerson(self, *args, **kwargs): return objecttypes.SalesPerson(self, *args, **kwargs)
-    def SalesReturn(self, *args, **kwargs): return objecttypes.SalesReturn(self, *args, **kwargs)
-    def ShipmentOrder(self, *args, **kwargs): return objecttypes.ShipmentOrder(self, *args, **kwargs)
-    def Tax(self, *args, **kwargs): return objecttypes.Tax(self, *args, **kwargs)
-    def TaxAuthority(self, *args, **kwargs): return objecttypes.TaxAuthority(self, *args, **kwargs)
-    def TaxExemption(self, *args, **kwargs): return objecttypes.TaxExemption(self, *args, **kwargs)
-    def TaxGroup(self, *args, **kwargs): return objecttypes.TaxGroup(self, *args, **kwargs)
-    def TransferOrder(self, *args, **kwargs): return objecttypes.TransferOrder(self, *args, **kwargs)
-    def User(self, *args, **kwargs): return objecttypes.User(self, *args, **kwargs)
-    def Warehouse(self, *args, **kwargs): return objecttypes.Warehouse(self, *args, **kwargs)
+# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
+# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
+
+from .core import ZohoAPIBase
+from . import objecttypes
+
+class ZohoInventory(ZohoAPIBase):
+    _scope = "ZohoInventory.FullAccess.all"
+
+    def get_endpoint(self, region):
+        return f"https://www.zohoapis.{self._regionmap[region]}/inventory/v1"
+
+    def Account(self, *args, **kwargs): return objecttypes.Account(self, *args, **kwargs)
+    def Bill(self, *args, **kwargs): return objecttypes.Bill(self, *args, **kwargs)
+    def Brand(self, *args, **kwargs): return objecttypes.Brand(self, *args, **kwargs)
+    def Bundle(self, *args, **kwargs): return objecttypes.Bundle(self, *args, **kwargs)
+    def CompositeItem(self, *args, **kwargs): return objecttypes.CompositeItem(self, *args, **kwargs)
+    def Contact(self, *args, **kwargs): return objecttypes.Contact(self, *args, **kwargs)
+    def CustomerPayment(self, *args, **kwargs): return objecttypes.CustomerPayment(self, *args, **kwargs)
+    def Currency(self, *args, **kwargs): return objecttypes.Currency(self, *args, **kwargs)
+    def Document(self, *args, **kwargs): return objecttypes.Document(self, *args, **kwargs)
+    def Invoice(self, *args, **kwargs): return objecttypes.Invoice(self, *args, **kwargs)
+    def Item(self, *args, **kwargs): return objecttypes.Item(self, *args, **kwargs)
+    def ItemAdjustment(self, *args, **kwargs): return objecttypes.ItemAdjustment(self, *args, **kwargs)
+    def ItemGroup(self, *args, **kwargs): return objecttypes.ItemGroup(self, *args, **kwargs)
+    def Organization(self, *args, **kwargs): return objecttypes.Organization(self, *args, **kwargs)
+    def Package(self, *args, **kwargs): return objecttypes.Package(self, *args, **kwargs)
+    def PriceList(self, *args, **kwargs): return objecttypes.PriceList(self, *args, **kwargs)
+    def PurchaseOrder(self, *args, **kwargs): return objecttypes.PurchaseOrder(self, *args, **kwargs)
+    def PurchaseReceive(self, *args, **kwargs): return objecttypes.PurchaseReceive(self, *args, **kwargs)
+    def RetainerInvoice(self, *args, **kwargs): return objecttypes.RetainerInvoice(self, *args, **kwargs)
+    def SalesOrder(self, *args, **kwargs): return objecttypes.SalesOrder(self, *args, **kwargs)
+    def SalesPerson(self, *args, **kwargs): return objecttypes.SalesPerson(self, *args, **kwargs)
+    def SalesReturn(self, *args, **kwargs): return objecttypes.SalesReturn(self, *args, **kwargs)
+    def ShipmentOrder(self, *args, **kwargs): return objecttypes.ShipmentOrder(self, *args, **kwargs)
+    def Tax(self, *args, **kwargs): return objecttypes.Tax(self, *args, **kwargs)
+    def TaxAuthority(self, *args, **kwargs): return objecttypes.TaxAuthority(self, *args, **kwargs)
+    def TaxExemption(self, *args, **kwargs): return objecttypes.TaxExemption(self, *args, **kwargs)
+    def TaxGroup(self, *args, **kwargs): return objecttypes.TaxGroup(self, *args, **kwargs)
+    def TransferOrder(self, *args, **kwargs): return objecttypes.TransferOrder(self, *args, **kwargs)
+    def User(self, *args, **kwargs): return objecttypes.User(self, *args, **kwargs)
+    def Warehouse(self, *args, **kwargs): return objecttypes.Warehouse(self, *args, **kwargs)
```

### Comparing `pyZohoAPI-0.9.1/pyzohoapi/objecttypes/__init__.py` & `pyzohoapi-1.0.0/pyzohoapi/objecttypes/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,94 @@
-# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
-# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
-
-from ..core import ZohoObjectBase
-from .mixins import *
-
-def ZohoObjectFactory(name,
-    urlPath=None, responseKey=None, pluralResponseKey=None,
-    idKey=None, numberKey=None, raw=False,
-    mixins=[]):
-    """ Factory function to create a Zoho Object type
-
-    Unless overridden by the optional paremters, `name` is used to determine how
-    Zoho API objects are accessed and parsed.
-
-    * The URL used will be https:/{api-root}/{pluralized `name` -or- `urlPath`}
-    * A list of objects is under the JSON key `pluralizedResponseKey` -or- `responseKey` pluralized -or- `name` pluralized
-    * A single object of objects is under the JSON key `responseKey` -or- `name`
-    * The object ID is under the JSON key `idKey` -or- `name` _id
-    * The object Number is under the JSON key `numberKey` -or- `name` _number
-
-    :param name: object-class name; the basis of the API URL path unless overridden.
-    :param urlPath: sets th API URL path
-    :param responseKey: sets the singular (and maybe plural) response key(s).
-    :param pluralResponseKey: sets the plural response key.
-    :param idKey: sets the id field key.
-    :param numberKey: sets the number field key.
-    :param raw: handle the response body as raw data rather than json for non-list responses
-    :param mixins: list of object-type mixins. Defaults to [].
-    :return: ZohoObject sub-class
-    """
-    return type(name, tuple([ZohoObjectBase] + mixins), {
-        '__name__': name,
-        '_type': urlPath if urlPath else f"{name.lower()}s",
-        '_singular': responseKey if responseKey else name.lower(),
-        '_plural': pluralResponseKey if pluralResponseKey else f"{responseKey}s" if responseKey else f"{name.lower()}s",
-        '_id_field': idKey if idKey else f"{name.lower()}_id",
-        '_number_field': numberKey if numberKey else f"{name.lower()}_number",
-        '_is_raw': raw,
-    })
-
-Account = ZohoObjectFactory("ChartOfAccount", idKey="account_id")
-Bill = ZohoObjectFactory("Bill", mixins=[HasCustomFields])
-Brand = ZohoObjectFactory("Brand")
-Bundle = ZohoObjectFactory("Bundle")
-CompositeItem = ZohoObjectFactory("CompositeItem",
-    responseKey="composite_item", idKey="composite_item_id",
-    mixins=[HasActivate, HasBundle, HasCustomFields])
-Contact = ZohoObjectFactory("Contact", mixins=[HasActivate, HasAddresses, HasCustomFields])
-CreditNote = ZohoObjectFactory("CreditNode", mixins=[HasCustomFields])
-Currency = ZohoObjectFactory("Currency", urlPath="settings/currencies",
-    pluralResponseKey="currencies")
-CustomerPayment = ZohoObjectFactory("CustomerPayment",
-    idKey="payment_id", numberKey="payment_number", mixins=[HasCustomFields])
-Document = ZohoObjectFactory("Document", raw=True)
-Invoice = ZohoObjectFactory("Invoice", mixins=[HasCustomFields])
-Item = ZohoObjectFactory("Item", mixins=[HasActivate, HasCustomFields, HasImage])
-ItemAdjustment = ZohoObjectFactory("ItemAdjustment",
-    urlPath="inventoryadjustments", responseKey="inventory_adjustment",
-    idKey="inventory_adjustment_id")
-ItemGroup = ZohoObjectFactory("ItemGroup", idKey="group_id",
-    responseKey="group", mixins=[HasActivate])
-Organization = ZohoObjectFactory("Organization")
-Package = ZohoObjectFactory("Package", mixins=[HasCustomFields])
-PriceList = ZohoObjectFactory("PriceList", urlPath="pricebooks",
-    responseKey="pricebook", idKey="pricebook_id",
-    mixins=[HasActivate])
-PurchaseOrder = ZohoObjectFactory("PurchaseOrder", mixins=[HasCustomFields])
-PurchaseReceive = ZohoObjectFactory("PurchaseReceive", mixins=[HasCustomFields])
-RetainerInvoice = ZohoObjectFactory("RetainerInvoice", mixins=[HasDraft, HasVoid])
-SalesOrder = ZohoObjectFactory("SalesOrder",
-    mixins=[HasConfirm, HasCustomFields, HasVoid])
-SalesPerson = ZohoObjectFactory("SalesPerson")
-SalesReturn = ZohoObjectFactory("SalesReturn")
-ShipmentOrder = ZohoObjectFactory("ShipmentOrder",
-    responseKey="shipmentorder", idKey="shipment_id",
-    numberKey="shipment_number", mixins=[HasCustomFields, HasDelivered])
-Tax = ZohoObjectFactory("Tax", urlPath="settings/taxes",
-    pluralResponseKey="taxes")
-TaxAuthority = ZohoObjectFactory("Tax", urlPath="settings/taxauthorities",
-    responseKey="tax_authority", pluralResponseKey="tax_authorities",
-    idKey="tax_authority_id")
-TaxExemption = ZohoObjectFactory("Tax", urlPath="settings/taxexemptions",
-    responseKey="tax_exemption", idKey="tax_exemption_id")
-TaxGroup = ZohoObjectFactory("Tax", urlPath="settings/taxgroups",
-    responseKey="tax_group", idKey="tax_group_id")
-TransferOrder = ZohoObjectFactory("TransferOrder",
-    responseKey="transfer_order",
-    idKey="transfer_order_id", numberKey="transfer_order_number")
-User = ZohoObjectFactory("User", mixins=[HasActivate, HasCustomFields])
-Warehouse = ZohoObjectFactory("Warehouse", urlPath="settings/warehouses",
-    mixins=[HasActivate])
+# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
+# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
+
+from pyzohoapi.objecttypes.mixins.CompositeItemOps import HasBundle
+from ..core import ZohoObjectBase
+from .mixins import HasActivate, HasAddresses, HasConfirm, HasCustomFields, HasDelivered, HasDraft, HasImage, HasVoid
+
+
+def ZohoObjectFactory(name,
+    urlPath=None, responseKey=None, pluralResponseKey=None,
+    idKey=None, numberKey=None, raw=False,
+    mixins=[]):
+    """ Factory function to create a Zoho Object type
+
+    Unless overridden by the optional parameters, `name` is used to determine how
+    Zoho API objects are accessed and parsed.
+
+    * The URL used will be https:/{api-root}/{pluralized `name` -or- `urlPath`}
+    * A list of objects is under the JSON key `pluralizedResponseKey` -or- `responseKey` pluralized -or- `name` pluralized
+    * A single object is under the JSON key `responseKey` -or- `name`
+    * The object ID is under the JSON key `idKey` -or- `{name}_id`
+    * The object Number is under the JSON key `numberKey` -or- `{name}_number`
+
+    :param name: object-class name; the basis of the API URL path unless overridden.
+    :param urlPath: sets th API URL path
+    :param responseKey: sets the singular (and maybe plural) response key(s).
+    :param pluralResponseKey: sets the plural response key.
+    :param idKey: sets the id field key.
+    :param numberKey: sets the number field key.
+    :param raw: handle the response body as raw data rather than json for non-list responses
+    :param mixins: list of object-type mixins. Defaults to [].
+    :return: ZohoObject sub-class
+    """
+    return type(name, tuple([ZohoObjectBase] + mixins), {
+        '__name__': name,
+        '_type': urlPath if urlPath else f"{name.lower()}s",
+        '_singular': responseKey if responseKey else name.lower(),
+        '_plural': pluralResponseKey if pluralResponseKey else f"{responseKey}s" if responseKey else f"{name.lower()}s",
+        '_id_field': idKey if idKey else f"{name.lower()}_id",
+        '_number_field': numberKey if numberKey else f"{name.lower()}_number",
+        '_is_raw': raw,
+    })
+
+Account = ZohoObjectFactory("ChartOfAccount", idKey="account_id")
+Bill = ZohoObjectFactory("Bill", mixins=[HasCustomFields])
+Brand = ZohoObjectFactory("Brand")
+Bundle = ZohoObjectFactory("Bundle")
+CompositeItem = ZohoObjectFactory("CompositeItem",
+    responseKey="composite_item", idKey="composite_item_id",
+    mixins=[HasActivate, HasBundle, HasCustomFields])
+Contact = ZohoObjectFactory("Contact", mixins=[HasActivate, HasAddresses, HasCustomFields])
+CreditNote = ZohoObjectFactory("CreditNode", mixins=[HasCustomFields])
+Currency = ZohoObjectFactory("Currency", urlPath="settings/currencies",
+    pluralResponseKey="currencies")
+CustomerPayment = ZohoObjectFactory("CustomerPayment",
+    idKey="payment_id", numberKey="payment_number", mixins=[HasCustomFields])
+Document = ZohoObjectFactory("Document", raw=True)
+Invoice = ZohoObjectFactory("Invoice", mixins=[HasCustomFields])
+Item = ZohoObjectFactory("Item", mixins=[HasActivate, HasCustomFields, HasImage])
+ItemAdjustment = ZohoObjectFactory("ItemAdjustment",
+    urlPath="inventoryadjustments", responseKey="inventory_adjustment",
+    idKey="inventory_adjustment_id")
+ItemGroup = ZohoObjectFactory("ItemGroup", idKey="group_id",
+    responseKey="group", mixins=[HasActivate])
+Organization = ZohoObjectFactory("Organization")
+Package = ZohoObjectFactory("Package", mixins=[HasCustomFields])
+PriceList = ZohoObjectFactory("PriceList", urlPath="pricebooks",
+    responseKey="pricebook", idKey="pricebook_id",
+    mixins=[HasActivate])
+PurchaseOrder = ZohoObjectFactory("PurchaseOrder", mixins=[HasCustomFields])
+PurchaseReceive = ZohoObjectFactory("PurchaseReceive", mixins=[HasCustomFields])
+RetainerInvoice = ZohoObjectFactory("RetainerInvoice", mixins=[HasDraft, HasVoid])
+SalesOrder = ZohoObjectFactory("SalesOrder",
+    mixins=[HasConfirm, HasCustomFields, HasVoid])
+SalesPerson = ZohoObjectFactory("SalesPerson")
+SalesReturn = ZohoObjectFactory("SalesReturn")
+ShipmentOrder = ZohoObjectFactory("ShipmentOrder",
+    responseKey="shipmentorder", idKey="shipment_id",
+    numberKey="shipment_number", mixins=[HasCustomFields, HasDelivered])
+Tax = ZohoObjectFactory("Tax", urlPath="settings/taxes",
+    pluralResponseKey="taxes")
+TaxAuthority = ZohoObjectFactory("Tax", urlPath="settings/taxauthorities",
+    responseKey="tax_authority", pluralResponseKey="tax_authorities",
+    idKey="tax_authority_id")
+TaxExemption = ZohoObjectFactory("Tax", urlPath="settings/taxexemptions",
+    responseKey="tax_exemption", idKey="tax_exemption_id")
+TaxGroup = ZohoObjectFactory("Tax", urlPath="settings/taxgroups",
+    responseKey="tax_group", idKey="tax_group_id")
+TransferOrder = ZohoObjectFactory("TransferOrder",
+    responseKey="transfer_order",
+    idKey="transfer_order_id", numberKey="transfer_order_number")
+User = ZohoObjectFactory("User", mixins=[HasActivate, HasCustomFields])
+Warehouse = ZohoObjectFactory("Warehouse", urlPath="settings/warehouses",
+    mixins=[HasActivate])
```

### Comparing `pyZohoAPI-0.9.1/pyzohoapi/objecttypes/mixins/__init__.py` & `pyzohoapi-1.0.0/pyzohoapi/objecttypes/mixins/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
-# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
-
-from ...exceptions import *
-
-from .CompositeItemOps import HasBundle
-from .CustomFields import HasCustomFields
-
-__all__ = [
-    'HasActivate',
-    'HasAddresses',
-    'HasBundle',
-    'HasConfirm', 'HasDraft', 'HasVoid', 'HasDelivered',
-    'HasCustomFields',
-    'HasImage',
-]
-
-class HasActivate:
-    """Adds `Activate()` and `Deactivate()`"""
-    def _do_operation(self, status, funcname):
-        if self._id and self._data:
-            try:
-                self._api.post(self._url_fragment(extraPath=[status]))
-                self.status = status
-                return True
-            except ZohoException as e:
-                return False
-        raise ZohoInvalidOpError(funcname, self)
-
-    def Activate(self):
-        return self._do_operation('active', "Activate")
-
-    def Deactivate(self):
-        return self._do_operation('inactive', "Deactivate")
-
-
-class HasImage:
-    """Adds `AddImage()`, `DeleteImage()` and `GetImage()`"""
-    def AddImage(self, name, image, type="image/jpeg"):
-        if self._id:
-            file = {'image': (name, image, type)}
-            return self._api.post(self._url_fragment(extraPath=['image']), files=file)
-        raise ZohoInvalidOpError("AddImage", self)
-
-    def DeleteImage(self):
-        if self._id:
-            return self._api.delete(self._url_fragment(extraPath=['image']))
-        raise ZohoInvalidOpError("AddImage", self)
-
-    def GetImage(self):
-        if self._id and self._data:
-            return self._api.get(self._url_fragment(extraPath=['image']), "")
-        raise ZohoInvalidOpError("GetImage", self)
-
-
-class _HasStatus:
-    def _mark(self, status):
-        if self._id:
-            try:
-                self._api.post(self._url_fragment(extraPath=['status', status]))
-                return True
-            except ZohoException as e:
-                return False
-        return None
-
-
-class HasConfirm(_HasStatus):
-    """Adds `Confirm()`"""
-    def Confirm(self):
-        if not self._id:
-            raise ZohoInvalidOpError("Confirm", self)
-        return self._mark('confirmed')
-
-
-class HasDelivered(_HasStatus):
-    """Adds `Delivered()`"""
-    def Delivered(self):
-        if not self._id:
-            raise ZohoInvalidOpError("Delivered", self)
-        return self._mark('delivered')
-
-
-class HasDraft(_HasStatus):
-    """Adds `Draft()`"""
-    def Draft(self):
-        if not self._id:
-            raise ZohoInvalidOpError("Draft", self)
-        return self._mark('draft')
-
-
-class HasVoid(_HasStatus):
-    """Adds `Void()`"""
-    def Void(self):
-        if not self._id:
-            raise ZohoInvalidOpError("Void", self)
-        return self._mark('void')
-
-
-class _HasAspect:
-    def _updateAspect(self, aspect, aspect_id, data):
-        data = self._api.put(self._url_fragment(extraPath=[aspect, aspect_id]), data, "")
-        if data['code'] == 0:
-            return True
-        return False
-
-
-class HasAddresses(_HasAspect):
-    """Adds `UpdateBilling()` and `UpdateShipping()`"""
-    def UpdateBilling(self):
-        if self._id and self._data:
-            self._updateAspect('address', self.billing_address.address_id, self.billing_address.to_python())
-            return self
-        raise ZohoInvalidOpError("UpdateBilling", self)
-    def UpdateShipping(self):
-        if self._id and self._data:
-            self._updateAspect('address', self.shipping_address.address_id, self.shipping_address.to_python())
-            return self
-        raise ZohoInvalidOpError("UpdateShipping", self)
+# This file is part of pyZohoAPI, Copyright (C) Todd D. Esposito 2021.
+# Distributed under the MIT License (see https://opensource.org/licenses/MIT).
+
+from ...exceptions import ZohoException, ZohoInvalidOpError
+
+from .CompositeItemOps import HasBundle
+from .CustomFields import HasCustomFields
+
+__all__ = [
+    'HasActivate',
+    'HasAddresses',
+    'HasBundle',
+    'HasConfirm', 'HasDraft', 'HasVoid', 'HasDelivered',
+    'HasCustomFields',
+    'HasImage',
+]
+
+class HasActivate:
+    """Adds `Activate()` and `Deactivate()`"""
+    def _do_operation(self, status, funcname):
+        if self._id and self._data:
+            try:
+                self._api.post(self._url_fragment(extraPath=[status]))
+                self.status = status
+                return True
+            except ZohoException as e:
+                return False
+        raise ZohoInvalidOpError(funcname, self)
+
+    def Activate(self):
+        return self._do_operation('active', "Activate")
+
+    def Deactivate(self):
+        return self._do_operation('inactive', "Deactivate")
+
+
+class HasImage:
+    """Adds `AddImage()`, `DeleteImage()` and `GetImage()`"""
+    def AddImage(self, name, image, type="image/jpeg"):
+        if self._id:
+            file = {'image': (name, image, type)}
+            return self._api.post(self._url_fragment(extraPath=['image']), files=file)
+        raise ZohoInvalidOpError("AddImage", self)
+
+    def DeleteImage(self):
+        if self._id:
+            return self._api.delete(self._url_fragment(extraPath=['image']))
+        raise ZohoInvalidOpError("AddImage", self)
+
+    def GetImage(self):
+        if self._id and self._data:
+            return self._api.get(self._url_fragment(extraPath=['image']), "")
+        raise ZohoInvalidOpError("GetImage", self)
+
+
+class _HasStatus:
+    def _mark(self, status):
+        if self._id:
+            try:
+                self._api.post(self._url_fragment(extraPath=['status', status]))
+                return True
+            except ZohoException as e:
+                return False
+        return None
+
+
+class HasConfirm(_HasStatus):
+    """Adds `Confirm()`"""
+    def Confirm(self):
+        if not self._id:
+            raise ZohoInvalidOpError("Confirm", self)
+        return self._mark('confirmed')
+
+
+class HasDelivered(_HasStatus):
+    """Adds `Delivered()`"""
+    def Delivered(self):
+        if not self._id:
+            raise ZohoInvalidOpError("Delivered", self)
+        return self._mark('delivered')
+
+
+class HasDraft(_HasStatus):
+    """Adds `Draft()`"""
+    def Draft(self):
+        if not self._id:
+            raise ZohoInvalidOpError("Draft", self)
+        return self._mark('draft')
+
+
+class HasVoid(_HasStatus):
+    """Adds `Void()`"""
+    def Void(self):
+        if not self._id:
+            raise ZohoInvalidOpError("Void", self)
+        return self._mark('void')
+
+
+class _HasAspect:
+    def _updateAspect(self, aspect, aspect_id, data):
+        data = self._api.put(self._url_fragment(extraPath=[aspect, aspect_id]), data, "")
+        if data['code'] == 0:
+            return True
+        return False
+
+
+class HasAddresses(_HasAspect):
+    """Adds `UpdateBilling()` and `UpdateShipping()`"""
+    def UpdateBilling(self):
+        if self._id and self._data:
+            self._updateAspect('address', self.billing_address.address_id, self.billing_address.to_python())
+            return self
+        raise ZohoInvalidOpError("UpdateBilling", self)
+    def UpdateShipping(self):
+        if self._id and self._data:
+            self._updateAspect('address', self.shipping_address.address_id, self.shipping_address.to_python())
+            return self
+        raise ZohoInvalidOpError("UpdateShipping", self)
```

### Comparing `pyZohoAPI-0.9.1/README.md` & `pyzohoapi-1.0.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,77 @@
-# pyZohoAPI (v0.9.1)
- **pyZohoAPI** provides Pythonic access to Zoho APIs in the Finance Plus suite:
- * **Books**
- * *Checkout*<sup>*</sup>
- * *Expense*<sup>*</sup>
- * **Inventory**
- * *Invoice*<sup>*</sup>
- * *Subscriptions*<sup>*</sup>
-
-<sup>*</sup> Support is planned, but not yet available.
-
-[![PyPI](https://img.shields.io/pypi/v/pyzohoapi)](https://pypi.org/project/pyzohoapi/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyzohoapi)](https://pypi.org/project/pyzohoapi/)
-![License](https://img.shields.io/github/license/tdesposito/pyZohoAPI)
-[![Documentation Status](https://readthedocs.org/projects/pyzohoapi/badge/?version=latest)](https://pyzohoapi.readthedocs.io/en/latest/?badge=latest)
-
-## Installing pyZohoAPI
-<!-- start installation -->
-
-You'll need at least **Python 3.6** to install pyZohoAPI.
-
-### Via PyPI
-```console
-$ python -m pip install pyzohoapi
-```
-
-### From Source
-We use [Poetry](https://python-poetry.org/) for virtual environment and
-dependency management.
-```console
-$ git clone https://github.com/tdesposito/pyZohoAPI.git
-$ cd pyZohoAPI
-$ poetry install
-$ poetry build
-$ pip install dist/*.whl
-```
-<!-- end installation -->
-
-## Basic Usage
-
-<!-- start basic-usage -->
-```python
->>> from pyzohoapi import ZohoInventory
->>> api = ZohoInventory("{your-orginization-id}", "{your-region}",
-...   client_id="{your-client-id}",
-...   client_secret="{your-client-secret}",
-...   refresh_token="{your-refresh-token}"
-... )
->>> contact = api.Contact(email="test@example.com").First()
->>> contact.IsLoaded
-True
->>> contact.first_name
-'test'
->>> contact.first_name = "Changed"
->>> contact.Update()
-```
-<!-- end basic-usage -->
-
-See the [full documentation on ReadTheDocs](https://pyzohoapi.readthedocs.io/en/latest/)
-
-## Contributing
-Pull Requests gladly considered!
+# pyZohoAPI (v1.0.0)
+
+**pyZohoAPI** provides Pythonic access to Zoho APIs in the Finance Plus suite:
+
+* **Books**
+* *Checkout*<sup>*</sup>
+* *Expense*<sup>*</sup>
+* **Inventory**
+* *Invoice*<sup>*</sup>
+* *Subscriptions*<sup>*</sup>
+
+<sup>*</sup> Support is planned, but not yet available.
+
+[![PyPI](https://img.shields.io/pypi/v/pyzohoapi)](https://pypi.org/project/pyzohoapi/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyzohoapi)](https://pypi.org/project/pyzohoapi/)
+![License](https://img.shields.io/github/license/tdesposito/pyZohoAPI)
+[![Documentation Status](https://readthedocs.org/projects/pyzohoapi/badge/?version=latest)](https://pyzohoapi.readthedocs.io/en/latest/?badge=latest)
+
+## Installing pyZohoAPI
+
+<!-- start installation -->
+
+You'll need at least **Python 3.6** to install pyZohoAPI.
+
+### Via PyPI
+
+```console
+$ python -m pip install pyzohoapi
+```
+
+### From Source
+
+We use [Poetry](https://python-poetry.org/) for virtual environment and
+dependency management.
+
+```console
+$ git clone https://github.com/tdesposito/pyZohoAPI.git
+$ cd pyZohoAPI
+$ poetry install
+$ poetry build
+$ pip install dist/*.whl
+```
+<!-- end installation -->
+
+## Basic Usage
+
+<!-- start basic-usage -->
+
+```python
+>>> from pyzohoapi import ZohoInventory
+>>> api = ZohoInventory("{your-orginization-id}", "{your-region}",
+...   client_id="{your-client-id}",
+...   client_secret="{your-client-secret}",
+...   refresh_token="{your-refresh-token}"
+... )
+>>> contact = api.Contact(email="test@example.com").First()
+>>> contact.IsLoaded
+True
+>>> contact.first_name
+'test'
+>>> contact.first_name = "Changed"
+>>> contact.Update()
+```
+<!-- end basic-usage -->
+
+See the [full documentation on ReadTheDocs](https://pyzohoapi.readthedocs.io/en/latest/).
+
+## Contributing
+
+[Pull Requests](https://github.com/tdesposito/pyZohoAPI/pulls) gladly
+considered! Please use our pull request template when submitting your pull
+request.
+
+| Thanks Contributors! |
+| :------------------: |
+| ![Shubham Agawane](https://avatars.githubusercontent.com/s-agawane?size=80) 
+[Shubham Agawane](https://github.com/s-agawane) |
```

### Comparing `pyZohoAPI-0.9.1/PKG-INFO` & `pyzohoapi-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyzohoapi
-Version: 0.9.1
+Name: pyZohoAPI
+Version: 1.0.0
 Summary: Pythonic access to Zoho APIs in the Finance Plus suite.
 Home-page: https://github.com/tdesposito/pyZohoAPI
 License: MIT
 Keywords: api,zoho api,zoho books,zoho inventory,zoho
 Author: Todd Esposito
 Author-email: todd@toddesposito.com
 Requires-Python: >=3.6,<4.0
@@ -12,61 +12,72 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: simplejson (>=3.17.5,<4.0.0)
 Project-URL: Documentation, https://pyzohoapi.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/tdesposito/pyZohoAPI
 Description-Content-Type: text/markdown
 
-# pyZohoAPI (v0.9.1)
- **pyZohoAPI** provides Pythonic access to Zoho APIs in the Finance Plus suite:
- * **Books**
- * *Checkout*<sup>*</sup>
- * *Expense*<sup>*</sup>
- * **Inventory**
- * *Invoice*<sup>*</sup>
- * *Subscriptions*<sup>*</sup>
+# pyZohoAPI (v1.0.0)
+
+**pyZohoAPI** provides Pythonic access to Zoho APIs in the Finance Plus suite:
+
+* **Books**
+* *Checkout*<sup>*</sup>
+* *Expense*<sup>*</sup>
+* **Inventory**
+* *Invoice*<sup>*</sup>
+* *Subscriptions*<sup>*</sup>
 
 <sup>*</sup> Support is planned, but not yet available.
 
 [![PyPI](https://img.shields.io/pypi/v/pyzohoapi)](https://pypi.org/project/pyzohoapi/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyzohoapi)](https://pypi.org/project/pyzohoapi/)
 ![License](https://img.shields.io/github/license/tdesposito/pyZohoAPI)
 [![Documentation Status](https://readthedocs.org/projects/pyzohoapi/badge/?version=latest)](https://pyzohoapi.readthedocs.io/en/latest/?badge=latest)
 
 ## Installing pyZohoAPI
+
 <!-- start installation -->
 
 You'll need at least **Python 3.6** to install pyZohoAPI.
 
 ### Via PyPI
+
 ```console
 $ python -m pip install pyzohoapi
 ```
 
 ### From Source
+
 We use [Poetry](https://python-poetry.org/) for virtual environment and
 dependency management.
+
 ```console
 $ git clone https://github.com/tdesposito/pyZohoAPI.git
 $ cd pyZohoAPI
 $ poetry install
 $ poetry build
 $ pip install dist/*.whl
 ```
 <!-- end installation -->
 
 ## Basic Usage
 
 <!-- start basic-usage -->
+
 ```python
 >>> from pyzohoapi import ZohoInventory
 >>> api = ZohoInventory("{your-orginization-id}", "{your-region}",
 ...   client_id="{your-client-id}",
 ...   client_secret="{your-client-secret}",
 ...   refresh_token="{your-refresh-token}"
 ... )
@@ -76,12 +87,20 @@
 >>> contact.first_name
 'test'
 >>> contact.first_name = "Changed"
 >>> contact.Update()
 ```
 <!-- end basic-usage -->
 
-See the [full documentation on ReadTheDocs](https://pyzohoapi.readthedocs.io/en/latest/)
+See the [full documentation on ReadTheDocs](https://pyzohoapi.readthedocs.io/en/latest/).
 
 ## Contributing
-Pull Requests gladly considered!
+
+[Pull Requests](https://github.com/tdesposito/pyZohoAPI/pulls) gladly
+considered! Please use our pull request template when submitting your pull
+request.
+
+| Thanks Contributors! |
+| :------------------: |
+| ![Shubham Agawane](https://avatars.githubusercontent.com/s-agawane?size=80) 
+[Shubham Agawane](https://github.com/s-agawane) |
```

