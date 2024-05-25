# Comparing `tmp/viser-0.1.8.tar.gz` & `tmp/viser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viser-0.1.8.tar", last modified: Tue Nov  7 00:03:53 2023, max compression
+gzip compressed data, was "viser-0.1.9.tar", last modified: Tue Nov  7 03:02:44 2023, max compression
```

## Comparing `viser-0.1.8.tar` & `viser-0.1.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.997102 viser-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-07 00:02:12.000000 viser-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-11-07 00:03:52.997102 viser-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-11-07 00:02:12.000000 viser-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-11-07 00:02:12.000000 viser-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 00:03:52.997102 viser-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.973101 viser-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.977102 viser-0.1.8/src/viser/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_client_autobuild.py
--rw-r--r--   0 runner    (1001) docker     (127)    25019 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_gui_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19285 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_gui_handles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.977102 viser-0.1.8/src/viser/_icons/
--rw-r--r--   0 runner    (1001) docker     (127)  5436416 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_icons/tabler-icons.tar
--rw-r--r--   0 runner    (1001) docker     (127)      570 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)   152177 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_icons_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_icons_generate_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    31224 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_message_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13603 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_scene_handles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    19537 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/_viser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.973101 viser-0.1.8/src/viser/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.985102 viser-0.1.8/src/viser/client/build/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.985102 viser-0.1.8/src/viser/client/build/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-07 00:03:48.000000 viser-0.1.8/src/viser/client/build/assets/index-a156f4a4.css
--rw-r--r--   0 runner    (1001) docker     (127)  3183683 2023-11-07 00:03:48.000000 viser-0.1.8/src/viser/client/build/assets/index-f73875e3.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.989102 viser-0.1.8/src/viser/client/build/hdri/
--rw-r--r--   0 runner    (1001) docker     (127)  1540678 2023-11-07 00:03:47.000000 viser-0.1.8/src/viser/client/build/hdri/potsdamer_platz_1k.hdr
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-11-07 00:03:48.000000 viser-0.1.8/src/viser/client/build/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-11-07 00:03:47.000000 viser-0.1.8/src/viser/client/build/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-07 00:03:47.000000 viser-0.1.8/src/viser/client/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-07 00:03:47.000000 viser-0.1.8/src/viser/client/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.993102 viser-0.1.8/src/viser/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/extras/_record3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/extras/_urdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.993102 viser-0.1.8/src/viser/extras/colmap/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/extras/colmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/extras/colmap/_colmap_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.993102 viser-0.1.8/src/viser/infra/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/infra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/infra/_async_message_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15776 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/infra/_infra.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/infra/_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/infra/_typescript_interface_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.993102 viser-0.1.8/src/viser/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/scripts/dev_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.997102 viser-0.1.8/src/viser/theme/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/theme/_titlebar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.997102 viser-0.1.8/src/viser/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/_se2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/_se3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/_so2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12803 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/_so3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.997102 viser-0.1.8/src/viser/transforms/hints/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/hints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.997102 viser-0.1.8/src/viser/transforms/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-07 00:02:12.000000 viser-0.1.8/src/viser/transforms/utils/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 00:03:52.977102 viser-0.1.8/src/viser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-11-07 00:03:52.000000 viser-0.1.8/src/viser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-11-07 00:03:52.000000 viser-0.1.8/src/viser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 00:03:52.000000 viser-0.1.8/src/viser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-07 00:03:52.000000 viser-0.1.8/src/viser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-07 00:03:52.000000 viser-0.1.8/src/viser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-07 00:03:52.000000 viser-0.1.8/src/viser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.711210 viser-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-07 03:00:21.000000 viser-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-11-07 03:02:44.711210 viser-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-11-07 03:00:21.000000 viser-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-11-07 03:00:21.000000 viser-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-07 03:02:44.711210 viser-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.691209 viser-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.695209 viser-0.1.9/src/viser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_client_autobuild.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25019 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_gui_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19285 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_gui_handles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.695209 viser-0.1.9/src/viser/_icons/
+-rw-r--r--   0 runner    (1001) docker     (127)  5436416 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_icons/tabler-icons.tar
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152177 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_icons_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_icons_generate_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31224 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_message_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13603 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_scene_handles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19498 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/_viser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.691209 viser-0.1.9/src/viser/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.703209 viser-0.1.9/src/viser/client/build/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.703209 viser-0.1.9/src/viser/client/build/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-07 03:02:39.000000 viser-0.1.9/src/viser/client/build/assets/index-a156f4a4.css
+-rw-r--r--   0 runner    (1001) docker     (127)  3183683 2023-11-07 03:02:39.000000 viser-0.1.9/src/viser/client/build/assets/index-f73875e3.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.703209 viser-0.1.9/src/viser/client/build/hdri/
+-rw-r--r--   0 runner    (1001) docker     (127)  1540678 2023-11-07 03:02:37.000000 viser-0.1.9/src/viser/client/build/hdri/potsdamer_platz_1k.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2023-11-07 03:02:39.000000 viser-0.1.9/src/viser/client/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-11-07 03:02:37.000000 viser-0.1.9/src/viser/client/build/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-07 03:02:37.000000 viser-0.1.9/src/viser/client/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-07 03:02:37.000000 viser-0.1.9/src/viser/client/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.707210 viser-0.1.9/src/viser/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/extras/_record3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/extras/_urdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.707210 viser-0.1.9/src/viser/extras/colmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/extras/colmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/extras/colmap/_colmap_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.707210 viser-0.1.9/src/viser/infra/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/infra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/infra/_async_message_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16160 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/infra/_infra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/infra/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/infra/_typescript_interface_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.707210 viser-0.1.9/src/viser/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/scripts/dev_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.707210 viser-0.1.9/src/viser/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/theme/_titlebar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.711210 viser-0.1.9/src/viser/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/_se2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/_se3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/_so2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/_so3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.711210 viser-0.1.9/src/viser/transforms/hints/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/hints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.711210 viser-0.1.9/src/viser/transforms/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-11-07 03:00:21.000000 viser-0.1.9/src/viser/transforms/utils/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 03:02:44.695209 viser-0.1.9/src/viser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2023-11-07 03:02:44.000000 viser-0.1.9/src/viser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-11-07 03:02:44.000000 viser-0.1.9/src/viser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 03:02:44.000000 viser-0.1.9/src/viser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-07 03:02:44.000000 viser-0.1.9/src/viser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2023-11-07 03:02:44.000000 viser-0.1.9/src/viser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-07 03:02:44.000000 viser-0.1.9/src/viser.egg-info/top_level.txt
```

### Comparing `viser-0.1.8/LICENSE` & `viser-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/PKG-INFO` & `viser-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viser
-Version: 0.1.8
+Version: 0.1.9
 Summary: 3D visualization + Python
 License: MIT
 Project-URL: GitHub, https://github.com/nerfstudio-project/viser
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `viser-0.1.8/README.md` & `viser-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/pyproject.toml` & `viser-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "viser"
-version = "0.1.8"
+version = "0.1.9"
 description = "3D visualization + Python"
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `viser-0.1.8/src/viser/__init__.py` & `viser-0.1.9/src/viser/__init__.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_client_autobuild.py` & `viser-0.1.9/src/viser/_client_autobuild.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_gui_api.py` & `viser-0.1.9/src/viser/_gui_api.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_gui_handles.py` & `viser-0.1.9/src/viser/_gui_handles.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_icons/tabler-icons.tar` & `viser-0.1.9/src/viser/_icons/tabler-icons.tar`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_icons.py` & `viser-0.1.9/src/viser/_icons.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_icons_enum.py` & `viser-0.1.9/src/viser/_icons_enum.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_icons_generate_enum.py` & `viser-0.1.9/src/viser/_icons_generate_enum.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_message_api.py` & `viser-0.1.9/src/viser/_message_api.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_messages.py` & `viser-0.1.9/src/viser/_messages.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_scene_handles.py` & `viser-0.1.9/src/viser/_scene_handles.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_tunnel.py` & `viser-0.1.9/src/viser/_tunnel.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/_viser.py` & `viser-0.1.9/src/viser/_viser.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         if got_lock:
             self._atomic_lock.release()
             self._locked_thread_id = -1
 
     def flush(self) -> None:
         """Flush the outgoing message buffer. Any buffered messages will immediately be
         sent. (by default they are windowed)"""
-        self._state.server._flush_event_from_client_id[self.client_id].set()
+        self._state.server.flush_client(self.client_id)
 
 
 # We can serialize the state of a ViserServer via a tuple of
 # (serialized message, timestamp) pairs.
 SerializedServerState = Tuple[Tuple[bytes, float], ...]
 
 
@@ -528,8 +528,8 @@
         if got_lock:
             self._atomic_lock.release()
             self._locked_thread_id = -1
 
     def flush(self) -> None:
         """Flush the outgoing message buffer. Any buffered messages will immediately be
         sent. (by default they are windowed)"""
-        self._server._broadcast_buffer.flush()
+        self._server.flush()
```

