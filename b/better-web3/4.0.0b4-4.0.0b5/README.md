# Comparing `tmp/better_web3-4.0.0b4.tar.gz` & `tmp/better_web3-4.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-4.0.0b4.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b5.tar", max compression
```

## Comparing `better_web3-4.0.0b4.tar` & `better_web3-4.0.0b5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b4/better_web3/__init__.py
--rw-r--r--   0        0        0     1752 2024-05-25 04:36:12.324383 better_web3-4.0.0b4/better_web3/caip_2.py
--rw-r--r--   0        0        0    11052 2024-05-25 05:59:38.348397 better_web3-4.0.0b4/better_web3/chain.py
--rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b4/better_web3/contract.py
--rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b4/better_web3/models.py
--rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b4/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b4/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      698 2024-01-10 21:46:32.920666 better_web3-4.0.0b4/better_web3/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b4/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3533 2024-01-10 21:46:32.922666 better_web3-4.0.0b4/better_web3/utils/__pycache__/eth.cpython-312.pyc
--rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0      707 2024-01-10 21:46:32.927171 better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-312.pyc
--rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b4/better_web3/utils/eth.py
--rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b4/better_web3/utils/other.py
--rw-r--r--   0        0        0      521 2024-05-25 06:19:17.607211 better_web3-4.0.0b4/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b4/README.md
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b5/better_web3/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-25 06:30:15.222893 better_web3-4.0.0b5/better_web3/caip_2.py
+-rw-r--r--   0        0        0    11108 2024-05-25 06:31:33.209089 better_web3-4.0.0b5/better_web3/chain.py
+-rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b5/better_web3/contract.py
+-rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b5/better_web3/models.py
+-rw-r--r--   0        0        0      137 2024-05-25 06:19:06.436481 better_web3-4.0.0b5/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b5/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      286 2024-05-25 06:27:06.720178 better_web3-4.0.0b5/better_web3/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b5/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0      885 2024-05-25 06:27:06.721182 better_web3-4.0.0b5/better_web3/utils/__pycache__/eth.cpython-312.pyc
+-rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0      707 2024-05-25 06:27:06.721687 better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-312.pyc
+-rw-r--r--   0        0        0      434 2024-05-25 06:19:06.433481 better_web3-4.0.0b5/better_web3/utils/eth.py
+-rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b5/better_web3/utils/other.py
+-rw-r--r--   0        0        0      521 2024-05-25 06:33:26.730371 better_web3-4.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b5/README.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b5/PKG-INFO
```

### Comparing `better_web3-4.0.0b4/better_web3/caip_2.py` & `better_web3-4.0.0b5/better_web3/caip_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,16 @@
         explorers=chain_caip2_data.explorers,
         eip1559=eip1559,
         **chain_kwargs,
     )
 
 
 def get_chain(chain_id: int, **chain_kwargs) -> Chain:
-    chains_caip2_data = request_chains_caip_2_data()
-    chain_caip2_data = chains_caip2_data[chain_id]
-
+    chain_caip2_data = request_chains_caip_2_data()[chain_id]
     if "rpc" in chain_kwargs:
-        chains_caip2_data.rpc_list.insert(0, chain_kwargs.pop("rpc"))
+        chain_caip2_data.rpc_list.insert(0, chain_kwargs.pop("rpc"))
 
     return _chain_from_caip_2_data(chain_caip2_data, **chain_kwargs)
 
 
 def get_chains(chain_ids: Iterable[int]) -> list[Chain]:
     return [get_chain(chain_id) for chain_id in chain_ids]
```

### Comparing `better_web3-4.0.0b4/better_web3/chain.py` & `better_web3-4.0.0b5/better_web3/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Iterable
+from typing import Iterable, AsyncGenerator
 
 from better_proxy import Proxy
 from eth_account.signers.local import LocalAccount
 from eth_typing import ChecksumAddress, HexStr, Address, Hash32
 from eth_utils import to_wei
 from hexbytes import HexBytes
 from web3 import AsyncWeb3, AsyncHTTPProvider
@@ -274,22 +274,20 @@
 
     async def balances(
             self,
             addresses: Iterable[ChecksumAddress],
             block_identifier: BlockIdentifier = "latest",
             batch_size: int = None,
             delay: int = None,
-    ):
+    ) -> AsyncGenerator[tuple[ChecksumAddress, Wei], None]:
         batch_size = batch_size or self.default_batch_request_size
         delay = delay or self.default_batch_request_delay
 
         addresses = list(addresses)
-        results = []
 
         for i in range(0, len(addresses), batch_size):
             batch_addresses = addresses[i:i + batch_size]
-            batch_results = await self._balances(batch_addresses, block_identifier)
-            results.extend(batch_results)
+            for address, balance in zip(batch_addresses, await self._balances(batch_addresses, block_identifier)):
+                yield address, Wei(balance)
+
             if delay > 0 and i + batch_size < len(addresses):
                 await asyncio.sleep(delay)
-
-        return results
```

### Comparing `better_web3-4.0.0b4/better_web3/models.py` & `better_web3-4.0.0b5/better_web3/models.py`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b4/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-4.0.0b5/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b4/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-4.0.0b5/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b4/better_web3/utils/__pycache__/other.cpython-312.pyc` & `better_web3-4.0.0b5/better_web3/utils/__pycache__/other.cpython-312.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xcb0d0d0a
-moddate:  0x4fa1e364 (Mon Aug 21 17:39:27 2023 UTC)
+moddate:  0xeb830b66 (Tue Apr  2 04:04:59 2024 UTC)
 files sz: 406
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `better_web3-4.0.0b4/pyproject.toml` & `better_web3-4.0.0b5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "better-web3"
-version = "4.0.0.b4"
+version = "4.0.0.b5"
 description = "Web3 stuff"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/better_web3"
 packages = [{include = "better_web3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `better_web3-4.0.0b4/README.md` & `better_web3-4.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b4/PKG-INFO` & `better_web3-4.0.0b5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 4.0.0b4
+Version: 4.0.0b5
 Summary: Web3 stuff
 Home-page: https://github.com/alenkimov/better_web3
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

