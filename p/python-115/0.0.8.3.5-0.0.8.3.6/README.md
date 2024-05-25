# Comparing `tmp/python_115-0.0.8.3.5.tar.gz` & `tmp/python_115-0.0.8.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.3.5.tar", max compression
+gzip compressed data, was "python_115-0.0.8.3.6.tar", max compression
```

## Comparing `python_115-0.0.8.3.5.tar` & `python_115-0.0.8.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.5/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.5/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.5/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.5/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.5/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8669 2024-05-25 05:50:21.865251 python_115-0.0.8.3.5/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.5/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.5/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.5/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.5/p115/component/cipher.py
--rwxr-xr-x   0        0        0   246390 2024-05-25 05:26:13.883965 python_115-0.0.8.3.5/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.5/p115/component/exception.py
--rwxr-xr-x   0        0        0    56840 2024-05-25 05:49:19.298545 python_115-0.0.8.3.5/p115/component/fs.py
--rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.3.5/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.5/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.5/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.3.5/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.3.5/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.3.5/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.3.5/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.5/p115/py.typed
--rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.3.5/p115/tool/__init__.py
--rw-r--r--   0        0        0     1665 2024-05-25 05:50:34.034333 python_115-0.0.8.3.5/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.5/readme.md
--rw-r--r--   0        0        0    36371 1970-01-01 00:00:00.000000 python_115-0.0.8.3.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.6/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.6/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.6/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.6/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.6/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.6/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.6/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.6/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8669 2024-05-25 05:50:21.865251 python_115-0.0.8.3.6/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.6/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.6/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.6/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.6/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.6/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.6/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.6/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.6/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   246404 2024-05-25 12:33:44.062810 python_115-0.0.8.3.6/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.6/p115/component/exception.py
+-rwxr-xr-x   0        0        0    60836 2024-05-25 12:32:04.821744 python_115-0.0.8.3.6/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.3.6/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.6/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.6/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.3.6/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.3.6/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.3.6/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.3.6/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.6/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.3.6/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-25 12:34:05.067947 python_115-0.0.8.3.6/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.6/readme.md
+-rw-r--r--   0        0        0    36371 1970-01-01 00:00:00.000000 python_115-0.0.8.3.6/PKG-INFO
```

### Comparing `python_115-0.0.8.3.5/LICENSE` & `python_115-0.0.8.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/cmd/iterdir.py` & `python_115-0.0.8.3.6/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/cmd/qrcode.py` & `python_115-0.0.8.3.6/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/__init__.py` & `python_115-0.0.8.3.6/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/cipher.py` & `python_115-0.0.8.3.6/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/client.py` & `python_115-0.0.8.3.6/p115/component/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 RequestVarT = TypeVar("RequestVarT", dict, Callable)
 RSA_ENCODER: Final = P115RSACipher()
 ECDH_ENCODER: Final = P115ECDHCipher()
 CRE_SHARE_LINK_search = re_compile(r"/s/(?P<share_code>\w+)(\?password=(?P<receive_code>\w+))?").search
 APP_VERSION: Final = "99.99.99.99"
 
-request = partial(httpx_request, parse=lambda _, content: loads(content))
+request = partial(httpx_request, parse=lambda _, content: loads(content), verify=False)
 
 
 def to_base64(s: bytes | str, /) -> str:
     if isinstance(s, str):
         s = bytes(s, "utf-8")
     return str(b64encode(s), "ascii")
```

### Comparing `python_115-0.0.8.3.5/p115/component/fs.py` & `python_115-0.0.8.3.6/p115/component/fs.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 
 from collections import deque, ChainMap
 from collections.abc import (
     Callable, Iterable, Iterator, Mapping, MutableMapping, Sequence, 
 )
 from datetime import datetime
 from io import BytesIO, TextIOWrapper
-from os import fsdecode, fspath, makedirs, scandir, stat_result, PathLike
-from os import path as ospath
+from os import (
+    path as ospath, fsdecode, fspath, makedirs, remove, rmdir, scandir, stat_result, PathLike
+)
+from pathlib import Path
 from posixpath import join as joinpath, splitext
 from shutil import SameFileError
 from stat import S_IFDIR, S_IFREG
 from typing import cast, Literal, Optional, Self
 from uuid import uuid4
 
 from filewrap import SupportsRead
