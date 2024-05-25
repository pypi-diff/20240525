# Comparing `tmp/g910_gkeys-0.4.1.tar.gz` & `tmp/g910_gkeys-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g910_gkeys-0.4.1.tar", last modified: Sat May 25 19:09:29 2024, max compression
+gzip compressed data, was "g910_gkeys-0.4.2.tar", last modified: Sat May 25 19:22:54 2024, max compression
```

## Comparing `g910_gkeys-0.4.1.tar` & `g910_gkeys-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:09:29.393764 g910_gkeys-0.4.1/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    35147 2022-10-18 18:43:19.000000 g910_gkeys-0.4.1/LICENSE
--rw-r--r--   0 marcel    (1000) marcel    (1000)    50224 2024-05-25 19:09:29.393764 g910_gkeys-0.4.1/PKG-INFO
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     8702 2024-05-25 18:58:57.000000 g910_gkeys-0.4.1/README.md
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:09:29.389763 g910_gkeys-0.4.1/g910_gkeys/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/__init__.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:09:29.389763 g910_gkeys-0.4.1/g910_gkeys/data_mappers/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/data_mappers/__init__.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     7166 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/data_mappers/bytearrays.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    23223 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/data_mappers/char_uinput_mapper.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      333 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/data_mappers/supported_configs.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    15071 2024-05-25 18:58:57.000000 g910_gkeys-0.4.1/g910_gkeys/data_mappers/supported_devices.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     9988 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/data_mappers/uinput_all_keys.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     5927 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/g910_gkeys.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)    12936 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/layout_config_helpers.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:09:29.389763 g910_gkeys-0.4.1/g910_gkeys/lib/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/lib/__init__.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     6086 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/lib/keyboard.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     4678 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/lib/usb_device.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:09:29.393764 g910_gkeys-0.4.1/g910_gkeys/misc/
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/misc/__init__.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     8829 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/misc/config.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      929 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/misc/helper.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1755 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/misc/logger.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      867 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/misc/memory_leds.py
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      702 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/g910_gkeys/misc/notify.py
-drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:09:29.393764 g910_gkeys-0.4.1/g910_gkeys.egg-info/
--rw-r--r--   0 marcel    (1000) marcel    (1000)    50224 2024-05-25 19:09:29.000000 g910_gkeys-0.4.1/g910_gkeys.egg-info/PKG-INFO
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      830 2024-05-25 19:09:29.000000 g910_gkeys-0.4.1/g910_gkeys.egg-info/SOURCES.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2024-05-25 19:09:29.000000 g910_gkeys-0.4.1/g910_gkeys.egg-info/dependency_links.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)       58 2024-05-25 19:09:29.000000 g910_gkeys-0.4.1/g910_gkeys.egg-info/entry_points.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)       35 2024-05-25 19:09:29.000000 g910_gkeys-0.4.1/g910_gkeys.egg-info/requires.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)       11 2024-05-25 19:09:29.000000 g910_gkeys-0.4.1/g910_gkeys.egg-info/top_level.txt
--rw-rw-r--   0 marcel    (1000) marcel    (1000)     1311 2024-05-25 18:58:57.000000 g910_gkeys-0.4.1/pyproject.toml
--rw-rw-r--   0 marcel    (1000) marcel    (1000)       38 2024-05-25 19:09:29.393764 g910_gkeys-0.4.1/setup.cfg
--rw-rw-r--   0 marcel    (1000) marcel    (1000)      112 2023-09-17 08:35:57.000000 g910_gkeys-0.4.1/setup.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:22:54.833632 g910_gkeys-0.4.2/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    35147 2022-10-18 18:43:19.000000 g910_gkeys-0.4.2/LICENSE
+-rw-r--r--   0 marcel    (1000) marcel    (1000)    50224 2024-05-25 19:22:54.833632 g910_gkeys-0.4.2/PKG-INFO
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     8702 2024-05-25 19:10:38.000000 g910_gkeys-0.4.2/README.md
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:22:54.829632 g910_gkeys-0.4.2/g910_gkeys/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/__init__.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:22:54.829632 g910_gkeys-0.4.2/g910_gkeys/data_mappers/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/data_mappers/__init__.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     7166 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/data_mappers/bytearrays.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    23223 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/data_mappers/char_uinput_mapper.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      333 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/data_mappers/supported_configs.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    15111 2024-05-25 19:10:38.000000 g910_gkeys-0.4.2/g910_gkeys/data_mappers/supported_devices.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     9988 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/data_mappers/uinput_all_keys.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     5927 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/g910_gkeys.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)    12936 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/layout_config_helpers.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:22:54.829632 g910_gkeys-0.4.2/g910_gkeys/lib/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/lib/__init__.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     6086 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/lib/keyboard.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     4678 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/lib/usb_device.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:22:54.829632 g910_gkeys-0.4.2/g910_gkeys/misc/
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        0 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/misc/__init__.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     8829 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/misc/config.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      929 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/misc/helper.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1755 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/misc/logger.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      867 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/misc/memory_leds.py
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      702 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/g910_gkeys/misc/notify.py
+drwxrwxr-x   0 marcel    (1000) marcel    (1000)        0 2024-05-25 19:22:54.829632 g910_gkeys-0.4.2/g910_gkeys.egg-info/
+-rw-r--r--   0 marcel    (1000) marcel    (1000)    50224 2024-05-25 19:22:54.000000 g910_gkeys-0.4.2/g910_gkeys.egg-info/PKG-INFO
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      830 2024-05-25 19:22:54.000000 g910_gkeys-0.4.2/g910_gkeys.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)        1 2024-05-25 19:22:54.000000 g910_gkeys-0.4.2/g910_gkeys.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       58 2024-05-25 19:22:54.000000 g910_gkeys-0.4.2/g910_gkeys.egg-info/entry_points.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       35 2024-05-25 19:22:54.000000 g910_gkeys-0.4.2/g910_gkeys.egg-info/requires.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       11 2024-05-25 19:22:54.000000 g910_gkeys-0.4.2/g910_gkeys.egg-info/top_level.txt
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)     1311 2024-05-25 19:10:38.000000 g910_gkeys-0.4.2/pyproject.toml
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)       38 2024-05-25 19:22:54.833632 g910_gkeys-0.4.2/setup.cfg
+-rw-rw-r--   0 marcel    (1000) marcel    (1000)      112 2023-09-17 08:35:57.000000 g910_gkeys-0.4.2/setup.py
```

### Comparing `g910_gkeys-0.4.1/LICENSE` & `g910_gkeys-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/PKG-INFO` & `g910_gkeys-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g910-gkeys
-Version: 0.4.1
+Version: 0.4.2
 Summary: Support for Logitech G910 GKeys on GNU/Linux
 Author-email: Jan Šubelj <jan.subelj010@gmail.com>, Marcel Grolms <support@suabo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,15 +691,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-uinput==0.11.2
 Requires-Dist: pyusb==1.2.1
 
