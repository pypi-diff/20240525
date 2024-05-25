# Comparing `tmp/fdlogger-24.5.21.tar.gz` & `tmp/fdlogger-24.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdlogger-24.5.21.tar", last modified: Tue May 21 16:58:51 2024, max compression
+gzip compressed data, was "fdlogger-24.5.25.tar", last modified: Sat May 25 16:07:31 2024, max compression
```

## Comparing `fdlogger-24.5.21.tar` & `fdlogger-24.5.25.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.910135 fdlogger-24.5.21/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-05-21 16:05:29.000000 fdlogger-24.5.21/LICENSE
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22907 2024-05-21 16:58:51.909135 fdlogger-24.5.21/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22023 2024-05-21 16:50:55.000000 fdlogger-24.5.21/README.md
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.884135 fdlogger-24.5.21/fdlogger/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   113266 2024-05-21 16:43:49.000000 fdlogger-24.5.21/fdlogger/__main__.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.893135 fdlogger-24.5.21/fdlogger/data/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/JetBrainsMono-Regular.ttf
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/MASTER.SCP
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3051 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/arrl_sect.dat
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/cwmacros_fd.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/dialog.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/fd_preferences.json
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/k6gte-fieldday.desktop
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)   108154 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/main.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/opon.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    31170 2024-05-21 16:29:04.000000 fdlogger-24.5.21/fdlogger/data/settings.ui
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/data/startup.ui
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.897135 fdlogger-24.5.21/fdlogger/icon/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/cloud_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/cloud_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/cloud_red.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/gear16x16.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/k6gte-fdlogger.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/logo.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio.svg
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio_green.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio_grey.png
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/icon/radio_red.png
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.902135 fdlogger-24.5.21/fdlogger/lib/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/__init__.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11160 2024-05-21 16:07:31.000000 fdlogger-24.5.21/fdlogger/lib/cat_interface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/cwinterface.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13600 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/database.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/edit_opon.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/lookup.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4949 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/n1mm.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6922 2024-05-21 16:35:17.000000 fdlogger-24.5.21/fdlogger/lib/settings.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-05-21 16:45:04.000000 fdlogger-24.5.21/fdlogger/lib/version.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2024-05-21 16:05:29.000000 fdlogger-24.5.21/fdlogger/lib/versiontest.py
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.908135 fdlogger-24.5.21/fdlogger.egg-info/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22907 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/PKG-INFO
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1218 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/SOURCES.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/dependency_links.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/entry_points.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/requires.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       40 2024-05-21 16:58:51.000000 fdlogger-24.5.21/fdlogger.egg-info/top_level.txt
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1180 2024-05-21 16:45:04.000000 fdlogger-24.5.21/pyproject.toml
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-05-21 16:58:51.910135 fdlogger-24.5.21/setup.cfg
-drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:58:51.905135 fdlogger-24.5.21/testing/
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/inject_multicast.py
--rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/inject_udp.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/multicast_listener.py
--rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2024-05-21 16:05:29.000000 fdlogger-24.5.21/testing/simulant.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-25 16:07:31.625788 fdlogger-24.5.25/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    35149 2024-05-21 16:05:29.000000 fdlogger-24.5.25/LICENSE
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22959 2024-05-25 16:07:31.624788 fdlogger-24.5.25/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22075 2024-05-25 16:07:08.000000 fdlogger-24.5.25/README.md
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-25 16:07:31.556788 fdlogger-24.5.25/fdlogger/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   113347 2024-05-25 16:07:08.000000 fdlogger-24.5.25/fdlogger/__main__.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-25 16:07:31.608788 fdlogger-24.5.25/fdlogger/data/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   203952 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/JetBrainsMono-Regular.ttf
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   331983 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/MASTER.SCP
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3051 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/arrl_sect.dat
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/cwmacros_fd.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    10325 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/dialog.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      592 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/fd_preferences.json
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      213 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/k6gte-fieldday.desktop
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)   108154 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/main.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2247 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/opon.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    31170 2024-05-21 16:29:04.000000 fdlogger-24.5.25/fdlogger/data/settings.ui
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     3812 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/data/startup.ui
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-25 16:07:31.615788 fdlogger-24.5.25/fdlogger/icon/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      626 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/cloud_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      641 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/cloud_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      482 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/cloud_red.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      605 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/gear16x16.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2876 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/k6gte-fdlogger.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    96313 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/logo.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     5972 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/radio.svg
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1234 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/radio_green.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1258 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/radio_grey.png
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      957 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/icon/radio_red.png
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-25 16:07:31.621788 fdlogger-24.5.25/fdlogger/lib/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        0 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/lib/__init__.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    11160 2024-05-21 16:07:31.000000 fdlogger-24.5.25/fdlogger/lib/cat_interface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1661 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/lib/cwinterface.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    13600 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/lib/database.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      363 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/lib/edit_opon.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    14064 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/lib/lookup.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     4949 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/lib/n1mm.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     6922 2024-05-21 16:35:17.000000 fdlogger-24.5.25/fdlogger/lib/settings.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       47 2024-05-25 16:07:08.000000 fdlogger-24.5.25/fdlogger/lib/version.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1289 2024-05-21 16:05:29.000000 fdlogger-24.5.25/fdlogger/lib/versiontest.py
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-25 16:07:31.623788 fdlogger-24.5.25/fdlogger.egg-info/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)    22959 2024-05-25 16:07:31.000000 fdlogger-24.5.25/fdlogger.egg-info/PKG-INFO
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1218 2024-05-25 16:07:31.000000 fdlogger-24.5.25/fdlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)        1 2024-05-25 16:07:31.000000 fdlogger-24.5.25/fdlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       51 2024-05-25 16:07:31.000000 fdlogger-24.5.25/fdlogger.egg-info/entry_points.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       35 2024-05-25 16:07:31.000000 fdlogger-24.5.25/fdlogger.egg-info/requires.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       40 2024-05-25 16:07:31.000000 fdlogger-24.5.25/fdlogger.egg-info/top_level.txt
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     1180 2024-05-25 16:07:08.000000 fdlogger-24.5.25/pyproject.toml
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)       38 2024-05-25 16:07:31.625788 fdlogger-24.5.25/setup.cfg
+drwxr-xr-x   0 mbridak   (1000) mbridak   (1000)        0 2024-05-25 16:07:31.623788 fdlogger-24.5.25/testing/
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)     2714 2024-05-21 16:05:29.000000 fdlogger-24.5.25/testing/inject_multicast.py
+-rw-r--r--   0 mbridak   (1000) mbridak   (1000)      862 2024-05-21 16:05:29.000000 fdlogger-24.5.25/testing/inject_udp.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)     1051 2024-05-21 16:05:29.000000 fdlogger-24.5.25/testing/multicast_listener.py
+-rwxr-xr-x   0 mbridak   (1000) mbridak   (1000)    10948 2024-05-21 16:05:29.000000 fdlogger-24.5.25/testing/simulant.py
```

### Comparing `fdlogger-24.5.21/LICENSE` & `fdlogger-24.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/PKG-INFO` & `fdlogger-24.5.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 24.5.21
+Version: 24.5.25
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -98,14 +98,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [24.5.25] Fixed crash changing modes with no CAT.
 - [24.5.21] Add sending CW via CAT(rigctld)
 - [24.2.21] Added OPON.
 - [24.2.19] Corrected the datetime.utcnow() deprecation to work on Python 3.9+
 - [24.2.11] Trapped a KeyError in get_state()
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23.11.9] Merged from @wvolz fixing crash related to tuning to a non ham band.
 - [23.6.25] Fixed missing Canadian sections.
