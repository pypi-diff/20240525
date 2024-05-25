# Comparing `tmp/python_115-0.0.8.3.3.tar.gz` & `tmp/python_115-0.0.8.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.3.3.tar", max compression
+gzip compressed data, was "python_115-0.0.8.3.4.tar", max compression
```

## Comparing `python_115-0.0.8.3.3.tar` & `python_115-0.0.8.3.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.3/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.3/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.3/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.3/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.3/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.3/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.3/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.3/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.3.3/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.3/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.3/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.3/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.3/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.3/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.3/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.3/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.3/p115/component/cipher.py
--rwxr-xr-x   0        0        0   246303 2024-05-25 02:41:34.435405 python_115-0.0.8.3.3/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.3/p115/component/exception.py
--rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.3.3/p115/component/fs.py
--rwxr-xr-x   0        0        0    48067 2024-05-24 16:16:56.781105 python_115-0.0.8.3.3/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.3/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.3/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.3.3/p115/component/labellist.py
--rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.3.3/p115/component/offline.py
--rwxr-xr-x   0        0        0     4338 2024-05-24 16:52:21.603382 python_115-0.0.8.3.3/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6373 2024-05-24 16:52:41.937491 python_115-0.0.8.3.3/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.3/p115/py.typed
--rwxr-xr-x   0        0        0     5009 2024-05-25 03:38:35.132652 python_115-0.0.8.3.3/p115/tool/__init__.py
--rw-r--r--   0        0        0     1665 2024-05-25 03:39:19.421181 python_115-0.0.8.3.3/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.3/readme.md
--rw-r--r--   0        0        0    36371 1970-01-01 00:00:00.000000 python_115-0.0.8.3.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.4/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.4/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.4/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.4/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.4/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.3.4/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.4/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.4/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.4/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.4/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   246390 2024-05-25 05:26:13.883965 python_115-0.0.8.3.4/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.4/p115/component/exception.py
+-rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.3.4/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.3.4/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.4/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.4/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.3.4/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.3.4/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.3.4/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.3.4/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.4/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.3.4/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-25 05:35:31.473053 python_115-0.0.8.3.4/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.4/readme.md
+-rw-r--r--   0        0        0    36371 1970-01-01 00:00:00.000000 python_115-0.0.8.3.4/PKG-INFO
```

### Comparing `python_115-0.0.8.3.3/LICENSE` & `python_115-0.0.8.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/cmd/iterdir.py` & `python_115-0.0.8.3.4/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/cmd/qrcode.py` & `python_115-0.0.8.3.4/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/component/__init__.py` & `python_115-0.0.8.3.4/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/component/cipher.py` & `python_115-0.0.8.3.4/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/component/client.py` & `python_115-0.0.8.3.4/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2308,14 +2308,15 @@
                 # - 所有: 0
                 # - 文档: 1
                 # - 图片: 2
                 # - 音频: 3
                 # - 视频: 4
                 # - 压缩包: 5
                 # - 应用: 6
+                # - 书籍: 7
         """
         api = "https://webapi.115.com/files/search"
         if isinstance(payload, str):
             payload = {
                 "aid": 1, "cid": 0, "format": "json", "limit": 32, "offset": 0, 
                 "show_dir": 1, "search_value": payload, 
             }
@@ -2820,15 +2821,15 @@
         *lables: str,
         async_: Literal[False, True] = False, 
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """添加标签（可以接受多个）
         POST https://webapi.115.com/label/add_multi
 
-        可传入多个 label 描述，每个 label 的格式都是 "{label_name}\x07{color}"，例如 "tag\x07#FF0000"
+        可传入多个 label 描述，每个 label 的格式都是 "{label_name}" 或 "{label_name}\x07{color}"，例如 "tag\x07#FF0000"
         """
         api = "https://webapi.115.com/label/add_multi"
         payload = [("name[]", label) for label in lables if label]
         if not payload:
             return {"state": False, "message": "no op"}
         if (headers := request_kwargs.get("headers")):
             headers = request_kwargs["headers"] = dict(headers)
@@ -2907,15 +2908,15 @@
     ) -> dict | Awaitable[dict]:
         """编辑标签
         POST https://webapi.115.com/label/edit
         payload:
             - id: int | str # 标签 id
             - name: str = <default>  # 标签名
             - color: str = <default> # 标签颜色，支持 css 颜色语法
