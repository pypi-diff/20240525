# Comparing `tmp/clickgen-2.2.2.tar.gz` & `tmp/clickgen-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickgen-2.2.2.tar", last modified: Wed Apr 24 13:21:32 2024, max compression
+gzip compressed data, was "clickgen-2.2.3.tar", last modified: Sat May 25 15:15:14 2024, max compression
```

## Comparing `clickgen-2.2.2.tar` & `clickgen-2.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-24 13:21:01.000000 clickgen-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-24 13:21:32.017013 clickgen-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-24 13:21:01.000000 clickgen-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-24 13:21:01.000000 clickgen-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-24 13:21:32.017013 clickgen-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 13:21:01.000000 clickgen-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.005013 clickgen-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.009013 clickgen-2.2.2/src/clickgen/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/configparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/cursors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.009013 clickgen-2.2.2/src/clickgen/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/libs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/libs/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/libs/colors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.013013 clickgen-2.2.2/src/clickgen/packer/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/packer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/packer/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/packer/windows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/packer/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/packer/x11.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.013013 clickgen-2.2.2/src/clickgen/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/parser/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/parser/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/parser/png.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/parser/png.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.013013 clickgen-2.2.2/src/clickgen/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/scripts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/scripts/clickgen.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/scripts/clickgen.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6234 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/scripts/ctgen.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/scripts/ctgen.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/src/clickgen/writer/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/writer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/writer/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/writer/windows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-24 13:21:01.000000 clickgen-2.2.2/src/clickgen/writer/x11.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 13:21:29.000000 clickgen-2.2.2/src/clickgen/writer/x11.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/src/clickgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-24 13:21:32.000000 clickgen-2.2.2/src/clickgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:21:31.000000 clickgen-2.2.2/src/clickgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:21:32.017013 clickgen-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-24 13:21:01.000000 clickgen-2.2.2/tests/test_configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-24 13:21:01.000000 clickgen-2.2.2/tests/test_cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 13:21:01.000000 clickgen-2.2.2/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.241830 clickgen-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-25 15:14:42.000000 clickgen-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-25 15:15:14.241830 clickgen-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-25 15:14:42.000000 clickgen-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-25 15:14:42.000000 clickgen-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-25 15:15:14.241830 clickgen-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-25 15:14:42.000000 clickgen-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.229830 clickgen-2.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.233830 clickgen-2.2.3/src/clickgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/configparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/cursors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.233830 clickgen-2.2.3/src/clickgen/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/libs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/libs/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/libs/colors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.233830 clickgen-2.2.3/src/clickgen/packer/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/packer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/packer/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/packer/windows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/packer/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/packer/x11.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.237830 clickgen-2.2.3/src/clickgen/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/parser/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/parser/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/parser/png.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/parser/png.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.237830 clickgen-2.2.3/src/clickgen/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/scripts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/scripts/clickgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/scripts/clickgen.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/scripts/ctgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/scripts/ctgen.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.237830 clickgen-2.2.3/src/clickgen/writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/writer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/writer/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/writer/windows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-25 15:14:42.000000 clickgen-2.2.3/src/clickgen/writer/x11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-25 15:15:11.000000 clickgen-2.2.3/src/clickgen/writer/x11.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.237830 clickgen-2.2.3/src/clickgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-25 15:15:14.000000 clickgen-2.2.3/src/clickgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-25 15:15:14.000000 clickgen-2.2.3/src/clickgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 15:15:14.000000 clickgen-2.2.3/src/clickgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-25 15:15:14.000000 clickgen-2.2.3/src/clickgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-25 15:15:14.000000 clickgen-2.2.3/src/clickgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 15:15:14.000000 clickgen-2.2.3/src/clickgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 15:15:14.237830 clickgen-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-25 15:14:42.000000 clickgen-2.2.3/tests/test_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-25 15:14:42.000000 clickgen-2.2.3/tests/test_cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-25 15:14:42.000000 clickgen-2.2.3/tests/test_parser.py
```

### Comparing `clickgen-2.2.2/LICENSE` & `clickgen-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/PKG-INFO` & `clickgen-2.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickgen
-Version: 2.2.2
+Version: 2.2.3
 Summary: The hassle-free cursor building toolbox.
 Home-page: https://github.com/ful1e5/clickgen
 Author: Abdulkaiz Khatri
 Author-email: kaizmandhu@gmail.com
 Project-URL: Source, https://github.com/ful1e5/clickgen
 Project-URL: Download, https://pypi.org/project/clickgen/#files
 Project-URL: Bug Tracker, https://github.com/ful1e5/clickgen/issues
