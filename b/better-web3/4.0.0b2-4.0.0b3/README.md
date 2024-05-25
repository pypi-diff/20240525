# Comparing `tmp/better_web3-4.0.0b2.tar.gz` & `tmp/better_web3-4.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_web3-4.0.0b2.tar", max compression
+gzip compressed data, was "better_web3-4.0.0b3.tar", max compression
```

## Comparing `better_web3-4.0.0b2.tar` & `better_web3-4.0.0b3.tar`

### file list

```diff
@@ -1,49 +1,20 @@
--rw-r--r--   0        0        0      577 2024-04-02 09:30:25.140486 better_web3-4.0.0b2/better_web3/__init__.py
--rw-r--r--   0        0        0    10519 2023-08-11 17:57:06.795000 better_web3-4.0.0b2/better_web3/batch_call.py
--rw-r--r--   0        0        0    14763 2024-04-02 12:00:11.715704 better_web3-4.0.0b2/better_web3/chain.py
--rw-r--r--   0        0        0      191 2024-04-02 09:22:28.122802 better_web3-4.0.0b2/better_web3/chains/__init__.py
--rw-r--r--   0        0        0     1233 2024-04-02 09:06:03.839102 better_web3-4.0.0b2/better_web3/chains/chains.py
--rw-r--r--   0        0        0      759 2024-04-02 08:52:35.875360 better_web3-4.0.0b2/better_web3/chains/models.py
--rw-r--r--   0        0        0     1581 2024-04-02 04:32:21.450710 better_web3-4.0.0b2/better_web3/contract.py
--rw-r--r--   0        0        0      243 2024-04-02 09:22:28.128804 better_web3-4.0.0b2/better_web3/contracts/__init__.py
--rw-r--r--   0        0        0      525 2023-12-16 17:27:00.084000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      406 2024-01-10 21:45:55.898445 better_web3-4.0.0b2/better_web3/contracts/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0      687 2023-12-16 17:27:30.383000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_abi.cpython-311.pyc
--rw-r--r--   0        0        0      568 2024-01-10 21:46:32.919665 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_abi.cpython-312.pyc
--rw-r--r--   0        0        0      351 2023-12-16 17:27:40.401000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_paths.cpython-311.pyc
--rw-r--r--   0        0        0      305 2024-01-10 21:46:32.928171 better_web3-4.0.0b2/better_web3/contracts/__pycache__/_paths.cpython-312.pyc
--rw-r--r--   0        0        0     1949 2023-12-16 17:27:33.403000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/disperse.cpython-311.pyc
--rw-r--r--   0        0        0     1612 2024-01-10 21:46:32.931171 better_web3-4.0.0b2/better_web3/contracts/__pycache__/disperse.cpython-312.pyc
--rw-r--r--   0        0        0     3886 2023-12-16 17:27:35.432000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc20.cpython-311.pyc
--rw-r--r--   0        0        0     3263 2024-01-10 21:46:32.932171 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc20.cpython-312.pyc
--rw-r--r--   0        0        0     5434 2023-12-16 17:27:37.100000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc721.cpython-311.pyc
--rw-r--r--   0        0        0     4409 2024-01-10 21:46:32.933172 better_web3-4.0.0b2/better_web3/contracts/__pycache__/erc721.cpython-312.pyc
--rw-r--r--   0        0        0     9841 2023-12-16 17:27:28.421000 better_web3-4.0.0b2/better_web3/contracts/__pycache__/multicall.cpython-311.pyc
--rw-r--r--   0        0        0     7989 2024-01-10 21:46:32.919665 better_web3-4.0.0b2/better_web3/contracts/__pycache__/multicall.cpython-312.pyc
--rw-r--r--   0        0        0      352 2023-07-07 12:07:06.130000 better_web3-4.0.0b2/better_web3/contracts/_abi.py
--rw-r--r--   0        0        0       99 2023-06-05 07:41:10.829000 better_web3-4.0.0b2/better_web3/contracts/_paths.py
--rw-r--r--   0        0        0     1193 2023-06-23 09:34:50.869000 better_web3-4.0.0b2/better_web3/contracts/abi/disperse.json
--rw-r--r--   0        0        0     6301 2023-06-05 07:31:23.813000 better_web3-4.0.0b2/better_web3/contracts/abi/erc1155.json
--rw-r--r--   0        0        0     5904 2023-06-05 07:28:46.510000 better_web3-4.0.0b2/better_web3/contracts/abi/erc20.json
--rw-r--r--   0        0        0     6755 2023-06-05 07:31:36.520000 better_web3-4.0.0b2/better_web3/contracts/abi/erc721.json
--rw-r--r--   0        0        0     8859 2023-06-04 08:00:02.863000 better_web3-4.0.0b2/better_web3/contracts/abi/multicall_v3.json
--rw-r--r--   0        0        0      655 2024-04-02 04:32:21.461710 better_web3-4.0.0b2/better_web3/contracts/disperse.py
--rw-r--r--   0        0        0     1545 2024-04-02 04:32:21.446709 better_web3-4.0.0b2/better_web3/contracts/erc20.py
--rw-r--r--   0        0        0     2644 2024-04-02 04:32:21.458714 better_web3-4.0.0b2/better_web3/contracts/erc721.py
--rw-r--r--   0        0        0     5777 2024-04-02 06:36:40.841552 better_web3-4.0.0b2/better_web3/contracts/multicall.py
--rw-r--r--   0        0        0      255 2024-04-02 08:49:51.858266 better_web3-4.0.0b2/better_web3/models.py
--rw-r--r--   0        0        0      554 2024-04-02 09:30:25.133484 better_web3-4.0.0b2/better_web3/utils/__init__.py
--rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      698 2024-01-10 21:46:32.920666 better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-311.pyc
--rw-r--r--   0        0        0     3533 2024-01-10 21:46:32.922666 better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-312.pyc
--rw-r--r--   0        0        0     3719 2023-12-16 17:27:36.000000 better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     2780 2024-01-10 21:46:32.923666 better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-312.pyc
--rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-311.pyc
--rw-r--r--   0        0        0      707 2024-01-10 21:46:32.927171 better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-312.pyc
--rw-r--r--   0        0        0     3143 2024-04-02 09:30:25.131514 better_web3-4.0.0b2/better_web3/utils/eth.py
--rw-r--r--   0        0        0      360 2024-04-01 16:25:26.575693 better_web3-4.0.0b2/better_web3/utils/file.py
--rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b2/better_web3/utils/other.py
--rw-r--r--   0        0        0      563 2024-05-24 05:30:30.290708 better_web3-4.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b2/README.md
--rw-r--r--   0        0        0     1483 1970-01-01 00:00:00.000000 better_web3-4.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0      224 2024-05-25 04:36:12.322385 better_web3-4.0.0b3/better_web3/__init__.py
+-rw-r--r--   0        0        0     1752 2024-05-25 04:36:12.324383 better_web3-4.0.0b3/better_web3/caip_2.py
+-rw-r--r--   0        0        0    11052 2024-05-25 05:59:38.348397 better_web3-4.0.0b3/better_web3/chain.py
+-rw-r--r--   0        0        0      497 2024-05-25 05:44:27.207734 better_web3-4.0.0b3/better_web3/contract.py
+-rw-r--r--   0        0        0      933 2024-05-24 15:45:44.526320 better_web3-4.0.0b3/better_web3/models.py
+-rw-r--r--   0        0        0      504 2024-05-25 05:40:55.256224 better_web3-4.0.0b3/better_web3/utils/__init__.py
+-rw-r--r--   0        0        0      917 2023-12-16 17:27:32.282000 better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      698 2024-01-10 21:46:32.920666 better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     4358 2023-12-16 17:27:34.414000 better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-311.pyc
+-rw-r--r--   0        0        0     3533 2024-01-10 21:46:32.922666 better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-312.pyc
+-rw-r--r--   0        0        0     3719 2023-12-16 17:27:36.000000 better_web3-4.0.0b3/better_web3/utils/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     2780 2024-01-10 21:46:32.923666 better_web3-4.0.0b3/better_web3/utils/__pycache__/file.cpython-312.pyc
+-rw-r--r--   0        0        0      837 2023-12-16 17:27:37.593000 better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-311.pyc
+-rw-r--r--   0        0        0      707 2024-01-10 21:46:32.927171 better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-312.pyc
+-rw-r--r--   0        0        0      470 2024-05-25 05:40:55.251225 better_web3-4.0.0b3/better_web3/utils/eth.py
+-rw-r--r--   0        0        0      331 2024-05-25 05:40:55.259224 better_web3-4.0.0b3/better_web3/utils/file.py
+-rw-r--r--   0        0        0      406 2024-04-02 04:04:59.695626 better_web3-4.0.0b3/better_web3/utils/other.py
+-rw-r--r--   0        0        0      521 2024-05-25 05:40:55.254223 better_web3-4.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      760 2024-04-02 09:22:28.119803 better_web3-4.0.0b3/README.md
+-rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 better_web3-4.0.0b3/PKG-INFO
```

### Comparing `better_web3-4.0.0b2/better_web3/chains/chains.py` & `better_web3-4.0.0b3/better_web3/caip_2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,58 @@
+from typing import Iterable
+from functools import lru_cache
+
 import requests
 
 from .models import CAIP2ChainData