-            - sort: int = <default> # 序号
+            - sort: int = <default>  # 序号
         """
         api = "https://webapi.115.com/label/edit"
         request_kwargs.pop("parse", None)
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
     @overload
     def label_list(
@@ -3347,15 +3348,15 @@
     ) -> dict | Awaitable[dict]:
         """接收分享链接的某些文件或文件夹
         POST https://webapi.115.com/share/receive
         payload:
             - share_code: str
             - receive_code: str
             - file_id: int | str             # 有多个时，用逗号 "," 分隔
-            - cid: int | str = 0             # 这是你网盘的文件夹 cid
+            - cid: int | str = <default>     # 这是你网盘的文件夹 cid
             - user_id: int | str = <default>
         """
         api = "https://webapi.115.com/share/receive"
         payload = {"cid": 0, **payload}
         request_kwargs.pop("parse", None)
         return self.request(api, "POST", data=payload, async_=async_, **request_kwargs)
 
@@ -4933,15 +4934,15 @@
         **request_kwargs, 
     ) -> dict | Awaitable[dict]:
         """秒传接口，此接口是对 `upload_init` 的封装。
         NOTE: 
             - 文件大小 和 sha1 是必需的，只有 sha1 是没用的。
             - 如果文件大于等于 1 MB (1048576 B)，就需要 2 次检验一个范围哈希，就必须提供 `read_range_bytes_or_hash`
         """
-        if filesize >= 1 << 20:
+        if filesize >= 1 << 20 and read_range_bytes_or_hash is None:
             raise ValueError("filesize >= 1 MB, thus need pass the `read_range_bytes_or_hash` argument")
         if async_:
             async def async_request():
                 nonlocal async_, file_sha1, read_range_bytes_or_hash
                 async_ = cast(Literal[True], async_)
                 file_sha1 = file_sha1.upper()
                 target = f"U_1_{pid}"
```

### Comparing `python_115-0.0.8.3.3/p115/component/fs.py` & `python_115-0.0.8.3.4/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/component/fs_base.py` & `python_115-0.0.8.3.4/p115/component/fs_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         if type(self) is not type(path) or self.fs.client != path.fs.client:
             return False
         return self.id > path.id
 
     def __hash__(self, /) -> int:
         return hash((self.fs.client, self.id))
 
+    def __index__(self, /) -> int:
+        return self.id
+
     def __iter__(self, /) -> Iterator[str]:
         return iter(self.__dict__)
 
     def __le__(self, path, /) -> bool:
         if type(self) is not type(path) or self.fs.client != path.fs.client:
             return False
         return self.id <= self.id
```

### Comparing `python_115-0.0.8.3.3/p115/component/fs_share.py` & `python_115-0.0.8.3.4/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/component/fs_zip.py` & `python_115-0.0.8.3.4/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/p115/component/offline.py` & `python_115-0.0.8.3.4/p115/component/offline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,49 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__all__ = ["P115Offline"]
+__all__ = ["P115Offline", "P115OfflineClearEnum"]
 
 from asyncio import run
 from collections.abc import Callable, Iterable, Iterator
+from enum import Enum
 from hashlib import sha1
 from time import time
 from types import MappingProxyType
+from typing import Self
 
 from magnet2torrent import Magnet2Torrent # type: ignore
 
 from .client import check_response, P115Client
+from .fs import P115Path
+
+
+class P115OfflineClearEnum(Enum):
+    completed = 0
+    all = 1
+    failed = 2
+    downloading = 3
+    completed_and_files = 4
+    failed_and_files = 5
+
+    @classmethod
+    def ensure(cls, val, /) -> Self:
+        if isinstance(val, cls):
+            return val
+        try:
+            if isinstance(val, str):
+                return cls[val]
+        except KeyError:
+            pass
+        return cls(val)
 
 
 class P115Offline:
+    "离线任务列表"
     __slots__ = ("client", "_sign_time")
 
     client: P115Client
     _sign_time: MappingProxyType
 
     def __init__(self, /, client: str | P115Client):
         if isinstance(client, str):
@@ -38,43 +62,63 @@
                 return item
         raise LookupError(f"no such hash: {hash!r}")
 
     def __iter__(self, /) -> Iterator[dict]:
         return self.iter()
 
     def __len__(self, /) -> int:
+        "计算共有多少个离线任务"
         return check_response(self.client.offline_list())["count"]
 
     def __repr__(self, /) -> str:
         cls = type(self)
         module = cls.__module__
         name = cls.__qualname__
         if module != "__main__":
             name = module + "." + name
         return f"<{name}(client={self.client!r}) at {hex(id(self))}>"
 
     @property
+    def download_paths_raw(self, /) -> list[dict]:
+        "离线下载的目录列表"
+        return check_response(self.client.offline_download_path())["data"]
+
+    @property
+    def download_paths(self, /) -> list[P115Path]:
+        "离线下载的目录列表"
+        as_path = self.client.fs.as_path
+        return [as_path(int(attr["file_id"])) for attr in self.download_paths_raw]
+
+    @property
     def sign_time(self, /) -> MappingProxyType:
+        "签名和时间等信息"
         try:
             sign_time = self._sign_time
             if time() - sign_time["time"] < 30 * 60:
                 return sign_time
         except AttributeError:
             pass
         info = check_response(self.client.offline_info())
         sign_time = self._sign_time = MappingProxyType({"sign": info["sign"], "time": info["time"]})
         return sign_time
 
+    @property
+    def torrent_path(self, /) -> P115Path:
+        "添加 BT 种子任务的默认上传路径"
+        client = self.client
+        return client.fs.as_path(int(client.offline_upload_torrent_path()['cid']))
+
     def add(
         self, 
         urls: str | Iterable[str], 
         /, 
         pid: None | int = None, 
         savepath: None | str = None, 
     ) -> dict:
+        "用（1 个或若干个）链接创建离线任务"
         payload: dict
         if isinstance(urls, str):
             payload = {"url": urls}
             method = self.client.offline_add_url
         else:
             payload = {f"url[{i}]": url for i, url in enumerate(urls)}
             if not payload:
@@ -91,14 +135,15 @@
         self, 
         torrent_or_magnet_or_sha1_or_fid: int | bytes | str, 
         /, 
         pid: None | int = None, 
         savepath: None | str = None, 
         predicate: None | str | Callable[[dict], bool] = None, 
     ) -> dict:
+        "用 BT 种子创建离线任务"
         resp = check_response(self.torrent_info(torrent_or_magnet_or_sha1_or_fid))
         if predicate is None:
             wanted = ",".join(
                 str(i) for i, info in enumerate(resp["torrent_filelist_web"])
                 if info["wanted"]
             )
         elif isinstance(predicate, str):
@@ -114,32 +159,39 @@
             "savepath": resp["torrent_name"] if savepath is None else savepath, 
         }
         if pid is not None:
             payload["wp_path_id"] = pid
         payload.update(self.sign_time)
         return check_response(self.client.offline_add_torrent(payload))
 
-    # TOOD: 使用 enum
-    def clear(self, /, flag: int = 1) -> dict:
+    def clear(
+        self, 
+        /, 
+        flag: int | str | P115OfflineClearEnum = P115OfflineClearEnum.all, 
+    ) -> dict:
         """清空离线任务列表
