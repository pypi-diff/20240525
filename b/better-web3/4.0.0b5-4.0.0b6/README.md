# Comparing `tmp/better_web3-4.0.0b5.tar.gz` & `tmp/better_web3-4.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-4.0.0b5.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b6.tar", max compression
```

## Comparing `better_web3-4.0.0b5.tar` & `better_web3-4.0.0b6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b5/better_web3/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b5/better_web3/caip_2.py
--rw-r--r--   0        0        0    11108 2024-05-25 06:31:33.209089 better_web3-4.0.0b5/better_web3/chain.py
--rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b5/better_web3/contract.py
--rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b5/better_web3/models.py
--rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b5/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b5/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      286 2024-05-25 06:27:06.720178 better_web3-4.0.0b5/better_web3/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b5/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0      885 2024-05-25 06:27:06.721182 better_web3-4.0.0b5/better_web3/utils/__pycache__/eth.cpython-312.pyc
--rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0      707 2024-05-25 06:27:06.721687 better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-312.pyc
--rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b5/better_web3/utils/eth.py
--rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b5/better_web3/utils/other.py
--rw-r--r--   0        0        0      521 2024-05-25 06:33:26.730371 better_web3-4.0.0b5/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b5/README.md
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b6/better_web3/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b6/better_web3/caip_2.py
+-rw-r--r--   0        0        0    11093 2024-05-25 07:08:34.914763 better_web3-4.0.0b6/better_web3/chain.py
+-rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b6/better_web3/contract.py
+-rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b6/better_web3/models.py
+-rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b6/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b6/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      286 2024-05-25 06:27:06.720178 better_web3-4.0.0b6/better_web3/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0      885 2024-05-25 06:27:06.721182 better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-312.pyc
+-rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0      707 2024-05-25 06:27:06.721687 better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-312.pyc
+-rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b6/better_web3/utils/eth.py
+-rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b6/better_web3/utils/other.py
+-rw-r--r--   0        0        0      521 2024-05-25 07:09:09.142412 better_web3-4.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b6/README.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b6/PKG-INFO
```

### Comparing `better_web3-4.0.0b5/better_web3/caip_2.py` & `better_web3-4.0.0b6/better_web3/caip_2.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/better_web3/chain.py` & `better_web3-4.0.0b6/better_web3/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,22 +89,22 @@
     def proxy(self) -> Proxy | None:
         return self._proxy
 
     @proxy.setter
     def proxy(self, proxy: str | Proxy | None):
         if proxy is None:
             self._proxy = None
-            if "proxies" in self.provider._request_kwargs:
-                del self.provider._request_kwargs["proxies"]
+            if "proxy" in self.provider._request_kwargs:
+                del self.provider._request_kwargs["proxy"]
             return
 
         if isinstance(proxy, str):
             self._proxy = Proxy.from_str(proxy)
 
-        self.provider._request_kwargs["proxies"] = self._proxy.as_proxies_dict
+        self.provider._request_kwargs["proxy"] = self._proxy.as_url
 
     def tx_urls(
             self, tx_hash: HexBytes | HexStr | str,
     ) -> dict[str: str]:  # dict[explorer_name: url]
         if not self.explorers:
             raise ValueError("No explorers")
```

### Comparing `better_web3-4.0.0b5/better_web3/models.py` & `better_web3-4.0.0b6/better_web3/models.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-4.0.0b6/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/better_web3/utils/__pycache__/eth.cpython-312.pyc` & `better_web3-4.0.0b6/better_web3/utils/__pycache__/eth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-312.pyc` & `better_web3-4.0.0b6/better_web3/utils/__pycache__/other.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/pyproject.toml` & `better_web3-4.0.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "better-web3"
-version = "4.0.0.b5"
+version = "4.0.0.b6"
 description = "Web3 stuff"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/better_web3"
 packages = [{include = "better_web3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `better_web3-4.0.0b5/README.md` & `better_web3-4.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b5/PKG-INFO` & `better_web3-4.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 4.0.0b5
+Version: 4.0.0b6
 Summary: Web3 stuff
 Home-page: https://github.com/alenkimov/better_web3
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

