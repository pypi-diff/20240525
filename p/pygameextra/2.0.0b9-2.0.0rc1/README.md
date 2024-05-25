# Comparing `tmp/pygameextra-2.0.0b9.tar.gz` & `tmp/pygameextra-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameextra-2.0.0b9.tar", last modified: Sun Jul 30 14:51:39 2023, max compression
+gzip compressed data, was "pygameextra-2.0.0rc1.tar", last modified: Fri Aug 25 09:48:03 2023, max compression
```

## Comparing `pygameextra-2.0.0b9.tar` & `pygameextra-2.0.0rc1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/
--rw-rw-rw-   0        0        0     1084 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/LICENSE
--rw-rw-rw-   0        0        0      530 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.131538 pygameextra-2.0.0b9/pygameextra/
--rw-rw-rw-   0        0        0     2295 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/button.py
--rw-rw-rw-   0        0        0     1002 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/colors.py
--rw-rw-rw-   0        0        0     4998 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/debug.py
--rw-rw-rw-   0        0        0    18693 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/display.py
--rw-rw-rw-   0        0        0     3108 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/draw.py
--rw-rw-rw-   0        0        0     2533 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/event.py
--rw-rw-rw-   0        0        0     1509 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/fill.py
--rw-rw-rw-   0        0        0     1419 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/fingersupport.py
--rw-rw-rw-   0        0        0    38624 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/font.ttf
--rw-rw-rw-   0        0        0     2324 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/fpslogger.py
--rw-rw-rw-   0        0        0      598 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/image.py
--rw-rw-rw-   0        0        0     4015 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/infinitygrid.py
--rw-rw-rw-   0        0        0      617 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/math.py
--rw-rw-rw-   0        0        0     2710 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/modified.py
--rw-rw-rw-   0        0        0     2812 2023-02-01 15:24:48.000000 pygameextra-2.0.0b9/pygameextra/mouse.py
--rw-rw-rw-   0        0        0     6747 2023-07-30 14:49:17.000000 pygameextra-2.0.0b9/pygameextra/pnzc.py
--rw-rw-rw-   0        0        0      145 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/pygame.py
--rw-rw-rw-   0        0        0     5159 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/recorder.py
--rw-rw-rw-   0        0        0      226 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/rect.py
--rw-rw-rw-   0        0        0      568 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/settings.py
--rw-rw-rw-   0        0        0     2084 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/sheet_handlers.py
--rw-rw-rw-   0        0        0     1477 2023-01-29 12:06:34.000000 pygameextra-2.0.0b9/pygameextra/smooth.py
--rw-rw-rw-   0        0        0      267 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/sorters.py
--rw-rw-rw-   0        0        0     2993 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/sprite.py
--rw-rw-rw-   0        0        0     1098 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/text.py
--rw-rw-rw-   0        0        0      343 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/time.py
--rw-rw-rw-   0        0        0      119 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra/version.py
-drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.162776 pygameextra-2.0.0b9/pygameextra.egg-info/
--rw-rw-rw-   0        0        0      530 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1114 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-30 14:51:37.000000 pygameextra-2.0.0b9/pygameextra.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/pygameextra_tester/
--rw-rw-rw-   0        0        0      353 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/Xbutton.png
--rw-rw-rw-   0        0        0      548 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/Ybutton.png
--rw-rw-rw-   0        0        0    12382 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/columns.png
--rw-rw-rw-   0        0        0      654 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/debug_icon.png
--rw-rw-rw-   0        0        0      491 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/mario_01.png
--rw-rw-rw-   0        0        0     2194 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/mouse_middle.png
--rw-rw-rw-   0        0        0      332 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/pygameextra_tester/rows.png
--rw-rw-rw-   0        0        0       42 2023-07-30 14:51:39.209650 pygameextra-2.0.0b9/setup.cfg
--rw-rw-rw-   0        0        0     1137 2023-01-29 01:13:53.000000 pygameextra-2.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-25 09:48:03.623826 pygameextra-2.0.0rc1/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/LICENSE
+-rw-rw-rw-   0        0        0      531 2023-08-25 09:48:03.592125 pygameextra-2.0.0rc1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-25 09:48:03.435390 pygameextra-2.0.0rc1/pygameextra/
+-rw-rw-rw-   0        0        0     2328 2023-08-25 07:24:52.000000 pygameextra-2.0.0rc1/pygameextra/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/button.py
+-rw-rw-rw-   0        0        0     1002 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/colors.py
+-rw-rw-rw-   0        0        0     4998 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/debug.py
+-rw-rw-rw-   0        0        0    18827 2023-08-25 07:13:15.000000 pygameextra-2.0.0rc1/pygameextra/display.py
+-rw-rw-rw-   0        0        0     3108 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/draw.py
+-rw-rw-rw-   0        0        0     2533 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/event.py
+-rw-rw-rw-   0        0        0     1509 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/fill.py
+-rw-rw-rw-   0        0        0     1419 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/fingersupport.py
+-rw-rw-rw-   0        0        0    38624 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/font.ttf
+-rw-rw-rw-   0        0        0     2324 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/fpslogger.py
+-rw-rw-rw-   0        0        0      598 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/image.py
+-rw-rw-rw-   0        0        0     4015 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/infinitygrid.py
+-rw-rw-rw-   0        0        0      619 2023-08-25 07:18:29.000000 pygameextra-2.0.0rc1/pygameextra/math.py
+-rw-rw-rw-   0        0        0     2998 2023-08-25 07:10:09.000000 pygameextra-2.0.0rc1/pygameextra/modified.py
+-rw-rw-rw-   0        0        0     2812 2023-02-01 15:24:48.000000 pygameextra-2.0.0rc1/pygameextra/mouse.py
+-rw-rw-rw-   0        0        0     6747 2023-07-30 14:49:17.000000 pygameextra-2.0.0rc1/pygameextra/pnzc.py
+-rw-rw-rw-   0        0        0      145 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/pygame.py
+-rw-rw-rw-   0        0        0     5238 2023-08-25 08:01:17.000000 pygameextra-2.0.0rc1/pygameextra/recorder.py
+-rw-rw-rw-   0        0        0      226 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/rect.py
+-rw-rw-rw-   0        0        0      568 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/settings.py
+-rw-rw-rw-   0        0        0     2084 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/sheet_handlers.py
+-rw-rw-rw-   0        0        0     1477 2023-01-29 12:06:34.000000 pygameextra-2.0.0rc1/pygameextra/smooth.py
+-rw-rw-rw-   0        0        0      267 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/sorters.py
+-rw-rw-rw-   0        0        0     2993 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/sprite.py
+-rw-rw-rw-   0        0        0     1098 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/text.py
+-rw-rw-rw-   0        0        0      343 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra/time.py
+-rw-rw-rw-   0        0        0      556 2023-08-25 07:41:27.000000 pygameextra-2.0.0rc1/pygameextra/tsx.py
+-rw-rw-rw-   0        0        0      210 2023-08-25 09:46:03.000000 pygameextra-2.0.0rc1/pygameextra/version.py
+drwxrwxrwx   0        0        0        0 2023-08-25 09:48:03.482265 pygameextra-2.0.0rc1/pygameextra.egg-info/
+-rw-rw-rw-   0        0        0      531 2023-08-25 09:48:02.000000 pygameextra-2.0.0rc1/pygameextra.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1133 2023-08-25 09:48:02.000000 pygameextra-2.0.0rc1/pygameextra.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-25 09:48:02.000000 pygameextra-2.0.0rc1/pygameextra.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-08-25 09:48:02.000000 pygameextra-2.0.0rc1/pygameextra.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-08-25 09:48:02.000000 pygameextra-2.0.0rc1/pygameextra.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-08-25 09:48:02.000000 pygameextra-2.0.0rc1/pygameextra.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-25 09:48:03.592125 pygameextra-2.0.0rc1/pygameextra_tester/
+-rw-rw-rw-   0        0        0      353 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra_tester/Xbutton.png
+-rw-rw-rw-   0        0        0      548 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra_tester/Ybutton.png
+-rw-rw-rw-   0        0        0    15578 2023-08-25 07:54:21.000000 pygameextra-2.0.0rc1/pygameextra_tester/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra_tester/columns.png
+-rw-rw-rw-   0        0        0      654 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra_tester/debug_icon.png
+-rw-rw-rw-   0        0        0      491 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra_tester/mario_01.png
+-rw-rw-rw-   0        0        0     2194 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra_tester/mouse_middle.png
+-rw-rw-rw-   0        0        0      332 2023-01-29 01:13:53.000000 pygameextra-2.0.0rc1/pygameextra_tester/rows.png
+-rw-rw-rw-   0        0        0       42 2023-08-25 09:48:03.623826 pygameextra-2.0.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1131 2023-08-25 09:46:03.000000 pygameextra-2.0.0rc1/setup.py
```

### Comparing `pygameextra-2.0.0b9/LICENSE` & `pygameextra-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/PKG-INFO` & `pygameextra-2.0.0rc1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygameextra
-Version: 2.0.0b9
+Version: 2.0.0rc1
 Summary: Pygame. Made easier.
 Author: Red
 Author-email: redtonehair@gmail.com
 Keywords: python
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pygameextra-2.0.0b9/pygameextra/__init__.py` & `pygameextra-2.0.0rc1/pygameextra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pygameextra.sheet_handlers import *
 from pygameextra.sprite import *
 from pygameextra.modified import *
 from pygameextra.version import get as get_version
 from pygameextra import event, time, fill, mouse, settings, colors, draw, math, text, button, rect
 from pygameextra.recorder import comment, padding_comment
 from pygameextra.event import Pquit