-
         :param flag: 操作目标
-            - 0: 已完成
-            - 1: 全部（默认值）
-            - 2: 已失败
-            - 3: 进行中
-            - 4: 已完成+删除源文件
-            - 5: 全部+删除源文件
+            - 已完成: 0, 'completed', P115OfflineClearEnum.completed
+            - 全部: 1, 'all', P115OfflineClearEnum.all # 默认值
+            - 已失败: 2, 'failed', P115OfflineClearEnum.failed
+            - 进行中: 3, 'downloading', P115OfflineClearEnum.downloading
+            - 已完成+删除源文件: 4, 'completed_and_files', P115OfflineClearEnum.completed_and_files
+            - 全部+删除源文件: 5, 'failed_and_files', P115OfflineClearEnum.failed_and_files
         """
-        return check_response(self.client.offline_clear(flag))
+        flag = P115OfflineClearEnum(flag)
+        return check_response(self.client.offline_clear(flag.value))
 
     def get(self, hash: str, /, default=None):
+        "用 infohash 查询离线任务"
         return next((item for item in self if item["info_hash"] == hash), default)
 
     def iter(self, /, start_page: int = 1) -> Iterator[dict]:
+        """迭代获取离线任务
+        :start_page: 开始页数，从 1 开始计数，迭代从这个页数开始，到最大页数结束
+        """
         if start_page < 1:
             page = 1
         else:
             page = start_page
         resp = check_response(self.client.offline_list(page))
         if not resp["tasks"]:
             return
@@ -153,36 +205,51 @@
             if count != resp["count"]:
                 raise RuntimeError("detected count changes during iteration")
             if not resp["tasks"]:
                 return
             yield from resp["tasks"]
 
     def list(self, /, page: int = 0) -> list[dict]:
+        """获取离线任务列表
+        :param page: 获取第 `page` 页的数据，从 1 开始计数，如果小于等于 0 则返回全部
+        """
         if page <= 0:
             return list(self.iter())
         return check_response(self.client.offline_list(page))["tasks"]
 
     def remove(
         self, 
         hashes: str | Iterable[str], 
         /, 
         remove_files: bool = False, 
     ) -> dict:
+        """用 infohash 查询并移除（1 个或若干个）离线任务
+        :param hashes: （1 个或若干个）离线任务的 infohash
+        :param remove_files: 移除任务时是否也删除已转存的文件
+        """
         if isinstance(hashes, str):
             payload = {"hash[0]": hashes}
         else:
             payload = {f"hash[{i}]": h for i, h in enumerate(hashes)}
             if not payload:
                 raise ValueError("no `hash` specified")
         if remove_files:
             payload["flag"] = "1"
         payload.update(self.sign_time)
         return check_response(self.client.offline_remove(payload))
 
     def torrent_info(self, torrent_or_magnet_or_sha1_or_fid: int | bytes | str, /) -> dict:
+        """获取种子的信息
+        :param torrent_or_magnet_or_sha1_or_fid: BT 种子
+            - bytes: 种子的二进制数据（如果种子从未被人上传过 115，就会先被上传）
+            - str:
+                - 磁力链接
+                - 种子文件的 sha1，但要求这个种子曾被人上传到 115
+            - int: 种子文件在你的网盘上的文件 id
+        """
         torrent = None
         if isinstance(torrent_or_magnet_or_sha1_or_fid, int):
             fid = torrent_or_magnet_or_sha1_or_fid
             resp = check_response(self.client.fs_file(fid))
             sha = resp["data"][0]["sha1"]
         elif isinstance(torrent_or_magnet_or_sha1_or_fid, bytes):
             torrent = torrent_or_magnet_or_sha1_or_fid
```

### Comparing `python_115-0.0.8.3.3/p115/component/recyclebin.py` & `python_115-0.0.8.3.4/p115/component/recyclebin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from collections.abc import Iterable, Iterator
 
 from .client import check_response, P115Client
 
 
 class P115Recyclebin:
-    "封装回收站"
+    "回收站"
     __slots__ = ("client", "password")
 
     def __init__(
         self, 
         client: str | P115Client, 
         /, 
         password: int | str = "",
```

### Comparing `python_115-0.0.8.3.3/p115/component/sharing.py` & `python_115-0.0.8.3.4/p115/component/sharing.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __all__ = ["P115Sharing"]
 
 from collections.abc import Iterable, Iterator
 from typing import Literal
 
 from .client import check_response, P115Client
+from .fs import P115Path
 
 
 class P115Sharing:
-    "封装自己的分享列表"
+    "自己的分享列表"
     __slots__ = "client",
 
     def __init__(self, client: str | P115Client, /):
         if isinstance(client, str):
             client = P115Client(client)
         self.client = client
 
@@ -51,14 +52,18 @@
         cls = type(self)
         module = cls.__module__
         name = cls.__qualname__
         if module != "__main__":
             name = module + "." + name
         return f"<{name}(client={self.client!r}) at {hex(id(self))}>"
 
+    @property
+    def receive_path(self, /) -> P115Path:
+        return self.client.fs.as_path("我的接收")
+
     @check_response
     def add(
         self, 
         file_ids: int | str | Iterable[int | str], 
         /, 
         is_asc: Literal[0, 1] = 1, 
         order: str = "file_name", 
@@ -88,17 +93,19 @@
     def clear(self, /) -> dict:
         "清空分享列表"
         return self.client.share_update({
             "share_code": ",".join(item["share_code"] for item in self), 
             "action": "cancel", 
         })
 
-    def code_of(self, snap_id: int, /) -> str:
+    def code_of(self, code_or_id: int | str, /) -> str:
         "获取 id 对应的分享码"
-        return self[snap_id]["share_code"]
+        if isinstance(code_or_id, str):
+            return code_or_id
+        return self[code_or_id]["share_code"]
 
     def get(
         self, 
         code_or_id: int | str, 
         /, 
         default=None, 
     ):
@@ -149,41 +156,37 @@
     @check_response
     def remove(
         self, 
         code_or_id_s: int | str | Iterable[int | str], 
         /, 
     ) -> dict:
         "用分享码或 id 查询并删除分享"
-        def share_code_of(code_or_id: int | str) -> str:
-            if isinstance(code_or_id, str):
-                return code_or_id
-            return self[code_or_id]["share_code"]
         if isinstance(code_or_id_s, (int, str)):
-            share_code = share_code_of(code_or_id_s)
+            share_code = self.code_of(code_or_id_s)
         else:
-            share_code = ",".join(map(share_code_of, code_or_id_s))
+            share_code = ",".join(map(self.code_of, code_or_id_s))
             if not share_code:
                 raise ValueError("no `share_code` or `snap_id` specified")
         return self.client.share_update({
             "share_code": share_code, 
             "action": "cancel", 
         })
 
     @check_response
     def update(
         self, 
+        code_or_id: int | str, 
         /, 
-        share_code: str, 
         **payload, 
     ) -> dict:
-        """更新分享信息
+        """用分享码或 id 查询并更新分享信息
         payload:
-            - share_code: str
             - receive_code: str = <default>         # 访问密码（口令）
             - share_duration: int = <default>       # 分享天数: 1(1天), 7(7天), -1(长期)
             - is_custom_code: 0 | 1 = <default>     # 用户自定义口令（不用管）
             - auto_fill_recvcode: 0 | 1 = <default> # 分享链接自动填充口令（不用管）
             - share_channel: int = <default>        # 分享渠道代码（不用管）
             - action: str = <default>               # 操作: 取消分享 "cancel"
         """
