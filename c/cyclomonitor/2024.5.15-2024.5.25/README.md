# Comparing `tmp/cyclomonitor-2024.5.15.tar.gz` & `tmp/cyclomonitor-2024.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclomonitor-2024.5.15.tar", last modified: Wed May 15 12:38:09 2024, max compression
+gzip compressed data, was "cyclomonitor-2024.5.25.tar", last modified: Sat May 25 12:41:32 2024, max compression
```

## Comparing `cyclomonitor-2024.5.15.tar` & `cyclomonitor-2024.5.25.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/LICENSE
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.5.15/MANIFEST.in
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43427 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/PKG-INFO
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     2069 2024-05-13 03:01:31.000000 cyclomonitor-2024.5.15/README.md
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/privacy-policy.md
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1574 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/pyproject.toml
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       15 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/requirements.txt
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/setup.cfg
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1834 2024-05-15 12:35:47.000000 cyclomonitor-2024.5.15/setup.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.630746 cyclomonitor-2024.5.15/src/
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.634745 cyclomonitor-2024.5.15/src/cyclomonitor/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      189 2024-04-15 00:43:27.000000 cyclomonitor-2024.5.15/src/cyclomonitor/__init__.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     4713 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/src/cyclomonitor/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10874 2024-05-15 12:28:39.000000 cyclomonitor-2024.5.15/src/cyclomonitor/atcf.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    12462 2024-05-15 12:29:29.000000 cyclomonitor-2024.5.15/src/cyclomonitor/cli.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    35681 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.15/src/cyclomonitor/cyclomonitor.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/src/cyclomonitor/dir_calc.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.15/src/cyclomonitor/errors.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/global_vars.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.634745 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    13524 2024-05-13 23:52:17.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/__main__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5008 2024-05-13 23:49:26.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5012 2024-05-13 23:49:25.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/C.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/__init__.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/en_US.json
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/src/cyclomonitor/locales/
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.15/src/cyclomonitor/locales/C.json
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     7862 2024-05-13 22:50:42.000000 cyclomonitor-2024.5.15/src/cyclomonitor/locales/__init__.py
--rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.15/src/cyclomonitor/locales/en_US.json
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/server_vars.py
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.15/src/cyclomonitor/uptime.py
-drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-15 12:38:09.638745 cyclomonitor-2024.5.15/src/cyclomonitor.egg-info/
--rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      767 2024-05-15 12:38:09.000000 cyclomonitor-2024.5.15/src/cyclomonitor.egg-info/SOURCES.txt
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-25 12:41:32.496550 cyclomonitor-2024.5.25/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    34523 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.25/LICENSE
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      263 2024-04-14 18:11:55.000000 cyclomonitor-2024.5.25/MANIFEST.in
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    43427 2024-05-25 12:41:32.496550 cyclomonitor-2024.5.25/PKG-INFO
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     2069 2024-05-13 03:01:31.000000 cyclomonitor-2024.5.25/README.md
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      640 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.25/privacy-policy.md
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1574 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.25/pyproject.toml
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       15 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.25/requirements.txt
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)       38 2024-05-25 12:41:32.496550 cyclomonitor-2024.5.25/setup.cfg
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     1834 2024-05-25 12:36:39.000000 cyclomonitor-2024.5.25/setup.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-25 12:41:32.480550 cyclomonitor-2024.5.25/src/
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-25 12:41:32.488550 cyclomonitor-2024.5.25/src/cyclomonitor/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      270 2024-05-22 11:35:46.000000 cyclomonitor-2024.5.25/src/cyclomonitor/__init__.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     4713 2024-05-12 22:10:41.000000 cyclomonitor-2024.5.25/src/cyclomonitor/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    10708 2024-05-25 00:26:07.000000 cyclomonitor-2024.5.25/src/cyclomonitor/atcf.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    12287 2024-05-25 12:25:52.000000 cyclomonitor-2024.5.25/src/cyclomonitor/cli.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    36066 2024-05-22 11:48:07.000000 cyclomonitor-2024.5.25/src/cyclomonitor/cyclomonitor.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1050 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.25/src/cyclomonitor/dir_calc.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      239 2024-03-22 16:35:02.000000 cyclomonitor-2024.5.25/src/cyclomonitor/errors.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      801 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.25/src/cyclomonitor/global_vars.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-25 12:41:32.492550 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)    13524 2024-05-13 23:52:17.000000 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      185 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/__main__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5008 2024-05-13 23:49:26.000000 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/ibtracs_ALL.sql
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     5012 2024-05-13 23:49:25.000000 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-25 12:41:32.492550 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/locales/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/locales/C.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1945 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/locales/__init__.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1381 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/locales/en_US.json
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-25 12:41:32.496550 cyclomonitor-2024.5.25/src/cyclomonitor/locales/
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.25/src/cyclomonitor/locales/C.json
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)     7862 2024-05-13 22:50:42.000000 cyclomonitor-2024.5.25/src/cyclomonitor/locales/__init__.py
+-rw-rw-r--   0 ntvmb     (1000) ntvmb     (1000)    14230 2024-05-13 22:53:22.000000 cyclomonitor-2024.5.25/src/cyclomonitor/locales/en_US.json
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1794 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.25/src/cyclomonitor/server_vars.py
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)     1192 2024-04-14 12:39:59.000000 cyclomonitor-2024.5.25/src/cyclomonitor/uptime.py
+drwxrwxr-x   0 ntvmb     (1000) ntvmb     (1000)        0 2024-05-25 12:41:32.496550 cyclomonitor-2024.5.25/src/cyclomonitor.egg-info/
+-rw-r--r--   0 ntvmb     (1000) ntvmb     (1000)      767 2024-05-25 12:41:32.000000 cyclomonitor-2024.5.25/src/cyclomonitor.egg-info/SOURCES.txt
```

### Comparing `cyclomonitor-2024.5.15/LICENSE` & `cyclomonitor-2024.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/PKG-INFO` & `cyclomonitor-2024.5.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclomonitor
-Version: 2024.5.15
+Version: 2024.5.25
 Summary: Discord bot that helps you keep tabs on tropical cyclones.
 Home-page: https://github.com/ntvmb/cyclomonitor
 Author: Nathaniel Greenwell
 Author-email: Nathaniel Greenwell <nategreenwell@live.com>
 Maintainer-email: Nathaniel Greenwell <nategreenwell@live.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