+from pygameextra.tsx import TSX
 
 __version__ = get_version()
 
 
 def init(display_init_size: tuple = None):
     pygame.mixer.pre_init(frequency=44100, size=16, channels=1, buffer=512)
     pygame.init()
```

### Comparing `pygameextra-2.0.0b9/pygameextra/button.py` & `pygameextra-2.0.0rc1/pygameextra/button.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/colors.py` & `pygameextra-2.0.0rc1/pygameextra/colors.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/debug.py` & `pygameextra-2.0.0rc1/pygameextra/debug.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/display.py` & `pygameextra-2.0.0rc1/pygameextra/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """PYGAME EXTRA Display script
 This script manages all display functions"""
+from typing import Union
 
 import pygame
 from pygameextra.modified import Surface
 import pygameextra.settings as settings
 import pygameextra.recorder as recorder
 import pygameextra.time
 
@@ -17,18 +18,19 @@
     DISPLAY_MODE_RESIZABLE: pygame.RESIZABLE,
     DISPLAY_MODE_FULLSCREEN: pygame.FULLSCREEN,
     DISPLAY_MODE_HIDDEN: pygame.HIDDEN
 }
 # Display Others...
 DISPLAY_DEFAULT_TITLE = "pygameextra window"
 display_reference = Surface
-max_size = (700, 700)
+max_size = (0, 0)
+
 
 # Functions