-        return self.client.share_update({"share_code": share_code, **payload})
+        payload["share_code"] = self.code_of(code_or_id)
+        return self.client.share_update(payload)
```

### Comparing `python_115-0.0.8.3.3/p115/tool/__init__.py` & `python_115-0.0.8.3.4/p115/tool/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,23 +79,23 @@
     :param sample_count: 单个文字的采样次数，共会执行 10 * sample_count 次识别
     :param crack: 破解验证码图片，输入图片的二进制数据，输出识别的字符串
 
     :return: 是否破解成功
 
     你可以反复尝试，直到破解成功，代码如下
 
-        while not crack_115_captcha(client):
+        while not crack_captcha(client):
             pass
 
     如果你需要检测是否存在验证码，然后进行破解，代码如下
 
         resp = client.download_url_web("a")
         if not resp["state"] and resp["code"] == 911:
             print("出现验证码，尝试破解")
-            while not crack_115_captcha(client):
+            while not crack_captcha(client):
                 print("破解失败，再次尝试")
     """
     global CAPTCHA_CRACK
     if crack is None:
         try:
             crack = CAPTCHA_CRACK
         except NameError:
```

### Comparing `python_115-0.0.8.3.3/pyproject.toml` & `python_115-0.0.8.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.3.3"
+version = "0.0.8.3.4"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.3.3/readme.md` & `python_115-0.0.8.3.4/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.3/PKG-INFO` & `python_115-0.0.8.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.3.3
+Version: 0.0.8.3.4
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