-
-from .. import Chain
+from . import Chain
 
 
-def request_chains_data() -> dict[int: CAIP2ChainData]:
+@lru_cache
+def request_chains_caip_2_data() -> dict[int: CAIP2ChainData]:
     """
-    Возвращает словарь формата {ID сети: Информации о сети в формате CAIP-2}
+    :returns: {chain ID: CAIP-2 chain data}
     """
     response = requests.get("https://chainid.network/chains.json")
-    return {chain_data["chainId"]: CAIP2ChainData(**chain_data) for chain_data in response.json()}
+    data = response.json()
+    return {chain_data["chainId"]: CAIP2ChainData(**chain_data) for chain_data in data}
 
 
-def chain_from_caip_2(
-    chain_data: CAIP2ChainData,
+def _chain_from_caip_2_data(
+    chain_caip2_data: CAIP2ChainData,
     **chain_kwargs,
 ) -> Chain:
     target_rpc = None
-    for rpc in chain_data.rpc_list:  # type: str
+    for rpc in chain_caip2_data.rpc_list:  # type: str
         if rpc.startswith("http") and "$" not in rpc:
             target_rpc = rpc
             break
 
     if not target_rpc:
-        raise ValueError("Specify at least one http rpc")
+        raise ValueError("No http rpc")
 
-    eip1559 = "EIP1559" in {feature.name for feature in chain_data.features} if chain_data.features else False
+    eip1559 = "EIP1559" in {feature.name for feature in chain_caip2_data.features} if chain_caip2_data.features else False
 
     return Chain(
         target_rpc,
-        name=chain_data.name,
-        short_name=chain_data.short_name,
-        info_url=chain_data.info_url,
-        native_currency=chain_data.native_currency,
-        explorers=chain_data.explorers,
+        name=chain_caip2_data.name,
+        short_name=chain_caip2_data.short_name,
+        info_url=chain_caip2_data.info_url,
+        native_currency=chain_caip2_data.native_currency,
+        explorers=chain_caip2_data.explorers,
         eip1559=eip1559,
         **chain_kwargs,
     )
+
+
+def get_chain(chain_id: int, **chain_kwargs) -> Chain:
+    chains_caip2_data = request_chains_caip_2_data()
+    chain_caip2_data = chains_caip2_data[chain_id]
+
+    if "rpc" in chain_kwargs:
+        chains_caip2_data.rpc_list.insert(0, chain_kwargs.pop("rpc"))
+
+    return _chain_from_caip_2_data(chain_caip2_data, **chain_kwargs)
+
+
+def get_chains(chain_ids: Iterable[int]) -> list[Chain]:
+    return [get_chain(chain_id) for chain_id in chain_ids]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `better_web3-4.0.0b2/better_web3/chains/models.py` & `better_web3-4.0.0b3/better_web3/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 from pydantic import BaseModel, Field
 
-from ..models import NativeCurrency, Explorer
+
+class Explorer(BaseModel):
+    name: str
+    url: str
+    standard: str
+    # icon: str | None = None
+
+
+class NativeCurrency(BaseModel):
+    name: str = "Ether"
+    symbol: str = "ETH"
+    decimals: int = 18
 
 
 class Feature(BaseModel):
     name: str
 
 
 class CAIP2ChainData(BaseModel):
```

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-311.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/__init__.cpython-312.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-311.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/eth.cpython-312.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/eth.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-311.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/file.cpython-312.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/file.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-311.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/better_web3/utils/__pycache__/other.cpython-312.pyc` & `better_web3-4.0.0b3/better_web3/utils/__pycache__/other.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/pyproject.toml` & `better_web3-4.0.0b3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "better-web3"
-version = "4.0.0.b2"
-description = "Chains, Contracts, batch calls and other Web3 stuff!"
+version = "4.0.0.b3"
+description = "Web3 stuff"
 authors = ["Alen <alen.kimov@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/alenkimov/better_web3"
 packages = [{include = "better_web3"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `better_web3-4.0.0b2/README.md` & `better_web3-4.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `better_web3-4.0.0b2/PKG-INFO` & `better_web3-4.0.0b3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: better-web3
-Version: 4.0.0b2
-Summary: Chains, Contracts, batch calls and other Web3 stuff!
+Version: 4.0.0b3
+Summary: Web3 stuff
 Home-page: https://github.com/alenkimov/better_web3
 Author: Alen
 Author-email: alen.kimov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

