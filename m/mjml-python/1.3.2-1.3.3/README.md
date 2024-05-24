# Comparing `tmp/mjml_python-1.3.2-cp37-abi3-win_amd64.whl.zip` & `tmp/mjml_python-1.3.3-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 474931 bytes, number of entries: 8
--rw-r--r--  4.6 unx     4963 b- defN 24-Mar-16 22:16 mjml_python-1.3.2.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 24-Mar-16 22:16 mjml_python-1.3.2.dist-info/WHEEL
--rw-r--r--  4.6 unx     1095 b- defN 24-Mar-16 22:16 mjml_python-1.3.2.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       99 b- defN 24-Mar-16 22:16 mjml/__init__.py
--rw-r--r--  4.6 unx      826 b- defN 24-Mar-16 22:16 mjml/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-Mar-16 22:16 mjml/py.typed
--rwxr-xr-x  4.6 unx  1431040 b- defN 24-Mar-16 22:16 mjml/mjml.pyd
--rw-r--r--  4.6 unx      608 b- defN 24-Mar-16 22:16 mjml_python-1.3.2.dist-info/RECORD
-8 files, 1438726 bytes uncompressed, 473879 bytes compressed:  67.1%
+Zip file size: 474359 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     5014 b- defN 24-May-24 22:33 mjml_python-1.3.3.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 24-May-24 22:33 mjml_python-1.3.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1095 b- defN 24-May-24 22:33 mjml_python-1.3.3.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       99 b- defN 24-May-24 22:33 mjml/__init__.py
+-rw-r--r--  4.6 unx      826 b- defN 24-May-24 22:33 mjml/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-24 22:33 mjml/py.typed
+-rwxr-xr-x  4.6 unx  1435136 b- defN 24-May-24 22:33 mjml/mjml.pyd
+-rw-r--r--  4.6 unx      608 b- defN 24-May-24 22:33 mjml_python-1.3.3.dist-info/RECORD
+8 files, 1442873 bytes uncompressed, 473307 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: mjml_python-1.3.2.dist-info/METADATA
+Filename: mjml_python-1.3.3.dist-info/METADATA
 Comment: 
 
-Filename: mjml_python-1.3.2.dist-info/WHEEL
+Filename: mjml_python-1.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: mjml_python-1.3.2.dist-info/license_files/LICENSE
+Filename: mjml_python-1.3.3.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: mjml/__init__.py
 Comment: 
 
 Filename: mjml/__init__.pyi
 Comment: 
 
 Filename: mjml/py.typed
 Comment: 
 
 Filename: mjml/mjml.pyd
 Comment: 
 
-Filename: mjml_python-1.3.2.dist-info/RECORD
+Filename: mjml_python-1.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mjml_python-1.3.2.dist-info/METADATA` & `mjml_python-1.3.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: mjml-python
-Version: 1.3.2
+Version: 1.3.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 Summary: A Python wrapper for MRML (Rust port of MJML).
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/mgd020/mjml-python
 Project-URL: Bug Tracker, https://github.com/mgd020/mjml-python/issues
+Project-URL: Homepage, https://github.com/mgd020/mjml-python
 
 # mjml-python
 
 Compile MJML at runtime without an external Node service/process. It is a Python wrapper for [MRML](https://github.com/jdrouet/mrml) (Rust port of [MJML](https://github.com/mjmlio/mjml)).
 
 ## Why
```

## Comparing `mjml_python-1.3.2.dist-info/license_files/LICENSE` & `mjml_python-1.3.3.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `mjml_python-1.3.2.dist-info/RECORD` & `mjml_python-1.3.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-mjml_python-1.3.2.dist-info/METADATA,sha256=tnX1WhX_kpOzcbQ9VT3FUTulzZok6bEr1UVaL6rMwf4,4963
-mjml_python-1.3.2.dist-info/WHEEL,sha256=_iayJa0atk_VQUEAv18tpdaLoItnUzb_8P_y87jfWxc,95
-mjml_python-1.3.2.dist-info/license_files/LICENSE,sha256=Ogx1hV6q5PLAjCw0garKjEiH7GUmFydh4DuWyd5VOs4,1095
+mjml_python-1.3.3.dist-info/METADATA,sha256=4twm4BK06At9YpNoMCPWm-1QQVhV74AlIU2-WzUyQLg,5014
+mjml_python-1.3.3.dist-info/WHEEL,sha256=_iayJa0atk_VQUEAv18tpdaLoItnUzb_8P_y87jfWxc,95
+mjml_python-1.3.3.dist-info/license_files/LICENSE,sha256=Ogx1hV6q5PLAjCw0garKjEiH7GUmFydh4DuWyd5VOs4,1095
 mjml/__init__.py,sha256=2dJmpc4qHjvXHjqcsnJ6bJgRlD9e7pB4Oqe6RoEzmLQ,99
 mjml/__init__.pyi,sha256=-6SLESiNwxBIanERBO1zbJLbk6QC82PNFYiWn0E8njE,826
 mjml/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mjml/mjml.pyd,sha256=osw7aP1NFX72j-ss5PJ_a_CCKEMrVTRH4Uj6j2IPZ5Y,1431040
-mjml_python-1.3.2.dist-info/RECORD,,
+mjml/mjml.pyd,sha256=CyXptuaa9YEuH8jdnkGvTA-nS2AeD1o6rVz4lDJw_Xg,1435136
+mjml_python-1.3.3.dist-info/RECORD,,
```

