# Comparing `tmp/edurpa_document-0.0.3-py3-none-any.whl.zip` & `tmp/edurpa_document-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5995 bytes, number of entries: 9
+Zip file size: 6052 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-28 07:01 EduRPA/__init__.py
--rw-rw-rw-  2.0 fat     4817 b- defN 24-Apr-28 06:18 EduRPA/Document/DocumentAutomation.py
+-rw-rw-rw-  2.0 fat     4982 b- defN 24-May-25 10:20 EduRPA/Document/DocumentAutomation.py
 -rw-rw-rw-  2.0 fat      428 b- defN 24-Apr-28 06:21 EduRPA/Document/__init__.py
 -rw-rw-rw-  2.0 fat     2624 b- defN 24-Apr-28 06:18 EduRPA/Document/transform.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-28 07:01 edurpa_document-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2019 b- defN 24-Apr-28 07:01 edurpa_document-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 07:01 edurpa_document-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-28 07:01 edurpa_document-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      759 b- defN 24-Apr-28 07:01 edurpa_document-0.0.3.dist-info/RECORD
-9 files, 11834 bytes uncompressed, 4671 bytes compressed:  60.5%
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2019 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      759 b- defN 24-May-25 10:20 edurpa_document-0.0.4.dist-info/RECORD
+9 files, 11999 bytes uncompressed, 4728 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: EduRPA/Document/__init__.py
 Comment: 
 
 Filename: EduRPA/Document/transform.py
 Comment: 
 
-Filename: edurpa_document-0.0.3.dist-info/LICENSE
+Filename: edurpa_document-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_document-0.0.3.dist-info/METADATA
+Filename: edurpa_document-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_document-0.0.3.dist-info/WHEEL
+Filename: edurpa_document-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_document-0.0.3.dist-info/top_level.txt
+Filename: edurpa_document-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_document-0.0.3.dist-info/RECORD
+Filename: edurpa_document-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Document/DocumentAutomation.py

```diff
@@ -4,17 +4,21 @@
 from robot.api.deco import keyword, not_keyword
 import cv2
 import json
 from openpyxl import Workbook
 from datetime import datetime
 
 from .transform import perspective_transform, resize_image
-
+from robot.libraries.BuiltIn import BuiltIn
 class DocumentAutomation:
     def __init__(self, lang, performance, *args, **kwargs):
+        if BuiltIn.dry_run_active:
+            # If running dryrun, ignore initialization
+            return
+        
         cfg = Cfg.load_config_from_name("vgg_seq2seq")
         cfg["device"] = "cpu"
         vgg_seq2seq = Predictor(cfg)
 
         cfg = Cfg.load_config_from_name("vgg_transformer")
         cfg["device"] = "cpu"
         vgg_transformer = Predictor(cfg)
```

## Comparing `edurpa_document-0.0.3.dist-info/LICENSE` & `edurpa_document-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_document-0.0.3.dist-info/METADATA` & `edurpa_document-0.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-document
-Version: 0.0.3
+Version: 0.0.4
 Summary: education librabry for RPA
 Home-page: https://github.com/edu-rpa/edu-rpa-library
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