@@ -59,77 +59,84 @@
  https://dev.to/ful1e5/lets-give-recognition-to-those-supporting-our-work-on-github-sponsors-b00 -->
 
 ![shoutout-sponsors](https://sponsor-spotlight.vercel.app/sponsor?login=ful1e5)
 
 > **Note**
 > The project's success depends on sponsorships. Meeting sponsorship goals for [ful1e5](https://github.com/ful1e5) GitHub Account will drive new releases and ongoing development.
 
-- **2023-08-23:** `ctgen` CLI supports `.json` and `.yaml`/`.yml` as configuration file.
-- **2023-08-17:** Cursor size settings moved to `[cursors.fallback_settings]` in config. See [changelog-08172023](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-6747666)
-- **2022-06-15:** Docker Image support deprecated due to cross-platform compatibility.
-- **2022-07-09:** :warning: All the **functionality and modules are removed from older versions in `v2.0.0`**.
-  I will be restricting any updates to the `>=v1.2.0` versions to security updates and hotfixes.
-  Check updated documentations for [building cursors from API](#api-examples) and [CLIs](#usage) usage.
+-   **2024-05-24:** Clickgen now allows cursor bitmap re-canvasing by specifying size using the `cursor_size:canvas_size` format. See [changelog-05212024](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-9511166)
+-   **2023-08-23:** `ctgen` CLI supports `.json` and `.yaml`/`.yml` as configuration file.
+-   **2023-08-17:** Cursor size settings moved to `[cursors.fallback_settings]` in config. See [changelog-08172023](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-6747666)
+-   **2022-06-15:** Docker Image support deprecated due to cross-platform compatibility.
+-   **2022-07-09:** :warning: All the **functionality and modules are removed from older versions in `v2.0.0`**.
+    I will be restricting any updates to the `>=v1.2.0` versions to security updates and hotfixes.
+    Check updated documentations for [building cursors from API](#api-examples) and [CLIs](#usage) usage.
 
 ## Requirements
 
-- Python version 3.7.5 or higher
-- [Pillow](https://pypi.org/project/Pillow) >= 8.1.1
-- [PyYaml](https://pypi.org/project/PyYaml) >= 6.0.1
-- [attrs](https://pypi.org/project/attrs) >= 15.0.0
-- [numpy](https://pypi.org/project/numpy) >= 1.21.6
-- [toml](https://pypi.org/project/toml) >= 0.10.2
+-   Python version 3.7.5 or higher
+-   [Pillow](https://pypi.org/project/Pillow) >= 8.1.1
+-   [PyYaml](https://pypi.org/project/PyYaml) >= 6.0.1
+-   [attrs](https://pypi.org/project/attrs) >= 15.0.0
+-   [numpy](https://pypi.org/project/numpy) >= 1.21.6
+-   [toml](https://pypi.org/project/toml) >= 0.10.2
 
 ## Install
 
 ```bash
 pip3 install clickgen
 ```
 
 > **Note**
 > Distributions' packages are not affiliated with clickgen developers.
 > If you encounter any issues with the incorrect installation, you should contact the package maintainer first.
 
 ### Arch Linux
 
-- [AUR](https://aur.archlinux.org/packages/python-clickgen)
+-   [AUR](https://aur.archlinux.org/packages/python-clickgen)
 
 ## Usage
 
 ### `clickgen` CLI
 
 #### Linux Format (XCursor)
 
 For example, if you have to build [ponter.png](https://github.com/ful1e5/clickgen/blob/main/samples/pngs/pointer.png)
 file to Linux Format:
 
-```
+```bash
 clickgen samples/pngs/pointer.png -x 10 -y 10 -s 22 24 32 -p x11
 ```
 
 You also **build animated Xcursor** by providing multiple png files to argument and animation delay with `-d`:
 
-```
+```bash
 clickgen samples/pngs/wait-001.png samples/pngs/wait-001.png -d 3 -x 10 -y 10 -s 22 24 32 -p x11
 ```
 
 #### Windows Formats (.cur and .ani)
 
 To build [ponter.png](https://github.com/ful1e5/clickgen/blob/main/samples/pngs/pointer.png)
 file to Windows Format (`.cur`):
 
-> **Warning: Windows Cursor only support single size.**
+> **Warning: Windows Animated Cursor only support single size.**
 
-```
+```bash
 clickgen samples/pngs/pointer.png -x 10 -y 10 -s 32 -p windows
 ```
 
-For **animated Windows Cursor** (`.ani`):
+You can also specify the size in the `size:canvas_size` format to enable canvasing:
 
+```bash
+clickgen samples/pngs/pointer.png -x 10 -y 10 -s 20:32 -p windows
 ```
+
+For **animated Windows Cursor** (`.ani`):
+
+```bash
 clickgen samples/pngs/wait-001.png samples/pngs/wait-001.png -d 3 -x 10 -y 10 -s 32 -p windows
 ```
 
 For more information, run `clickgen --help`.
 
 ### `ctgen` CLI
 
@@ -139,21 +146,21 @@
 ctgen sample/sample.json
 ctgen sample/sample.toml
 ctgen sample/sample.yaml
 ```
 
 You also provide multiple theme configuration file once as following:
 
-```
+```bash
 ctgen sample/sample.toml sample/sample.json
 ```
 
 Override theme's `name` of theme with `-n` option:
 
-```
+```bash
 ctgen sample/sample.toml -n "New Theme"
 ```
 
 You can run `ctgen --help` to view all available options and you also check
 [samples](https://github.com/ful1e5/clickgen/blob/main/samples) directory for more information.
 
 ### API Examples
```

### Comparing `clickgen-2.2.2/README.md` & `clickgen-2.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,77 +13,84 @@
  https://dev.to/ful1e5/lets-give-recognition-to-those-supporting-our-work-on-github-sponsors-b00 -->
 
 ![shoutout-sponsors](https://sponsor-spotlight.vercel.app/sponsor?login=ful1e5)
 
 > **Note**
 > The project's success depends on sponsorships. Meeting sponsorship goals for [ful1e5](https://github.com/ful1e5) GitHub Account will drive new releases and ongoing development.
 
-- **2023-08-23:** `ctgen` CLI supports `.json` and `.yaml`/`.yml` as configuration file.
-- **2023-08-17:** Cursor size settings moved to `[cursors.fallback_settings]` in config. See [changelog-08172023](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-6747666)
-- **2022-06-15:** Docker Image support deprecated due to cross-platform compatibility.
-- **2022-07-09:** :warning: All the **functionality and modules are removed from older versions in `v2.0.0`**.
-  I will be restricting any updates to the `>=v1.2.0` versions to security updates and hotfixes.
-  Check updated documentations for [building cursors from API](#api-examples) and [CLIs](#usage) usage.
+-   **2024-05-24:** Clickgen now allows cursor bitmap re-canvasing by specifying size using the `cursor_size:canvas_size` format. See [changelog-05212024](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-9511166)
+-   **2023-08-23:** `ctgen` CLI supports `.json` and `.yaml`/`.yml` as configuration file.
+-   **2023-08-17:** Cursor size settings moved to `[cursors.fallback_settings]` in config. See [changelog-08172023](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-6747666)
+-   **2022-06-15:** Docker Image support deprecated due to cross-platform compatibility.
+-   **2022-07-09:** :warning: All the **functionality and modules are removed from older versions in `v2.0.0`**.
+    I will be restricting any updates to the `>=v1.2.0` versions to security updates and hotfixes.
+    Check updated documentations for [building cursors from API](#api-examples) and [CLIs](#usage) usage.
 
 ## Requirements
 
-- Python version 3.7.5 or higher
-- [Pillow](https://pypi.org/project/Pillow) >= 8.1.1
-- [PyYaml](https://pypi.org/project/PyYaml) >= 6.0.1
-- [attrs](https://pypi.org/project/attrs) >= 15.0.0
-- [numpy](https://pypi.org/project/numpy) >= 1.21.6
-- [toml](https://pypi.org/project/toml) >= 0.10.2
+-   Python version 3.7.5 or higher
+-   [Pillow](https://pypi.org/project/Pillow) >= 8.1.1
+-   [PyYaml](https://pypi.org/project/PyYaml) >= 6.0.1
+-   [attrs](https://pypi.org/project/attrs) >= 15.0.0
+-   [numpy](https://pypi.org/project/numpy) >= 1.21.6
+-   [toml](https://pypi.org/project/toml) >= 0.10.2
 
 ## Install
 
 ```bash
 pip3 install clickgen
 ```
 
 > **Note**
 > Distributions' packages are not affiliated with clickgen developers.
 > If you encounter any issues with the incorrect installation, you should contact the package maintainer first.
 
 ### Arch Linux
 
-- [AUR](https://aur.archlinux.org/packages/python-clickgen)
+-   [AUR](https://aur.archlinux.org/packages/python-clickgen)
 
 ## Usage
 
 ### `clickgen` CLI
 
 #### Linux Format (XCursor)
 
 For example, if you have to build [ponter.png](https://github.com/ful1e5/clickgen/blob/main/samples/pngs/pointer.png)
 file to Linux Format:
 
-```
+```bash
 clickgen samples/pngs/pointer.png -x 10 -y 10 -s 22 24 32 -p x11
 ```
 
 You also **build animated Xcursor** by providing multiple png files to argument and animation delay with `-d`:
 
-```
+```bash
 clickgen samples/pngs/wait-001.png samples/pngs/wait-001.png -d 3 -x 10 -y 10 -s 22 24 32 -p x11
 ```
 
 #### Windows Formats (.cur and .ani)
 
 To build [ponter.png](https://github.com/ful1e5/clickgen/blob/main/samples/pngs/pointer.png)
 file to Windows Format (`.cur`):
 
-> **Warning: Windows Cursor only support single size.**
+> **Warning: Windows Animated Cursor only support single size.**
 
-```
+```bash
 clickgen samples/pngs/pointer.png -x 10 -y 10 -s 32 -p windows
 ```
 
-For **animated Windows Cursor** (`.ani`):
+You can also specify the size in the `size:canvas_size` format to enable canvasing:
 
+```bash
+clickgen samples/pngs/pointer.png -x 10 -y 10 -s 20:32 -p windows
 ```
+
+For **animated Windows Cursor** (`.ani`):
+
+```bash
 clickgen samples/pngs/wait-001.png samples/pngs/wait-001.png -d 3 -x 10 -y 10 -s 32 -p windows
 ```
 
 For more information, run `clickgen --help`.
 
 ### `ctgen` CLI
 
@@ -93,21 +100,21 @@
 ctgen sample/sample.json
 ctgen sample/sample.toml
 ctgen sample/sample.yaml
 ```
 
 You also provide multiple theme configuration file once as following:
 
-```
+```bash
 ctgen sample/sample.toml sample/sample.json
 ```
 
 Override theme's `name` of theme with `-n` option:
 
-```
+```bash
 ctgen sample/sample.toml -n "New Theme"
 ```
 
 You can run `ctgen --help` to view all available options and you also check
 [samples](https://github.com/ful1e5/clickgen/blob/main/samples) directory for more information.
 
 ### API Examples
```

### Comparing `clickgen-2.2.2/pyproject.toml` & `clickgen-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/setup.cfg` & `clickgen-2.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen/configparser.py` & `clickgen-2.2.3/src/clickgen/configparser.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen/configparser.pyi` & `clickgen-2.2.3/src/clickgen/configparser.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 from clickgen.libs.colors import print_warning as print_warning
 from clickgen.parser import open_blob as open_blob
 from clickgen.parser.png import DELAY as DELAY, SIZES as SIZES
 from clickgen.writer.windows import to_win as to_win
 from clickgen.writer.x11 import to_x11 as to_x11
 from pathlib import Path
-from typing import Any, Dict, List, TypeVar
+from typing import Any, TypeVar
 
 class ThemeSection:
     name: str
     comment: str
     website: str
     def __init__(self, name, comment, website) -> None: ...
     def __lt__(self, other): ...
     def __le__(self, other): ...
     def __gt__(self, other): ...
     def __ge__(self, other): ...
 
-def parse_theme_section(d: Dict[str, Any], **kwargs) -> ThemeSection: ...
+def parse_theme_section(d: dict[str, Any], **kwargs) -> ThemeSection: ...
 
 class ConfigSection:
     bitmaps_dir: Path
     out_dir: Path
-    platforms: List[str]
+    platforms: list[str]
     def __init__(self, bitmaps_dir, out_dir, platforms) -> None: ...
     def __lt__(self, other): ...
     def __le__(self, other): ...
     def __gt__(self, other): ...
     def __ge__(self, other): ...
 
-def parse_config_section(fp: Path, d: Dict[str, Any], **kwargs) -> ConfigSection: ...
+def parse_config_section(fp: Path, d: dict[str, Any], **kwargs) -> ConfigSection: ...
 T = TypeVar('T')
 
 class CursorSection:
     x11_cursor_name: str | None
     x11_cursor: bytes | None
-    x11_symlinks: List[str]
+    x11_symlinks: list[str]
     win_cursor_name: str | None
     win_cursor: bytes | None
     def __init__(self, x11_cursor_name, x11_cursor, x11_symlinks, win_cursor_name, win_cursor) -> None: ...
     def __lt__(self, other): ...
     def __le__(self, other): ...
     def __gt__(self, other): ...
     def __ge__(self, other): ...
 
-def parse_cursors_section(d: Dict[str, Any], config: ConfigSection, **kwargs) -> List[CursorSection]: ...
+def parse_cursors_section(d: dict[str, Any], config: ConfigSection, **kwargs) -> list[CursorSection]: ...
 
 class ClickgenConfig:
     theme: ThemeSection
     config: ConfigSection
-    cursors: List[CursorSection]
+    cursors: list[CursorSection]
     def __init__(self, theme, config, cursors) -> None: ...
     def __lt__(self, other): ...
     def __le__(self, other): ...
     def __gt__(self, other): ...
     def __ge__(self, other): ...
 
 def parse_toml_file(fp: Path, **kwargs) -> ClickgenConfig: ...
```

### Comparing `clickgen-2.2.2/src/clickgen/cursors.py` & `clickgen-2.2.3/src/clickgen/cursors.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,30 @@
 from PIL.Image import Image
 
 
 class CursorImage:
     image: Image
     hotspot: Tuple[int, int]
     nominal: int
+    re_canvas: bool
 
-    def __init__(self, image: Image, hotspot: Tuple[int, int], nominal: int) -> None:
+    def __init__(
+        self,
+        image: Image,
+        hotspot: Tuple[int, int],
+        nominal: int,
+        re_canvas: bool = False,
+    ) -> None:
         self.image = image
         self.hotspot = hotspot
         self.nominal = nominal
+        self.re_canvas = re_canvas
 
     def __repr__(self) -> str:
-        return f"CursorImage(image={self.image!r}, hotspot={self.hotspot!r}, nominal={self.nominal!r})"
+        return f"CursorImage(image={self.image!r}, hotspot={self.hotspot!r}, nominal={self.nominal!r}, re_canvas={self.re_canvas!r})"
 
 
 class CursorFrame:
     images: List[CursorImage]
     delay: int
 
     def __init__(self, images: List[CursorImage], delay: int = 0) -> None:
```

### Comparing `clickgen-2.2.2/src/clickgen/cursors.pyi` & `clickgen-2.2.3/src/clickgen/cursors.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from PIL.Image import Image as Image
-from typing import Iterator, List, Tuple
+from typing import Iterator
 
 class CursorImage:
     image: Image
-    hotspot: Tuple[int, int]
+    hotspot: tuple[int, int]
     nominal: int
-    def __init__(self, image: Image, hotspot: Tuple[int, int], nominal: int) -> None: ...
+    re_canvas: bool
+    def __init__(self, image: Image, hotspot: tuple[int, int], nominal: int, re_canvas: bool = False) -> None: ...
 
 class CursorFrame:
-    images: List[CursorImage]
+    images: list[CursorImage]
     delay: int
-    def __init__(self, images: List[CursorImage], delay: int = 0) -> None: ...
+    def __init__(self, images: list[CursorImage], delay: int = 0) -> None: ...
     def __getitem__(self, item: int) -> CursorImage: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[CursorImage]: ...
```

### Comparing `clickgen-2.2.2/src/clickgen/libs/colors.py` & `clickgen-2.2.3/src/clickgen/libs/colors.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen/libs/colors.pyi` & `clickgen-2.2.3/src/clickgen/libs/colors.pyi`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen/packer/windows.py` & `clickgen-2.2.3/src/clickgen/packer/windows.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen/packer/x11.py` & `clickgen-2.2.3/src/clickgen/packer/x11.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen/parser/__init__.py` & `clickgen-2.2.3/src/clickgen/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen/parser/png.pyi` & `clickgen-2.2.3/src/clickgen/parser/png.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from _typeshed import Incomplete
 from clickgen.cursors import CursorFrame as CursorFrame, CursorImage as CursorImage
 from clickgen.parser.base import BaseParser as BaseParser
-from typing import List, Tuple
 
 SIZES: Incomplete
 DELAY: int
 
 class SinglePNGParser(BaseParser):
     MAGIC: Incomplete
     @classmethod
     def can_parse(cls, blob: bytes) -> bool: ...
     sizes: Incomplete
     delay: Incomplete
     hotspot: Incomplete
     frames: Incomplete
-    def __init__(self, blob: bytes, hotspot: Tuple[int, int], sizes: List[int] | None = None, delay: int | None = None) -> None: ...
+    def __init__(self, blob: bytes, hotspot: tuple[int, int], sizes: list[int | str] | None = None, delay: int | None = None) -> None: ...
 
 class MultiPNGParser(BaseParser):
     @classmethod
-    def can_parse(cls, blobs: List[bytes]) -> bool: ...
+    def can_parse(cls, blobs: list[bytes]) -> bool: ...
     frames: Incomplete
-    def __init__(self, blobs: List[bytes], hotspot: Tuple[int, int], sizes: List[int] | None = None, delay: int | None = None) -> None: ...
+    def __init__(self, blobs: list[bytes], hotspot: tuple[int, int], sizes: list[int | str] | None = None, delay: int | None = None) -> None: ...
```

### Comparing `clickgen-2.2.2/src/clickgen/scripts/clickgen.py` & `clickgen-2.2.3/src/clickgen/scripts/clickgen.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,16 +58,17 @@
     )
     parser.add_argument(
         "-s",
         "--sizes",
         dest="sizes",
         nargs="+",
         default=SIZES,
-        type=int,
-        help="Set pixel-size for cursor.",
+        type=str,
+        help="""Specify the cursor size(s) either as a single integer value or
+        in the 'size:canvas_size' format to resize the cursor to a specific canvas size.""",
     )
     parser.add_argument(
         "-d",
         "--delay",
         default=DELAY,
         type=int,
         help="Set delay between frames of cursor.",
```

### Comparing `clickgen-2.2.2/src/clickgen/scripts/ctgen.py` & `clickgen-2.2.3/src/clickgen/scripts/ctgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,17 @@
 
     parser.add_argument(
         "-s",
         "--sizes",
         dest="sizes",
         nargs="+",
         default=None,
-        type=int,
-        help=""" Change cursor size.
-        Multiple sizes are assigned to XCursor
-        while one size will be assigned to Windows.""",
+        type=str,
+        help="""Specify the cursor size(s) either as a single integer value or
+        in the 'size:canvas_size' format to resize the cursor to a specific canvas size.""",
     )
 
     parser.add_argument(
         "-p",
         "--platforms",
         choices=["windows", "x11"],
         default=None,
```

### Comparing `clickgen-2.2.2/src/clickgen/scripts/ctgen.pyi` & `clickgen-2.2.3/src/clickgen/scripts/ctgen.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from clickgen.configparser import parse_config_file as parse_config_file
 from clickgen.libs.colors import blue as blue, bold as bold, cyan as cyan, fail as fail, magenta as magenta, print_done as print_done, print_info as print_info, print_subtext as print_subtext, print_text as print_text
 from clickgen.packer.windows import pack_win as pack_win
 from clickgen.packer.x11 import pack_x11 as pack_x11
-from typing import Any, Dict, Generator
+from typing import Any, Generator
 
-def get_kwargs(args) -> Dict[str, Any]: ...
+def get_kwargs(args) -> dict[str, Any]: ...
 def cwd(path) -> Generator[None, None, None]: ...
 def main() -> None: ...
```

### Comparing `clickgen-2.2.2/src/clickgen/writer/windows.py` & `clickgen-2.2.3/src/clickgen/writer/windows.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,28 +43,29 @@
         # |   48 |              32 |     38.4 → 39 |                48 |
         # |   64 |     42.666 → 43 |     51.2 → 52 |                64 |
         # |   96 |              64 |     76.8 → 77 |                96 |
         # |  128 |     85.333 → 86 |   102.4 → 103 |               128 |
         # |  256 |   170.666 → 171 |   204.8 → 205 |               256 |
 
         blob = BytesIO()
-        if width <= 32 or height <= 32:
-            re_canvas(32, clone).save(blob, "PNG")
-        elif width <= 48 or height <= 48:
-            re_canvas(48, clone).save(blob, "PNG")
-        elif width <= 64 or height <= 64:
-            re_canvas(64, clone).save(blob, "PNG")
-        elif width <= 96 or height <= 96:
-            re_canvas(96, clone).save(blob, "PNG")
-        elif width <= 128 or height <= 128:
-            re_canvas(128, clone).save(blob, "PNG")
-        elif width <= 256 or height <= 256:
-            re_canvas(256, clone).save(blob, "PNG")
+        if not image.re_canvas:
+            if width <= 32 or height <= 32:
+                re_canvas(32, clone).save(blob, "PNG")
+            elif width <= 48 or height <= 48:
+                re_canvas(48, clone).save(blob, "PNG")
+            elif width <= 64 or height <= 64:
+                re_canvas(64, clone).save(blob, "PNG")
+            elif width <= 96 or height <= 96:
+                re_canvas(96, clone).save(blob, "PNG")
+            elif width <= 128 or height <= 128:
+                re_canvas(128, clone).save(blob, "PNG")
+            else:
+                re_canvas(256, clone).save(blob, "PNG")
         else:
-            raise ValueError(f"Unable to re-canvas windows cursors: {width}x{height}")
+            image.image.save(blob, "PNG")
 
         blob.seek(0)
         image_data.append(blob.read())
         x_offset, y_offset = image.hotspot
         directory.append(
             ICON_DIR_ENTRY.pack(
                 height & 0xFF,
```

### Comparing `clickgen-2.2.2/src/clickgen/writer/windows.pyi` & `clickgen-2.2.3/src/clickgen/writer/windows.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from _typeshed import Incomplete
 from clickgen.cursors import CursorFrame as CursorFrame
-from typing import List, Tuple
 
 MAGIC: bytes
 ICO_TYPE_CUR: int
 ICON_DIR: Incomplete
 ICON_DIR_ENTRY: Incomplete
 
 def to_cur(frame: CursorFrame) -> bytes: ...
@@ -20,11 +19,11 @@
 RIFF_HEADER: Incomplete
 CHUNK_HEADER: Incomplete
 ANIH_HEADER: Incomplete
 UNSIGNED: Incomplete
 SEQUENCE_FLAG: int
 ICON_FLAG: int
 
-def get_ani_cur_list(frames: List[CursorFrame]) -> bytes: ...
-def get_ani_rate_chunk(frames: List[CursorFrame]) -> bytes: ...
-def to_ani(frames: List[CursorFrame]) -> bytes: ...
-def to_win(frames: List[CursorFrame]) -> Tuple[str, bytes]: ...
+def get_ani_cur_list(frames: list[CursorFrame]) -> bytes: ...
+def get_ani_rate_chunk(frames: list[CursorFrame]) -> bytes: ...
+def to_ani(frames: list[CursorFrame]) -> bytes: ...
+def to_win(frames: list[CursorFrame]) -> tuple[str, bytes]: ...
```

### Comparing `clickgen-2.2.2/src/clickgen/writer/x11.py` & `clickgen-2.2.3/src/clickgen/writer/x11.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/src/clickgen.egg-info/PKG-INFO` & `clickgen-2.2.3/src/clickgen.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickgen
-Version: 2.2.2
+Version: 2.2.3
 Summary: The hassle-free cursor building toolbox.
 Home-page: https://github.com/ful1e5/clickgen
 Author: Abdulkaiz Khatri
 Author-email: kaizmandhu@gmail.com
 Project-URL: Source, https://github.com/ful1e5/clickgen
 Project-URL: Download, https://pypi.org/project/clickgen/#files
 Project-URL: Bug Tracker, https://github.com/ful1e5/clickgen/issues
@@ -59,77 +59,84 @@
  https://dev.to/ful1e5/lets-give-recognition-to-those-supporting-our-work-on-github-sponsors-b00 -->
 
 ![shoutout-sponsors](https://sponsor-spotlight.vercel.app/sponsor?login=ful1e5)
 
 > **Note**
 > The project's success depends on sponsorships. Meeting sponsorship goals for [ful1e5](https://github.com/ful1e5) GitHub Account will drive new releases and ongoing development.
 
-- **2023-08-23:** `ctgen` CLI supports `.json` and `.yaml`/`.yml` as configuration file.
-- **2023-08-17:** Cursor size settings moved to `[cursors.fallback_settings]` in config. See [changelog-08172023](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-6747666)
-- **2022-06-15:** Docker Image support deprecated due to cross-platform compatibility.
-- **2022-07-09:** :warning: All the **functionality and modules are removed from older versions in `v2.0.0`**.
-  I will be restricting any updates to the `>=v1.2.0` versions to security updates and hotfixes.
-  Check updated documentations for [building cursors from API](#api-examples) and [CLIs](#usage) usage.
+-   **2024-05-24:** Clickgen now allows cursor bitmap re-canvasing by specifying size using the `cursor_size:canvas_size` format. See [changelog-05212024](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-9511166)
+-   **2023-08-23:** `ctgen` CLI supports `.json` and `.yaml`/`.yml` as configuration file.
+-   **2023-08-17:** Cursor size settings moved to `[cursors.fallback_settings]` in config. See [changelog-08172023](https://github.com/ful1e5/clickgen/discussions/59#discussioncomment-6747666)
+-   **2022-06-15:** Docker Image support deprecated due to cross-platform compatibility.
+-   **2022-07-09:** :warning: All the **functionality and modules are removed from older versions in `v2.0.0`**.
+    I will be restricting any updates to the `>=v1.2.0` versions to security updates and hotfixes.
+    Check updated documentations for [building cursors from API](#api-examples) and [CLIs](#usage) usage.
 
 ## Requirements
 
-- Python version 3.7.5 or higher
-- [Pillow](https://pypi.org/project/Pillow) >= 8.1.1
-- [PyYaml](https://pypi.org/project/PyYaml) >= 6.0.1
-- [attrs](https://pypi.org/project/attrs) >= 15.0.0
-- [numpy](https://pypi.org/project/numpy) >= 1.21.6
-- [toml](https://pypi.org/project/toml) >= 0.10.2
+-   Python version 3.7.5 or higher
+-   [Pillow](https://pypi.org/project/Pillow) >= 8.1.1
+-   [PyYaml](https://pypi.org/project/PyYaml) >= 6.0.1
+-   [attrs](https://pypi.org/project/attrs) >= 15.0.0
+-   [numpy](https://pypi.org/project/numpy) >= 1.21.6
+-   [toml](https://pypi.org/project/toml) >= 0.10.2
 
 ## Install
 
 ```bash
 pip3 install clickgen
 ```
 
 > **Note**
 > Distributions' packages are not affiliated with clickgen developers.
 > If you encounter any issues with the incorrect installation, you should contact the package maintainer first.
 
 ### Arch Linux
 
-- [AUR](https://aur.archlinux.org/packages/python-clickgen)
+-   [AUR](https://aur.archlinux.org/packages/python-clickgen)
 
 ## Usage
 
 ### `clickgen` CLI
 
 #### Linux Format (XCursor)
 
 For example, if you have to build [ponter.png](https://github.com/ful1e5/clickgen/blob/main/samples/pngs/pointer.png)
 file to Linux Format:
 
-```
+```bash
 clickgen samples/pngs/pointer.png -x 10 -y 10 -s 22 24 32 -p x11
 ```
 
 You also **build animated Xcursor** by providing multiple png files to argument and animation delay with `-d`:
 
-```
+```bash
 clickgen samples/pngs/wait-001.png samples/pngs/wait-001.png -d 3 -x 10 -y 10 -s 22 24 32 -p x11
 ```
 
 #### Windows Formats (.cur and .ani)
 
 To build [ponter.png](https://github.com/ful1e5/clickgen/blob/main/samples/pngs/pointer.png)
 file to Windows Format (`.cur`):
 
-> **Warning: Windows Cursor only support single size.**
+> **Warning: Windows Animated Cursor only support single size.**
 
-```
+```bash
 clickgen samples/pngs/pointer.png -x 10 -y 10 -s 32 -p windows
 ```
 
-For **animated Windows Cursor** (`.ani`):
+You can also specify the size in the `size:canvas_size` format to enable canvasing:
 
+```bash
+clickgen samples/pngs/pointer.png -x 10 -y 10 -s 20:32 -p windows
 ```
+
+For **animated Windows Cursor** (`.ani`):
+
+```bash
 clickgen samples/pngs/wait-001.png samples/pngs/wait-001.png -d 3 -x 10 -y 10 -s 32 -p windows
 ```
 
 For more information, run `clickgen --help`.
 
 ### `ctgen` CLI
 
@@ -139,21 +146,21 @@
 ctgen sample/sample.json
 ctgen sample/sample.toml
 ctgen sample/sample.yaml
 ```
 
 You also provide multiple theme configuration file once as following:
 
-```
+```bash
 ctgen sample/sample.toml sample/sample.json
 ```
 
 Override theme's `name` of theme with `-n` option:
 
-```
+```bash
 ctgen sample/sample.toml -n "New Theme"
 ```
 
 You can run `ctgen --help` to view all available options and you also check
 [samples](https://github.com/ful1e5/clickgen/blob/main/samples) directory for more information.
 
 ### API Examples
```

### Comparing `clickgen-2.2.2/src/clickgen.egg-info/SOURCES.txt` & `clickgen-2.2.3/src/clickgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/tests/test_configparser.py` & `clickgen-2.2.3/tests/test_configparser.py`

 * *Files identical despite different names*

### Comparing `clickgen-2.2.2/tests/test_cursors.py` & `clickgen-2.2.3/tests/test_cursors.py`

 * *Files identical despite different names*