@@ -95,15 +97,15 @@
 class P115Path(P115PathBase):
     fs: P115FileSystem
 
     def copy(
         self, 
         /, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         overwrite_or_ignore: Optional[bool] = None, 
     ) -> Optional[Self]:
         attr = self.fs.copy(
             self, 
             dst_path, 
             pid=pid, 
             overwrite_or_ignore=overwrite_or_ignore, 
@@ -131,51 +133,51 @@
         self.__dict__.update(self.fs.makedirs(self, exist_ok=exist_ok))
         return self
 
     def move(
         self, 
         /, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Self:
         attr = self.fs.move(self, dst_path, pid)
         if attr:
             self.__dict__.update(attr)
         return self
 
     def remove(self, /, recursive: bool = True) -> dict:
         return self.fs.remove(self, recursive=recursive)
 
     def rename(
         self, 
         /, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Self:
         attr = self.fs.rename(self, dst_path, pid)
         if attr:
             self.__dict__.update(attr)
         return self
 
     def renames(
         self, 
         /, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Self:
         attr = self.fs.renames(self, dst_path, pid)
         if attr:
             self.__dict__.update(attr)
         return self
 
     def replace(
         self, 
         /, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Self:
         attr = self.fs.replace(self, dst_path, pid)
         if attr:
             self.__dict__.update(attr)
         return self
 
     def rmdir(self, /) -> dict:
@@ -274,17 +276,17 @@
         file: None | str | bytes | bytearray | memoryview | PathLike = None, 
         /, 
     ):
         if file is None:
             return self.touch(id_or_path)
         elif isinstance(file, PathLike):
             if ospath.isdir(file):
-                return list(self.upload_tree(file, id_or_path, no_root=True, overwrite_or_ignore=True))
+                return list(self.upload_tree(file, id_or_path, no_root=True, overwrite=True))
             else:
-                return self.upload(file, id_or_path, overwrite_or_ignore=True)
+                return self.upload(file, id_or_path, overwrite=True)
         elif isinstance(file, str):
             return self.write_text(id_or_path, file)
         else:
             return self.write_bytes(id_or_path, file)
 
     @classmethod
     def login(
@@ -394,15 +396,17 @@
     def fs_search(self, payload: str | dict, /) -> dict:
         return self.client.fs_search(payload)
 
     @check_response
     def space_summury(self, /) -> dict:
         return self.client.fs_space_summury()
 
-    def _upload(self, file, name, pid: int = 0) -> dict:
+    def _upload(self, file, name, pid: Optional[int] = None) -> dict:
+        if pid is None:
+            pid = self.id
         if not hasattr(file, "getbuffer") or len(file.getbuffer()) > 0:
             try:
                 file.seek(0, 1)
             except:
                 pass
             else:
                 resp = self.client.upload_file(file, name, pid)
@@ -524,15 +528,15 @@
                 for k in tuple(k for k in path_to_id if startswith(k, old_path)):
                     pop_path(k)
 
     def iterdir(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         refresh: bool = False, 
         **kwargs, 
     ) -> Iterator[AttrDict]:
         path_to_id = self.path_to_id
         attr_cache = self.attr_cache
         get_version = self.get_version
         version = None
@@ -685,15 +689,15 @@
                         pass
         return attr
 
     def _attr_path(
         self, 
         path: str | PathLike[str] | Sequence[str], 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     )  -> AttrDict:
         if isinstance(path, PathLike):
             path = fspath(path)
         if isinstance(path, str):
             if path.startswith("/"):
                 pid = 0
         elif path and path[0] == "":
@@ -730,34 +734,31 @@
                 raise FileNotFoundError(errno.ENOENT, f"no such file {name!r} (in {pid!r})")
         return attr
 
     def attr(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     )  -> AttrDict:
         if isinstance(id_or_path, P115Path):
-            return self._attr(id_or_path.id)
+            return id_or_path.__dict__
         elif isinstance(id_or_path, dict):
-            attr = id_or_path
-            if "id" in attr:
-                return self._attr(attr["id"])
-            return self._attr_path(attr["path"])
+            return id_or_path
         elif isinstance(id_or_path, int):
             return self._attr(id_or_path)
         else:
             return self._attr_path(id_or_path, pid)
 
     def copy(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         overwrite_or_ignore: Optional[bool] = None, 
         recursive: bool = False, 
     ) -> Optional[dict]:
         src_patht = self.get_patht(src_path, pid)
         dst_patht = self.get_patht(dst_path, pid)
         src_fullpath = joins(src_patht)
         dst_fullpath = joins(dst_patht)
@@ -846,20 +847,22 @@
                 if resp["data"]:
                     dst_name = resp["data"][str(dst_id)]
                 self.fs_move(dst_id, dst_pid)
             finally:
                 self.fs_delete(tempdir_id)
             return self.attr(dst_id)
 
+    # TODO: 去除 overwrite_or_ignore 参数，拆分为 overwrite 和 onerror
+    # TODO: 支持多线程操作
     def copytree(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType = "", 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         overwrite_or_ignore: Optional[bool] = None, 
         **kwargs, 
     ) -> Optional[dict]:
         src_attr = self.attr(src_path, pid)
         src_id = src_attr["id"]
         if not src_attr["is_directory"]:
             return self.copy(
@@ -941,41 +944,41 @@
             )
         return ls
 
     def desc(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         desc: None | str = None, 
     ) -> str:
         fid = self.get_id(id_or_path, pid)
         if fid == 0:
             return ""
         if desc is None:
             return check_response(self.client.fs_desc_get(fid))["desc"]
         else:
             return check_response(self.client.fs_desc(fid, desc))["file_description"]
 
     def get_ancestors(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> list[dict]:
         attr = self.attr(id_or_path, pid)
         ls = self._dir_get_ancestors(attr["parent_id"])
         ls.append({"name": attr["name"], "id": attr["id"], "parent_id": attr["parent_id"], "is_directory": attr["is_directory"]})
         return ls
 
     def dirlen(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> int:
         return self.fs_files(self.get_id(id_or_path, pid), limit=1)["count"]
 
     def get_id_from_pickcode(self, /, pickcode: str = "") -> int:
         if not pickcode:
             return 0
         return self.get_info_from_pickcode(pickcode)["id"]
@@ -983,23 +986,23 @@
     def get_info_from_pickcode(self, /, pickcode: str) -> dict:
         return self.client.download_url(pickcode, strict=False, detail=True).__dict__
 
     def get_pickcode(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> str:
         return self.attr(id_or_path, pid).get("pickcode", "")
 
     def get_url(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         headers: Optional[Mapping] = None, 
         detail: bool = False, 
     ) -> str:
         attr = self.attr(id_or_path, pid)
         if attr["is_directory"]:
             raise IsADirectoryError(errno.EISDIR, f"{attr['path']!r} (id={attr['id']!r}) is a directory")
         return self.client.download_url(
@@ -1022,15 +1025,15 @@
             headers=headers, 
         )
 
     def hide(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         show: None | bool = None, 
     ) -> bool:
         if show is None:
             return self.attr(id_or_path, pid)["hidden"]
         else:
             fid = self.get_id(id_or_path, pid)
             if fid == 0:
@@ -1053,15 +1056,15 @@
             show = not self.hidden_mode
         check_response(self.client.fs_hidden_switch({"show": int(show), "safe_pwd": password or self.password}))
 
     def is_empty(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> bool:
         attr: dict | P115Path
         if isinstance(id_or_path, P115Path):
             attr = id_or_path
         else:
             try:
                 attr = self.attr(id_or_path, pid)
@@ -1071,15 +1074,15 @@
             return self.dirlen(attr["id"]) > 0
         return attr["size"] == 0
 
     def iter_repeat(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         page_size: int = 1150, 
     ) -> Iterator[dict]:
         if page_size <= 0:
             page_size = 1150
         payload = {
             "file_id": self.get_id(id_or_path, pid), 
             "offset": 0, 
@@ -1093,23 +1096,23 @@
                 break
             payload["offset"] += page_size # type: ignore
 
     def labels(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> list[dict]:
         return self.attr(id_or_path, pid)["labels"]
 
     def makedirs(
         self, 
         path: str | PathLike[str] | Sequence[str] | AttrDict, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         exist_ok: bool = False, 
     ) -> dict:
         if isinstance(path, dict):
             patht, parents = splits(path["path"])
         elif isinstance(path, (str, PathLike)):
             patht, parents = splits(fspath(path))
         else:
@@ -1144,15 +1147,15 @@
             raise FileExistsError(errno.EEXIST, f"{path!r} (in {pid!r}) exists")
         return attr
 
     def mkdir(
         self, 
         path: str | PathLike[str] | Sequence[str], 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> dict:
         if isinstance(path, (str, PathLike)):
             patht, parents = splits(fspath(path))
         else:
             patht = [p for p in path if p]
             parents = 0
         if not patht or patht == [""]:
@@ -1181,15 +1184,15 @@
         return self.attr(int(resp["cid"]))
 
     def move(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Optional[dict]:
         try:
             dst_attr = self.attr(dst_path, pid)
         except FileNotFoundError:
             return self.rename(src_path, dst_path, pid)
         src_attr = self.attr(src_path, pid)
         src_id = src_attr["id"]
@@ -1209,15 +1212,15 @@
         raise FileExistsError(errno.EEXIST, f"destination {dst_id!r} already exists")
 
     # TODO: 由于 115 网盘不支持删除里面有超过 5 万个文件等文件夹，因此需要增加参数，支持在失败后，拆分任务，返回一个 Future 对象，可以获取已完成和未完成，并且可以随时取消
     def remove(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         recursive: bool = False, 
     ) -> dict:
         attr = self.attr(id_or_path, pid)
         id = attr["id"]
         clear_cache = self._clear_cache
         if attr["is_directory"]:
             if not recursive:
@@ -1232,15 +1235,15 @@
         clear_cache(attr)
         return attr
 
     def removedirs(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Optional[dict]:
         try:
             attr = self.attr(id_or_path, pid)
         except FileNotFoundError:
             return None
         if not attr["is_directory"]:
             raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
@@ -1268,15 +1271,15 @@
 
     # TODO: 支持 dst_path 从 src_path 开始的相对路径
     def rename(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         replace: bool = False, 
     ) -> Optional[dict]:
         src_patht = self.get_patht(src_path, pid)
         dst_patht = self.get_patht(dst_path, pid)
         src_fullpath = joins(src_patht)
         dst_fullpath = joins(dst_patht)
         if src_patht == dst_patht:
@@ -1354,36 +1357,36 @@
                 raise
 
     def renames(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Optional[dict]:
         result = self.rename(src_path, dst_path, pid=pid)
         if result:
             self.removedirs(result["parent_id"])
             return result
         return None
 
     def replace(
         self, 
         /, 
         src_path: IDOrPathType, 
         dst_path: IDOrPathType, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> Optional[dict]:
         return self.rename(src_path, dst_path, pid=pid, replace=True)
 
     def rmdir(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> dict:
         attr = self.attr(id_or_path, pid)
         id = attr["id"]
         if id == 0:
             raise PermissionError(errno.EPERM, "remove the root directory is not allowed")
         elif not attr["is_directory"]:
             raise NotADirectoryError(errno.ENOTDIR, f"{id_or_path!r} (in {pid!r}) is not a directory")
@@ -1393,23 +1396,23 @@
         self._clear_cache(attr) 
         return attr
 
     def rmtree(
         self, 
         id_or_path: IDOrPathType, 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> dict:
         return self.remove(id_or_path, pid, recursive=True)
 
     def score(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         score: None | int = None, 
     ) -> int:
         if score is None:
             return self.attr(id_or_path, pid).get("score", 0)
         else:
             fid = self.get_id(id_or_path, pid)
             if fid == 0:
@@ -1417,15 +1420,15 @@
             self.client.fs_score(fid, score)
             return score
 
     def search(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         search_value: str = "", 
         page_size: int = 1_000, 
         offset: int = 0, 
         **kwargs, 
     ) -> Iterator[P115Path]:
         assert page_size > 0
         attr = self.attr(id_or_path, pid)
@@ -1462,15 +1465,15 @@
             if offset >= resp["count"]:
                 break
 
     def star(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         star: None | bool = None, 
     ) -> bool:
         if star is None:
             return self.attr(id_or_path, pid).get("star", False)
         else:
             fid = self.get_id(id_or_path, pid)
             if fid == 0:
@@ -1478,15 +1481,15 @@
             check_response(self.client.fs_star(fid, star))
             return star
 
     def stat(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> stat_result:
         attr = self.attr(id_or_path, pid)
         is_dir = attr["is_directory"]
         return stat_result((
             (S_IFDIR if is_dir else S_IFREG) | 0o777, # mode
             cast(int, attr["id"]), # ino
             cast(int, attr["parent_id"]), # dev
@@ -1499,147 +1502,260 @@
             cast(float, attr.get("ctime", 0)), # ctime
         ))
 
     def touch(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> dict:
         try:
             return self.attr(id_or_path, pid)
         except FileNotFoundError:
             if isinstance(id_or_path, int):
                 raise ValueError(f"no such id: {id_or_path!r}")
             return self.upload(BytesIO(), id_or_path, pid=pid)
 
     # TODO: 增加功能，返回一个 Task 对象，可以获取上传进度，可随时取消
-    # TODO: 支持一个参数，不计算 sha1 等信息，直接就进行上传（就像网页版那样）
     def upload(
         self, 
         /, 
         file: bytes | str | PathLike | SupportsRead[bytes], 
         path: IDOrPathType = "", 
-        pid: Optional[int] = None, 
-        overwrite_or_ignore: Optional[bool] = None, 
+        pid: None | int = None, 
+        overwrite: bool = False, 
+        remove_success: bool = False, 
     ) -> dict:
-        fio: SupportsRead[bytes]
-        dirname: str | Sequence[str] = ""
         name: str = ""
-        if not path or isinstance(path, int):
-            pass
-        elif isinstance(path, (str, PathLike)):
-            dirname, name = ospath.split(path)
+        if not path:
+            pid = self.id if pid is None else self.get_id(pid)
         else:
-            *dirname, name = (p for p in path if p)
-        if hasattr(file, "read"):
-            fio = cast(SupportsRead[bytes], file)
+            attr: Mapping
+            if isinstance(path, int):
+                attr = self.attr(path)
+            elif isinstance(path, (str, PathLike)):
+                dirname, name = ospath.split(path)
+                attr = self.attr(dirname, pid)
+            elif isinstance(path, Sequence):
+                if len(path) == 1 and path[0] == "":
+                    attr = self.attr(0)
+                else:
+                    *dirname_t, name = path
+                    attr = self.attr(dirname_t, pid)
+            else:
+                attr = path
+            pid = attr["id"]
+            if attr["is_directory"]:
+                if name:
+                    try:
+                        attr = self.attr([name], pid)
+                        if attr["is_directory"]:
+                            pid = attr["id"]
+                            name = ""
+                    except FileNotFoundError:
+                        pass
+            if not attr["is_directory"]:
+                if name:
+                    raise NotADirectoryError(errno.ENOTDIR, f"parent path {attr['path']!r} is not directory")
+                elif overwrite:
+                    self.remove(attr)
+                    name = attr["name"]
+                    pid = attr["parent_id"]
+                else:
+                    raise FileExistsError(errno.EEXIST, f"remote path {attr['path']!r} already exists")
+
+        fio: SupportsRead[bytes]
+        if isinstance(file, SupportsRead):
+            fio = file
             if not name:
                 try:
-                    name = ospath.basename(file.name) # type: ignore
+                    name = ospath.basename(getattr(file, "name"))
                 except:
                     pass
         elif isinstance(file, (str, PathLike)):
             file = fsdecode(file)
             fio = open(file, "rb")
             if not name:
                 name = ospath.basename(file)
         else:
             fio = BytesIO(file)
-        if pid is None:
-            pid = self.id
-        if dirname:
-            pid = cast(int, self.makedirs(dirname, pid=pid, exist_ok=True)["id"])
-        if name:
+
+        resp = self._upload(fio, name, pid)
+        if remove_success and isinstance(file, (str, PathLike)):
             try:
-                attr = self._attr_path([name], pid)
-            except FileNotFoundError:
+                remove(file)
+            except OSError:
                 pass
-            else:
-                if overwrite_or_ignore is None:
-                    raise FileExistsError(errno.EEXIST, f"{path!r} (in {pid!r}) exists")
-                elif attr["is_directory"]:
-                    raise IsADirectoryError(errno.EISDIR, f"{path!r} (in {pid!r}) is a directory")
-                elif not overwrite_or_ignore:
-                    return attr
-                self.fs_delete(attr["id"])
-        return self._upload(fio, name, pid)
+        return resp
 
     # TODO: 为了提升速度，之后会支持多线程上传，以及直接上传不做检查
     # TODO: 返回上传任务的迭代器，包含进度相关信息，以及最终的响应信息
-    # TODO: 增加参数，onerror, predicate, submit 等
+    # TODO: 增加参数，predicate
+    # TODO: 增加参数，submit，可以把任务提交给线程池
     def upload_tree(
         self, 
         /, 
         local_path: str | PathLike[str] = ".", 
         path: IDOrPathType = "", 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         no_root: bool = False, 
-        overwrite_or_ignore: Optional[bool] = None, 
+        overwrite: bool = False, 
+        remove_success: bool = False, 
+        predicate: None | Callable[[Path], bool] = None, 
+        onerror: bool | Callable[[OSError], bool] = False, 
     ) -> Iterator[dict]:
+        remote_path_attr_map: None | dict[str, dict] = None
         try:
             attr = self.attr(path, pid)
         except FileNotFoundError:
             if isinstance(path, int):
                 raise ValueError(f"no such id: {path!r}")
-            attr = self.makedirs(path, pid, exist_ok=True)
+            attr = self.makedirs(path, pid=pid, exist_ok=True)
+            remote_path_attr_map = {}
         else:
             if not attr["is_directory"]:
-                raise NotADirectoryError(errno.ENOTDIR, f"{attr['path']!r} (id={attr['id']!r}) is not a directory")
-        pid = attr["id"]
+                raise NotADirectoryError(
+                    errno.ENOTDIR, 
+                    f"{attr['path']!r} (id={attr['id']!r}) is not a directory", 
+                )
+        pid = cast(int, attr["id"])
+
+        local_path = ospath.normpath(local_path)
         try:
-            it = scandir(local_path or ".")
-        except NotADirectoryError:
-            yield self.upload(
-                local_path, 
-                [ospath.basename(local_path)], 
-                pid=pid, 
-                overwrite_or_ignore=overwrite_or_ignore, 
-            )
-        else:
+            try:
+                if predicate is None:
+                    subpaths = tuple(scandir(local_path))
+                else:
+                    subpaths = tuple(filter(lambda e: predicate(Path(e)), scandir(local_path)))
+                if not subpaths:
+                    return
+            except NotADirectoryError:
+                try:
+                    yield self.upload(
+                        local_path, 
+                        [ospath.basename(local_path)], 
+                        pid=pid, 
+                        overwrite=overwrite, 
+                        remove_success=remove_success, 
+                    )
+                except OSError as e:
+                    if onerror is True:
+                        raise e
+                    elif onerror is False:
+                        pass
+                    else:
+                        onerror(e)
+                    return
             if not no_root:
-                attr = self.makedirs(ospath.basename(local_path), pid, exist_ok=True)
-                pid = attr["parent_id"]
-            for entry in it:
-                if entry.is_dir():
+                attr = self.makedirs(
+                    [ospath.basename(local_path)], 
+                    pid=pid, 
+                    exist_ok=True, 
+                )
+                pid = attr["id"]
+                remote_path_attr_map = {}
+            elif remote_path_attr_map is None:
+                remote_path_attr_map = {a["name"]: a for a in self.iterdir(pid)}
+        except OSError as e:
+            if onerror is True:
+                raise e
+            elif onerror is False:
+                pass
+            else:
+                onerror(e)
+            return
+
+        for entry in subpaths:
+            name = entry.name
+            isdir = entry.is_dir()
+            remote_path_attr = remote_path_attr_map.get(name)
+            if remote_path_attr and isdir != remote_path_attr["is_directory"]:
+                if onerror is True:
+                    raise FileExistsError(
+                        errno.EEXIST, 
+                        f"remote path {remote_path_attr['path']!r} already exists", 
+                    )
+                elif onerror is False:
+                    pass
+                else:
+                    onerror(FileExistsError(
+                        errno.EEXIST, 
+                        f"remote path {remote_path_attr['path']!r} already exists"), 
+                    )
+                return
+            if isdir:
+                if remote_path_attr is None:
                     yield from self.upload_tree(
-                        entry.path, 
-                        entry.name, 
+                        entry, 
+                        [name], 
                         pid=pid, 
                         no_root=True, 
-                        overwrite_or_ignore=overwrite_or_ignore, 
+                        overwrite=overwrite, 
+                        remove_success=remove_success, 
+                        onerror=onerror, 
                     )
                 else:
-                    yield self.upload(
-                        entry.path, 
-                        entry.name, 
-                        pid=pid, 
-                        overwrite_or_ignore=overwrite_or_ignore, 
+                    yield from self.upload_tree(
+                        entry, 
+                        remote_path_attr, 
+                        no_root=True, 
+                        overwrite=overwrite, 
+                        remove_success=remove_success, 
+                        onerror=onerror, 
                     )
-            return attr
+                if remove_success:
+                    try:
+                        rmdir(entry)
+                    except OSError:
+                        pass
+            else:
+                try:
+                    if remote_path_attr is None:
+                        yield self.upload(
+                            entry, 
+                            [name], 
+                            pid=pid, 
+                            overwrite=overwrite, 
+                            remove_success=remove_success, 
+                        )
+                    else:
+                        yield self.upload(
+                            entry, 
+                            remote_path_attr, 
+                            overwrite=overwrite, 
+                            remove_success=remove_success, 
+                        )
+                except OSError as e:
+                    if onerror is True:
+                        raise e
+                    elif onerror is False:
+                        pass
+                    else:
+                        onerror(e)
+                    return
 
     unlink = remove
 
     def write_bytes(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         data: bytes | bytearray | memoryview | SupportsRead[bytes] = b"", 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
     ) -> dict:
         if isinstance(data, (bytes, bytearray, memoryview)):
             data = BytesIO(data)
-        return self.upload(data, id_or_path, pid=pid, overwrite_or_ignore=True)
+        return self.upload(data, id_or_path, pid=pid, overwrite=True)
 
     def write_text(
         self, 
         id_or_path: IDOrPathType = "", 
         /, 
         text: str = "", 
-        pid: Optional[int] = None, 
+        pid: None | int = None, 
         encoding: Optional[str] = None, 
         errors: Optional[str] = None, 
         newline: Optional[str] = None, 
     ) -> dict:
         bio = BytesIO()
         if text:
             if encoding is None:
```

### Comparing `python_115-0.0.8.3.5/p115/component/fs_base.py` & `python_115-0.0.8.3.6/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/fs_share.py` & `python_115-0.0.8.3.6/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/fs_zip.py` & `python_115-0.0.8.3.6/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/labellist.py` & `python_115-0.0.8.3.6/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/offline.py` & `python_115-0.0.8.3.6/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/recyclebin.py` & `python_115-0.0.8.3.6/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/component/sharing.py` & `python_115-0.0.8.3.6/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/p115/tool/__init__.py` & `python_115-0.0.8.3.6/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/pyproject.toml` & `python_115-0.0.8.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.3.5"
+version = "0.0.8.3.6"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.3.5/readme.md` & `python_115-0.0.8.3.6/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.5/PKG-INFO` & `python_115-0.0.8.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.3.5
+Version: 0.0.8.3.6
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

