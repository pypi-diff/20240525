# Comparing `tmp/ossx-0.2.18a2.tar.gz` & `tmp/ossx-2.18.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossx-0.2.18a2.tar", max compression
+gzip compressed data, was "ossx-2.18.4.tar", max compression
```

## Comparing `ossx-0.2.18a2.tar` & `ossx-2.18.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1991 2024-04-16 12:23:46.786185 ossx-0.2.18a2/README.md
--rw-r--r--   0        0        0      143 2024-04-16 12:24:08.359535 ossx-0.2.18a2/ossx/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-17 06:05:55.724656 ossx-0.2.18a2/ossx/_http.py
--rw-r--r--   0        0        0    33002 2024-04-17 06:05:55.724889 ossx-0.2.18a2/ossx/bucket.py
--rw-r--r--   0        0        0     1439 2024-04-17 06:05:55.725027 ossx-0.2.18a2/ossx/models.py
--rw-r--r--   0        0        0      315 2024-04-17 06:05:55.725168 ossx-0.2.18a2/ossx/patch.py
--rw-r--r--   0        0        0     9835 2024-04-17 06:05:55.725340 ossx-0.2.18a2/ossx/select_response.py
--rw-r--r--   0        0        0     5962 2024-04-17 06:05:55.725783 ossx-0.2.18a2/ossx/utils.py
--rw-r--r--   0        0        0      495 2024-04-16 12:23:21.749178 ossx-0.2.18a2/pyproject.toml
--rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 ossx-0.2.18a2/PKG-INFO
+-rw-r--r--   0        0        0     1881 2024-05-25 04:40:42.741611 ossx-2.18.4/README.md
+-rw-r--r--   0        0        0      141 2024-05-25 04:40:42.741933 ossx-2.18.4/ossx/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-17 06:05:55.724656 ossx-2.18.4/ossx/_http.py
+-rw-r--r--   0        0        0    45455 2024-05-25 04:40:42.742377 ossx-2.18.4/ossx/bucket.py
+-rw-r--r--   0        0        0    12695 2024-05-25 04:40:42.742712 ossx-2.18.4/ossx/iterators.py
+-rw-r--r--   0        0        0     1439 2024-04-17 06:05:55.725027 ossx-2.18.4/ossx/models.py
+-rw-r--r--   0        0        0      315 2024-04-17 06:05:55.725168 ossx-2.18.4/ossx/patch.py
+-rw-r--r--   0        0        0     9835 2024-04-17 06:05:55.725340 ossx-2.18.4/ossx/select_response.py
+-rw-r--r--   0        0        0     6569 2024-05-25 04:40:42.743040 ossx-2.18.4/ossx/utils.py
+-rw-r--r--   0        0        0      520 2024-05-25 04:40:42.743774 ossx-2.18.4/pyproject.toml
+-rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 ossx-2.18.4/PKG-INFO
```

### Comparing `ossx-0.2.18a2/README.md` & `ossx-2.18.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # ossx
 