### Comparing `viser-0.1.8/src/viser/client/build/assets/index-a156f4a4.css` & `viser-0.1.9/src/viser/client/build/assets/index-a156f4a4.css`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/client/build/assets/index-f73875e3.js` & `viser-0.1.9/src/viser/client/build/assets/index-f73875e3.js`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/client/build/hdri/potsdamer_platz_1k.hdr` & `viser-0.1.9/src/viser/client/build/hdri/potsdamer_platz_1k.hdr`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/client/build/index.html` & `viser-0.1.9/src/viser/client/build/index.html`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/client/build/logo.svg` & `viser-0.1.9/src/viser/client/build/logo.svg`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/extras/_record3d.py` & `viser-0.1.9/src/viser/extras/_record3d.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/extras/_urdf.py` & `viser-0.1.9/src/viser/extras/_urdf.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/extras/colmap/_colmap_utils.py` & `viser-0.1.9/src/viser/extras/colmap/_colmap_utils.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/infra/__init__.py` & `viser-0.1.9/src/viser/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/infra/_async_message_buffer.py` & `viser-0.1.9/src/viser/infra/_async_message_buffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 from __future__ import annotations
 
 import asyncio
 import dataclasses
 import time
 from asyncio.events import AbstractEventLoop
-from typing import Any, AsyncGenerator, Dict, Optional, Sequence, Set, Union, cast
+from typing import Any, AsyncGenerator, Dict, Optional, Sequence, Union
 
 from typing_extensions import Literal, TypeGuard
 
 from ._messages import Message
 
 
 @dataclasses.dataclass
 class AsyncMessageBuffer:
     """Async iterable for keeping a persistent buffer of messages.
 
     Uses heuristics on message names to automatically cull out redundant messages."""
 
     event_loop: AbstractEventLoop
     message_event: asyncio.Event = dataclasses.field(default_factory=asyncio.Event)