-def set_caption(title=DISPLAY_DEFAULT_TITLE): pygame.display.set_caption(title)
+def set_caption(title: str = DISPLAY_DEFAULT_TITLE): pygame.display.set_caption(title)
 
 
 def set_icon(icon: [Surface, pygame.Surface]):
     """Set icon
     context(icon: Surface or pygame.Surface) -> None
 
     Parameters:
@@ -69,18 +71,19 @@
 
     for item in flags:  # Go through all the flags
         final_flags = final_flags | item  # Combine all the flags into the final flags variable
     dis = pygame.display.set_mode(size, final_flags)  # Create the display surface
     dis = Surface(surface=dis, layer=-1)
     dis.display_tag = True
 
-
     set_caption(title)
     # noinspection PyTypeChecker
-    set_icon(Surface(surface=pygame.image.fromstring(b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00`\xb4\xff=^\xb4\xff\xffY\xb3\xf9(\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\\\xad\xf5\x19^\xb3\xfe\xfb^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xfe\xf3U\xbf\xff\x0c\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x80\xbf\xff\x04]\xb4\xfe\xe8^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb3\xfd\xd9\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xc5^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xfe\xb0\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb3\xff\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffL\x9e\xe5\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff]\xb4\xffR\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffT\xa8\xf1\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffY\xb3\xf9(\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffZ\xaf\xf9\xff0|\xbe\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xfe\xf3U\xbf\xff\x0c\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\\\xb0\xfa\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff]\xb3\xfe\xffM\x98\xda\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffO\x9c\xde\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfd\xf9^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbe\xff^\xb4\xff\xffS\xa1\xe5\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb2\xfd{^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xffR\xa5\xed\xffj\xb9\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb5\xffL^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xffI\x9a\xe1\xfff\xb7\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00_\xb6\xff#^\xb3\xfe\xfe^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffA\x90\xd5\xffa\xb5\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb2\xfe\xb7^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffv\xbf\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffS\xa2\xe7\xff_\xb5\xfd\x83\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x8d\xca\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffP\x9d\xe1\xff^\xb3\xfe\xf1]\xa2\xff\x0b\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x84\xc5\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffN\x99\xdb\xff]\xb3\xfd\xfeZ\xb3\xff%\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffy\xc1\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xff[\xaf\xf8\xff\\\xb2\xfc\xff^\xb5\xffL\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffd\xb7\xff\xff]\xb2\xfd{\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffh\xb9\xff\xff]\xb4\xfd\xa7\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffm\xbb\xff\xff]\xb3\xfe\xd2\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xff]\xb4\xfe\xefU\xaa\xff\t\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00b\xb1\xff\r^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x91\xcb\xff\xff_\xb4\xfe\xfec\xb8\xff$\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00Y\xb3\xf9(^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x95\xcd\xff\xffc\xb6\xff\xff^\xb2\xffI\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\\\xb3\xffP^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xffk\xba\xff\xff_\xb4\xfft\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00_\xb3\xff|^\xb4\xff\xff\\\xb2\xfd\xa3\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00', (32, 32), 'RGBA')))
+    set_icon(Surface(surface=pygame.image.fromstring(
+        b'\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00`\xb4\xff=^\xb4\xff\xffY\xb3\xf9(\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\\\xad\xf5\x19^\xb3\xfe\xfb^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xfe\xf3U\xbf\xff\x0c\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x80\xbf\xff\x04]\xb4\xfe\xe8^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb3\xfd\xd9\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xc5^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xfe\xb0\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb3\xff\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffL\x9e\xe5\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff]\xb4\xffR\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffT\xa8\xf1\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffY\xb3\xf9(\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffZ\xaf\xf9\xff0|\xbe\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xfe\xf3U\xbf\xff\x0c\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\\\xb0\xfa\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff]\xb3\xfe\xffM\x98\xda\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffO\x9c\xde\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb3\xfd\xf9^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbe\xff^\xb4\xff\xffS\xa1\xe5\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb2\xfd{^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xff/{\xbd\xff/{\xbd\xffR\xa5\xed\xffj\xb9\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00^\xb5\xffL^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff/{\xbd\xff/{\xbd\xffI\x9a\xe1\xfff\xb7\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00_\xb6\xff#^\xb3\xfe\xfe^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffA\x90\xd5\xffa\xb5\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xff_\xb3\xfd\x94\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb2\xfe\xb7^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffv\xbf\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffS\xa2\xe7\xff_\xb5\xfd\x83\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x8d\xca\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffL\x96\xd7\xffL\x96\xd7\xffP\x9d\xe1\xff^\xb3\xfe\xf1]\xa2\xff\x0b\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x84\xc5\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffZ\xae\xf7\xffL\x96\xd7\xffN\x99\xdb\xff]\xb3\xfd\xfeZ\xb3\xff%\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xffy\xc1\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xff[\xaf\xf8\xff\\\xb2\xfc\xff^\xb5\xffL\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffd\xb7\xff\xff]\xb2\xfd{\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffx\xc0\xff\xffx\xc0\xff\xffh\xb9\xff\xff]\xb4\xfd\xa7\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xffx\xc0\xff\xffm\xbb\xff\xff]\xb3\xfe\xd2\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00]\xb4\xfe\xbf^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff^\xb4\xff\xff]\xb4\xfe\xefU\xaa\xff\t\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00b\xb1\xff\r^\xb3\xfe\xf4^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x91\xcb\xff\xff_\xb4\xfe\xfec\xb8\xff$\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00Y\xb3\xf9(^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xff\x96\xce\xff\xff\x95\xcd\xff\xffc\xb6\xff\xff^\xb2\xffI\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\\\xb3\xffP^\xb4\xff\xff^\xb4\xff\xff^\xb4\xff\xff\x96\xce\xff\xffk\xba\xff\xff_\xb4\xfft\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00_\xb3\xff|^\xb4\xff\xff\\\xb2\xfd\xa3\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00',
+        (32, 32), 'RGBA')))
 
     context(dis)
     return dis
 
 
 def update(framerate: int = None, area: tuple = None):
     """Updates the entire display or an area of it
