# Comparing `tmp/report_pdf_wrapper-0.3.0-py3-none-any.whl.zip` & `tmp/report_pdf_wrapper-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5380 bytes, number of entries: 7
+Zip file size: 5375 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       68 b- defN 24-May-24 17:55 report_pdf_wrapper/__init__.py
--rw-r--r--  2.0 unx    13180 b- defN 24-May-24 18:39 report_pdf_wrapper/report_pdf_wrapper.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      712 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      623 b- defN 24-May-24 18:40 report_pdf_wrapper-0.3.0.dist-info/RECORD
-7 files, 15762 bytes uncompressed, 4258 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx    13190 b- defN 24-May-24 18:43 report_pdf_wrapper/report_pdf_wrapper.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-24 18:44 report_pdf_wrapper-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      712 b- defN 24-May-24 18:44 report_pdf_wrapper-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-24 18:44 report_pdf_wrapper-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-24 18:44 report_pdf_wrapper-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      623 b- defN 24-May-24 18:44 report_pdf_wrapper-0.4.0.dist-info/RECORD
+7 files, 15772 bytes uncompressed, 4253 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: report_pdf_wrapper/__init__.py
 Comment: 
 
 Filename: report_pdf_wrapper/report_pdf_wrapper.py
 Comment: 
 
-Filename: report_pdf_wrapper-0.3.0.dist-info/LICENSE
+Filename: report_pdf_wrapper-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: report_pdf_wrapper-0.3.0.dist-info/METADATA
+Filename: report_pdf_wrapper-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: report_pdf_wrapper-0.3.0.dist-info/WHEEL
+Filename: report_pdf_wrapper-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: report_pdf_wrapper-0.3.0.dist-info/top_level.txt
+Filename: report_pdf_wrapper-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: report_pdf_wrapper-0.3.0.dist-info/RECORD
+Filename: report_pdf_wrapper-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## report_pdf_wrapper/report_pdf_wrapper.py

```diff
@@ -20,19 +20,19 @@
             # create new document
             self.document = fitz.open()
         self.page = self.document.new_page()
         self.logo_path = logo_path
         if draw_dimensions:
             self.draw_dimensions()
 
-    def draw_report_pdf(self, page_num=0):
+    def draw_report_pdf(self, page_num=None):
         if self.logo_path is not None:
             self.draw_logo(self.logo_path)
         # if document is multiple pages, then add suffix to mutable widget keys to prevent duplication
-        if page_num != 0:
+        if page_num is not None:
             widget_suffix = f"_{page_num}"
         else:
             widget_suffix = ""
         self.draw_technician_info()
         self.draw_customer_info()
         self.draw_equipment_info(widget_suffix)
         self.draw_checklist(widget_suffix)
```

## Comparing `report_pdf_wrapper-0.3.0.dist-info/LICENSE` & `report_pdf_wrapper-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `report_pdf_wrapper-0.3.0.dist-info/METADATA` & `report_pdf_wrapper-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-pdf-wrapper
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple pip module for creating generic PDF reports.
 Home-page: https://github.com/nr-software/Report-PDF-Creation.git
 Author: Alex Nuccio
 Author-email: nrsoftwareservices@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