-    _flush_event: asyncio.Event = dataclasses.field(default_factory=asyncio.Event)
 
     message_counter: int = 0
-    message_from_id: Dict[int, Message] = dataclasses.field(default_factory=dict)
+    message_from_id: Dict[int, Union[Message, FlushSentinel]] = dataclasses.field(
+        default_factory=dict
+    )
     id_from_redundancy_key: Dict[str, int] = dataclasses.field(default_factory=dict)
 
-    def push(self, message: Message) -> None:
+    def push(self, message: Union[Message, FlushSentinel]) -> None:
         """Push a new message to our buffer, and remove old redundant ones."""
         # Add message to buffer.
         new_message_id = self.message_counter
         self.message_from_id[new_message_id] = message
         self.message_counter += 1
 
         # If an existing message with the same key already exists in our buffer, we
         # don't need the old one anymore. :-)
-        redundancy_key = message.redundancy_key()
+        if isinstance(message, Message):
+            redundancy_key = message.redundancy_key()
+        else:
+            redundancy_key = FLUSH_SENTINEL
+
         if redundancy_key is not None and redundancy_key in self.id_from_redundancy_key:
             old_message_id = self.id_from_redundancy_key.pop(redundancy_key)
             self.message_from_id.pop(old_message_id)
         self.id_from_redundancy_key[redundancy_key] = new_message_id
 
         # Notify consumers that a new message is available.
         self.event_loop.call_soon_threadsafe(self.message_event.set)
 