@@ -98,37 +101,37 @@
 
     pygameextra.time.tickBlock = False
     if settings.auto_fps:
         pygameextra.time.tick(framerate)
         pygameextra.time.tickBlock = True
 
 
-def blit(obj, pos=(0, 0), area=None):
+def blit(obj: Union['Surface', pygame.Surface], pos: tuple = (0, 0), area: tuple = None):
     display_reference.stamp(obj, pos, area)
     if not settings.recording:
         return
     if type(obj) == Surface:
         obj = obj.surface
     if display_reference.display_tag:
         recorder.record(recorder.Blit(obj, pos, area))
 
 
-def get_width():
+def get_width() -> int:
     return display_reference.size[0]
 
 
-def get_height():
+def get_height() -> int:
     return display_reference.size[1]
 
 
-def get_size():
+def get_size() -> tuple:
     return display_reference.size
 
 
-def get_max():
+def get_max() -> tuple:
     return max_size
 
 
 def backup_details():
     if make_data[2] == DISPLAY_MODE_RESIZABLE:
         make_data[0] = display_reference.size
-    return make_data.copy()
+    return make_data.copy()
```

### Comparing `pygameextra-2.0.0b9/pygameextra/draw.py` & `pygameextra-2.0.0rc1/pygameextra/draw.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/event.py` & `pygameextra-2.0.0rc1/pygameextra/event.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/fill.py` & `pygameextra-2.0.0rc1/pygameextra/fill.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/fingersupport.py` & `pygameextra-2.0.0rc1/pygameextra/fingersupport.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/font.ttf` & `pygameextra-2.0.0rc1/pygameextra/font.ttf`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/fpslogger.py` & `pygameextra-2.0.0rc1/pygameextra/fpslogger.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/image.py` & `pygameextra-2.0.0rc1/pygameextra/image.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/infinitygrid.py` & `pygameextra-2.0.0rc1/pygameextra/infinitygrid.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/math.py` & `pygameextra-2.0.0rc1/pygameextra/math.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import math
 # noinspection PyUnresolvedReferences
-from perlin_noise import PerlinNoise
+# from perlin_noise import PerlinNoise
 
 
 def center(rect: tuple):
     return rect[0]+rect[2]*.5, rect[1]+rect[3]*.5
 
 
 def dist(point_a: tuple, point_b: tuple):
```