### Comparing `cyclomonitor-2024.5.15/README.md` & `cyclomonitor-2024.5.25/README.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/privacy-policy.md` & `cyclomonitor-2024.5.25/privacy-policy.md`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/pyproject.toml` & `cyclomonitor-2024.5.25/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/setup.py` & `cyclomonitor-2024.5.25/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-__version__ = "2024.5.15"
+__version__ = "2024.5.25"
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
```

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/__main__.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/__main__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/atcf.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/atcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 winds = []
 pressures = []
 tc_classes = []
 lats_real = []
 longs_real = []
 movement_speeds = []
 movement_dirs = []
+long_cids = []
 log = logging.getLogger(__name__)
 
 # increase compatibility with python<3.11
 if not hasattr(datetime, "UTC"):
     datetime.UTC = datetime.timezone.utc
 
 
@@ -73,29 +74,28 @@
 async def main():
     print("CycloMonitor ATCF Module")
     print("CLI coming soon")
 
 
 def reset():
     """Reset ATCF data."""
-    global cyclones, names, timestamps, lats, longs, basins, winds, pressures
-    global tc_classes, lats_real, longs_real, movement_speeds, movement_dirs
     cyclones.clear()
     names.clear()
     timestamps.clear()
     lats.clear()
     longs.clear()
     basins.clear()
     winds.clear()
     pressures.clear()
     tc_classes.clear()
     lats_real.clear()
     longs_real.clear()
     movement_speeds.clear()
     movement_dirs.clear()
+    long_cids.clear()
 
 
 def parse_storm(line: str, *, mode="std"):
     """Parse ATCF data.
 
     Arguments:
     line -- the data to be parsed
@@ -127,14 +127,15 @@
             pressures.append(int(storm[8]))
         else:
             lats_real.append(float(storm[4]))
             longs_real.append(float(storm[5]))
             tc_classes.append(storm[7])
             movement_speeds.append(float(storm[10]))
             movement_dirs.append(float(storm[11]))
+            long_cids.append(storm[0])
     except (AssertionError, LookupError, ValueError) as e:
         # remove the faulty entry
         faulty_entry = len(cyclones) - 1
         for index, (cy, n, ts, lat, lon, b, w, p) in enumerate(
             zip_longest(
                 cyclones, names, timestamps, lats, longs, basins, winds, pressures
             )
@@ -203,14 +204,15 @@
                     cid = storm[0][2] + storm[0][3] + storm[6]
                     if cid == tc:
                         lats_real.append(float(storm[4]))
                         longs_real.append(float(storm[5]))
                         tc_classes.append(storm[7])
                         movement_speeds.append(float(storm[10]))
                         movement_dirs.append(float(storm[11]))
+                        long_cids.append(storm[0])
                         break
                 else:  # no break
                     raise ATCFError(ERROR_HDYGH)
     except Exception as e:
         raise ATCFError(ATCF_GET_INTERP_FAILED) from e
 
 
@@ -300,24 +302,18 @@
         index = -1
     if index == -1 or not name:
         try:
             index = cyclones.index(cid)
         except ValueError:
             return None
 
-    with open("interp_sector_file", "r") as f:
-        lines = f.readlines()
-        atcf_id = lines[index].split()[0].upper()
-
-    basin = atcf_id[:2]  # 2-char basin identifier
-    num = atcf_id[2:4]  # 2-digit storm number
-    jtwc_year = atcf_id[6:]  # Last 2 digits of the year
-    if basin == "AL":
-        nhc_basin = "AT"
-    elif basin == "EP" or basin == "CP":
+    basin = basins[index][:2]  # 2-char basin identifier
+    num = cyclones[index][:2]  # 2-digit storm number
+    jtwc_year = long_cids[index][6:]  # Last 2 digits of the year
+    if basin == "AT" or basin == "EP" or basin == "CP":
         nhc_basin = basin
     else:
         nhc_basin = None
 
     async with aiohttp.ClientSession(
         timeout=aiohttp.ClientTimeout(connect=10), raise_for_status=True
     ) as session:
```

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/cli.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,18 +353,14 @@
         movement_str,
     )
 
 
 def cli():
     """The main function of the CLI."""
     print(CLI_STARTUP)
