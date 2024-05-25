# Comparing `tmp/drawlib-0.1.8.tar.gz` & `tmp/drawlib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawlib-0.1.8.tar", max compression
+gzip compressed data, was "drawlib-0.1.9.tar", max compression
```

## Comparing `drawlib-0.1.8.tar` & `drawlib-0.1.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.8/README.md
--rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.8/drawlib/.pylintrc
--rw-r--r--   0        0        0     1039 2024-05-21 14:46:50.727969 drawlib-0.1.8/drawlib/__init__.py
--rw-r--r--   0        0        0      688 2024-05-21 13:52:08.835136 drawlib-0.1.8/drawlib/__main__.py
--rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.8/drawlib/apis.py
--rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.8/drawlib/assets/__init__.py
--rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.8/drawlib/assets/v0_1/__init__.py
--rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.8/drawlib/assets/v0_1/fonticons/__init__.py
--rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.8/drawlib/assets/v0_1/fonts/__init__.py
--rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.8/drawlib/v0_1/__init__.py
--rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.8/drawlib/v0_1/__main__.py
--rw-r--r--   0        0        0     2438 2024-05-24 01:25:55.873169 drawlib-0.1.8/drawlib/v0_1/apis.py
--rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.8/drawlib/v0_1/private/__init__.py
--rw-r--r--   0        0        0    12860 2024-05-21 14:42:32.950675 drawlib-0.1.8/drawlib/v0_1/private/command.py
--rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.8/drawlib/v0_1/private/core/__init__.py
--rw-r--r--   0        0        0    12776 2024-05-22 11:20:38.275207 drawlib-0.1.8/drawlib/v0_1/private/core/colors.py
--rw-r--r--   0        0        0    13652 2024-05-24 15:37:46.743882 drawlib-0.1.8/drawlib/v0_1/private/core/dimage.py
--rw-r--r--   0        0        0    23777 2024-05-24 01:28:49.886237 drawlib-0.1.8/drawlib/v0_1/private/core/fonts.py
--rw-r--r--   0        0        0    33167 2024-05-24 01:28:33.651901 drawlib-0.1.8/drawlib/v0_1/private/core/model.py
--rw-r--r--   0        0        0    18865 2024-05-19 04:26:51.380337 drawlib-0.1.8/drawlib/v0_1/private/core/theme.py
--rw-r--r--   0        0        0    12976 2024-05-24 01:43:09.114237 drawlib-0.1.8/drawlib/v0_1/private/core/theme_officials.py
--rw-r--r--   0        0        0    51534 2024-05-17 08:42:26.352080 drawlib-0.1.8/drawlib/v0_1/private/core/theme_styles.py
--rw-r--r--   0        0        0    28300 2024-05-17 11:42:16.612394 drawlib-0.1.8/drawlib/v0_1/private/core/util.py
--rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/__init__.py
--rw-r--r--   0        0        0    15548 2024-05-24 01:29:18.823658 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/base.py
--rw-r--r--   0        0        0     7992 2024-05-17 04:55:01.315534 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/canvas.py
--rw-r--r--   0        0        0     5309 2024-05-24 16:33:38.203652 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/image.py
--rw-r--r--   0        0        0     6593 2024-05-17 04:01:22.784734 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/line.py
--rw-r--r--   0        0        0     4297 2024-05-17 04:01:28.386700 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_arrow.py
--rw-r--r--   0        0        0    12132 2024-05-17 12:08:03.060649 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_polygon.py
--rw-r--r--   0        0        0    16466 2024-05-17 04:01:43.093731 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/patches.py
--rw-r--r--   0        0        0     3264 2024-05-17 04:02:22.095588 drawlib-0.1.8/drawlib/v0_1/private/core_canvas/text.py
--rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.8/drawlib/v0_1/private/download.py
--rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.8/drawlib/v0_1/private/dutil.py
--rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.8/drawlib/v0_1/private/icons/__init__.py
--rw-r--r--   0        0        0   902368 2024-05-17 00:56:51.813460 drawlib-0.1.8/drawlib/v0_1/private/icons/phosphor.py
--rw-r--r--   0        0        0     1998 2024-05-17 04:04:01.158522 drawlib-0.1.8/drawlib/v0_1/private/icons/util.py
--rw-r--r--   0        0        0     1206 2024-05-21 13:50:52.977426 drawlib-0.1.8/drawlib/v0_1/private/logging.py
--rw-r--r--   0        0        0     6689 2024-05-21 13:34:20.888010 drawlib-0.1.8/drawlib/v0_1/private/settings.py
--rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.8/drawlib/v0_1/private/smartarts/__init__.py
--rw-r--r--   0        0        0     3482 2024-05-17 07:07:04.377539 drawlib-0.1.8/drawlib/v0_1/private/smartarts/bubblespeech.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.8/drawlib/v0_1/private/smartarts/cycle.py
--rw-r--r--   0        0        0      686 2024-05-17 01:14:56.535422 drawlib-0.1.8/drawlib/v0_1/private/smartarts/dsart.py
--rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.8/drawlib/v0_1/private/smartarts/groups.py
--rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.8/drawlib/v0_1/private/smartarts/pyramid.py
--rw-r--r--   0        0        0     5905 2024-05-17 01:19:04.280798 drawlib-0.1.8/drawlib/v0_1/private/smartarts/sourcecode.py
--rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.8/drawlib/v0_1/private/smartarts/table.py
--rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.8/drawlib/v0_1/private/smartarts/tree.py
--rw-r--r--   0        0        0    10163 2024-05-20 09:07:41.448465 drawlib-0.1.8/drawlib/v0_1/private/util.py
--rw-r--r--   0        0        0      407 2024-05-17 07:28:29.821380 drawlib-0.1.8/drawlib/v0_1/private/validators/__init__.py
--rw-r--r--   0        0        0     7382 2024-05-17 07:25:34.994200 drawlib-0.1.8/drawlib/v0_1/private/validators/args.py
--rw-r--r--   0        0        0     1576 2024-05-17 07:25:58.475653 drawlib-0.1.8/drawlib/v0_1/private/validators/color.py
--rw-r--r--   0        0        0     3275 2024-05-17 08:44:34.098244 drawlib-0.1.8/drawlib/v0_1/private/validators/coordinate.py
--rw-r--r--   0        0        0      891 2024-05-17 08:44:42.485495 drawlib-0.1.8/drawlib/v0_1/private/validators/image.py
--rw-r--r--   0        0        0     1249 2024-05-17 08:44:59.932902 drawlib-0.1.8/drawlib/v0_1/private/validators/line.py
--rw-r--r--   0        0        0     1332 2024-05-17 08:45:07.566582 drawlib-0.1.8/drawlib/v0_1/private/validators/shape.py
--rw-r--r--   0        0        0      660 2024-05-17 07:27:28.907431 drawlib-0.1.8/drawlib/v0_1/private/validators/smartarts.py
--rw-r--r--   0        0        0     2276 2024-05-17 08:45:25.563109 drawlib-0.1.8/drawlib/v0_1/private/validators/style.py
--rw-r--r--   0        0        0      824 2024-05-17 07:27:54.398157 drawlib-0.1.8/drawlib/v0_1/private/validators/text.py
--rw-r--r--   0        0        0     2270 2024-05-17 08:45:46.188412 drawlib-0.1.8/drawlib/v0_1/private/validators/types.py
--rw-r--r--   0        0        0      712 2024-05-24 16:35:25.217531 drawlib-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-04-05 18:42:05.538150 drawlib-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     2421 2024-05-04 15:36:12.546708 drawlib-0.1.9/README.md
+-rw-r--r--   0        0        0       27 2024-03-29 11:45:48.926601 drawlib-0.1.9/drawlib/.pylintrc
+-rw-r--r--   0        0        0     1039 2024-05-24 16:36:12.950348 drawlib-0.1.9/drawlib/__init__.py
+-rw-r--r--   0        0        0      688 2024-05-21 13:52:08.835136 drawlib-0.1.9/drawlib/__main__.py
+-rw-r--r--   0        0        0      777 2024-04-07 14:54:59.159171 drawlib-0.1.9/drawlib/apis.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:27:54.821931 drawlib-0.1.9/drawlib/assets/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-01 10:34:11.053352 drawlib-0.1.9/drawlib/assets/v0_1/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 07:28:01.917218 drawlib-0.1.9/drawlib/assets/v0_1/fonticons/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-13 15:48:11.439423 drawlib-0.1.9/drawlib/assets/v0_1/fonts/__init__.py
+-rw-r--r--   0        0        0     1084 2024-04-07 03:53:05.340986 drawlib-0.1.9/drawlib/v0_1/__init__.py
+-rw-r--r--   0        0        0      663 2024-04-06 12:40:11.972278 drawlib-0.1.9/drawlib/v0_1/__main__.py
+-rw-r--r--   0        0        0     2438 2024-05-24 01:25:55.873169 drawlib-0.1.9/drawlib/v0_1/apis.py
+-rw-r--r--   0        0        0      763 2024-04-06 11:52:52.776827 drawlib-0.1.9/drawlib/v0_1/private/__init__.py
+-rw-r--r--   0        0        0    12860 2024-05-21 14:42:32.950675 drawlib-0.1.9/drawlib/v0_1/private/command.py
+-rw-r--r--   0        0        0      548 2024-04-07 14:22:07.928062 drawlib-0.1.9/drawlib/v0_1/private/core/__init__.py
+-rw-r--r--   0        0        0    12776 2024-05-22 11:20:38.275207 drawlib-0.1.9/drawlib/v0_1/private/core/colors.py
+-rw-r--r--   0        0        0    13653 2024-05-24 16:43:28.601010 drawlib-0.1.9/drawlib/v0_1/private/core/dimage.py
+-rw-r--r--   0        0        0    23777 2024-05-24 01:28:49.886237 drawlib-0.1.9/drawlib/v0_1/private/core/fonts.py
+-rw-r--r--   0        0        0    33167 2024-05-24 01:28:33.651901 drawlib-0.1.9/drawlib/v0_1/private/core/model.py
+-rw-r--r--   0        0        0    18865 2024-05-19 04:26:51.380337 drawlib-0.1.9/drawlib/v0_1/private/core/theme.py
+-rw-r--r--   0        0        0    12976 2024-05-24 01:43:09.114237 drawlib-0.1.9/drawlib/v0_1/private/core/theme_officials.py
+-rw-r--r--   0        0        0    51534 2024-05-17 08:42:26.352080 drawlib-0.1.9/drawlib/v0_1/private/core/theme_styles.py
+-rw-r--r--   0        0        0    28300 2024-05-17 11:42:16.612394 drawlib-0.1.9/drawlib/v0_1/private/core/util.py
+-rw-r--r--   0        0        0      548 2024-04-27 02:06:25.820510 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/__init__.py
+-rw-r--r--   0        0        0    15548 2024-05-24 01:29:18.823658 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/base.py
+-rw-r--r--   0        0        0     7992 2024-05-17 04:55:01.315534 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/canvas.py
+-rw-r--r--   0        0        0     5310 2024-05-24 16:43:37.387790 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/image.py
+-rw-r--r--   0        0        0     6593 2024-05-17 04:01:22.784734 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/line.py
+-rw-r--r--   0        0        0     4297 2024-05-17 04:01:28.386700 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/original_arrow.py
+-rw-r--r--   0        0        0    12132 2024-05-17 12:08:03.060649 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/original_polygon.py
+-rw-r--r--   0        0        0    16466 2024-05-17 04:01:43.093731 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/patches.py
+-rw-r--r--   0        0        0     3264 2024-05-17 04:02:22.095588 drawlib-0.1.9/drawlib/v0_1/private/core_canvas/text.py
+-rw-r--r--   0        0        0     2067 2024-05-03 16:29:49.262484 drawlib-0.1.9/drawlib/v0_1/private/download.py
+-rw-r--r--   0        0        0      881 2024-05-02 13:00:20.440339 drawlib-0.1.9/drawlib/v0_1/private/dutil.py
+-rw-r--r--   0        0        0      589 2024-04-13 03:31:11.518478 drawlib-0.1.9/drawlib/v0_1/private/icons/__init__.py
+-rw-r--r--   0        0        0   902368 2024-05-17 00:56:51.813460 drawlib-0.1.9/drawlib/v0_1/private/icons/phosphor.py
+-rw-r--r--   0        0        0     1998 2024-05-17 04:04:01.158522 drawlib-0.1.9/drawlib/v0_1/private/icons/util.py
+-rw-r--r--   0        0        0     1206 2024-05-21 13:50:52.977426 drawlib-0.1.9/drawlib/v0_1/private/logging.py
+-rw-r--r--   0        0        0     6689 2024-05-21 13:34:20.888010 drawlib-0.1.9/drawlib/v0_1/private/settings.py
+-rw-r--r--   0        0        0      589 2024-04-25 02:41:30.472250 drawlib-0.1.9/drawlib/v0_1/private/smartarts/__init__.py
+-rw-r--r--   0        0        0     3482 2024-05-17 07:07:04.377539 drawlib-0.1.9/drawlib/v0_1/private/smartarts/bubblespeech.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:18.451455 drawlib-0.1.9/drawlib/v0_1/private/smartarts/cycle.py
+-rw-r--r--   0        0        0      686 2024-05-17 01:14:56.535422 drawlib-0.1.9/drawlib/v0_1/private/smartarts/dsart.py
+-rw-r--r--   0        0        0      660 2024-04-14 23:53:28.113177 drawlib-0.1.9/drawlib/v0_1/private/smartarts/groups.py
+-rw-r--r--   0        0        0      619 2024-04-14 23:53:33.993167 drawlib-0.1.9/drawlib/v0_1/private/smartarts/pyramid.py
+-rw-r--r--   0        0        0     5905 2024-05-17 01:19:04.280798 drawlib-0.1.9/drawlib/v0_1/private/smartarts/sourcecode.py
+-rw-r--r--   0        0        0      426 2024-04-14 23:53:43.397670 drawlib-0.1.9/drawlib/v0_1/private/smartarts/table.py
+-rw-r--r--   0        0        0      651 2024-04-14 23:53:50.199157 drawlib-0.1.9/drawlib/v0_1/private/smartarts/tree.py
+-rw-r--r--   0        0        0    10163 2024-05-20 09:07:41.448465 drawlib-0.1.9/drawlib/v0_1/private/util.py
+-rw-r--r--   0        0        0      407 2024-05-17 07:28:29.821380 drawlib-0.1.9/drawlib/v0_1/private/validators/__init__.py
+-rw-r--r--   0        0        0     7382 2024-05-17 07:25:34.994200 drawlib-0.1.9/drawlib/v0_1/private/validators/args.py
+-rw-r--r--   0        0        0     1576 2024-05-17 07:25:58.475653 drawlib-0.1.9/drawlib/v0_1/private/validators/color.py
+-rw-r--r--   0        0        0     3275 2024-05-17 08:44:34.098244 drawlib-0.1.9/drawlib/v0_1/private/validators/coordinate.py
+-rw-r--r--   0        0        0      891 2024-05-17 08:44:42.485495 drawlib-0.1.9/drawlib/v0_1/private/validators/image.py
+-rw-r--r--   0        0        0     1249 2024-05-17 08:44:59.932902 drawlib-0.1.9/drawlib/v0_1/private/validators/line.py
+-rw-r--r--   0        0        0     1332 2024-05-17 08:45:07.566582 drawlib-0.1.9/drawlib/v0_1/private/validators/shape.py
+-rw-r--r--   0        0        0      660 2024-05-17 07:27:28.907431 drawlib-0.1.9/drawlib/v0_1/private/validators/smartarts.py
+-rw-r--r--   0        0        0     2276 2024-05-17 08:45:25.563109 drawlib-0.1.9/drawlib/v0_1/private/validators/style.py
+-rw-r--r--   0        0        0      824 2024-05-17 07:27:54.398157 drawlib-0.1.9/drawlib/v0_1/private/validators/text.py
+-rw-r--r--   0        0        0     2270 2024-05-17 08:45:46.188412 drawlib-0.1.9/drawlib/v0_1/private/validators/types.py
+-rw-r--r--   0        0        0      712 2024-05-24 16:51:47.199276 drawlib-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 drawlib-0.1.9/PKG-INFO
```

### Comparing `drawlib-0.1.8/LICENSE.txt` & `drawlib-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/README.md` & `drawlib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/__init__.py` & `drawlib-0.1.9/drawlib/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 - drawlib.v0_1: API v0.1 interface (latest)
 
 """
 
 from typing import Final
 
 # please update here when you release new version
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 # might not be changed
 LIB_NAME: Final[str] = "drawlib"
 AUTHOR: Final[str] = "Yuichi Ito"
 CONTACT: Final[str] = "yuichi@yuichi.com"
 __version__: Final[str] = VERSION
```

### Comparing `drawlib-0.1.8/drawlib/__main__.py` & `drawlib-0.1.9/drawlib/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/apis.py` & `drawlib-0.1.9/drawlib/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/__init__.py` & `drawlib-0.1.9/drawlib/v0_1/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/__main__.py` & `drawlib-0.1.9/drawlib/v0_1/__main__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/apis.py` & `drawlib-0.1.9/drawlib/v0_1/apis.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/__init__.py` & `drawlib-0.1.9/drawlib/v0_1/private/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/command.py` & `drawlib-0.1.9/drawlib/v0_1/private/command.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/__init__.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/colors.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/colors.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/dimage.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/dimage.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,15 +217,15 @@
             raise ValueError('arg "file" must be str.')
 
         abspath = get_script_relative_path(file)
         directory = os.path.dirname(abspath)
         os.makedirs(directory, exist_ok=True)
         self._pilimg.save(abspath, quality=95)
 
-    '''
+    """
     @error_handler
     def border(
         self,
         width: int,
         color: Union[Tuple[int, int, int], Tuple[int, int, int, float]],
     ) -> Dimage:
         print(color)
