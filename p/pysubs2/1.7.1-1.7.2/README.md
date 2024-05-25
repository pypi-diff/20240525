# Comparing `tmp/pysubs2-1.7.1.tar.gz` & `tmp/pysubs2-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysubs2-1.7.1.tar", last modified: Sun May 19 13:28:05 2024, max compression
+gzip compressed data, was "pysubs2-1.7.2.tar", last modified: Sat May 25 21:25:40 2024, max compression
```

## Comparing `pysubs2-1.7.1.tar` & `pysubs2-1.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/
--rw-rw-r--   0 azar      (1000) azar      (1000)     1063 2024-05-19 00:27:32.000000 pysubs2-1.7.1/LICENSE.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)       82 2024-05-19 13:25:10.000000 pysubs2-1.7.1/MANIFEST.in
--rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-19 13:28:05.047193 pysubs2-1.7.1/PKG-INFO
--rw-rw-r--   0 azar      (1000) azar      (1000)     1883 2024-05-05 13:10:42.000000 pysubs2-1.7.1/README.md
--rw-rw-r--   0 azar      (1000) azar      (1000)       85 2023-11-25 17:38:44.000000 pysubs2-1.7.1/pyproject.toml
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.043193 pysubs2-1.7.1/pysubs2/
--rw-rw-r--   0 azar      (1000) azar      (1000)      783 2024-05-05 12:46:10.000000 pysubs2-1.7.1/pysubs2/__init__.py
--rw-rw-r--   0 azar      (1000) azar      (1000)      134 2023-11-25 17:38:44.000000 pysubs2-1.7.1/pysubs2/__main__.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    11916 2024-05-05 16:31:09.000000 pysubs2-1.7.1/pysubs2/cli.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1503 2024-05-19 13:25:10.000000 pysubs2-1.7.1/pysubs2/common.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2318 2024-05-05 12:46:10.000000 pysubs2-1.7.1/pysubs2/exceptions.py
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.043193 pysubs2-1.7.1/pysubs2/formats/
--rw-rw-r--   0 azar      (1000) azar      (1000)     2515 2024-05-18 22:16:41.000000 pysubs2-1.7.1/pysubs2/formats/__init__.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2959 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/base.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2101 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/jsonformat.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     5970 2024-05-19 00:09:39.000000 pysubs2-1.7.1/pysubs2/formats/microdvd.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1970 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/mpl2.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     7484 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/subrip.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    16795 2024-05-05 14:45:39.000000 pysubs2-1.7.1/pysubs2/formats/substation.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4100 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/tmp.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1788 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/formats/webvtt.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1607 2024-05-05 12:42:39.000000 pysubs2-1.7.1/pysubs2/formats/whisper.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     6291 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/ssaevent.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    23833 2024-05-18 22:28:04.000000 pysubs2-1.7.1/pysubs2/ssafile.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4031 2024-05-04 22:58:07.000000 pysubs2-1.7.1/pysubs2/ssastyle.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4739 2024-05-05 12:11:24.000000 pysubs2-1.7.1/pysubs2/time.py
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/pysubs2.egg-info/
--rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/PKG-INFO
--rw-rw-r--   0 azar      (1000) azar      (1000)     1382 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/SOURCES.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)        1 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/dependency_links.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)       49 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/entry_points.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)        8 2024-05-19 13:28:05.000000 pysubs2-1.7.1/pysubs2.egg-info/top_level.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)     1469 2024-05-19 13:28:05.051193 pysubs2-1.7.1/setup.cfg
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/tests/
-drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-19 13:28:05.047193 pysubs2-1.7.1/tests/data/
--rw-rw-r--   0 azar      (1000) azar      (1000)   180220 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/EBGaramond08-Italic.ttf
--rw-rw-r--   0 azar      (1000) azar      (1000)   280540 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/EBGaramond08-Regular.ttf
--rw-rw-r--   0 azar      (1000) azar      (1000)      343 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/LICENSE.txt
--rw-rw-r--   0 azar      (1000) azar      (1000)   622857 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_aegisub.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)   622702 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_no_events.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)   622836 2024-05-05 14:45:39.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)     3149 2023-11-25 17:38:44.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_images_aegisub.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)     3128 2024-05-05 14:45:39.000000 pysubs2-1.7.1/tests/data/subtitle_with_attached_images_pysubs2_ref.ass
--rw-rw-r--   0 azar      (1000) azar      (1000)     4308 2024-05-04 23:54:09.000000 pysubs2-1.7.1/tests/test_attachment.py
--rw-rw-r--   0 azar      (1000) azar      (1000)    17652 2024-05-05 16:36:24.000000 pysubs2-1.7.1/tests/test_cli.py
--rw-rw-r--   0 azar      (1000) azar      (1000)      266 2024-05-05 00:12:16.000000 pysubs2-1.7.1/tests/test_common.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1757 2024-05-05 12:11:24.000000 pysubs2-1.7.1/tests/test_parse_tags.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     2246 2024-05-05 00:09:46.000000 pysubs2-1.7.1/tests/test_ssaevent.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     4009 2024-05-04 23:59:43.000000 pysubs2-1.7.1/tests/test_ssafile.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     1252 2024-05-05 00:11:48.000000 pysubs2-1.7.1/tests/test_ssastyle.py
--rw-rw-r--   0 azar      (1000) azar      (1000)     7386 2024-05-05 00:07:52.000000 pysubs2-1.7.1/tests/test_time.py
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-25 21:25:40.668774 pysubs2-1.7.2/
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1063 2024-05-19 00:27:32.000000 pysubs2-1.7.2/LICENSE.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)       82 2024-05-19 13:25:10.000000 pysubs2-1.7.2/MANIFEST.in
+-rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-25 21:25:40.668774 pysubs2-1.7.2/PKG-INFO
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1883 2024-05-05 13:10:42.000000 pysubs2-1.7.2/README.md
+-rw-rw-r--   0 azar      (1000) azar      (1000)       85 2023-11-25 17:38:44.000000 pysubs2-1.7.2/pyproject.toml
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-25 21:25:40.644773 pysubs2-1.7.2/pysubs2/
+-rw-rw-r--   0 azar      (1000) azar      (1000)      783 2024-05-05 12:46:10.000000 pysubs2-1.7.2/pysubs2/__init__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      134 2023-11-25 17:38:44.000000 pysubs2-1.7.2/pysubs2/__main__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    11916 2024-05-05 16:31:09.000000 pysubs2-1.7.2/pysubs2/cli.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1503 2024-05-25 21:23:07.000000 pysubs2-1.7.2/pysubs2/common.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2318 2024-05-05 12:46:10.000000 pysubs2-1.7.2/pysubs2/exceptions.py
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-25 21:25:40.648773 pysubs2-1.7.2/pysubs2/formats/
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2515 2024-05-18 22:16:41.000000 pysubs2-1.7.2/pysubs2/formats/__init__.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2959 2024-05-05 12:11:24.000000 pysubs2-1.7.2/pysubs2/formats/base.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2101 2024-05-25 21:21:03.000000 pysubs2-1.7.2/pysubs2/formats/jsonformat.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     5970 2024-05-19 00:09:39.000000 pysubs2-1.7.2/pysubs2/formats/microdvd.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1970 2024-05-05 12:11:24.000000 pysubs2-1.7.2/pysubs2/formats/mpl2.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     7484 2024-05-05 12:11:24.000000 pysubs2-1.7.2/pysubs2/formats/subrip.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    16795 2024-05-05 14:45:39.000000 pysubs2-1.7.2/pysubs2/formats/substation.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4100 2024-05-05 12:11:24.000000 pysubs2-1.7.2/pysubs2/formats/tmp.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1788 2024-05-05 12:11:24.000000 pysubs2-1.7.2/pysubs2/formats/webvtt.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1607 2024-05-05 12:42:39.000000 pysubs2-1.7.2/pysubs2/formats/whisper.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     6291 2024-05-05 12:11:24.000000 pysubs2-1.7.2/pysubs2/ssaevent.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    23833 2024-05-18 22:28:04.000000 pysubs2-1.7.2/pysubs2/ssafile.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4031 2024-05-04 22:58:07.000000 pysubs2-1.7.2/pysubs2/ssastyle.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4739 2024-05-05 12:11:24.000000 pysubs2-1.7.2/pysubs2/time.py
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-25 21:25:40.668774 pysubs2-1.7.2/pysubs2.egg-info/
+-rw-r--r--   0 azar      (1000) azar      (1000)     3183 2024-05-25 21:25:40.000000 pysubs2-1.7.2/pysubs2.egg-info/PKG-INFO
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1382 2024-05-25 21:25:40.000000 pysubs2-1.7.2/pysubs2.egg-info/SOURCES.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)        1 2024-05-25 21:25:40.000000 pysubs2-1.7.2/pysubs2.egg-info/dependency_links.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)       49 2024-05-25 21:25:40.000000 pysubs2-1.7.2/pysubs2.egg-info/entry_points.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)        8 2024-05-25 21:25:40.000000 pysubs2-1.7.2/pysubs2.egg-info/top_level.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1469 2024-05-25 21:25:40.668774 pysubs2-1.7.2/setup.cfg
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-25 21:25:40.652773 pysubs2-1.7.2/tests/
+drwxrwxr-x   0 azar      (1000) azar      (1000)        0 2024-05-25 21:25:40.668774 pysubs2-1.7.2/tests/data/
+-rw-rw-r--   0 azar      (1000) azar      (1000)   180220 2023-11-25 17:38:44.000000 pysubs2-1.7.2/tests/data/EBGaramond08-Italic.ttf
+-rw-rw-r--   0 azar      (1000) azar      (1000)   280540 2023-11-25 17:38:44.000000 pysubs2-1.7.2/tests/data/EBGaramond08-Regular.ttf
+-rw-rw-r--   0 azar      (1000) azar      (1000)      343 2023-11-25 17:38:44.000000 pysubs2-1.7.2/tests/data/LICENSE.txt
+-rw-rw-r--   0 azar      (1000) azar      (1000)   622857 2023-11-25 17:38:44.000000 pysubs2-1.7.2/tests/data/subtitle_with_attached_fonts_aegisub.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)   622702 2023-11-25 17:38:44.000000 pysubs2-1.7.2/tests/data/subtitle_with_attached_fonts_no_events.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)   622836 2024-05-05 14:45:39.000000 pysubs2-1.7.2/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3149 2023-11-25 17:38:44.000000 pysubs2-1.7.2/tests/data/subtitle_with_attached_images_aegisub.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)     3128 2024-05-05 14:45:39.000000 pysubs2-1.7.2/tests/data/subtitle_with_attached_images_pysubs2_ref.ass
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4308 2024-05-04 23:54:09.000000 pysubs2-1.7.2/tests/test_attachment.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)    17652 2024-05-05 16:36:24.000000 pysubs2-1.7.2/tests/test_cli.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)      266 2024-05-05 00:12:16.000000 pysubs2-1.7.2/tests/test_common.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1757 2024-05-05 12:11:24.000000 pysubs2-1.7.2/tests/test_parse_tags.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     2246 2024-05-05 00:09:46.000000 pysubs2-1.7.2/tests/test_ssaevent.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     4009 2024-05-04 23:59:43.000000 pysubs2-1.7.2/tests/test_ssafile.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     1252 2024-05-05 00:11:48.000000 pysubs2-1.7.2/tests/test_ssastyle.py
+-rw-rw-r--   0 azar      (1000) azar      (1000)     7386 2024-05-05 00:07:52.000000 pysubs2-1.7.2/tests/test_time.py
```

### Comparing `pysubs2-1.7.1/LICENSE.txt` & `pysubs2-1.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/PKG-INFO` & `pysubs2-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubs2
-Version: 1.7.1
+Version: 1.7.2
 Summary: A library for editing subtitle files
 Home-page: https://github.com/tkarabela/pysubs2
 Author: Tomas Karabela
 Author-email: tkarabela@seznam.cz
 License: MIT
 Project-URL: Documentation, https://pysubs2.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/tkarabela/pysubs2/issues
