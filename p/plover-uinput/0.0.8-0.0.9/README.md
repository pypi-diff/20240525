# Comparing `tmp/plover_uinput-0.0.8.tar.gz` & `tmp/plover_uinput-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover_uinput-0.0.8.tar", last modified: Mon May 20 18:15:48 2024, max compression
+gzip compressed data, was "plover_uinput-0.0.9.tar", last modified: Tue May 21 10:51:22 2024, max compression
```

## Comparing `plover_uinput-0.0.8.tar` & `plover_uinput-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 18:15:48.063193 plover_uinput-0.0.8/
--rw-r--r--   0 olai      (1000) users      (100)     1053 2024-05-20 16:28:07.000000 plover_uinput-0.0.8/LICENSE
--rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 18:15:48.063193 plover_uinput-0.0.8/PKG-INFO
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 18:15:48.062193 plover_uinput-0.0.8/plover_uinput/
--rw-r--r--   0 olai      (1000) users      (100)     9544 2024-05-20 18:13:58.000000 plover_uinput-0.0.8/plover_uinput/__init__.py
--rw-r--r--   0 olai      (1000) users      (100)      130 2024-05-20 16:28:07.000000 plover_uinput-0.0.8/plover_uinput/all_keys.py
--rw-r--r--   0 olai      (1000) users      (100)    10000 2024-05-20 16:28:07.000000 plover_uinput-0.0.8/plover_uinput/keys.py
--rw-r--r--   0 olai      (1000) users      (100)     2019 2024-05-20 16:28:07.000000 plover_uinput-0.0.8/plover_uinput/symbols.py
-drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-20 18:15:48.063193 plover_uinput-0.0.8/plover_uinput.egg-info/
--rw-r--r--   0 olai      (1000) users      (100)     2458 2024-05-20 18:15:48.000000 plover_uinput-0.0.8/plover_uinput.egg-info/PKG-INFO
--rw-r--r--   0 olai      (1000) users      (100)      374 2024-05-20 18:15:48.000000 plover_uinput-0.0.8/plover_uinput.egg-info/SOURCES.txt
--rw-r--r--   0 olai      (1000) users      (100)        1 2024-05-20 18:15:48.000000 plover_uinput-0.0.8/plover_uinput.egg-info/dependency_links.txt
--rw-r--r--   0 olai      (1000) users      (100)      119 2024-05-20 18:15:48.000000 plover_uinput-0.0.8/plover_uinput.egg-info/entry_points.txt
--rw-r--r--   0 olai      (1000) users      (100)       45 2024-05-20 18:15:48.000000 plover_uinput-0.0.8/plover_uinput.egg-info/requires.txt
--rw-r--r--   0 olai      (1000) users      (100)       14 2024-05-20 18:15:48.000000 plover_uinput-0.0.8/plover_uinput.egg-info/top_level.txt
--rw-r--r--   0 olai      (1000) users      (100)       89 2024-05-20 16:28:07.000000 plover_uinput-0.0.8/pyproject.toml
--rw-r--r--   0 olai      (1000) users      (100)      993 2024-05-20 16:58:01.000000 plover_uinput-0.0.8/readme.md
--rw-r--r--   0 olai      (1000) users      (100)      670 2024-05-20 18:15:48.063193 plover_uinput-0.0.8/setup.cfg
--rw-r--r--   0 olai      (1000) users      (100)       62 2024-05-20 16:28:07.000000 plover_uinput-0.0.8/setup.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-21 10:51:21.999084 plover_uinput-0.0.9/
+-rw-r--r--   0 olai      (1000) users      (100)     1053 2024-05-20 16:28:07.000000 plover_uinput-0.0.9/LICENSE
+-rw-r--r--   0 olai      (1000) users      (100)     2460 2024-05-21 10:51:21.999084 plover_uinput-0.0.9/PKG-INFO
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-21 10:51:21.998084 plover_uinput-0.0.9/plover_uinput/
+-rw-r--r--   0 olai      (1000) users      (100)     9886 2024-05-21 10:51:13.000000 plover_uinput-0.0.9/plover_uinput/__init__.py
+-rw-r--r--   0 olai      (1000) users      (100)      130 2024-05-20 16:28:07.000000 plover_uinput-0.0.9/plover_uinput/all_keys.py
+-rw-r--r--   0 olai      (1000) users      (100)    10000 2024-05-20 16:28:07.000000 plover_uinput-0.0.9/plover_uinput/keys.py
+-rw-r--r--   0 olai      (1000) users      (100)     1936 2024-05-21 10:47:18.000000 plover_uinput-0.0.9/plover_uinput/symbols.py
+drwxr-xr-x   0 olai      (1000) users      (100)        0 2024-05-21 10:51:21.999084 plover_uinput-0.0.9/plover_uinput.egg-info/
+-rw-r--r--   0 olai      (1000) users      (100)     2460 2024-05-21 10:51:21.000000 plover_uinput-0.0.9/plover_uinput.egg-info/PKG-INFO
+-rw-r--r--   0 olai      (1000) users      (100)      374 2024-05-21 10:51:21.000000 plover_uinput-0.0.9/plover_uinput.egg-info/SOURCES.txt
+-rw-r--r--   0 olai      (1000) users      (100)        1 2024-05-21 10:51:21.000000 plover_uinput-0.0.9/plover_uinput.egg-info/dependency_links.txt
+-rw-r--r--   0 olai      (1000) users      (100)      119 2024-05-21 10:51:21.000000 plover_uinput-0.0.9/plover_uinput.egg-info/entry_points.txt
+-rw-r--r--   0 olai      (1000) users      (100)       45 2024-05-21 10:51:21.000000 plover_uinput-0.0.9/plover_uinput.egg-info/requires.txt
+-rw-r--r--   0 olai      (1000) users      (100)       14 2024-05-21 10:51:21.000000 plover_uinput-0.0.9/plover_uinput.egg-info/top_level.txt
+-rw-r--r--   0 olai      (1000) users      (100)       89 2024-05-20 16:28:07.000000 plover_uinput-0.0.9/pyproject.toml
+-rw-r--r--   0 olai      (1000) users      (100)      993 2024-05-20 16:58:01.000000 plover_uinput-0.0.9/readme.md
+-rw-r--r--   0 olai      (1000) users      (100)      672 2024-05-21 10:51:21.999084 plover_uinput-0.0.9/setup.cfg
+-rw-r--r--   0 olai      (1000) users      (100)       62 2024-05-20 16:28:07.000000 plover_uinput-0.0.9/setup.py
```

### Comparing `plover_uinput-0.0.8/LICENSE` & `plover_uinput-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.8/PKG-INFO` & `plover_uinput-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.8
+Version: 0.0.9
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
-Requires-Python: >=3.11
+Requires-Python: >=3.9.18
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover>=4.0.0rc2
 Requires-Dist: evdev>=1.7.0
 Requires-Dist: xkbcommon>=0.8
 
 # Plover output plugin for linux using uinput
