# Comparing `tmp/ddir-3.1.1-py3-none-any.whl.zip` & `tmp/ddir-3.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15004 bytes, number of entries: 13
--rw-r--r--  2.0 unx     4924 b- defN 24-May-16 14:58 ddir/__init__.py
--rw-r--r--  2.0 unx     4445 b- defN 24-May-16 14:58 ddir/__main__.py
--rw-r--r--  2.0 unx      156 b- defN 24-May-16 14:58 ddir/__version__.py
--rw-r--r--  2.0 unx    12671 b- defN 24-May-16 14:58 ddir/diff.py
--rw-r--r--  2.0 unx      673 b- defN 24-May-16 14:58 ddir/initialize.py
--rw-r--r--  2.0 unx     2600 b- defN 24-May-16 14:58 ddir/legacy.py
--rw-r--r--  2.0 unx     5828 b- defN 24-May-16 14:58 ddir/target.py
--rw-r--r--  2.0 unx     1211 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4541 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      969 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/RECORD
-13 files, 38159 bytes uncompressed, 13414 bytes compressed:  64.8%
+Zip file size: 14977 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     4924 b- defN 24-May-25 07:03 ddir/__init__.py
+-rw-r--r--  2.0 unx     4445 b- defN 24-May-25 07:03 ddir/__main__.py
+-rw-r--r--  2.0 unx      156 b- defN 24-May-25 07:03 ddir/__version__.py
+-rw-r--r--  2.0 unx    12522 b- defN 24-May-25 07:03 ddir/diff.py
+-rw-r--r--  2.0 unx      673 b- defN 24-May-25 07:03 ddir/initialize.py
+-rw-r--r--  2.0 unx     2600 b- defN 24-May-25 07:03 ddir/legacy.py
+-rw-r--r--  2.0 unx     5828 b- defN 24-May-25 07:03 ddir/target.py
+-rw-r--r--  2.0 unx     1211 b- defN 24-May-25 07:03 ddir-3.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4541 b- defN 24-May-25 07:03 ddir-3.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-25 07:03 ddir-3.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-25 07:03 ddir-3.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-25 07:03 ddir-3.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      969 b- defN 24-May-25 07:03 ddir-3.1.2.dist-info/RECORD
+13 files, 38010 bytes uncompressed, 13387 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: ddir/legacy.py
 Comment: 
 
 Filename: ddir/target.py
 Comment: 
 
-Filename: ddir-3.1.1.dist-info/LICENSE
+Filename: ddir-3.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: ddir-3.1.1.dist-info/METADATA
+Filename: ddir-3.1.2.dist-info/METADATA
 Comment: 
 
-Filename: ddir-3.1.1.dist-info/WHEEL
+Filename: ddir-3.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: ddir-3.1.1.dist-info/entry_points.txt
+Filename: ddir-3.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ddir-3.1.1.dist-info/top_level.txt
+Filename: ddir-3.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ddir-3.1.1.dist-info/RECORD
+Filename: ddir-3.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddir/__version__.py

```diff
@@ -1,7 +1,7 @@
 """
 This module holds the version of ddir.
 
 It contains a placeholder for the version number, which is replaced by the build script.
 """
 
-VERSION = '3.1.1'
+VERSION = '3.1.2'
```

## ddir/diff.py

```diff
@@ -7,19 +7,19 @@
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import date, datetime
 from enum import Enum
 from hashlib import md5
-from os import sep, listdir, mkdir, stat
+from os import sep, listdir, stat
 from os.path import exists, isfile, isdir
 from random import randint as rand
 from re import match
-from shutil import copy2 as cp
+from shutil import copy2 as cp, copytree
 from time import localtime, strftime
 from typing import List
 
 from ddir import ENCODING, ProgramError
 from ddir.target import Target
 
 
@@ -356,22 +356,16 @@
 
 
 def _copy_file_or_directory(source: str, target: str) -> None:
     if isfile(source):
         cp(source, target)
         print(f'Copied/overridden file {source} to {target}')
     elif isdir(source):
-        mkdir(target)
-
-        for file in listdir(source):
-            abs_target = sep.join([source, file])
-            abs_source = sep.join([target, file])
-
-            cp(abs_target, abs_source)
-            print(f'Copied/overridden file {abs_target} to {target}')
+        copytree(source, target, copy_function=cp)
+        print(f'Copied/overridden directory {source} to {target}')
     else:
         print(f'{source} does not exist anymore, thus is skipped')
 
 
 def _copy_with_mode_check(mode: int, diff: Diff, source: str, target: str) -> None:
     mode = _get_mode_from_selection(mode, diff)
```

## Comparing `ddir-3.1.1.dist-info/LICENSE` & `ddir-3.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ddir-3.1.1.dist-info/METADATA` & `ddir-3.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddir
-Version: 3.1.1
+Version: 3.1.2
 Summary: Diff a directory and sync changes.
 License: Public Domain
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ddir
```

## Comparing `ddir-3.1.1.dist-info/RECORD` & `ddir-3.1.2.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ddir/__init__.py,sha256=hhcbMVrBNnaITOn7qp9LtkF6cXaZcwIxGh9ew2IKgsA,4924
 ddir/__main__.py,sha256=oV1gLrsOBY4j91BquC-W3m6CDSTJ-dXpICrZrjKQMgk,4445
-ddir/__version__.py,sha256=I_Yi3h702ANpgAIAp7MxgB9Vd10cnwlnVUSyVbU0f80,156
-ddir/diff.py,sha256=6a-v1Hw8RUyhzsf8KJmvdVsH3pUelWBBj4_6gq2IJjk,12671
+ddir/__version__.py,sha256=lB1x5q-fSXAWgUQFpIWfhzgpEOXMhQVN9o49do2PZKE,156
+ddir/diff.py,sha256=L4sHnI5Q_MrLe-Q-dVjwlYUgEEoGZIkNT0mL4Kvf9i4,12522
 ddir/initialize.py,sha256=XbgoD4YBxEsLfP5zabvuGIcOd2hAzHAYuBaPgeCY260,673
 ddir/legacy.py,sha256=shoCl9H9ZEO7Z_hh6urAyrUWzWnfgpygJsE7NIiBfGo,2600
 ddir/target.py,sha256=DK4riv1VBpjkomsulZeoc6JjPPcVL4Gp731y_ey9Oqo,5828
-ddir-3.1.1.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
-ddir-3.1.1.dist-info/METADATA,sha256=nOLx4x_JtC5_X_4MR2CAj8k5ZCPx4SALefg1FxlZeKs,4541
-ddir-3.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ddir-3.1.1.dist-info/entry_points.txt,sha256=uEQJqxm8H6cL_TYsi1-Vd7vdRnesOSVPbnr4noyXnwE,44
-ddir-3.1.1.dist-info/top_level.txt,sha256=F7NGOmHjOI4UseDtkAR3bTsbwIxLi4Gy8KaMMpIl6Ws,5
-ddir-3.1.1.dist-info/RECORD,,
+ddir-3.1.2.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
+ddir-3.1.2.dist-info/METADATA,sha256=JxJgPYDfcDuso7lVerC2d7ndcPSSmdG22_Orz_XlXE0,4541
+ddir-3.1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ddir-3.1.2.dist-info/entry_points.txt,sha256=uEQJqxm8H6cL_TYsi1-Vd7vdRnesOSVPbnr4noyXnwE,44
+ddir-3.1.2.dist-info/top_level.txt,sha256=F7NGOmHjOI4UseDtkAR3bTsbwIxLi4Gy8KaMMpIl6Ws,5
+ddir-3.1.2.dist-info/RECORD,,
```

