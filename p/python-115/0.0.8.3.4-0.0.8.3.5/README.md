# Comparing `tmp/python_115-0.0.8.3.4.tar.gz` & `tmp/python_115-0.0.8.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.3.4.tar", max compression
+gzip compressed data, was "python_115-0.0.8.3.5.tar", max compression
```

## Comparing `python_115-0.0.8.3.4.tar` & `python_115-0.0.8.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.4/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.4/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.4/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.4/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.4/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.3.4/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.4/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.4/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.4/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.4/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.4/p115/component/cipher.py
--rwxr-xr-x   0        0        0   246390 2024-05-25 05:26:13.883965 python_115-0.0.8.3.4/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.4/p115/component/exception.py
--rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.3.4/p115/component/fs.py
--rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.3.4/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.4/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.4/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.3.4/p115/component/labellist.py
--rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.3.4/p115/component/offline.py
--rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.3.4/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.3.4/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.4/p115/py.typed
--rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.3.4/p115/tool/__init__.py
--rw-r--r--   0        0        0     1665 2024-05-25 05:35:31.473053 python_115-0.0.8.3.4/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.4/readme.md
--rw-r--r--   0        0        0    36371 1970-01-01 00:00:00.000000 python_115-0.0.8.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.5/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.5/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.5/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.5/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.5/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8669 2024-05-25 05:50:21.865251 python_115-0.0.8.3.5/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.5/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.5/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.5/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.5/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.5/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   246390 2024-05-25 05:26:13.883965 python_115-0.0.8.3.5/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.5/p115/component/exception.py
+-rwxr-xr-x   0        0        0    56840 2024-05-25 05:49:19.298545 python_115-0.0.8.3.5/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48126 2024-05-25 05:15:40.231659 python_115-0.0.8.3.5/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.5/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.5/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     8021 2024-05-25 04:37:00.607790 python_115-0.0.8.3.5/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     9833 2024-05-25 05:35:13.360543 python_115-0.0.8.3.5/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4332 2024-05-25 04:00:41.560248 python_115-0.0.8.3.5/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6430 2024-05-25 05:33:52.499415 python_115-0.0.8.3.5/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.5/p115/py.typed
+-rwxr-xr-x   0        0        0     5001 2024-05-25 03:41:26.878366 python_115-0.0.8.3.5/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-25 05:50:34.034333 python_115-0.0.8.3.5/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.5/readme.md
+-rw-r--r--   0        0        0    36371 1970-01-01 00:00:00.000000 python_115-0.0.8.3.5/PKG-INFO
```

### Comparing `python_115-0.0.8.3.4/LICENSE` & `python_115-0.0.8.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/cmd/iterdir.py` & `python_115-0.0.8.3.5/p115/cmd/iterdir.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 else:
     from .init import subparsers
 
     parser = subparsers.add_parser("iterdir", description=__doc__)
 
 
 def main(args):
-    from p115 import P115FileSystem, __version__
+    from p115 import P115FileSystem, P115Path, __version__
 
     if args.version:
         print(".".join(map(str, __version__)))
         raise SystemExit(0)
 
     from os.path import expanduser, dirname, join as joinpath
     from sys import stdout
@@ -144,17 +144,17 @@
             if not (result is None or isinstance(result, bytes)):
                 result = bytes(str(result), "utf-8")
             if result:
                 write(result)
                 write(b"\n")
         return
 
-    def get_key(path, key):
+    def get_key(path: P115Path, key: str):
         if key == "description":
-            return path.description
+            return path.desc
         elif key == "relpath":
             return path["path"][top_start:]
         else:
             return path.get(key)
 
     records = ({k: get_key(p, k) for k in keys} for p in path_it)
```

### Comparing `python_115-0.0.8.3.4/p115/cmd/qrcode.py` & `python_115-0.0.8.3.5/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/__init__.py` & `python_115-0.0.8.3.5/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/cipher.py` & `python_115-0.0.8.3.5/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/client.py` & `python_115-0.0.8.3.5/p115/component/client.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/fs.py` & `python_115-0.0.8.3.5/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/fs_base.py` & `python_115-0.0.8.3.5/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/fs_share.py` & `python_115-0.0.8.3.5/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/fs_zip.py` & `python_115-0.0.8.3.5/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/labellist.py` & `python_115-0.0.8.3.5/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/offline.py` & `python_115-0.0.8.3.5/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/recyclebin.py` & `python_115-0.0.8.3.5/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/component/sharing.py` & `python_115-0.0.8.3.5/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/p115/tool/__init__.py` & `python_115-0.0.8.3.5/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/pyproject.toml` & `python_115-0.0.8.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.3.4"
+version = "0.0.8.3.5"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
```

### Comparing `python_115-0.0.8.3.4/readme.md` & `python_115-0.0.8.3.5/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.4/PKG-INFO` & `python_115-0.0.8.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.3.4
+Version: 0.0.8.3.5
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