```

### Comparing `plover_uinput-0.0.8/plover_uinput/__init__.py` & `plover_uinput-0.0.9/plover_uinput/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+# Notes for building and deploying:
+# `python3 -m build` REMEMBER TO CHANGE VERSION NUMBER FIRST
+# `twine upload dist/*`
+
 from evdev import UInput, ecodes as e, util
 
 from .symbols import generate_symbols
 from time import sleep
 
 from plover.oslayer.keyboardcontrol import KeyboardEmulation as OldKeyboardEmulation
 from plover import log
 import os  # To read the layout variable
 
-# If keys has character then send_key key with no modifiers (the function should have a string input, that gets split into a list and read from the mods dictionary)
-# Else if symbols has character then send_key base_key with modifiers from the symbols dictionary generated
-# Else, input unicode
-
 # === Import or create `parse_key_combo` function ===
 try:
     from plover.key_combo import parse_key_combo
 except ImportError:
     log.warning("With new KeyCombo interface")
     from plover.key_combo import KeyCombo
 
@@ -175,14 +175,30 @@
     "Eject": e.KEY_EJECTCD,
     "AudioPause": e.KEY_PAUSE,
     "AudioPlay": e.KEY_PLAY,
     "AudioNext": e.KEY_NEXT,  # Maybe VIDEO_NEXT or NEXTSONG
     "AudioRewind": e.KEY_REWIND,
     "KbdBrightnessUp": e.KEY_KBDILLUMUP,
     "KbdBrightnessDown": e.KEY_KBDILLUMDOWN,