```

### Comparing `fdlogger-24.5.21/README.md` & `fdlogger-24.5.25/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [24.5.25] Fixed crash changing modes with no CAT.
 - [24.5.21] Add sending CW via CAT(rigctld)
 - [24.2.21] Added OPON.
 - [24.2.19] Corrected the datetime.utcnow() deprecation to work on Python 3.9+
 - [24.2.11] Trapped a KeyError in get_state()
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23.11.9] Merged from @wvolz fixing crash related to tuning to a non ham band.
 - [23.6.25] Fixed missing Canadian sections.
```

### Comparing `fdlogger-24.5.21/fdlogger/__main__.py` & `fdlogger-24.5.25/fdlogger/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1366,30 +1366,31 @@
         self.section_entry.clear()
         self.callsign_entry.setFocus()
 
     def changeband(self):
         """change band"""
         if self.band != self.band_selector.currentText():
             self.band = self.band_selector.currentText()
-            if self.cat_control:
+            if self.cat_control is not None:
                 self.cat_control.set_vfo(
                     int(float(self.fakefreq(self.band, self.mode)) * 1000)
                 )
             self.send_status_udp()
 
     def changemode(self):
         """change mode"""
         if self.mode != self.mode_selector.currentText():
             self.mode = self.mode_selector.currentText()
-            if self.mode == "PH":
-                if int(self.oldfreq) < 10000000:
-                    self.cat_control.set_mode("LSB")
-                else:
-                    self.cat_control.set_mode("USB")
-            self.cat_control.set_mode(self.mode)
+            if self.cat_control is not None:
+                if self.mode == "PH":
+                    if int(self.oldfreq) < 10000000:
+                        self.cat_control.set_mode("LSB")
+                    else:
+                        self.cat_control.set_mode("USB")
+                self.cat_control.set_mode(self.mode)
             self.send_status_udp()
 
     def changepower(self):
         """change power"""
         self.preference["power"] = str(self.power_selector.value())
         self.writepreferences()
