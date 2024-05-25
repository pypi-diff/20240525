# Comparing `tmp/kv_azure_blob-0.1.5.tar.gz` & `tmp/kv_azure_blob-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_azure_blob-0.1.5.tar", last modified: Sat May 18 18:55:04 2024, max compression
+gzip compressed data, was "kv_azure_blob-0.1.6.tar", last modified: Sat May 25 05:09:09 2024, max compression
```

## Comparing `kv_azure_blob-0.1.5.tar` & `kv_azure_blob-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.484403 kv_azure_blob-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-18 18:55:04.474402 kv_azure_blob-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1063 2024-05-12 08:47:51.000000 kv_azure_blob-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      608 2024-05-18 18:55:01.000000 kv_azure_blob-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-18 18:55:04.484403 kv_azure_blob-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.464402 kv_azure_blob-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.464402 kv_azure_blob-0.1.5/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.464402 kv_azure_blob-0.1.5/src/kv/azure/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.474402 kv_azure_blob-0.1.5/src/kv/azure/blob/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-05-12 07:36:23.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-05-12 08:28:05.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3845 2024-05-18 18:54:50.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/blob.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2979 2024-05-12 08:41:36.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/container.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      569 2024-05-12 08:38:57.000000 kv_azure_blob-0.1.5/src/kv/azure/blob/util.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-18 18:55:04.474402 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-18 18:55:04.000000 kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 05:09:09.143990 kv_azure_blob-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-25 05:09:09.143990 kv_azure_blob-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1063 2024-05-12 08:47:51.000000 kv_azure_blob-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      608 2024-05-25 05:09:06.000000 kv_azure_blob-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 05:09:09.143990 kv_azure_blob-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 05:09:09.133990 kv_azure_blob-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 05:09:09.133990 kv_azure_blob-0.1.6/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 05:09:09.133990 kv_azure_blob-0.1.6/src/kv/azure/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 05:09:09.143990 kv_azure_blob-0.1.6/src/kv/azure/blob/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-05-12 07:36:23.000000 kv_azure_blob-0.1.6/src/kv/azure/blob/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      104 2024-05-12 08:28:05.000000 kv_azure_blob-0.1.6/src/kv/azure/blob/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3925 2024-05-25 05:06:00.000000 kv_azure_blob-0.1.6/src/kv/azure/blob/blob.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3059 2024-05-25 05:05:32.000000 kv_azure_blob-0.1.6/src/kv/azure/blob/container.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      617 2024-05-25 05:08:38.000000 kv_azure_blob-0.1.6/src/kv/azure/blob/util.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 05:09:09.143990 kv_azure_blob-0.1.6/src/kv_azure_blob.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1471 2024-05-25 05:09:09.000000 kv_azure_blob-0.1.6/src/kv_azure_blob.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      372 2024-05-25 05:09:09.000000 kv_azure_blob-0.1.6/src/kv_azure_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 05:09:09.000000 kv_azure_blob-0.1.6/src/kv_azure_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-05-25 05:09:09.000000 kv_azure_blob-0.1.6/src/kv_azure_blob.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-05-25 05:09:09.000000 kv_azure_blob-0.1.6/src/kv_azure_blob.egg-info/top_level.txt
```

### Comparing `kv_azure_blob-0.1.5/PKG-INFO` & `kv_azure_blob-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.5
+Version: 0.1.6
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
```

### Comparing `kv_azure_blob-0.1.5/README.md` & `kv_azure_blob-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `kv_azure_blob-0.1.5/pyproject.toml` & `kv_azure_blob-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-azure-blob"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "KV API implementation on Azure Blob Storage"
 dependencies = [
   "azure-storage-blob", "aiohttp", "haskellian", "lazy-loader"
 ]
```

### Comparing `kv_azure_blob-0.1.5/src/kv/azure/blob/blob.py` & `kv_azure_blob-0.1.6/src/kv/azure/blob/blob.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import TypeVar, Generic, Callable, Awaitable, AsyncIterable, Sequence, overload
 from dataclasses import dataclass
+from datetime import datetime
 from haskellian import asyn_iter as AI, iter as I, either as E, Either, Right, promise as P
 from kv.api import LocatableKV, InvalidData, DBError
 from kv.azure.blob import BlobContainerKV
 from azure.storage.blob.aio import BlobServiceClient
 
 A = TypeVar('A')
 
@@ -93,10 +94,10 @@
     return results.mapl(DBError) | I.flatten | list
   
   async def _items(self, batch_size: int | None = None) -> AsyncIterable[Either[DBError | InvalidData, tuple[str, A]]]:
     for container in await self._containers():
       async for item in self._kv(container).items(batch_size):
         yield item
 
-  def url(self, key: str) -> str:
+  def url(self, key: str, *, expiry: datetime | None = None) -> str:
     container, blob = self.split_key(key)
-    return self._kv(container).url(blob)
+    return self._kv(container).url(blob, expiry=expiry)
```

### Comparing `kv_azure_blob-0.1.5/src/kv/azure/blob/container.py` & `kv_azure_blob-0.1.6/src/kv/azure/blob/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import TypeVar, Generic, Callable, ParamSpec, Awaitable, Never, Sequence, AsyncIterable
 from functools import wraps
 from dataclasses import dataclass
+from datetime import datetime
 from haskellian import either as E, Either, Left, Right, asyn_iter as AI
 from azure.core.exceptions import ResourceNotFoundError
 from azure.storage.blob.aio import ContainerClient
 from kv.api import DBError, InvalidData, InexistentItem, LocatableKV
 from .util import blob_url
 
 A = TypeVar('A')
@@ -78,10 +79,10 @@
     for key in keys.value:
       item = await self._read(key)
       if item.tag == 'left':
         yield Left(item.value)
       else:
         yield Right((key, item.value))
 
-  def url(self, key: str) -> str:
+  def url(self, key: str, *, expiry: datetime | None = None) -> str:
     bc = self.client().get_blob_client(key)
-    return blob_url(bc)
+    return blob_url(bc, expiry=expiry)
```

### Comparing `kv_azure_blob-0.1.5/src/kv/azure/blob/util.py` & `kv_azure_blob-0.1.6/src/kv/azure/blob/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from datetime import datetime, timedelta
-from azure.storage.blob import BlobSasPermissions, generate_blob_sas, BlobClient, ContainerClient
+from azure.storage.blob import BlobSasPermissions, generate_blob_sas, BlobClient
 
 def blob_url(
   client: BlobClient,
-  expiry: datetime = datetime.now() + timedelta(days=1),
+  expiry: datetime | None = None,
   permission = BlobSasPermissions(read=True)
 ) -> str:
   account_name: str = client.account_name # type: ignore
   account_key = client.credential.account_key
+  if expiry is None:
+    expiry = datetime.now() + timedelta(days=int(1e6)) # aka never
   token = generate_blob_sas(account_name, client.container_name, client.blob_name, account_key=account_key, expiry=expiry, permission=permission)
   return f"{client.url}?{token}"
```

### Comparing `kv_azure_blob-0.1.5/src/kv_azure_blob.egg-info/PKG-INFO` & `kv_azure_blob-0.1.6/src/kv_azure_blob.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kv-azure-blob
-Version: 0.1.5
+Version: 0.1.6
 Summary: KV API implementation on Azure Blob Storage
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/marciclabas/python-storage.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: azure-storage-blob
 Requires-Dist: aiohttp
```