-    if version_info.major == 3 and version_info.minor < 11:
-        log.warning(
-            CLI_OLD_PY_VERSION.format(f"{version_info.major}.{version_info.minor}")
-        )
     while True:
         try:
             request = input("cyclomonitor> ")
         except EOFError:
             print("\n", end="")
             break
         except KeyboardInterrupt:
```

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/cyclomonitor.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/cyclomonitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     datetime.time(8, 0, tzinfo=datetime.UTC),
     datetime.time(14, 0, tzinfo=datetime.UTC),
     datetime.time(20, 0, tzinfo=datetime.UTC),
 ]
 log = logging.getLogger(__name__)
 languages = ["C", "en_US"]
 emojis = {}
+most_recent_dissipation = None
 
 
 class monitor(commands.Cog):
     """This class governs automated routines."""
 
     def __init__(self, bot):
         self.bot = bot
@@ -72,45 +73,56 @@
         self.last_ibtracs_update = global_vars.get("last_ibtracs_update")
         self.is_best_track_updating = False
 
     def cog_unload(self):
         logging.info(LOG_MONITOR_STOP)
         self.auto_update.cancel()
 
-    def should_suppress(self, prev_timestamps: list):
+    @staticmethod
+    def should_suppress(prev_timestamps: dict):
         """Compare two lists of timestamps and return a boolean."""
         suppressed = []
-        for index, (cyclone, timestamp, p_timestamp) in enumerate(
-            zip(atcf.cyclones, atcf.timestamps, prev_timestamps)
+        for index, (cyclone, timestamp) in enumerate(
+            zip(atcf.cyclones, atcf.timestamps)
         ):
-            try:
-                # will this system request for a suppression?
-                suppressed.append(p_timestamp >= timestamp)
-            except IndexError:
-                suppressed.append(False)
-            logging.debug(LOG_TIMESTAMP_COMPARISON.format(cyclone, suppressed[index]))
+            if cyclone == most_recent_dissipation:
+                suppressed.append(True)
+            else:
+                try:
+                    # will this system request for a suppression?
+                    suppressed.append(prev_timestamps[cyclone] >= timestamp)
+                except LookupError:
+                    suppressed.append(False)
+                logging.debug(
+                    LOG_TIMESTAMP_COMPARISON.format(cyclone, suppressed[index])
+                )
         if not atcf.cyclones:
             suppressed.append(False)
         # only suppress an automatic update if all active systems requested a suppression
         for do_suppress in suppressed:
             if not do_suppress:
                 return False
         return True
 
     @tasks.loop(time=times)
     async def auto_update(self):
         logging.info(LOG_AUTO_UPDATE_BEGIN)
-        prev_timestamps = atcf.timestamps.copy()
+        prev_timestamps = {
+            cid: time for cid, time in zip(atcf.cyclones, atcf.timestamps)
+        }
         try:
             await atcf.get_data()
         except atcf.ATCFError as e:
             logging.exception(ERROR_AUTO_UPDATE_FAILED)
             return
         self.last_update = math.floor(time.time())
         global_vars.write("last_update", self.last_update)
+        for cid in prev_timestamps:
+            if cid not in atcf.cyclones:
+                most_recent_dissipation = cid
         if self.should_suppress(prev_timestamps):
             # try alternate source
             logging.warn(LOG_SUPPRESSED)
             try:
                 await atcf.get_data_alt()
             except atcf.ATCFError as e:
                 logging.exception(ERROR_AUTO_UPDATE_FAILED)
```

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/dir_calc.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/dir_calc.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/global_vars.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/global_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/__init__.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_ALL.sql` & `cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/ibtracs_ALL.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql` & `cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/ibtracs_LAST3.sql`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/C.json` & `cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/__init__.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/ibtracs/locales/en_US.json` & `cyclomonitor-2024.5.25/src/cyclomonitor/ibtracs/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/locales/C.json` & `cyclomonitor-2024.5.25/src/cyclomonitor/locales/C.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/locales/__init__.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/locales/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/locales/en_US.json` & `cyclomonitor-2024.5.25/src/cyclomonitor/locales/en_US.json`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/server_vars.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/server_vars.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor/uptime.py` & `cyclomonitor-2024.5.25/src/cyclomonitor/uptime.py`

 * *Files identical despite different names*

### Comparing `cyclomonitor-2024.5.15/src/cyclomonitor.egg-info/SOURCES.txt` & `cyclomonitor-2024.5.25/src/cyclomonitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

