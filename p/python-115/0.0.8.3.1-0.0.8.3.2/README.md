# Comparing `tmp/python_115-0.0.8.3.1.tar.gz` & `tmp/python_115-0.0.8.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.8.3.1.tar", max compression
+gzip compressed data, was "python_115-0.0.8.3.2.tar", max compression
```

## Comparing `python_115-0.0.8.3.1.tar` & `python_115-0.0.8.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.1/LICENSE
--rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.1/p115/__init__.py
--rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.1/p115/__main__.py
--rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.1/p115/cmd/__init__.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.1/p115/cmd/download.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.1/p115/cmd/fuse.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.1/p115/cmd/fuse_share.py
--rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.1/p115/cmd/init.py
--rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.3.1/p115/cmd/iterdir.py
--rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.1/p115/cmd/qrcode.py
--rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.1/p115/cmd/rename.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.1/p115/cmd/shell.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.1/p115/cmd/upload.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.1/p115/cmd/webdav.py
--rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.1/p115/cmd/webdav_share.py
--rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.1/p115/component/__init__.py
--rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.1/p115/component/cipher.py
--rwxr-xr-x   0        0        0   246219 2024-05-24 16:29:48.050265 python_115-0.0.8.3.1/p115/component/client.py
--rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.1/p115/component/exception.py
--rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.3.1/p115/component/fs.py
--rwxr-xr-x   0        0        0    48067 2024-05-24 16:16:56.781105 python_115-0.0.8.3.1/p115/component/fs_base.py
--rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.1/p115/component/fs_share.py
--rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.1/p115/component/fs_zip.py
--rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.3.1/p115/component/labellist.py
--rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.3.1/p115/component/offline.py
--rwxr-xr-x   0        0        0     4338 2024-05-24 16:52:21.603382 python_115-0.0.8.3.1/p115/component/recyclebin.py
--rwxr-xr-x   0        0        0     6373 2024-05-24 16:52:41.937491 python_115-0.0.8.3.1/p115/component/sharing.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.1/p115/py.typed
--rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8.3.1/p115/tool/__init__.py
--rw-r--r--   0        0        0     1617 2024-05-24 17:04:58.609686 python_115-0.0.8.3.1/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.1/readme.md
--rw-r--r--   0        0        0    36305 1970-01-01 00:00:00.000000 python_115-0.0.8.3.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.8.3.2/LICENSE
+-rwxr-xr-x   0        0        0      151 2024-05-21 07:08:07.171541 python_115-0.0.8.3.2/p115/__init__.py
+-rwxr-xr-x   0        0        0      244 2024-05-23 14:40:16.555713 python_115-0.0.8.3.2/p115/__main__.py
+-rwxr-xr-x   0        0        0      161 2024-04-19 14:59:47.539120 python_115-0.0.8.3.2/p115/cmd/__init__.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.2/p115/cmd/download.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.2/p115/cmd/fuse.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.2/p115/cmd/fuse_share.py
+-rwxr-xr-x   0        0        0      326 2024-04-27 09:40:34.029692 python_115-0.0.8.3.2/p115/cmd/init.py
+-rwxr-xr-x   0        0        0     8651 2024-05-22 14:45:05.591986 python_115-0.0.8.3.2/p115/cmd/iterdir.py
+-rwxr-xr-x   0        0        0     1841 2024-05-22 14:45:36.712906 python_115-0.0.8.3.2/p115/cmd/qrcode.py
+-rwxr-xr-x   0        0        0       42 2024-04-30 16:16:17.658218 python_115-0.0.8.3.2/p115/cmd/rename.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.2/p115/cmd/shell.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.2/p115/cmd/upload.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.2/p115/cmd/webdav.py
+-rwxr-xr-x   0        0        0       41 2024-04-28 16:16:41.957216 python_115-0.0.8.3.2/p115/cmd/webdav_share.py
+-rwxr-xr-x   0        0        0     1002 2024-05-22 14:18:52.612216 python_115-0.0.8.3.2/p115/component/__init__.py
+-rwxr-xr-x   0        0        0     7920 2024-05-12 05:27:04.744352 python_115-0.0.8.3.2/p115/component/cipher.py
+-rwxr-xr-x   0        0        0   246219 2024-05-24 16:29:48.050265 python_115-0.0.8.3.2/p115/component/client.py
+-rw-r--r--   0        0        0      177 2024-05-12 14:24:38.577143 python_115-0.0.8.3.2/p115/component/exception.py
+-rwxr-xr-x   0        0        0    56840 2024-05-23 15:52:16.591932 python_115-0.0.8.3.2/p115/component/fs.py
+-rwxr-xr-x   0        0        0    48067 2024-05-24 16:16:56.781105 python_115-0.0.8.3.2/p115/component/fs_base.py
+-rwxr-xr-x   0        0        0    12244 2024-05-23 16:23:25.193254 python_115-0.0.8.3.2/p115/component/fs_share.py
+-rwxr-xr-x   0        0        0     9759 2024-05-22 18:08:28.417049 python_115-0.0.8.3.2/p115/component/fs_zip.py
+-rwxr-xr-x   0        0        0     4816 2024-05-22 14:03:48.259741 python_115-0.0.8.3.2/p115/component/labellist.py
+-rwxr-xr-x   0        0        0     7086 2024-05-22 14:03:58.992780 python_115-0.0.8.3.2/p115/component/offline.py
+-rwxr-xr-x   0        0        0     4338 2024-05-24 16:52:21.603382 python_115-0.0.8.3.2/p115/component/recyclebin.py
+-rwxr-xr-x   0        0        0     6373 2024-05-24 16:52:41.937491 python_115-0.0.8.3.2/p115/component/sharing.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.8.3.2/p115/py.typed
+-rwxr-xr-x   0        0        0     3217 2024-05-09 09:59:33.438651 python_115-0.0.8.3.2/p115/tool/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-24 17:07:45.978755 python_115-0.0.8.3.2/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.8.3.2/readme.md
+-rw-r--r--   0        0        0    36333 1970-01-01 00:00:00.000000 python_115-0.0.8.3.2/PKG-INFO
```

### Comparing `python_115-0.0.8.3.1/LICENSE` & `python_115-0.0.8.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/cmd/iterdir.py` & `python_115-0.0.8.3.2/p115/cmd/iterdir.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/cmd/qrcode.py` & `python_115-0.0.8.3.2/p115/cmd/qrcode.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/__init__.py` & `python_115-0.0.8.3.2/p115/component/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/cipher.py` & `python_115-0.0.8.3.2/p115/component/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/client.py` & `python_115-0.0.8.3.2/p115/component/client.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/fs.py` & `python_115-0.0.8.3.2/p115/component/fs.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/fs_base.py` & `python_115-0.0.8.3.2/p115/component/fs_base.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/fs_share.py` & `python_115-0.0.8.3.2/p115/component/fs_share.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/fs_zip.py` & `python_115-0.0.8.3.2/p115/component/fs_zip.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/labellist.py` & `python_115-0.0.8.3.2/p115/component/labellist.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/offline.py` & `python_115-0.0.8.3.2/p115/component/offline.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/recyclebin.py` & `python_115-0.0.8.3.2/p115/component/recyclebin.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/component/sharing.py` & `python_115-0.0.8.3.2/p115/component/sharing.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/p115/tool/__init__.py` & `python_115-0.0.8.3.2/p115/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/pyproject.toml` & `python_115-0.0.8.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.8.3.1"
+version = "0.0.8.3.2"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["115", "client"]
@@ -25,14 +25,15 @@
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 cachetools = "*"
 ecdsa = "*"
+glob_pattern = "*"
 http_response = "*"
 httpx = "*"
 httpx_request = "*"
 lz4 = "*"
 magnet2torrent = "*"
 multidict = "*"
 posixpatht = "*"
```

### Comparing `python_115-0.0.8.3.1/readme.md` & `python_115-0.0.8.3.2/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.8.3.1/PKG-INFO` & `python_115-0.0.8.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.8.3.1
+Version: 0.0.8.3.2
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: 115,client
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cachetools
 Requires-Dist: ecdsa
+Requires-Dist: glob_pattern
 Requires-Dist: http_response
 Requires-Dist: httpx
 Requires-Dist: httpx_request
 Requires-Dist: lz4
 Requires-Dist: magnet2torrent
 Requires-Dist: multidict
 Requires-Dist: posixpatht
```