-[![Build Status](https://travis-ci.org/aliyun/ossx.svg?branch=master)](https://travis-ci.org/aliyun/ossx)
-[![Coverage Status](https://coveralls.io/repos/github/aliyun/ossx/badge.svg?branch=master)](https://coveralls.io/github/aliyun/ossx?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/sswest/ossx/badge.svg?branch=main)](https://coveralls.io/github/sswest/ossx?branch=main)
 [![PyPI version](https://badge.fury.io/py/ossx.svg)](https://badge.fury.io/py/ossx)
 
 ossx is an Aliyun OSS SDK for Python Asyncio.
 
 You are free to extend this project, but it's recommended to always run the unit tests to ensure the existing functionality works as expected.
 
 ## Implementation Details
```

### Comparing `ossx-0.2.18a2/ossx/_http.py` & `ossx-2.18.4/ossx/_http.py`

 * *Files identical despite different names*

### Comparing `ossx-0.2.18a2/ossx/bucket.py` & `ossx-2.18.4/ossx/bucket.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from oss2 import Auth, Bucket, Service, compat, exceptions, models, utils, xml_utils
 from oss2.api import _Base, _make_range_string, logger
 from oss2.exceptions import ClientError
 from oss2.select_params import SelectParameters
 
 from . import _http as http
 from .models import GetSelectObjectMetaResult, SelectObjectResult
-from .utils import warp_async_data
+from .utils import async_copyfileobj, warp_async_data
 
 T = TypeVar("T")
 ObjectPermission = Literal["default", "private", "public-read", "public-read-write"]
 BucketPermission = Literal["private", "public-read", "public-read-write"]
 URLTypes = Union["URL", str]
 ProxyTypes = Union[URLTypes, "Proxy"]
 ProxiesTypes = Union[ProxyTypes, Dict[URLTypes, Union[None, ProxyTypes]]]
@@ -104,15 +104,15 @@
     async def list_buckets(
         self,
         prefix: str = "",
         marker: str = "",
         max_keys: int = 100,
         params: Optional[Dict[str, Any]] = None,
         headers: Optional[Union[dict, http.CaseInsensitiveDict]] = None,
-    ):
+    ) -> models.ListBucketsResult:
         return await super().list_buckets(prefix, marker, max_keys, params, headers)
 
     async def get_user_qos_info(self) -> models.GetUserQosInfoResult:
         return await super().get_user_qos_info()
 
     async def describe_regions(self, regions: str = "") -> models.DescribeRegionsResult:
         return await super().describe_regions(regions)
@@ -295,15 +295,15 @@
     async def select_object(
         self,
         key: str,
         sql: str,
         progress_callback: Optional[Callable[[int, Optional[int]], Any]] = None,
         select_params: Optional[Dict[str, str]] = None,
         byte_range: Optional[Tuple[int, int]] = None,
-        headers: Optional[Dict[str, str]] = None,
+        headers: Optional[Union[dict, http.CaseInsensitiveDict]] = None,
     ):
         range_select = False
         headers = http.CaseInsensitiveDict(headers)
         range_string = _make_range_string(byte_range)
         if range_string:
             headers["range"] = range_string
             range_select = True
@@ -332,33 +332,90 @@
         if select_params is not None and SelectParameters.EnablePayloadCrc in select_params:
             if str(select_params[SelectParameters.EnablePayloadCrc]).lower() == "true":
                 crc_enabled = True
         return SelectObjectResult(resp, progress_callback, crc_enabled)
 
     async def get_object_to_file(
         self,
-        key,
-        filename,
-        byte_range=None,
-        headers=None,
-        progress_callback=None,
-        process=None,
-        params=None,
-    ):
-        raise NotImplementedError
+        key: str,
+        filename: str,
+        byte_range: Optional[Tuple[int, int]] = None,
+        headers: Optional[Union[dict, http.CaseInsensitiveDict]] = None,
+        progress_callback: Optional[Callable[[int, Optional[int]], Any]] = None,
+        process: Optional[str] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> models.GetObjectResult:
+        logger.debug(
+            f"Start to get object to file, bucket: {self.bucket_name}"
+            f", key: {key}, file path: {filename}"
+        )
+        async with aiofiles.open(compat.to_unicode(filename), "wb") as f:
+            result = await self.get_object(
+                key,
+                byte_range=byte_range,
+                headers=headers,
+                progress_callback=progress_callback,
+                process=process,
+                params=params,
+            )
+            await async_copyfileobj(result, f, result.content_length, request_id=result.request_id)
+
+            if self.enable_crc and byte_range is None:
+                if (
+                    (headers is None)
+                    or ("Accept-Encoding" not in headers)
+                    or (headers["Accept-Encoding"] != "gzip")
+                ):
+                    utils.check_crc("get", result.client_crc, result.server_crc, result.request_id)
+
+        return result
 
     async def get_object_with_url(
-        self, sign_url, byte_range=None, headers=None, progress_callback=None
-    ):
-        raise NotImplementedError
+        self,
+        sign_url: str,
+        byte_range: Optional[Tuple[int, int]] = None,
+        headers: Optional[Union[dict, http.CaseInsensitiveDict]] = None,
+        progress_callback: Optional[Callable[[int, Optional[int]], Any]] = None,
+    ) -> models.GetObjectResult:
+        headers = http.CaseInsensitiveDict(headers)
+
+        range_string = _make_range_string(byte_range)
+        if range_string:
+            headers["range"] = range_string
+
+        logger.debug(
+            f"Start to get object with url, bucket: {self.bucket_name}, sign_url: {sign_url},"
+            f" range: {range_string}, headers: {headers}"
+        )
+        resp = await self._do_url("GET", sign_url, headers=headers)
+        return models.GetObjectResult(resp, progress_callback, self.enable_crc)
 
     async def get_object_with_url_to_file(
-        self, sign_url, filename, byte_range=None, headers=None, progress_callback=None
-    ):
-        raise NotImplementedError
+        self,
+        sign_url: str,
+        filename: str,
+        byte_range: Optional[Tuple[int, int]] = None,
+        headers: Optional[Union[dict, http.CaseInsensitiveDict]] = None,
+        progress_callback: Optional[Callable[[int, Optional[int]], Any]] = None,
+    ) -> models.GetObjectResult:
+        logger.debug(
+            f"Start to get object with url, bucket: {self.bucket_name}, sign_url: {sign_url}"
+            f", file path: {filename}, range: {byte_range}, headers: {headers}"
+        )
+
+        async with aiofiles.open(compat.to_unicode(filename), "wb") as f:
+            result = await self.get_object_with_url(
+                sign_url,
+                byte_range=byte_range,
+                headers=headers,
+                progress_callback=progress_callback,
+            )
+            await async_copyfileobj(result, f, result.content_length, request_id=result.request_id)
+
+        return result
 
     async def select_object_to_file(
         self,
         key: str,
         filename: str,
         sql: str,
         progress_callback: Optional[Callable[[int, Optional[int]], Any]] = None,
@@ -912,15 +969,241 @@
         return models.GetBucketPolicyResult(resp)
 
     async def delete_bucket_policy(self) -> models.RequestResult:
         result = super().delete_bucket_policy()
         resp = await result.resp
         return models.RequestResult(resp)
 
-    # TODO add more methods
+    async def put_bucket_request_payment(self, payer: str) -> models.RequestResult:
+        result = super().put_bucket_request_payment(payer)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_request_payment(self) -> models.GetBucketRequestPaymentResult:
+        return await super().get_bucket_request_payment()
+
+    async def put_bucket_qos_info(
+        self, bucket_qos_info: models.BucketQosInfo
+    ) -> models.RequestResult:
+        result = super().put_bucket_qos_info(bucket_qos_info)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_qos_info(self) -> models.GetBucketQosInfoResult:
+        return await super().get_bucket_qos_info()
+
+    async def delete_bucket_qos_info(self) -> models.RequestResult:
+        result = super().delete_bucket_qos_info()
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def set_bucket_storage_capacity(
+        self, user_qos: models.BucketUserQos
+    ) -> models.RequestResult:
+        result = super().set_bucket_storage_capacity(user_qos)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_storage_capacity(self) -> models.GetBucketUserQosResult:
+        return await super().get_bucket_storage_capacity()
+
+    async def put_async_fetch_task(
+        self, task_config: models.AsyncFetchTaskConfiguration
+    ) -> models.PutAsyncFetchTaskResult:
+        result = super().put_async_fetch_task(task_config)
+        resp = await result.resp
+        return models.PutAsyncFetchTaskResult(resp)
+
+    async def get_async_fetch_task(self, task_id: str) -> models.GetAsyncFetchTaskResult:
+        return await super().get_async_fetch_task(task_id)
+
+    async def put_bucket_inventory_configuration(
+        self, inventory_configuration: models.InventoryConfiguration
+    ) -> models.RequestResult:
+        result = super().put_bucket_inventory_configuration(inventory_configuration)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_inventory_configuration(
+        self, inventory_id: str
+    ) -> models.GetInventoryConfigurationResult:
+        return await super().get_bucket_inventory_configuration(inventory_id)
+
+    async def list_bucket_inventory_configurations(
+        self, continuation_token: Optional[str] = None
+    ) -> models.ListInventoryConfigurationsResult:
+        return await super().list_bucket_inventory_configurations(continuation_token)
+
+    async def delete_bucket_inventory_configuration(
+        self, inventory_id: str
+    ) -> models.RequestResult:
+        result = super().delete_bucket_inventory_configuration(inventory_id)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def init_bucket_worm(
+        self, retention_period_days: Optional[int] = None
+    ) -> models.InitBucketWormResult:
+        logger.debug(
+            "Start to init bucket worm, bucket: {0}, retention_period_days: {1}.".format(
+                self.bucket_name, retention_period_days
+            )
+        )
+        data = xml_utils.to_put_init_bucket_worm(retention_period_days)
+        headers = http.CaseInsensitiveDict()
+        headers["Content-MD5"] = utils.content_md5(data)
+        resp = await self.__do_bucket("POST", data=data, params={Bucket.WORM: ""}, headers=headers)
+        logger.debug(
+            "init bucket worm done, req_id: {0}, status_code: {1}".format(
+                resp.request_id, resp.status
+            )
+        )
+
+        result = models.InitBucketWormResult(resp)
+        result.worm_id = resp.headers.get("x-oss-worm-id")
+        return result
+
+    async def abort_bucket_worm(self) -> models.RequestResult:
+        result = super().abort_bucket_worm()
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def complete_bucket_worm(self, worm_id: Optional[str] = None) -> models.RequestResult:
+        result = super().complete_bucket_worm(worm_id)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def extend_bucket_worm(
+        self, worm_id: Optional[str] = None, retention_period_days: Optional[int] = None
+    ) -> models.RequestResult:
+        result = super().extend_bucket_worm(worm_id, retention_period_days)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_worm(self) -> models.GetBucketWormResult:
+        return await super().get_bucket_worm()
+
+    async def put_bucket_replication(self, rule: models.ReplicationRule) -> models.RequestResult:
+        result = super().put_bucket_replication(rule)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_replication(self) -> models.GetBucketReplicationResult:
+        return await super().get_bucket_replication()
+
+    async def delete_bucket_replication(self, rule_id: str) -> models.RequestResult:
+        result = super().delete_bucket_replication(rule_id)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_replication_location(self) -> models.GetBucketReplicationLocationResult:
+        return await super().get_bucket_replication_location()
+
+    async def get_bucket_replication_progress(
+        self, rule_id: str
+    ) -> models.GetBucketReplicationProgressResult:
+        return await super().get_bucket_replication_progress(rule_id)
+
+    async def put_bucket_transfer_acceleration(self, enabled: str) -> models.RequestResult:
+        result = super().put_bucket_transfer_acceleration(enabled)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_transfer_acceleration(self) -> models.GetBucketTransferAccelerationResult:
+        return await super().get_bucket_transfer_acceleration()
+
+    async def create_bucket_cname_token(self, domain: str) -> models.CreateBucketCnameTokenResult:
+        return await super().create_bucket_cname_token(domain)
+
+    async def get_bucket_cname_token(self, domain: str) -> models.GetBucketCnameTokenResult:
+        return await super().get_bucket_cname_token(domain)
+
+    async def put_bucket_cname(self, input: models.PutBucketCnameRequest) -> models.RequestResult:
+        result = super().put_bucket_cname(input)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def list_bucket_cname(self) -> models.ListBucketCnameResult:
+        return await super().list_bucket_cname()
+
+    async def delete_bucket_cname(self, domain: str) -> models.RequestResult:
+        result = super().delete_bucket_cname(domain)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def open_bucket_meta_query(self) -> models.RequestResult:
+        result = super().open_bucket_meta_query()
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_meta_query_status(self) -> models.GetBucketMetaQueryResult:
+        return await super().get_bucket_meta_query_status()
+
+    async def do_bucket_meta_query(
+        self, do_meta_query_request: models.MetaQuery
+    ) -> models.DoBucketMetaQueryResult:
+        return await super().do_bucket_meta_query(do_meta_query_request)
+
+    async def close_bucket_meta_query(self) -> models.RequestResult:
+        result = super().close_bucket_meta_query()
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def put_bucket_access_monitor(self, status: str) -> models.RequestResult:
+        result = super().put_bucket_access_monitor(status)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_access_monitor(self) -> models.GetBucketAccessMonitorResult:
+        return await super().get_bucket_access_monitor()
+
+    async def get_bucket_resource_group(self) -> models.GetBucketResourceGroupResult:
+        return await super().get_bucket_resource_group()
+
+    async def put_bucket_resource_group(self, resourceGroupId: str) -> models.RequestResult:
+        result = super().put_bucket_resource_group(resourceGroupId)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def put_bucket_style(self, styleName: str, content: str) -> models.RequestResult:
+        result = super().put_bucket_style(styleName, content)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_style(self, styleName: str) -> models.GetBucketStyleResult:
+        return await super().get_bucket_style(styleName)
+
+    async def list_bucket_style(self) -> models.ListBucketStyleResult:
+        return await super().list_bucket_style()
+
+    async def delete_bucket_style(self, styleName: str) -> models.RequestResult:
+        result = super().delete_bucket_style(styleName)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def async_process_object(
+        self,
+        key: str,
+        process: str,
+        headers: Optional[Union[dict, http.CaseInsensitiveDict]] = None,
+    ) -> models.AsyncProcessObject:
+        return await super().async_process_object(key, process, headers)
+
+    async def put_bucket_callback_policy(self, callbackPolicy: str) -> models.RequestResult:
+        result = super().put_bucket_callback_policy(callbackPolicy)
+        resp = await result.resp
+        return models.RequestResult(resp)
+
+    async def get_bucket_callback_policy(self) -> models.GetBucketPolicyResult:
+        return await super().get_bucket_callback_policy()
+
+    async def delete_bucket_callback_policy(self) -> models.RequestResult:
+        result = super().delete_bucket_callback_policy()
+        resp = await result.resp
+        return models.RequestResult(resp)
 
     def __do_object(self, method, key, **kwargs):
         if not self.bucket_name:
             raise exceptions.ClientError("Bucket name should not be null or empty.")
         if not key:
             raise exceptions.ClientError("key should not be null or empty.")
         return self._do(method, self.bucket_name, key, **kwargs)
```

### Comparing `ossx-0.2.18a2/ossx/models.py` & `ossx-2.18.4/ossx/models.py`

 * *Files identical despite different names*

### Comparing `ossx-0.2.18a2/ossx/select_response.py` & `ossx-2.18.4/ossx/select_response.py`

 * *Files identical despite different names*

### Comparing `ossx-0.2.18a2/ossx/utils.py` & `ossx-2.18.4/ossx/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,52 @@
+import os
 from inspect import isawaitable, iscoroutinefunction
 from io import BytesIO
 from typing import IO, AsyncIterable, Union
 
+from oss2.exceptions import InconsistentError
 from oss2.utils import (
     _CHUNK_SIZE,
     ClientError,
     Crc64,
     _BytesAndFileAdapter,
     _FileLikeAdapter,
     _get_data_size,
     _has_data_size_attr,
     _invoke_cipher_callback,
     _invoke_crc_callback,
     _IterableAdapter,
     to_bytes,
 )
 
+_WINDOWS = os.name == "nt"
+COPY_BUFSIZE = 1024 * 1024 if _WINDOWS else 64 * 1024
+
+
+async def async_copyfileobj(
+    fsrc,
+    fdst,
+    expected_len=None,
+    request_id="",
+    length=COPY_BUFSIZE,
+):
+    fsrc_read = fsrc.read
+    fdst_write = fdst.write
+    num_read = 0
+    while True:
+        buf = await fsrc_read(length)
+        if not buf:
+            break
+
+        num_read += len(buf)
+        await fdst_write(buf)
+
+    if expected_len and num_read != expected_len:
+        raise InconsistentError("IncompleteRead from source", request_id)
+
 
 def make_crc_adapter(data, init_crc=0, discard=0):
     """返回一个适配器，从而在读取 `data` ，即调用read或者对其进行迭代的时候，能够计算CRC。
 
     :param discard:
     :return:
     :param data: 可以是bytes、file object或iterable
```

### Comparing `ossx-0.2.18a2/PKG-INFO` & `ossx-2.18.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: ossx
-Version: 0.2.18a2
-Summary: aliyun oss sdk for python asyncio
+Version: 2.18.4
+Summary: aliyun oss sdk for python async
 Author: sswest
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiofiles (>=0.7.0,<0.8.0)
-Requires-Dist: httpx (==0.27.0)
-Requires-Dist: oss2 (==2.18.4)
+Requires-Dist: httpx (>=0.23,<0.24)
+Requires-Dist: oss2 (>=2.18,<3.0)
 Description-Content-Type: text/markdown
 
 # ossx
 
-[![Build Status](https://travis-ci.org/aliyun/ossx.svg?branch=master)](https://travis-ci.org/aliyun/ossx)
-[![Coverage Status](https://coveralls.io/repos/github/aliyun/ossx/badge.svg?branch=master)](https://coveralls.io/github/aliyun/ossx?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/sswest/ossx/badge.svg?branch=main)](https://coveralls.io/github/sswest/ossx?branch=main)
 [![PyPI version](https://badge.fury.io/py/ossx.svg)](https://badge.fury.io/py/ossx)
 
 ossx is an Aliyun OSS SDK for Python Asyncio.
 
 You are free to extend this project, but it's recommended to always run the unit tests to ensure the existing functionality works as expected.
 
 ## Implementation Details
```

