# Comparing `tmp/edurpa_cloud-0.0.1-py3-none-any.whl.zip` & `tmp/edurpa_cloud-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 10434 bytes, number of entries: 13
+Zip file size: 11171 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-17 16:24 EduRPA/__init__.py
 -rw-rw-rw-  2.0 fat    13103 b- defN 24-Apr-18 09:37 EduRPA/Google/Classroom.py
 -rw-rw-rw-  2.0 fat     1511 b- defN 24-Apr-23 16:12 EduRPA/Google/CustomOAuth.py
 -rw-rw-rw-  2.0 fat    11964 b- defN 24-Apr-18 09:38 EduRPA/Google/Form.py
 -rw-rw-rw-  2.0 fat      314 b- defN 24-Apr-21 05:45 EduRPA/Google/Utils.py
 -rw-rw-rw-  2.0 fat      469 b- defN 24-Apr-21 13:23 EduRPA/Google/__init__.py
+-rw-rw-rw-  2.0 fat     1577 b- defN 24-May-25 13:07 EduRPA/Storage/S3Storage.py
 -rw-rw-rw-  2.0 fat     1575 b- defN 24-Apr-28 06:10 EduRPA/Storage/Storage.py
--rw-rw-rw-  2.0 fat      306 b- defN 24-Apr-28 06:10 EduRPA/Storage/__init__.py
--rw-rw-rw-  2.0 fat     1088 b- defN 24-Apr-28 07:03 edurpa_cloud-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      716 b- defN 24-Apr-28 07:03 edurpa_cloud-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-28 07:03 edurpa_cloud-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-28 07:03 edurpa_cloud-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1052 b- defN 24-Apr-28 07:03 edurpa_cloud-0.0.1.dist-info/RECORD
-13 files, 32197 bytes uncompressed, 8674 bytes compressed:  73.1%
+-rw-rw-rw-  2.0 fat      312 b- defN 24-May-25 13:07 EduRPA/Storage/__init__.py
+-rw-rw-rw-  2.0 fat     1088 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      716 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1136 b- defN 24-May-25 13:07 edurpa_cloud-0.0.2.dist-info/RECORD
+14 files, 33864 bytes uncompressed, 9281 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -12,29 +12,32 @@
 
 Filename: EduRPA/Google/Utils.py
 Comment: 
 
 Filename: EduRPA/Google/__init__.py
 Comment: 
 
+Filename: EduRPA/Storage/S3Storage.py
+Comment: 
+
 Filename: EduRPA/Storage/Storage.py
 Comment: 
 
 Filename: EduRPA/Storage/__init__.py
 Comment: 
 
-Filename: edurpa_cloud-0.0.1.dist-info/LICENSE
+Filename: edurpa_cloud-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: edurpa_cloud-0.0.1.dist-info/METADATA
+Filename: edurpa_cloud-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: edurpa_cloud-0.0.1.dist-info/WHEEL
+Filename: edurpa_cloud-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: edurpa_cloud-0.0.1.dist-info/top_level.txt
+Filename: edurpa_cloud-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: edurpa_cloud-0.0.1.dist-info/RECORD
+Filename: edurpa_cloud-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## EduRPA/Storage/__init__.py

```diff
@@ -1,13 +1,13 @@
 name = 'edurpa_storage'
-from .Storage import Storage
+from .S3Storage import S3Storage
 from robotlibcore import DynamicCore
 
 class Storage(DynamicCore):
     def __init__(
         self
     ):
         # Register keyword libraries to LibCore
         libraries = [
-            Storage()
+            S3Storage()
         ]
         super().__init__(libraries)
```

## Comparing `edurpa_cloud-0.0.1.dist-info/LICENSE` & `edurpa_cloud-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `edurpa_cloud-0.0.1.dist-info/METADATA` & `edurpa_cloud-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edurpa-cloud
-Version: 0.0.1
+Version: 0.0.2
 Summary: Education Google RPA Librabry For Education
 Home-page: https://github.com/edu-rpa/edurpa-google
 Author: david
 Author-email: davidhuynh0222@gmail.com
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `edurpa_cloud-0.0.1.dist-info/RECORD` & `edurpa_cloud-0.0.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 EduRPA/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 EduRPA/Google/Classroom.py,sha256=ZUMo0Dlc46bFwAUnUHKrbOl_RzvOvVHWAQtfa3hJPqQ,13103
 EduRPA/Google/CustomOAuth.py,sha256=zyN2Iq8wwoXtwI9bBAtgecA7R9aZr3rfzswlsf8Bf4o,1511
 EduRPA/Google/Form.py,sha256=K4SdXFT6VKbreHnNebTjGtEDuJoPC7JnKD4t1xSB55Y,11964
 EduRPA/Google/Utils.py,sha256=oELOV-TFTQz_NDf9i0usZfXC9kbY4Xa_Kb1T7D8ssOw,314
 EduRPA/Google/__init__.py,sha256=q9wb2yVj8rKIsGf7UelAixwVKWk9CCKsQCzmUtCVzDM,469
+EduRPA/Storage/S3Storage.py,sha256=PHfCK_Dd1u24wFFuZu8Xqs916AzzysU_cHxOsXzM8nI,1577
 EduRPA/Storage/Storage.py,sha256=TIhaD373yDdHms9OANPhSUx0b5xLOp2IUru8t1Voeok,1575
-EduRPA/Storage/__init__.py,sha256=RnG0ZMCNSoap1wWLMdqect8FdCf6x2wWMmsi45rtEH8,306
-edurpa_cloud-0.0.1.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
-edurpa_cloud-0.0.1.dist-info/METADATA,sha256=zzkUiNriHFPqX_kl1mDSY1slIC8RDQf-hEGR2ndwUMQ,716
-edurpa_cloud-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-edurpa_cloud-0.0.1.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
-edurpa_cloud-0.0.1.dist-info/RECORD,,
+EduRPA/Storage/__init__.py,sha256=6QsHQApuwUyuN1yU9O87eeU0ai7frQScebeBuZoQLpk,312
+edurpa_cloud-0.0.2.dist-info/LICENSE,sha256=YgvlMcXsea3kZqp1y62n8AgkwZp6xXbWSYW17pT58Yg,1088
+edurpa_cloud-0.0.2.dist-info/METADATA,sha256=qNXIrAUfpNfEGQZUiV12fXPVWbFtG5jd5lHY-gfZxcw,716
+edurpa_cloud-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+edurpa_cloud-0.0.2.dist-info/top_level.txt,sha256=Wl0EDd9il1J3fz62-gLcRCpFYSlEbU4KVE_SNWkcpaI,7
+edurpa_cloud-0.0.2.dist-info/RECORD,,
```

