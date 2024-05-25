# Comparing `tmp/monisha-0.0.74.tar.gz` & `tmp/monisha-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.74.tar", last modified: Thu May 16 19:39:10 2024, max compression
+gzip compressed data, was "monisha-0.0.75.tar", last modified: Fri May 24 20:24:04 2024, max compression
```

## Comparing `monisha-0.0.74.tar` & `monisha-0.0.75.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:39:10.301141 monisha-0.0.74/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 19:39:06.000000 monisha-0.0.74/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:39:10.293141 monisha-0.0.74/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:39:10.297140 monisha-0.0.74/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function18.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function19.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/functions/function20.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:39:10.297140 monisha-0.0.74/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 19:39:06.000000 monisha-0.0.74/Monisha/scripts/eu.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 19:39:10.297140 monisha-0.0.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 19:39:06.000000 monisha-0.0.74/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:39:10.297140 monisha-0.0.74/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 19:39:10.000000 monisha-0.0.74/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-16 19:39:10.000000 monisha-0.0.74/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:39:10.000000 monisha-0.0.74/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 19:39:10.000000 monisha-0.0.74/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 19:39:10.000000 monisha-0.0.74/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:39:10.301141 monisha-0.0.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-16 19:39:06.000000 monisha-0.0.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:24:04.371502 monisha-0.0.75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-24 20:23:57.000000 monisha-0.0.75/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:24:04.367502 monisha-0.0.75/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:24:04.371502 monisha-0.0.75/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/functions/function20.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:24:04.371502 monisha-0.0.75/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-24 20:23:57.000000 monisha-0.0.75/Monisha/scripts/eu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-24 20:24:04.371502 monisha-0.0.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-24 20:23:57.000000 monisha-0.0.75/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:24:04.371502 monisha-0.0.75/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-24 20:24:04.000000 monisha-0.0.75/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-24 20:24:04.000000 monisha-0.0.75/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:24:04.000000 monisha-0.0.75/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-24 20:24:04.000000 monisha-0.0.75/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 20:24:04.000000 monisha-0.0.75/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:24:04.371502 monisha-0.0.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-24 20:23:57.000000 monisha-0.0.75/setup.py
```

### Comparing `monisha-0.0.74/LICENSE` & `monisha-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/__init__.py` & `monisha-0.0.75/Monisha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.74"
+version = "0.0.75"
 
 install = ["hachoir",
            "requests",
            "beautifulsoup4"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
```

### Comparing `monisha-0.0.74/Monisha/functions/__init__.py` & `monisha-0.0.75/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function01.py` & `monisha-0.0.75/Monisha/functions/function01.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     hours, minute = divmod(minute, 60)
     days, hours = divmod(hours, 24)
     year, days = divmod(days, 365)
     mos  = ((str(year) + "𝚢𝚎𝚊𝚛, ") if year else Scripted.DATA01)
     mos += ((str(days) + "𝚍𝚊𝚢𝚜, ") if days else Scripted.DATA01)
     mos += ((str(hours) + "𝚑𝚛𝚜, ") if hours else Scripted.DATA01)
     mos += ((str(minute) + "𝚖𝚒𝚗, ") if minute else Scripted.DATA01)
-    mos += ((str(seconds) + "𝚜𝚎𝚌") if seconds else Scripted.DATA06)
+    mos += ((str(seconds) + "𝚜𝚎𝚌") if seconds else Scripted.DATA04)
     return mos
 
 #=========================================================================
 
 def Timesod(moonos: int) -> str:
     mosems = 1 if moonos == Scripted.DATA02 else moonos
     moonse = mosems if 1 < mosems else 1
@@ -39,11 +39,11 @@
     hours, minute = divmod(minute, 60)
     days, hours = divmod(hours, 24)
     year, days = divmod(days, 365)
     mos  = ((str(year) + "year, ") if year else Scripted.DATA01)
     mos += ((str(days) + "days, ") if days else Scripted.DATA01)
     mos += ((str(hours) + "hrs, ") if hours else Scripted.DATA01)
     mos += ((str(minute) + "min, ") if minute else Scripted.DATA01)
-    mos += ((str(seconds) + "sec") if seconds else Scripted.DATA07)
+    mos += ((str(seconds) + "sec") if seconds else Scripted.DATA04)
     return mos
 
 #=========================================================================
```

### Comparing `monisha-0.0.74/Monisha/functions/function02.py` & `monisha-0.0.75/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function03.py` & `monisha-0.0.75/Monisha/functions/function03.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from ..scripts import Smbo
 #===================================================================================
 
-def progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=10, l02=10):
+def progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=5.55, l02=18):
     percenage = float(percentage)
     passngeso = min(max(percenage, 0), 100)
     cosmosses = int(passngeso // l01)
     outgoings = b01 * cosmosses
     outgoings += b02 * (l02 - cosmosses)
     return outgoings
 
 #===================================================================================
 
-async def Progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=10, l02=10):
+async def Progress(percentage, b01=Smbo.DATA02, b02=Smbo.DATA01, l01=5.55, l02=18):
     percenage = float(percentage)
     passngeso = min(max(percenage, 0), 100)
     cosmosses = int(passngeso // l01)
     outgoings = b01 * cosmosses
     outgoings += b02 * (l02 - cosmosses)
     return outgoings
```

### Comparing `monisha-0.0.74/Monisha/functions/function04.py` & `monisha-0.0.75/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function06.py` & `monisha-0.0.75/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function07.py` & `monisha-0.0.75/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function10.py` & `monisha-0.0.75/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function14.py` & `monisha-0.0.75/Monisha/functions/function14.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function15.py` & `monisha-0.0.75/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function16.py` & `monisha-0.0.75/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/functions/function17.py` & `monisha-0.0.75/Monisha/functions/function17.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import os, random
+import os
+import random
+from ..scripts import Scripted
 from urllib.parse import unquote
 from urllib.parse import urlparse
 #=========================================================================
 
 
 class SMessages:
     def __init__(self, **kwargs):
@@ -22,23 +24,32 @@
 
 #=========================================================================
 
     async def get02(filename):
         nameas = str(filename)
         finame = os.path.splitext(nameas)[0]
         exexon = os.path.splitext(nameas)[1]
-        exoexo = exexon if exexon else ".tmp"
-        moonus = finame if finame else "Unknown"
+        exoexo = exexon if exexon else Scripted.DATA06
+        moonus = finame if finame else Scripted.DATA13
         return SMessages(filename=moonus, extension=exoexo)
 
 #=========================================================================
 
     async def get03(filelink):
         try:
-            findoutne = urlparse(filelink)
-            filenameo = os.path.basename(findoutne.path)
-            filenames = unquote(filenameo)
-            return SMessages(result=filenames)
+            findne = urlparse(filelink)
+            fnameo = os.path.basename(findne.path)
+            moonus = unquote(fnameo)
+            return SMessages(filename=moonus, errors=None)
         except Exception as errors:
-            return SMessages(result="Unknown.tmp", errors=errors)
+            return SMessages(filename=Scripted.DATA14, errors=errors)
+
+#=========================================================================
+
+    async def get04(location):
+        try:
+            moonus = str(os.path.basename(location))
+            return SMessages(filename=moonus, errors=None)
+        except Exception as errors:
+            return SMessages(filename=Scripted.DATA14, errors=errors)
 
 #=========================================================================
```

### Comparing `monisha-0.0.74/Monisha/functions/function18.py` & `monisha-0.0.75/Monisha/functions/function18.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,86 @@
+from ..scripts import Scripted
 from hachoir.parser import createParser
 from hachoir.metadata import extractMetadata
-#=======================================================================================
+#=================================================================
 
-class SMessages:
-    def __init__(self, **kwargs):
-        self.width = kwargs.get("width", 0)
-        self.height = kwargs.get("height", 0)
-        self.duration = kwargs.get("duration", 0)
+class Metadatas:
 
-#=======================================================================================
+    async def title(flocation, default=Scripted.DATA03):
+        metadato = createParser(flocation)
+        metadata = extractMetadata(metadato)
+        if not metadata or metadata == None:
+            return default
+        title = metadata.get("title", default)
+        return title
 
-class Metadatas:
+#=================================================================
 
-    async def width(flocation):
+    async def artist(flocation, default=Scripted.DATA03):
         metadato = createParser(flocation)
         metadata = extractMetadata(metadato)
-        if metadata == None:
-            return 0
-        width = metadata.get("width") if metadata.has("width") else 0
+        if not metadata or metadata == None:
+            return default
+        title = metadata.get("artist", default)
+        return title
+
+#=================================================================
+
+    async def width(flocation, default=0):
+        metadato = createParser(flocation)
+        metadata = extractMetadata(metadato)
+        if not metadata or metadata == None:
+            return default
+        width = metadata.get("width", default)
         return width
 
-#=======================================================================================
+#=================================================================
 
-    async def height(flocation):
+    async def height(flocation, default=0):
         metadato = createParser(flocation)
         metadata = extractMetadata(metadato)
-        if metadata == None:
-            return 0
-        height = metadata.get("height") if metadata.has("height") else 0
+        if not metadata or metadata == None:
+            return default
+        height = metadata.get("height", default)
         return height
 
-#=======================================================================================
+#=================================================================
 
-    async def duration(flocation):
+    async def duration(flocation, default=0):
         metadato = createParser(flocation)
         metadata = extractMetadata(metadato)
-        if metadata == None:
-            return 0
-        duration = metadata.get("duration").seconds if metadata.has("duration") else 0
+        if not metadata or metadata == None:
+            return default
+        duration = metadata.get("duration", default).seconds
         return duration
 
-#=======================================================================================
+#=================================================================
 
     async def get01(flocation):
         metadato = createParser(flocation)
         metadata = extractMetadata(metadato)
-        if metadata == None:
+        if not metadata or metadata == None:
             return 0, 0, 0
-        width = metadata.get("width") if metadata.has("width") else 0
-        height = metadata.get("height") if metadata.has("height") else 0
-        duration = metadata.get("duration").seconds if metadata.has("duration") else 0
+        width = metadata.get("width", 0)
+        height = metadata.get("height", 0)
+        duration = metadata.get("duration", 0).seconds
         return width, height, duration
 
-#=======================================================================================
+#=================================================================
 
     async def get02(flocation):
+        zerosecn = 0
         metadato = createParser(flocation)
         metadata = extractMetadata(metadato)
-        if metadata == None:
-            return SMessages(width=0, height=0, duration=0)
-        width = metadata.get("width") if metadata.has("width") else 0
-        height = metadata.get("height") if metadata.has("height") else 0
-        duration = metadata.get("duration").seconds if metadata.has("duration") else 0
-        return SMessages(width=width, height=height, duration=duration)
+        if metadata == None or metadata == Scripted.DATA01:
+            return Scripted.DATA03, Scripted.DATA03, 0
+        title = metadata.get("title", Scripted.DATA03)
+        artist = metadata.get("artist", Scripted.DATA03)
+        duration = metadata.get("duration", zerosecn).seconds
+        return title, artist, duration
+
+#=================================================================
+
+
+
+
 
-#=======================================================================================
```

### Comparing `monisha-0.0.74/Monisha/functions/function19.py` & `monisha-0.0.75/Monisha/functions/function19.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from ..scripts import Numeo
 from decimal import Decimal, ROUND_DOWN
 #==================================================================================
 
 def views(sizes):
-
     if sizes == 0 or sizes < 0:
         return sizes
-
     indeu = 0
     power = 1000
     while sizes >= power and indeu < len(Numeo.DATA01) - 1:
         sizes /= power
         indeu += 1
-
     sized = float(Decimal(sizes).quantize(Decimal('0.01'), rounding=ROUND_DOWN))
     sizeo = str(int(sized)) if sized.is_integer() else str(round(sized, 2))
     moonu = sizeo + Numeo.DATA01[indeu]
     return moonu
 
 #==================================================================================
```

### Comparing `monisha-0.0.74/Monisha/functions/function20.py` & `monisha-0.0.75/Monisha/functions/function20.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/Monisha/scripts/es.py` & `monisha-0.0.75/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/PKG-INFO` & `monisha-0.0.75/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.74
+Version: 0.0.75
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.74 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.75 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.74/monisha.egg-info/PKG-INFO` & `monisha-0.0.75/monisha.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.74
+Version: 0.0.75
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.74 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.75 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.74/monisha.egg-info/SOURCES.txt` & `monisha-0.0.75/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.74/setup.py` & `monisha-0.0.75/setup.py`

 * *Files identical despite different names*