### Comparing `pygameextra-2.0.0b9/pygameextra/modified.py` & `pygameextra-2.0.0rc1/pygameextra/modified.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 """PYGAME EXTRA Modifications script
 This script manages all pygame modifications"""
+from typing import Union, List
 
 import pygame
+from pygameextra.rect import Rect
 from pygameextra.sorters import layer_sorter
 
 
 class SurfaceException(Exception):
     pass
 
 
 class Surface:
-    surface = None
-    size = None
-    layer = 0
-    display_tag = False
+    surface: pygame.Surface
+    size: tuple
+    layer: int
+    display_tag: False
 
-    def __init__(self, size=(0, 0), layer=0, surface: pygame.Surface = None):
+    def __init__(self, size: tuple = (0, 0), layer: int = 0, surface: pygame.Surface = None):
         if surface:
             self.size = surface.get_size()
             self.surface = surface
             self.layer = layer
         else:
             self.size = size
-            self.surface = pygame.Surface(size,pygame.SRCALPHA)
+            self.surface = pygame.Surface(size, pygame.SRCALPHA)
             self.layer = layer
         self.area = None  # Used by stamps function
         self.pos = None  # Used by stamps function
         self.frames = 1  # Used by sprite animation function, if used improperly
 
-    def stamp(self, source: ['Surface', pygame.Surface], position=(0, 0), area=None, special_flags: int = 0):
+    def stamp(self, source: Union['Surface', pygame.Surface], position: tuple = (0, 0), area: tuple = None,
+              special_flags: int = 0):
         if type(source) == pygame.Surface:
             self.surface.blit(source, position, area, special_flags)
         else:
             self.surface.blit(source.surface, position, area, special_flags)
 
-    def stamps(self, sources: list, positions: list = None, areas: list = None, special_flags: int = 0):
+    def stamps(self, sources: List[Union['Surface', pygame.Surface]], positions: List[tuple] = None,
+               areas: List[tuple] = None, special_flags: int = 0):
         if not positions:
             positions = [(0, 0)] * len(sources)
         if not areas:
             areas = [None] * len(sources)
         for i in range(len(sources)):
             sources[i].pos = positions[i]
             sources[i].area = areas[i]
         sources.sort(key=layer_sorter)
         for source in sources:
             self.surface.blit(source.surface, source.area, special_flags)
 
-    def bind(self, layer):
+    def bind(self, layer: int):
         if self.layer >= 0 and layer >= 0:
             self.layer = layer
         elif layer < 0:
             raise SurfaceException("Can't bind a surface to a display surface layer.")
         else:
             raise SurfaceException("Can't bind a display surface to a surface layer.")
 
@@ -66,12 +70,16 @@
 
     def set_at(self, x_y: tuple, color: tuple) -> None:
         return self.surface.set_at(x_y, color)
 
     def set_alpha(self, alpha: int, flags: int = 0) -> None:
         return self.surface.set_alpha(alpha, flags)
 
+    @property
+    def rect(self) -> Rect:
+        return self.surface.get_rect()
+
 
 def transparent_surface(area: tuple, alpha: int):
     new_surface = Surface(area)
     new_surface.set_alpha(alpha)
-    return new_surface
+    return new_surface
```

### Comparing `pygameextra-2.0.0b9/pygameextra/mouse.py` & `pygameextra-2.0.0rc1/pygameextra/mouse.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/pnzc.py` & `pygameextra-2.0.0rc1/pygameextra/pnzc.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/recorder.py` & `pygameextra-2.0.0rc1/pygameextra/recorder.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,22 +98,24 @@
         return (
             item.pos[0]-item.radius*.5,
             item.pos[1]-item.radius*.5,
             item.pos[0]+item.radius*.5,
             item.pos[1]+item.radius*.5,
         )
     elif type(item) == DrawPolygon:
-        rect = (0, 0, 1, 1)
+        max_x = -100
+        min_x = 100
+        max_y = -100
+        min_y = 100
         for point in item.points:
-            rect = (
-                min(rect[0], point[0]),
-                min(rect[1], point[1]),
-                max(rect[2], point[0]),
-                max(rect[3], point[1]),
-            )
+            max_x = max(max_x, point[0])
+            min_x = min(min_x, point[0])
+            max_y = max(max_y, point[1])
+            min_y = min(min_y, point[1])
+        return min_x, min_y, max_x-min_x, max_y-min_y
     return 0, 0, 1, 1
 
 
 def sorter(item):
     if type(item) == display.display_reference.size:
         return 0
     return 1
```

### Comparing `pygameextra-2.0.0b9/pygameextra/settings.py` & `pygameextra-2.0.0rc1/pygameextra/settings.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/sheet_handlers.py` & `pygameextra-2.0.0rc1/pygameextra/sheet_handlers.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/smooth.py` & `pygameextra-2.0.0rc1/pygameextra/smooth.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/sprite.py` & `pygameextra-2.0.0rc1/pygameextra/sprite.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra/text.py` & `pygameextra-2.0.0rc1/pygameextra/text.py`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra.egg-info/PKG-INFO` & `pygameextra-2.0.0rc1/pygameextra.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygameextra
-Version: 2.0.0b9
+Version: 2.0.0rc1
 Summary: Pygame. Made easier.
 Author: Red
 Author-email: redtonehair@gmail.com
 Keywords: python
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pygameextra-2.0.0b9/pygameextra.egg-info/SOURCES.txt` & `pygameextra-2.0.0rc1/pygameextra.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 pygameextra/settings.py
 pygameextra/sheet_handlers.py
 pygameextra/smooth.py
 pygameextra/sorters.py
 pygameextra/sprite.py
 pygameextra/text.py
 pygameextra/time.py
+pygameextra/tsx.py
 pygameextra/version.py
 pygameextra.egg-info/PKG-INFO
 pygameextra.egg-info/SOURCES.txt
 pygameextra.egg-info/dependency_links.txt
 pygameextra.egg-info/entry_points.txt
 pygameextra.egg-info/requires.txt
 pygameextra.egg-info/top_level.txt
```

### Comparing `pygameextra-2.0.0b9/pygameextra_tester/Ybutton.png` & `pygameextra-2.0.0rc1/pygameextra_tester/Ybutton.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra_tester/__init__.py` & `pygameextra-2.0.0rc1/pygameextra_tester/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,31 +12,34 @@
 bX = pe.Image(f"{sp}/Xbutton.png", size=(100, 100), position=(100, 0))
 bX2 = pe.Image(f"{sp}/Xbutton.png", size=(20, 20), position=(100, 0))
 sX = pe.Image(f"{sp}/Xbutton.png", size=(20, 20), position=(100, 0))
 bY = pe.Image(f"{sp}/Ybutton.png", size=(100, 100), position=(100, 0))
 bY2 = pe.Image(f"{sp}/Ybutton.png", size=(20, 20), position=(100, 0))
 
 # Sprite sheet sprites
-s1 = pe.Sprite(pe.Sheet(f"{sp}/rows.png", pe.SheetHorizontal(16, 16)), (250, 250), (0, 0), pivot="topleft")  # Rows sprite
-s2 = pe.Sprite(pe.Sheet(f"{sp}/columns.png", pe.SheetVertical(32, 32)), (250, 250), (250, 0), pivot="topleft")  # Columns sprite
+s1 = pe.Sprite(pe.Sheet(f"{sp}/rows.png", pe.SheetHorizontal(16, 16)), (250, 250), (0, 0),
+               pivot="topleft")  # Rows sprite
+s2 = pe.Sprite(pe.Sheet(f"{sp}/columns.png", pe.SheetVertical(32, 32)), (250, 250), (250, 0),
+               pivot="topleft")  # Columns sprite
 
 # Resized sprites
 s3 = pe.Sprite(f"{sp}/mario_01.png", (250, 250), pe.math.center((0, 250, 125, 125)))  # Resized sprite 1
 s3.size = 0.5
 
 s4 = pe.Sprite(f"{sp}/mario_01.png", (250, 250), pe.math.center((125, 250, 125, 125)))  # Resized sprite 2
 s4.size = 0.25
 
 s5 = pe.Sprite(f"{sp}/mario_01.png", (250, 250), pe.math.center((0, 375, 125, 125)))  # Resized sprite 3
 s5.size = 0.1
 
 s6 = pe.Sprite(f"{sp}/mario_01.png", (250, 250), pe.math.center((125, 375, 125, 125)))  # Resized sprite 4
 s6.size = 0.05
 
-s7 = pe.Sprite(f"{sp}/mario_01.png", (250, 250), pe.math.center((250, 250, 250, 250)), 90, pivot="center")  # Rotated sprite
+s7 = pe.Sprite(f"{sp}/mario_01.png", (250, 250), pe.math.center((250, 250, 250, 250)), 90,
+               pivot="center")  # Rotated sprite
 
 mouse_icon = pe.Image(f'{sp}/mouse_middle.png', (50, 50))
 debug_icon = pe.Image(f'{sp}/debug_icon.png', (50, 50))
 
 # Init sprites
 # s1.init()
 # s2.init()
@@ -54,60 +57,88 @@
     'sprite': pe.text.quick('Sprites', 15, pe.math.center((200, 200, 100, 50))),
     'shapes': pe.text.quick('Shapes', 15, pe.math.center((300, 200, 100, 50))),
     'mapping': pe.text.quick('Mapping', 15, pe.math.center((300, 250, 100, 50))),
     'math': pe.text.quick('Math', 15, pe.math.center((400, 200, 100, 50))),
     'math_lerp': pe.text.quick('Lerp', 15, pe.math.center((0, 200, 100, 50))),
     'math_center': pe.text.quick('Center', 15, pe.math.center((100, 200, 100, 50))),
     'math_dist': pe.text.quick('Distance', 15, pe.math.center((200, 200, 100, 50))),
+    'math_tsx': pe.text.quick('TSX', 15, pe.math.center((300, 200, 100, 50))),
     'math_back': pe.text.quick('< Math', 15, pe.math.center((0, 0, 100, 50))),
     '+': pe.text.quick('+', 15, pe.math.center((275, 200, 50, 50))),
     '-': pe.text.quick('-', 15, pe.math.center((175, 200, 50, 50))),
     'lerplength': pe.text.quick("100", 15, pe.math.center((225, 200, 50, 50))),
+    'distance': pe.text.quick("100", 15, pe.math.center((225, 200, 50, 50))),
+    'tsx_radius': pe.text.quick("100", 15, pe.math.center((225, 145, 50, 50))),
+    'tsx_segments': pe.text.quick("100", 15, pe.math.center((225, 200, 50, 50))),
+    'tsx_offset': pe.text.quick("100", 15, pe.math.center((225, 255, 50, 50))),
     'debug_label': pe.text.quick("Open Debug", 15, pe.math.center((400, 440, 90, 50))),
     'debug_close': pe.text.quick("Close Debug", 15, pe.math.center((400, 440, 90, 50)))
 }
 bt['math_back'].color = pe.colors.white
 bt['math_back'].init()
 bt['lerplength'].color = pe.colors.white
 bt['lerplength'].init()
+bt['tsx_radius'].color = pe.colors.white
+bt['tsx_radius'].init()
+bt['tsx_segments'].color = pe.colors.white
+bt['tsx_segments'].init()
+bt['tsx_offset'].color = pe.colors.white
+bt['tsx_offset'].init()
 bt['debug_label'].color = pe.colors.white
 bt['debug_label'].init()
 bt['debug_close'].color = pe.colors.white
 bt['debug_close'].init()
 s1.speed = .1  # Set sprite animation
 s2.speed = .2  # Set sprite animation
 s2.pong = True  # Enable sprite pong
 sO = 50  # Set slider variable
 sT = 50  # Set slider variable
 test = ""
 testall = 0
 testdrop = -100
 lerplength = .5
+tsx_segments = 100
+tsx = pe.TSX((250, 250), 100)
 log = Logger()
 
 
 # Button function
 def set_test(data):
     global test
     test = data
-    if "math_" in data:
+    if "math_" in data and not data == "math_tsx":
         settings.button_lock_timeout_time = .2
         settings.button_lock_hold = False
         pe.display.make((500, 500), "PGE Testing Utility", 1)
     else:
         settings.button_lock_timeout_time = .1
         settings.button_lock_hold = True
         pe.display.make((500, 500), "PGE Testing Utility", 0)
 
 
 def set_lerplength(data):
     global lerplength
     lerplength = data
 
 
+def set_tsx_radius(data):
+    global tsx
+    tsx.radius = data
+
+
+def set_tsx_segments(data):
+    global tsx_segments
+    tsx_segments = data
+
+
+def set_tsx_offset(data):
+    global tsx
+    tsx.offset = data
+
+
 # Test functions
 testscore = 0
 
 pe.settings.debugger = FreeInteractMode()
 
 
 # Main GAME LOOP
@@ -125,29 +156,31 @@
 
         settings.recording = False
         pe.draw.rect(pe.colors.verydarkgray, (350, 440, 150, 60))
         settings.recording = True
 
         if test == "slider":
             # noinspection PyShadowingNames
-            sO = pe.slider.boxed((125, 100, 250, 15, 20), (255, 0, 0), 0, 100, sO, (0, 0, 255), (0, 0, 0), (0, 255, 0), True, (0, 0, 255))
+            sO = pe.slider.boxed((125, 100, 250, 15, 20), (255, 0, 0), 0, 100, sO, (0, 0, 255), (0, 0, 0), (0, 255, 0),
+                                 True, (0, 0, 255))
             # noinspection PyShadowingNames
-            sT = pe.slider.normal((125, 150, 250, 15, 20), sX, 0, 100, sT, (255, 255, 255), (0, 255, 0), 5, True, (0, 0, 255), 3)
+            sT = pe.slider.normal((125, 150, 250, 15, 20), sX, 0, 100, sT, (255, 255, 255), (0, 255, 0), 5, True,
+                                  (0, 0, 255), 3)
         elif test == "button":
-            midpoint = pe.display.get_width()*.5 - 100
-            midheight = pe.display.get_height()*.5 - 50
+            midpoint = pe.display.get_width() * .5 - 100
+            midheight = pe.display.get_height() * .5 - 50
             x = 0
             y = 0
             while x < 99 and y < 99:
                 # bX2.position = (x+150, y+200)
                 # bX2.rect = bX2.object.get_rect(topleft=(x+150, y+200))
                 # bY2.position = (x + 150, y + 200)
                 # bY2.rect = bY2.object.get_rect(topleft=(x + 150, y + 200))
-                pe.button.rect((x+midpoint, y+midheight, 20, 20), pe.colors.red, pe.colors.green)
-                pe.button.image((x+midpoint+100, y+midheight, 20, 20), bX2, bY2)
+                pe.button.rect((x + midpoint, y + midheight, 20, 20), pe.colors.red, pe.colors.green)
+                pe.button.image((x + midpoint + 100, y + midheight, 20, 20), bX2, bY2)
                 x += 20
                 if x > 99:
                     x = 0
                     y += 20
         elif test == "sprite":
             pe.comment('Sprites')
             s1.display()
@@ -173,55 +206,70 @@
             pe.draw.rect(pe.colors.red, (325, 75, 100, 100), 5)
             pe.draw.rect(pe.colors.aqua, (335, 85, 80, 80), 0)
             pe.draw.line(pe.colors.red, (0, 250), (250, 500), 5)
             pe.draw.line(pe.colors.red, (250, 250), (0, 500), 5)
             pe.draw.ellipse(pe.colors.red, (250, 250, 250, 250))
 
         if test == "":
-            pe.button.rect((0, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['button'], action=set_test, data="button")
-            pe.button.rect((100, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['slider'], action=set_test, data="slider", disabled=pe.colors.gray)
-            pe.button.rect((200, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['sprite'], action=set_test, data="sprite")
-            pe.button.rect((200, 250, 100, 50), pe.colors.white, pe.colors.lightgray, bt['mapping'], action=set_test, data="mapping")
-            pe.button.rect((300, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['shapes'], action=set_test, data="shapes")
-            pe.button.rect((400, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math'], action=set_test, data="math")
+            pe.button.rect((0, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['button'], action=set_test,
+                           data="button")
+            pe.button.rect((100, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['slider'], action=set_test,
+                           data="slider", disabled=pe.colors.gray)
+            pe.button.rect((200, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['sprite'], action=set_test,
+                           data="sprite")
+            pe.button.rect((200, 250, 100, 50), pe.colors.white, pe.colors.lightgray, bt['mapping'], action=set_test,
+                           data="mapping")
+            pe.button.rect((300, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['shapes'], action=set_test,
+                           data="shapes")
+            pe.button.rect((400, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math'], action=set_test,
+                           data="math")
 
             settings.recording = False
             mouse_icon.display((350, 440))
             bt['debug_label'].display()
             settings.recording = True
 
         elif test == "math":
-            pe.button.rect((0, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math_lerp'], action=set_test, data="math_lerp")
-            pe.button.rect((100, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math_center'], action=set_test, data="math_center")
-            pe.button.rect((200, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math_dist'], action=set_test, data="math_dist")
+            pe.button.rect((0, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math_lerp'], action=set_test,
+                           data="math_lerp")
+            pe.button.rect((100, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math_center'],
+                           action=set_test, data="math_center")
+            pe.button.rect((200, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math_dist'], action=set_test,
+                           data="math_dist")
+            pe.button.rect((300, 200, 100, 50), pe.colors.white, pe.colors.lightgray, bt['math_tsx'], action=set_test,
+                           data="math_tsx")
         if test != "":
             if "math_" in test:
-                pe.button.rect((0, 0, 100, 50), pe.colors.verydarkgray, pe.colors.darkgray, bt['math_back'], action=set_test, data="math")
+                pe.button.rect((0, 0, 100, 50), pe.colors.verydarkgray, pe.colors.darkgray, bt['math_back'],
+                               action=set_test, data="math")
             elif test == "testall":
                 pass
             else:
                 pass
-                pe.button.rect((0, 0, 100, 50), pe.colors.white, pe.colors.lightgray, bt['back'], action=set_test, data="")
+                pe.button.rect((0, 0, 100, 50), pe.colors.white, pe.colors.lightgray, bt['back'], action=set_test,
+                               data="")
             #
 
         if test == "math_lerp":
             if pe.display.get_width() < 325 or pe.display.get_height() < 250:
                 x, y = 0, 0
                 s = pe.display.get_size()
-                while s[0]+x < 325 or s[1]+y < 250:
-                    if s[0]+x < 325:
+                while s[0] + x < 325 or s[1] + y < 250:
+                    if s[0] + x < 325:
                         x += 1
-                    if s[1]+y < 250:
+                    if s[1] + y < 250:
                         y += 1
-                pe.display.make((s[0]+x, s[1]+y), "PGE Testing Utility", 1)
-            pe.button.rect((175, 200, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['-'], set_lerplength, lerplength-.1)
+                pe.display.make((s[0] + x, s[1] + y), "PGE Testing Utility", 1)
+            pe.button.rect((175, 200, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['-'], set_lerplength,
+                           lerplength - .1)
             bt['lerplength'].text = f'{lerplength:.1f}'
             bt['lerplength'].init()
             bt['lerplength'].display()
-            pe.button.rect((275, 200, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['+'], set_lerplength, lerplength+.1)
+            pe.button.rect((275, 200, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['+'], set_lerplength,
+                           lerplength + .1)
             mp = pe.mouse.pos()
             lerp1 = pe.math.lerp((0, 0), mp, lerplength)
             lerp2 = pe.math.lerp((pe.display.get_width(), 0), mp, lerplength)
             lerp3 = pe.math.lerp((0, pe.display.get_height()), mp, lerplength)
             lerp4 = pe.math.lerp(pe.display.get_size(), mp, lerplength)
 
             lerp1max = pe.math.lerp((0, 0), mp, min(1, lerplength))
@@ -242,22 +290,46 @@
             pe.draw.line(pe.colors.pink, (0, pe.display.get_height()), lerp3, 3)
             pe.draw.line(pe.colors.pink, (pe.display.get_width(), pe.display.get_height()), lerp4, 3)
 
             pe.draw.line(pe.colors.white, (0, 0), lerp1max, 5)
             pe.draw.line(pe.colors.white, (pe.display.get_width(), 0), lerp2max, 5)
             pe.draw.line(pe.colors.white, (0, pe.display.get_height()), lerp3max, 5)
             pe.draw.line(pe.colors.white, (pe.display.get_width(), pe.display.get_height()), lerp4max, 5)
-
         elif test == "math_center":
-            pe.draw.circle(pe.colors.white, pe.math.center((0, 0, pe.display.get_width(), pe.display.get_height())), 5, 5)
+            pe.draw.circle(pe.colors.white, pe.math.center((0, 0, pe.display.get_width(), pe.display.get_height())), 5,
+                           5)
         elif test == "math_dist":
             pe.draw.line(pe.colors.red, (0, 0), pe.mouse.pos(), 2)
-            bt['lerplength'].text = f'{pe.math.dist((0, 0), pe.mouse.pos()):.3f}'
-            bt['lerplength'].init()
-            bt['lerplength'].display()
+            bt['distance'].text = f'{pe.math.dist((0, 0), pe.mouse.pos()):.3f}'
+            bt['distance'].init()
+            bt['distance'].display()
+        elif test == "math_tsx":
+            pe.button.rect((100, 145, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['-'], set_tsx_radius,
+                           tsx.radius - .3)
+            pe.button.rect((100, 200, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['-'], set_tsx_segments,
+                           max(2, tsx_segments - .1))
+            pe.button.rect((100, 255, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['-'], set_tsx_offset,
+                           tsx.offset - 1)
+            bt['tsx_radius'].text = f'radius {tsx.radius:.1f}'
+            bt['tsx_radius'].init()
+            bt['tsx_radius'].display()
+            bt['tsx_segments'].text = f'segments {int(tsx_segments)}'
+            bt['tsx_segments'].init()
+            bt['tsx_segments'].display()
+            bt['tsx_offset'].text = f'rotation offset {tsx.offset:.1f}'
+            bt['tsx_offset'].init()
+            bt['tsx_offset'].display()
+            pe.button.rect((350, 145, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['+'], set_tsx_radius,
+                           tsx.radius + .3)
+            pe.button.rect((350, 200, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['+'], set_tsx_segments,
+                           min(360, tsx_segments + .1))
+            pe.button.rect((350, 255, 50, 50), pe.colors.gray, pe.colors.darkgray, bt['+'], set_tsx_offset,
+                           tsx.offset + 1)
+            gen = (tsx[rotation] for rotation in range(0, 360, max(360 // int(tsx_segments), 1)))
+            pe.draw.polygon(pe.colors.red, list(gen), 2)
         log.render()
         pe.display.update(120)
         pe.stop_recording()
         if pe.mouse.clicked()[2]:
             pe.start_debug()
```

### Comparing `pygameextra-2.0.0b9/pygameextra_tester/columns.png` & `pygameextra-2.0.0rc1/pygameextra_tester/columns.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra_tester/debug_icon.png` & `pygameextra-2.0.0rc1/pygameextra_tester/debug_icon.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/pygameextra_tester/mouse_middle.png` & `pygameextra-2.0.0rc1/pygameextra_tester/mouse_middle.png`

 * *Files identical despite different names*

### Comparing `pygameextra-2.0.0b9/setup.py` & `pygameextra-2.0.0rc1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '2.0.0b9'
+version = '2.0.0rc1'
 short = 'Pygame. Made easier.'
 long = '''Pygame Extra is a mask for pygame, 
 you can easily make complex games and or apps with much less lines then you would of before, 
 Pygame Extra makes coding easier. 
 
 The online documentation can be found at: https://pygame-extra.readthedocs.io/en/latest/
 
@@ -16,15 +16,15 @@
     version=version,
     author="Red",
     author_email="redtonehair@gmail.com",
     description=short,
     long_description_content_type="text/markdown",
     long_description=long,
     packages=['pygameextra', 'pygameextra_tester'],
-    install_requires=['pygame', 'perlin-noise'],
+    install_requires=['pygame', 'numpy'],
     package_data={'pygameextra': ['font.ttf'], 'pygameextra_tester': [
         'columns.png', 'rows.png',
         'Xbutton.png', 'Ybutton.png',
         'mario_01.png',
         'debug_icon.png', 'mouse_middle.png'
     ]},
     keywords=['python'],
```

