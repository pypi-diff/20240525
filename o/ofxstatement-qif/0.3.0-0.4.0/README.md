# Comparing `tmp/ofxstatement_qif-0.3.0-py3-none-any.whl.zip` & `tmp/ofxstatement_qif-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3544 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 20:37 ofxstatement/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-20 20:37 ofxstatement/plugins/__init__.py
--rw-r--r--  2.0 unx     3917 b- defN 24-May-20 20:37 ofxstatement/plugins/qif.py
--rw-r--r--  2.0 unx     2102 b- defN 24-May-20 20:46 ofxstatement_qif-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-20 20:46 ofxstatement_qif-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-20 20:46 ofxstatement_qif-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      582 b- defN 24-May-20 20:46 ofxstatement_qif-0.3.0.dist-info/RECORD
-7 files, 6706 bytes uncompressed, 2496 bytes compressed:  62.8%
+Zip file size: 3673 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 24-May-25 11:19 ofxstatement_qif/__init__.py
+-rw-r--r--  2.0 unx     3917 b- defN 24-May-25 11:19 ofxstatement_qif/plugin.py
+-rw-r--r--  2.0 unx     2102 b- defN 24-May-25 11:28 ofxstatement_qif-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-25 11:28 ofxstatement_qif-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-May-25 11:28 ofxstatement_qif-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-May-25 11:28 ofxstatement_qif-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      603 b- defN 24-May-25 11:28 ofxstatement_qif-0.4.0.dist-info/RECORD
+7 files, 6786 bytes uncompressed, 2585 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: ofxstatement/__init__.py
+Filename: ofxstatement_qif/__init__.py
 Comment: 
 
-Filename: ofxstatement/plugins/__init__.py
+Filename: ofxstatement_qif/plugin.py
 Comment: 
 
-Filename: ofxstatement/plugins/qif.py
+Filename: ofxstatement_qif-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: ofxstatement_qif-0.3.0.dist-info/METADATA
+Filename: ofxstatement_qif-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: ofxstatement_qif-0.3.0.dist-info/WHEEL
+Filename: ofxstatement_qif-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: ofxstatement_qif-0.3.0.dist-info/top_level.txt
+Filename: ofxstatement_qif-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: ofxstatement_qif-0.3.0.dist-info/RECORD
+Filename: ofxstatement_qif-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ofxstatement/plugins/qif.py` & `ofxstatement_qif/plugin.py`

 * *Files identical despite different names*

## Comparing `ofxstatement_qif-0.3.0.dist-info/METADATA` & `ofxstatement_qif-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofxstatement-qif
-Version: 0.3.0
+Version: 0.4.0
 Summary: ofxstatement plugin for QIF files
 Author-email: R Vadai <rvadai@segence.com>
 Project-URL: repository, https://github.com/robvadai/ofxstatement-qif
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 
 Converts [Quicken Interchange Format (QIF)](https://en.wikipedia.org/wiki/Quicken_Interchange_Format) formatted bank transaction files to [Open Financial Exchange (OFX)](https://en.wikipedia.org/wiki/Open_Financial_Exchange) format.
 
 It is a plugin for [ofxstatement](https://github.com/kedder/ofxstatement).
 
 ## Usage
 ```shell
-$ ofxstatement convert -t qif transactions.qiv transactions.ofx
+$ ofxstatement convert -t qif transactions.qif transactions.ofx
 ```
 ## Configuration
 ```shell
 $ ofxstatement edit-config
 ```
 And enter e.g. this:
 ```
```