+    # Different cased duplicates may be unnecessary
+    # Possible solution if it causes errors: use lowercase string when getting keycodes from here
+    "BackSpace": e.KEY_BACKSPACE,
+    "Delete": e.KEY_DELETE,
+    "Up": e.KEY_UP,
+    "Down": e.KEY_DOWN,
+    "Left": e.KEY_LEFT,
+    "Right": e.KEY_RIGHT,
+    "Home": e.KEY_HOME,
+    "Insert": e.KEY_INSERT,
+    "End": e.KEY_END,
+    "Tab": e.KEY_TAB,
+    "Page_Up": e.KEY_PAGEUP,
+    "Page_Down": e.KEY_PAGEDOWN,
+    "Space": e.KEY_SPACE,
+    "space": e.KEY_SPACE,
 }
 
 
 class KeyboardEmulation(*([KeyboardEmulationBase] if have_output_plugin else [])):
     @classmethod
     def get_option_info(cls):
         return {}
```

### Comparing `plover_uinput-0.0.8/plover_uinput/keys.py` & `plover_uinput-0.0.9/plover_uinput/keys.py`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.8/plover_uinput/symbols.py` & `plover_uinput-0.0.9/plover_uinput/symbols.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from xkbcommon import xkb
 
 
-# TODO: allow the layout to be defined by the user (environment variable? or gui?)
 # layout can be "no", "us", "gb", "fr" or any other xkb layout
-def generate_symbols(layout="no"):
+def generate_symbols(layout="us"):
     ctx = xkb.Context()
     keymap = ctx.keymap_new_from_names(layout=layout)
     # The keymaps have to be "translated" to a US layout keyboard for evdev
     keymap_us = ctx.keymap_new_from_names(layout="us")
 
     # Modifier names from xkb, converted to strings
     level_mapping = {
```

### Comparing `plover_uinput-0.0.8/plover_uinput.egg-info/PKG-INFO` & `plover_uinput-0.0.9/plover_uinput.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: plover-uinput
-Version: 0.0.8
+Version: 0.0.9
 Summary: Plover output plugin for linux using evdev / uinput
 Home-page: https://github.com/LilleAila/plover-uinput
 Author: LilleAila
 License: MIT
 Keywords: plover plover_plugin
-Requires-Python: >=3.11
+Requires-Python: >=3.9.18
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: plover>=4.0.0rc2
 Requires-Dist: evdev>=1.7.0
 Requires-Dist: xkbcommon>=0.8
 
 # Plover output plugin for linux using uinput
```

### Comparing `plover_uinput-0.0.8/readme.md` & `plover_uinput-0.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `plover_uinput-0.0.8/setup.cfg` & `plover_uinput-0.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-uinput
-version = 0.0.8
+version = 0.0.9
 author = LilleAila
 description = Plover output plugin for linux using evdev / uinput
 long_description = file: readme.md, LICENSE
 long_description_content_type = text/markdown
 license = MIT
 url = https://github.com/LilleAila/plover-uinput
 keywords = plover plover_plugin
@@ -12,15 +12,15 @@
 [options]
 setup_requires = 
 	setuptools>=69.1.1
 install_requires = 
 	plover>=4.0.0rc2
 	evdev>=1.7.0
 	xkbcommon>=0.8
-python_requires = >=3.11
+python_requires = >=3.9.18
 packages = plover_uinput
 
 [options.entry_points]
 plover.extension = 
 	plover_uinput = plover_uinput:Main
 plover.output = 
 	plover_uinput = plover_uinput:KeyboardEmulation
```