```

### Comparing `pysubs2-1.7.1/README.md` & `pysubs2-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/__init__.py` & `pysubs2-1.7.2/pysubs2/__init__.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/cli.py` & `pysubs2-1.7.2/pysubs2/cli.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/common.py` & `pysubs2-1.7.2/pysubs2/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,11 +54,11 @@
         return SSA_ALIGNMENT[self.value - 1]
 
 
 SSA_ALIGNMENT: Tuple[int, ...] = (1, 2, 3, 9, 10, 11, 5, 6, 7)
 
 
 #: Version of the pysubs2 library.
-VERSION = "1.7.1"
+VERSION = "1.7.2"
 
 
 IntOrFloat = Union[int, float]
```

### Comparing `pysubs2-1.7.1/pysubs2/exceptions.py` & `pysubs2-1.7.2/pysubs2/exceptions.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/__init__.py` & `pysubs2-1.7.2/pysubs2/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/base.py` & `pysubs2-1.7.2/pysubs2/formats/base.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/jsonformat.py` & `pysubs2-1.7.2/pysubs2/formats/jsonformat.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Implementation of JSON subtitle pseudo-format (serialized pysubs2 internal representation)
 
     This is essentially SubStation Alpha as JSON.
     """
     @classmethod
     def guess_format(cls, text: str) -> Optional[str]:
         """See :meth:`pysubs2.formats.FormatBase.guess_format()`"""
-        if text.startswith("{\"") and "\"info:\"" in text:
+        if text.startswith("{\"") and "\"info\":" in text:
             return "json"
         else:
             return None
 
     @classmethod
     def from_file(cls, subs: "SSAFile", fp: TextIO, format_: str, **kwargs: Any) -> None:
         """See :meth:`pysubs2.formats.FormatBase.from_file()`"""
```

### Comparing `pysubs2-1.7.1/pysubs2/formats/microdvd.py` & `pysubs2-1.7.2/pysubs2/formats/microdvd.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/mpl2.py` & `pysubs2-1.7.2/pysubs2/formats/mpl2.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/subrip.py` & `pysubs2-1.7.2/pysubs2/formats/subrip.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/substation.py` & `pysubs2-1.7.2/pysubs2/formats/substation.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/tmp.py` & `pysubs2-1.7.2/pysubs2/formats/tmp.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/webvtt.py` & `pysubs2-1.7.2/pysubs2/formats/webvtt.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/formats/whisper.py` & `pysubs2-1.7.2/pysubs2/formats/whisper.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/ssaevent.py` & `pysubs2-1.7.2/pysubs2/ssaevent.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/ssafile.py` & `pysubs2-1.7.2/pysubs2/ssafile.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/ssastyle.py` & `pysubs2-1.7.2/pysubs2/ssastyle.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2/time.py` & `pysubs2-1.7.2/pysubs2/time.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/pysubs2.egg-info/PKG-INFO` & `pysubs2-1.7.2/pysubs2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubs2
-Version: 1.7.1
+Version: 1.7.2
 Summary: A library for editing subtitle files
 Home-page: https://github.com/tkarabela/pysubs2
 Author: Tomas Karabela
 Author-email: tkarabela@seznam.cz
 License: MIT
 Project-URL: Documentation, https://pysubs2.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/tkarabela/pysubs2/issues
```

### Comparing `pysubs2-1.7.1/pysubs2.egg-info/SOURCES.txt` & `pysubs2-1.7.2/pysubs2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/setup.cfg` & `pysubs2-1.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/data/EBGaramond08-Italic.ttf` & `pysubs2-1.7.2/tests/data/EBGaramond08-Italic.ttf`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/data/EBGaramond08-Regular.ttf` & `pysubs2-1.7.2/tests/data/EBGaramond08-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_aegisub.ass` & `pysubs2-1.7.2/tests/data/subtitle_with_attached_fonts_aegisub.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_no_events.ass` & `pysubs2-1.7.2/tests/data/subtitle_with_attached_fonts_no_events.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass` & `pysubs2-1.7.2/tests/data/subtitle_with_attached_fonts_pysubs2_ref.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/data/subtitle_with_attached_images_aegisub.ass` & `pysubs2-1.7.2/tests/data/subtitle_with_attached_images_aegisub.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/data/subtitle_with_attached_images_pysubs2_ref.ass` & `pysubs2-1.7.2/tests/data/subtitle_with_attached_images_pysubs2_ref.ass`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/test_attachment.py` & `pysubs2-1.7.2/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/test_cli.py` & `pysubs2-1.7.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/test_parse_tags.py` & `pysubs2-1.7.2/tests/test_parse_tags.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/test_ssaevent.py` & `pysubs2-1.7.2/tests/test_ssaevent.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/test_ssafile.py` & `pysubs2-1.7.2/tests/test_ssafile.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/test_ssastyle.py` & `pysubs2-1.7.2/tests/test_ssastyle.py`

 * *Files identical despite different names*

### Comparing `pysubs2-1.7.1/tests/test_time.py` & `pysubs2-1.7.2/tests/test_time.py`

 * *Files identical despite different names*

