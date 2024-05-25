# Comparing `tmp/muko-2.55-py3-none-any.whl.zip` & `tmp/muko-2.56-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 2390529 bytes, number of entries: 9
+Zip file size: 4034890 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
--rw-rw-rw-  2.0 fat   996864 b- defN 24-May-25 10:53 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   996864 b- defN 24-May-25 16:29 muko/cmuko.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat  1533192 b- defN 24-May-25 10:45 muko/cmuko.cpython-38-darwin.so
+-rw-rw-rw-  2.0 fat  5818368 b- defN 24-May-25 13:12 muko/cmuko.so
 -rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-May-25 10:53 muko-2.55.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1422 b- defN 24-May-25 10:53 muko-2.55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-25 10:53 muko-2.55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-May-25 10:53 muko-2.55.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      696 b- defN 24-May-25 10:53 muko-2.55.dist-info/RECORD
-9 files, 4616329 bytes uncompressed, 2389351 bytes compressed:  48.2%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-May-25 16:29 muko-2.56.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1423 b- defN 24-May-25 16:29 muko-2.56.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-25 16:29 muko-2.56.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-May-25 16:29 muko-2.56.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      769 b- defN 24-May-25 16:29 muko-2.56.dist-info/RECORD
+10 files, 10434771 bytes uncompressed, 4033610 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: muko/cmuko.cp38-win_amd64.pyd
 Comment: 
 
 Filename: muko/cmuko.cpython-38-darwin.so
 Comment: 
 
+Filename: muko/cmuko.so
+Comment: 
+
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.55.dist-info/LICENSE
+Filename: muko-2.56.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.55.dist-info/METADATA
+Filename: muko-2.56.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.55.dist-info/WHEEL
+Filename: muko-2.56.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.55.dist-info/top_level.txt
+Filename: muko-2.56.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-2.55.dist-info/RECORD
+Filename: muko-2.56.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.55.dist-info/LICENSE` & `muko-2.56.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.55.dist-info/METADATA` & `muko-2.56.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.55
+Version: 2.56
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
 Requires-Dist: opencv-python >=4.9.0.80
 Requires-Dist: diplib >=3.1.0
 Requires-Dist: rembg >=2.0.56
 Requires-Dist: easyocr >=1.7.1
 Requires-Dist: getmac >=0.9.4
 Requires-Dist: pydub >=0.25.1
 Requires-Dist: pygame >=2.5.2
-Requires-Dist: librosa >=0.8.1
+Requires-Dist: librosa >=0.10.0
 Requires-Dist: soundfile >=0.12.1
 Requires-Dist: oss2 >=2.18.4
 
 # Muko：加速实现AIGC、自动办公的中文编程工具
 
 ## 安装方式
     pip install muko
```