```

### Comparing `fdlogger-24.5.21/fdlogger/data/JetBrainsMono-Regular.ttf` & `fdlogger-24.5.25/fdlogger/data/JetBrainsMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/MASTER.SCP` & `fdlogger-24.5.25/fdlogger/data/MASTER.SCP`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/arrl_sect.dat` & `fdlogger-24.5.25/fdlogger/data/arrl_sect.dat`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/dialog.ui` & `fdlogger-24.5.25/fdlogger/data/dialog.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/fd_preferences.json` & `fdlogger-24.5.25/fdlogger/data/fd_preferences.json`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/main.ui` & `fdlogger-24.5.25/fdlogger/data/main.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/opon.ui` & `fdlogger-24.5.25/fdlogger/data/opon.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/settings.ui` & `fdlogger-24.5.25/fdlogger/data/settings.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/data/startup.ui` & `fdlogger-24.5.25/fdlogger/data/startup.ui`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/cloud_green.png` & `fdlogger-24.5.25/fdlogger/icon/cloud_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/cloud_grey.png` & `fdlogger-24.5.25/fdlogger/icon/cloud_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/gear16x16.png` & `fdlogger-24.5.25/fdlogger/icon/gear16x16.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/k6gte-fdlogger.png` & `fdlogger-24.5.25/fdlogger/icon/k6gte-fdlogger.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/logo.png` & `fdlogger-24.5.25/fdlogger/icon/logo.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/radio.svg` & `fdlogger-24.5.25/fdlogger/icon/radio.svg`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/radio_green.png` & `fdlogger-24.5.25/fdlogger/icon/radio_green.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/radio_grey.png` & `fdlogger-24.5.25/fdlogger/icon/radio_grey.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/icon/radio_red.png` & `fdlogger-24.5.25/fdlogger/icon/radio_red.png`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/lib/cat_interface.py` & `fdlogger-24.5.25/fdlogger/lib/cat_interface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/lib/cwinterface.py` & `fdlogger-24.5.25/fdlogger/lib/cwinterface.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/lib/database.py` & `fdlogger-24.5.25/fdlogger/lib/database.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/lib/lookup.py` & `fdlogger-24.5.25/fdlogger/lib/lookup.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/lib/n1mm.py` & `fdlogger-24.5.25/fdlogger/lib/n1mm.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/lib/settings.py` & `fdlogger-24.5.25/fdlogger/lib/settings.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger/lib/versiontest.py` & `fdlogger-24.5.25/fdlogger/lib/versiontest.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/fdlogger.egg-info/PKG-INFO` & `fdlogger-24.5.25/fdlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdlogger
-Version: 24.5.21
+Version: 24.5.25
 Summary: ARRL Field Day logger GUI
 Author-email: Michael Bridak <michael.bridak@gmail.com>
 Project-URL: Homepage, https://github.com/mbridak/FieldDayLogger
 Project-URL: Bug Tracker, https://github.com/mbridak/FieldDayLogger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -98,14 +98,15 @@
 Just search for the two places in the code 'FT8' is used and Bob's your dads
 brother.
 
 **WB8ERJ's blog writeup** [Mike's Tech Blog WB8ERJ](https://mikestechblog.com/field-day-logging-software-for-the-raspberry-pi/)
 
 ## Recent Changes
 
+- [24.5.25] Fixed crash changing modes with no CAT.
 - [24.5.21] Add sending CW via CAT(rigctld)
 - [24.2.21] Added OPON.
 - [24.2.19] Corrected the datetime.utcnow() deprecation to work on Python 3.9+
 - [24.2.11] Trapped a KeyError in get_state()
 - [24.1.27] Removed some datetime.utcnow() and pkgutil.getloader() deprecations.
 - [23.11.9] Merged from @wvolz fixing crash related to tuning to a non ham band.
 - [23.6.25] Fixed missing Canadian sections.
```

### Comparing `fdlogger-24.5.21/fdlogger.egg-info/SOURCES.txt` & `fdlogger-24.5.25/fdlogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/pyproject.toml` & `fdlogger-24.5.25/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fdlogger" 
-version = "24.5.21"
+version = "24.5.25"
 description = "ARRL Field Day logger GUI"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   { name="Michael Bridak", email="michael.bridak@gmail.com" },
 ]
 dependencies = [
```

### Comparing `fdlogger-24.5.21/testing/inject_multicast.py` & `fdlogger-24.5.25/testing/inject_multicast.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/testing/inject_udp.py` & `fdlogger-24.5.25/testing/inject_udp.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/testing/multicast_listener.py` & `fdlogger-24.5.25/testing/multicast_listener.py`

 * *Files identical despite different names*

### Comparing `fdlogger-24.5.21/testing/simulant.py` & `fdlogger-24.5.25/testing/simulant.py`

 * *Files identical despite different names*