-    def flush(self) -> None:
-        """Immediately send any buffered messages."""
-        self._flush_event.set()
-
     async def window_generator(
         self, client_id: int
     ) -> AsyncGenerator[Sequence[Message], None]:
         """Async iterator over messages. Loops infinitely, and waits when no messages
         are available."""
         # Wait for a first message to arrive.
         if len(self.message_from_id) == 0:
@@ -58,32 +59,21 @@
 
         window = MessageWindow(client_id=client_id)
         last_sent_id = -1
         while True:
             # Wait until there are new messages available.
             most_recent_message_id = self.message_counter - 1
             while last_sent_id >= most_recent_message_id:
-                next_message = asyncio.create_task(self.message_event.wait())
-                flush_wait = asyncio.create_task(self._flush_event.wait())
-                send_window = False
+                next_message = self.message_event.wait()
                 try:
-                    done, pending = await asyncio.wait(
-                        [flush_wait, next_message],
-                        timeout=window.max_time_until_ready(),
-                        return_when=asyncio.FIRST_COMPLETED,
+                    await asyncio.wait_for(
+                        next_message, timeout=window.max_time_until_ready()
                     )
-                    del pending
-                    if flush_wait in done:
-                        send_window = True
-                        self._flush_event.clear()
                     most_recent_message_id = self.message_counter - 1
                 except asyncio.TimeoutError:
-                    send_window = True
-
-                if send_window:
                     out = window.get_window_to_send()
                     if out is not None:
                         yield out
 
             # Try to yield the next message ID. Note that messages can be culled before
             # they're sent.
             last_sent_id += 1
@@ -96,72 +86,79 @@
                 await asyncio.sleep(1e-8)
 
             out = window.get_window_to_send()
             if out is not None:
                 yield out
 
 
-DONE_SENTINEL = "done_sentinel"
 DoneSentinel = Literal["done_sentinel"]
+DONE_SENTINEL: DoneSentinel = "done_sentinel"
+
+FlushSentinel = Literal["flush_sentinel"]
+FLUSH_SENTINEL: FlushSentinel = "flush_sentinel"
 
 
 def is_done_sentinel(x: Any) -> TypeGuard[DoneSentinel]:
     return x == DONE_SENTINEL
 
 
+def is_flush_sentinel(x: Any) -> TypeGuard[FlushSentinel]:
+    return x == FLUSH_SENTINEL
+
+
 @dataclasses.dataclass
 class MessageWindow:
     """Helper for building windows of messages to send to clients."""
 
     client_id: int
     """Client that this window will be sent to. Used for ignoring certain messages."""
 
     window_duration_sec: float = 1.0 / 60.0
     window_max_length: int = 256
 
+    flush: bool = False
     done: bool = False
 
     _window_start_time: float = -1
     _window: Dict[str, Message] = dataclasses.field(default_factory=dict)
     """We use a redundancy key -> message dictionary to track our window. This helps us
     eliminate redundant messages."""
 
-    def append_to_window(self, message: Union[Message, DoneSentinel]) -> None:
+    def append_to_window(
+        self, message: Union[Message, DoneSentinel, FlushSentinel]
+    ) -> None:
         """Append a message to our window."""
         if isinstance(message, Message):
             if message.excluded_self_client == self.client_id:
                 return
             if len(self._window) == 0:
                 self._window_start_time = time.time()
             self._window[message.redundancy_key()] = message
+        elif is_flush_sentinel(message):
+            self.flush = True
         else:
             assert is_done_sentinel(message)
             self.done = True
 
     async def wait_and_append_to_window(
         self,
-        message_task: asyncio.Task[Union[Message, DoneSentinel]],
-        flush_event: asyncio.Event,
+        message_task: asyncio.Task[Union[Message, DoneSentinel, FlushSentinel]],
     ) -> bool:
         """Async version of `append_to_window()`. Returns `True` if successful, `False`
         if timed out."""
         if len(self._window) == 0:
             self.append_to_window(await message_task)
             return True
 
-        flush_wait = asyncio.create_task(flush_event.wait())
-        done, pending = await asyncio.wait(
-            [message_task, flush_wait],
+        (done, pending) = await asyncio.wait(
+            [message_task],
             timeout=self.max_time_until_ready(),
-            return_when=asyncio.FIRST_COMPLETED,
         )
         del pending
-        if flush_wait in done:
-            flush_event.clear()
-        if message_task in cast(Set[Any], done):  # Cast to prevent type narrowing.
+        if message_task in done:  # Cast to prevent type narrowing.
             self.append_to_window(await message_task)
             return True
         return False
 
     def max_time_until_ready(self) -> Optional[float]:
         """Returns the maximum amount of time, in seconds, until we're ready to send the
         current window. If the window is empty, returns `None`."""
@@ -170,15 +167,18 @@
         elapsed = time.time() - self._window_start_time
         return max(0.0, self.window_duration_sec - elapsed)
 
     def get_window_to_send(self) -> Optional[Sequence[Message]]:
         """Returns window of messages if ready. Otherwise, returns None."""
         # Are we ready to send?
         ready = False
-        if (
+        if self.flush:
+            ready = True
+            self.flush = False
+        elif (
             len(self._window) > 0
             and time.time() - self._window_start_time >= self.window_duration_sec
         ):
             ready = True
         elif len(self._window) >= self.window_max_length:
             ready = True
```

### Comparing `viser-0.1.8/src/viser/infra/_infra.py` & `viser-0.1.9/src/viser/infra/_infra.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 import websockets.exceptions
 import websockets.server
 from typing_extensions import Literal, assert_never
 from websockets.legacy.server import WebSocketServerProtocol
 
 from ._async_message_buffer import (
     DONE_SENTINEL,
+    FLUSH_SENTINEL,
     AsyncMessageBuffer,
     DoneSentinel,
+    FlushSentinel,
     MessageWindow,
 )
 from ._messages import Message
 
 
 @dataclasses.dataclass
 class _ClientHandleState:
@@ -153,15 +155,15 @@
         self._http_server_root = http_server_root
         self._verbose = verbose
         self._client_api_version: Literal[0, 1] = client_api_version
 
         self._thread_executor = ThreadPoolExecutor(max_workers=32)
         self._shutdown_event = threading.Event()
 
-        self._flush_event_from_client_id: Dict[int, asyncio.Event] = {}
+        self._client_state_from_id: Dict[int, _ClientHandleState] = {}
 
     def start(self) -> None:
         """Start the server."""
 
         # Start server thread.
         ready_sem = threading.Semaphore(value=1)
         ready_sem.acquire()
@@ -193,14 +195,24 @@
         """Pushes a message onto the broadcast queue. Message will be sent to all clients.
 
         Broadcasted messages are persistent: if a new client connects to the server,
         they will receive a buffered set of previously broadcasted messages. The buffer
         is culled using the value of `message.redundancy_key()`."""
         self._broadcast_buffer.push(message)
 
+    def flush(self) -> None:
+        """Flush the outgoing message buffer for broadcasted messages. Any buffered
+        messages will immediately be sent. (by default they are windowed)"""
+        self._broadcast_buffer.push(FLUSH_SENTINEL)
+
+    def flush_client(self, client_id: int) -> None:
+        """Flush the outgoing message buffer for a particular client. Any buffered
+        messages will immediately be sent. (by default they are windowed)"""
+        self._client_state_from_id[client_id].message_buffer.put_nowait(FLUSH_SENTINEL)
+
     def _background_worker(self, ready_sem: threading.Semaphore) -> None:
         host = self._host
         port = self._port
         message_class = self._message_class
         http_server_root = self._http_server_root
 
         # Need to make a new event loop for notebook compatbility.
@@ -220,28 +232,28 @@
                 nonlocal connection_count
                 client_id = ClientId(connection_count)
                 connection_count += 1
 
                 nonlocal total_connections
                 total_connections += 1
 
-            self._flush_event_from_client_id[client_id] = asyncio.Event()
             if self._verbose:
                 rich.print(
                     f"[bold](viser)[/bold] Connection opened ({client_id},"
                     f" {total_connections} total),"
                     f" {len(self._broadcast_buffer.message_from_id)} persistent"
                     " messages"
                 )
 
             client_state = _ClientHandleState(
                 message_buffer=asyncio.Queue(),
                 event_loop=event_loop,
             )
             client_connection = ClientConnection(client_id, client_state)
+            self._client_state_from_id[client_id] = client_state
 
             def handle_incoming(message: Message) -> None:
                 self._thread_executor.submit(
                     error_print_wrapper(
                         lambda: self._handle_incoming_message(client_id, message)
                     )
                 )
@@ -260,15 +272,14 @@
             try:
                 # For each client: infinite loop over producers (which send messages)
                 # and consumers (which receive messages).
                 await asyncio.gather(
                     _client_producer(
                         websocket,
                         client_id,
-                        self._flush_event_from_client_id[client_id],
                         client_state.message_buffer.get,
                         self._client_api_version,
                     ),
                     _broadcast_producer(
                         websocket,
                         self._broadcast_buffer.window_generator(client_id).__anext__,
                         self._client_api_version,
@@ -283,22 +294,20 @@
                 # should exit.
                 #
                 # This is partially cosmetic: it allows us to safely finish pending
                 # queue get() tasks, which suppresses a "Task was destroyed but it is
                 # pending" error.
                 await client_state.message_buffer.put(DONE_SENTINEL)
 
-                # Trigger then delete the flush event.
-                self._flush_event_from_client_id.pop(client_id).set()
-
                 # Disconnection callbacks.
                 for cb in self._client_disconnect_cb:
                     cb(client_connection)
 
                 # Cleanup.
+                self._client_state_from_id.pop(client_id)
                 total_connections -= 1
                 if self._verbose:
                     rich.print(
                         f"[bold](viser)[/bold] Connection closed ({client_id},"
                         f" {total_connections} total)"
                     )
 
@@ -356,28 +365,26 @@
         event_loop.run_forever()
         rich.print("[bold](viser)[/bold] Server stopped")
 
 
 async def _client_producer(
     websocket: WebSocketServerProtocol,
     client_id: ClientId,
-    flush_event: asyncio.Event,
-    get_next: Callable[[], Coroutine[None, None, Union[Message, DoneSentinel]]],
+    get_next: Callable[
+        [], Coroutine[None, None, Union[Message, FlushSentinel, DoneSentinel]]
+    ],
     client_api_version: Literal[0, 1],
 ) -> None:
     """Infinite loop to send messages from a buffer to a single client."""
 
     window = MessageWindow(client_id=client_id)
     message_task = asyncio.create_task(get_next())
 
     while not window.done:
-        if (
-            await window.wait_and_append_to_window(message_task, flush_event)
-            and not window.done
-        ):
+        if await window.wait_and_append_to_window(message_task) and not window.done:
             message_task = asyncio.create_task(get_next())
         outgoing = window.get_window_to_send()
         if outgoing is not None:
             if client_api_version == 1:
                 serialized = msgpack.packb(
                     tuple(message.as_serializable_dict() for message in outgoing)
                 )
```

### Comparing `viser-0.1.8/src/viser/infra/_messages.py` & `viser-0.1.9/src/viser/infra/_messages.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/infra/_typescript_interface_gen.py` & `viser-0.1.9/src/viser/infra/_typescript_interface_gen.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/scripts/dev_checks.py` & `viser-0.1.9/src/viser/scripts/dev_checks.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/theme/_titlebar.py` & `viser-0.1.9/src/viser/theme/_titlebar.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/transforms/_base.py` & `viser-0.1.9/src/viser/transforms/_base.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/transforms/_se2.py` & `viser-0.1.9/src/viser/transforms/_se2.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/transforms/_se3.py` & `viser-0.1.9/src/viser/transforms/_se3.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/transforms/_so2.py` & `viser-0.1.9/src/viser/transforms/_so2.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/transforms/_so3.py` & `viser-0.1.9/src/viser/transforms/_so3.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser/transforms/utils/_utils.py` & `viser-0.1.9/src/viser/transforms/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `viser-0.1.8/src/viser.egg-info/PKG-INFO` & `viser-0.1.9/src/viser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viser
-Version: 0.1.8
+Version: 0.1.9
 Summary: 3D visualization + Python
 License: MIT
 Project-URL: GitHub, https://github.com/nerfstudio-project/viser
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `viser-0.1.8/src/viser.egg-info/SOURCES.txt` & `viser-0.1.9/src/viser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