-# Logitech G910 keyboard gkey support for GNU/Linux (Project version: v0.4.1)
+# Logitech G910 keyboard gkey support for GNU/Linux (Project version: v0.4.2)
 Because I didn't find any GKey support for Logitech G910 keyboard I decided to create this GKey mapper.
 Code is based on an [issue](https://github.com/CReimer/g910-gkey-uinput/issues/3)
 in [g910-gkey-uinput](https://github.com/CReimer/g910-gkey-uinput) project. I expanded the code, so that it is more 
 user-friendly to add functionality to GKeys.
 
 Everything is described in great depth (and actually much better) on [WIKI](https://github.com/JSubelj/g910-gkey-macro-support/wiki).
```

### Comparing `g910_gkeys-0.4.1/README.md` & `g910_gkeys-0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Logitech G910 keyboard gkey support for GNU/Linux (Project version: v0.4.1)
+# Logitech G910 keyboard gkey support for GNU/Linux (Project version: v0.4.2)
 Because I didn't find any GKey support for Logitech G910 keyboard I decided to create this GKey mapper.
 Code is based on an [issue](https://github.com/CReimer/g910-gkey-uinput/issues/3)
 in [g910-gkey-uinput](https://github.com/CReimer/g910-gkey-uinput) project. I expanded the code, so that it is more 
 user-friendly to add functionality to GKeys.
 
 Everything is described in great depth (and actually much better) on [WIKI](https://github.com/JSubelj/g910-gkey-macro-support/wiki).
```

### Comparing `g910_gkeys-0.4.1/g910_gkeys/data_mappers/bytearrays.py` & `g910_gkeys-0.4.2/g910_gkeys/data_mappers/bytearrays.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/data_mappers/char_uinput_mapper.py` & `g910_gkeys-0.4.2/g910_gkeys/data_mappers/char_uinput_mapper.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/data_mappers/supported_devices.py` & `g910_gkeys-0.4.2/g910_gkeys/data_mappers/supported_devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,17 @@
             b'\x11\xff\x0a\x0e\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00',
             b'\x11\xff\x0a\x0e\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00',
         ]
     }
 
     mediaKeys = {
         b'\x02\x08': "KEY_PLAYPAUSE",
-        b'\x02\x04': "KEY_STOP",
-        b'\x02\x02': "KEY_PREVIOUS",
-        b'\x02\x01': "KEY_NEXT",
+        b'\x02\x04': "KEY_STOPCD",
+        b'\x02\x02': "KEY_PREVIOUSSONG",
+        b'\x02\x01': "KEY_NEXTSONG",
         b'\x02\x40': "KEY_MUTE",
         b'\x02\x10': "KEY_VOLUMEUP",
         b'\x02\x20': "KEY_VOLUMEDOWN"
     }
 
     releaseEvents = {
         b'\x11\xff\x08\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00': 'MACRO_RELEASE',
@@ -111,17 +111,17 @@
         "MEMORY_1": b'\x11\xff\x0b\x1a\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00',  # M1 LED
         "MEMORY_2": b'\x11\xff\x0b\x1a\x02\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00',  # M2 LED
         "MEMORY_3": b'\x11\xff\x0b\x1a\x04\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'   # M3 LED
     }
 
     mediaKeys = {
         b'\x03\x08': "KEY_PLAYPAUSE",
-        b'\x03\x04': "KEY_STOP",
-        b'\x03\x02': "KEY_PREVIOUS",
-        b'\x03\x01': "KEY_NEXT",
+        b'\x03\x04': "KEY_STOPCD",
+        b'\x03\x02': "KEY_PREVIOUSSONG",
+        b'\x03\x01': "KEY_NEXTSONG",
         b'\x03\x10': "KEY_VOLUMEUP",
         b'\x03\x20': "KEY_VOLUMEDOWN",
         b'\x03\x40': "KEY_MUTE"
     }
 
     releaseEvents = {
         'KEY_G': b'\x11\xff\x0a\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00',      # G release
@@ -204,17 +204,17 @@
         "MEMORY_1": b'\x06\x10',  # M1 LED
         "MEMORY_2": b'\x06\x20',  # M2 LED
         "MEMORY_3": b'\x06\x40'   # M3 LED
     }
 
     mediaKeys = {
         b'\x02\x08': "KEY_PLAYPAUSE",
-        b'\x02\x04': "KEY_STOP",
-        b'\x02\x02': "KEY_PREVIOUS",
-        b'\x02\x01': "KEY_NEXT",
+        b'\x02\x04': "KEY_STOPCD",
+        b'\x02\x02': "KEY_PREVIOUSSONG",
+        b'\x02\x01': "KEY_NEXTSONG",
         b'\x02\x40': "KEY_MUTE",
         b'\x02\x10': "KEY_VOLUMEUP",
         b'\x02\x20': "KEY_VOLUMEDOWN"
     }
 
     releaseEvents = {
         'KEY_G': b'\x03\x00\x00\x00',    # G release
@@ -254,17 +254,17 @@
         b'\x03\x00\x00\x10\x00': "MEMORY_1",
         b'\x03\x00\x00\x20\x00': "MEMORY_2",
         b'\x03\x00\x00\x40\x00': "MEMORY_3"
     }
 
     mediaKeys = {
         b'\x02\x08': "KEY_PLAYPAUSE",
-        b'\x02\x04': "KEY_STOP",
-        b'\x02\x02': "KEY_PREVIOUS",
-        b'\x02\x01': "KEY_NEXT",
+        b'\x02\x04': "KEY_STOPCD",
+        b'\x02\x02': "KEY_PREVIOUSSONG",
+        b'\x02\x01': "KEY_NEXTSONG",
         b'\x02\x10': "KEY_MUTE",  # not 100% sure about those last 3
         b'\x02\x20': "KEY_VOLUMEDOWN",
         b'\x02\x40': "KEY_VOLUMEUP"
     }
 
     releaseEvents = {
         'KEY_G': b'\x03\x00\x00\x00\x00',   # M and G release
```

### Comparing `g910_gkeys-0.4.1/g910_gkeys/data_mappers/uinput_all_keys.py` & `g910_gkeys-0.4.2/g910_gkeys/data_mappers/uinput_all_keys.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/g910_gkeys.py` & `g910_gkeys-0.4.2/g910_gkeys/g910_gkeys.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/layout_config_helpers.py` & `g910_gkeys-0.4.2/g910_gkeys/layout_config_helpers.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/lib/keyboard.py` & `g910_gkeys-0.4.2/g910_gkeys/lib/keyboard.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/lib/usb_device.py` & `g910_gkeys-0.4.2/g910_gkeys/lib/usb_device.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/misc/config.py` & `g910_gkeys-0.4.2/g910_gkeys/misc/config.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/misc/helper.py` & `g910_gkeys-0.4.2/g910_gkeys/misc/helper.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/misc/logger.py` & `g910_gkeys-0.4.2/g910_gkeys/misc/logger.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/misc/memory_leds.py` & `g910_gkeys-0.4.2/g910_gkeys/misc/memory_leds.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys/misc/notify.py` & `g910_gkeys-0.4.2/g910_gkeys/misc/notify.py`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/g910_gkeys.egg-info/PKG-INFO` & `g910_gkeys-0.4.2/g910_gkeys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g910-gkeys
-Version: 0.4.1
+Version: 0.4.2
 Summary: Support for Logitech G910 GKeys on GNU/Linux
 Author-email: Jan Šubelj <jan.subelj010@gmail.com>, Marcel Grolms <support@suabo.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,15 +691,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-uinput==0.11.2
 Requires-Dist: pyusb==1.2.1
 
-# Logitech G910 keyboard gkey support for GNU/Linux (Project version: v0.4.1)
+# Logitech G910 keyboard gkey support for GNU/Linux (Project version: v0.4.2)
 Because I didn't find any GKey support for Logitech G910 keyboard I decided to create this GKey mapper.
 Code is based on an [issue](https://github.com/CReimer/g910-gkey-uinput/issues/3)
 in [g910-gkey-uinput](https://github.com/CReimer/g910-gkey-uinput) project. I expanded the code, so that it is more 
 user-friendly to add functionality to GKeys.
 
 Everything is described in great depth (and actually much better) on [WIKI](https://github.com/JSubelj/g910-gkey-macro-support/wiki).
```

### Comparing `g910_gkeys-0.4.1/g910_gkeys.egg-info/SOURCES.txt` & `g910_gkeys-0.4.2/g910_gkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g910_gkeys-0.4.1/pyproject.toml` & `g910_gkeys-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "g910-gkeys"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
     { name="Jan Šubelj", email="jan.subelj010@gmail.com" },
     { name="Marcel Grolms", email="support@suabo.de" }
 ]
 description = "Support for Logitech G910 GKeys on GNU/Linux"
 keywords = ["logitech", "keyboard", "gkey", "G910", "G915", "G815", "G710", "G510"]
 readme = "README.md"
```