@@ -233,17 +233,18 @@
         new_img = ImageOps.expand(
             self._pilimg,
             border=width,
             # pillow supports (R, G, B) and (R, G, B, A)
             fill=(color[0], color[1], color[2]),
         )
         return Dimage(new_img)
+    """
 
     @error_handler
-    def rotate(self, angle: float) -> Dimage:
+    def _rotate(self, angle: float) -> Dimage:
         """Get rotated new Dimage. Original Dimage is keeped.
 
         Get new Dimage which has rotated.
 
         Args:
             angle: between 0.0 ~ 360. pixel size can be changed. New area becomes transparent.
 
@@ -254,15 +255,14 @@
 
         newimg = self._pilimg.rotate(
             angle,
             resample=Image.Resampling.BICUBIC,
             expand=True,
         )
         return Dimage(newimg)
-    '''
 
     @error_handler
     def resize(self, width: int, height: int) -> Dimage:
         """Get resized new Dimage. Original Dimage is keeped.
 
         Get new Dimage which has resized.
```

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/fonts.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/fonts.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/model.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/model.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/theme.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/theme.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/theme_officials.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/theme_officials.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/theme_styles.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/theme_styles.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core/util.py` & `drawlib-0.1.9/drawlib/v0_1/private/core/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/__init__.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/base.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/base.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/canvas.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/image.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                 has_wrong_style = True
                 style.halign = "center"
             if style.valign != "center":
                 has_wrong_style = True
                 style.valign = "center"
             if has_wrong_style:
                 logger.warn("image() with angle only accepts ShapeTextStyle alignment center.")
-            pimg = pimg.rotate(angle)
+            pimg = pimg._rotate(angle)
 
         # xy shift
         if style.halign != "center" or style.valign != "center":
             #
             # memo. calculation
             # (image_width / 2) * (zoom / 0.72) * (canvas_width / 100)
             #   -> image_width * zoom * self._width / 1440
```

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/line.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/line.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_arrow.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/original_arrow.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/original_polygon.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/original_polygon.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/patches.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/patches.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/core_canvas/text.py` & `drawlib-0.1.9/drawlib/v0_1/private/core_canvas/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/download.py` & `drawlib-0.1.9/drawlib/v0_1/private/download.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/dutil.py` & `drawlib-0.1.9/drawlib/v0_1/private/dutil.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/icons/__init__.py` & `drawlib-0.1.9/drawlib/v0_1/private/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/icons/phosphor.py` & `drawlib-0.1.9/drawlib/v0_1/private/icons/phosphor.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/icons/util.py` & `drawlib-0.1.9/drawlib/v0_1/private/icons/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/logging.py` & `drawlib-0.1.9/drawlib/v0_1/private/logging.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/settings.py` & `drawlib-0.1.9/drawlib/v0_1/private/settings.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/smartarts/__init__.py` & `drawlib-0.1.9/drawlib/v0_1/private/smartarts/__init__.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/smartarts/bubblespeech.py` & `drawlib-0.1.9/drawlib/v0_1/private/smartarts/bubblespeech.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/smartarts/dsart.py` & `drawlib-0.1.9/drawlib/v0_1/private/smartarts/dsart.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/smartarts/groups.py` & `drawlib-0.1.9/drawlib/v0_1/private/smartarts/groups.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/smartarts/pyramid.py` & `drawlib-0.1.9/drawlib/v0_1/private/smartarts/pyramid.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/smartarts/sourcecode.py` & `drawlib-0.1.9/drawlib/v0_1/private/smartarts/sourcecode.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/smartarts/tree.py` & `drawlib-0.1.9/drawlib/v0_1/private/smartarts/tree.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/util.py` & `drawlib-0.1.9/drawlib/v0_1/private/util.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/args.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/args.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/color.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/color.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/coordinate.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/coordinate.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/image.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/image.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/line.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/line.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/shape.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/shape.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/smartarts.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/smartarts.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/style.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/style.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/text.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/text.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/drawlib/v0_1/private/validators/types.py` & `drawlib-0.1.9/drawlib/v0_1/private/validators/types.py`

 * *Files identical despite different names*

### Comparing `drawlib-0.1.8/pyproject.toml` & `drawlib-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "drawlib"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python drawing library. Illustration as Code."
 homepage = "https://www.drawlib.com"
 repository = "https://github.com/yuichi110/drawlib"
 authors = [ "Yuichi Ito <yuichi@yuichi.com>",]
 readme = "README.md"
 
 [tool.black]
```

### Comparing `drawlib-0.1.8/PKG-INFO` & `drawlib-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawlib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python drawing library. Illustration as Code.
 Home-page: https://www.drawlib.com
 Author: Yuichi Ito
 Author-email: yuichi@yuichi.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

