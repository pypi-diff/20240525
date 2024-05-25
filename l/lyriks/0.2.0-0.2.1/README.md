# Comparing `tmp/lyriks-0.2.0.tar.gz` & `tmp/lyriks-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyriks-0.2.0.tar", last modified: Sat May 25 01:13:45 2024, max compression
+gzip compressed data, was "lyriks-0.2.1.tar", last modified: Sat May 25 17:09:15 2024, max compression
```

## Comparing `lyriks-0.2.0.tar` & `lyriks-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 01:13:45.353452 lyriks-0.2.0/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 01:13:45.353452 lyriks-0.2.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 01:12:39.000000 lyriks-0.2.0/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 01:13:45.353452 lyriks-0.2.0/lyriks/
--rw-r--r--   0 max       (1000) max       (1000)      603 2024-05-25 01:03:46.000000 lyriks-0.2.0/lyriks/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1151 2024-05-25 01:13:11.000000 lyriks-0.2.0/lyriks/cli.py
--rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.0/lyriks/genie_client.py
--rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.0/lyriks/lyrics.py
--rw-r--r--   0 max       (1000) max       (1000)     5548 2024-05-25 01:10:13.000000 lyriks-0.2.0/lyriks/lyrics_fetcher.py
--rw-r--r--   0 max       (1000) max       (1000)     1973 2024-05-25 00:28:29.000000 lyriks-0.2.0/lyriks/mb_client.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 01:13:45.353452 lyriks-0.2.0/lyriks.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 01:13:19.000000 lyriks-0.2.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 01:13:45.353452 lyriks-0.2.0/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 17:09:15.128557 lyriks-0.2.1/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 17:09:15.128557 lyriks-0.2.1/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 17:07:44.000000 lyriks-0.2.1/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 17:09:15.128557 lyriks-0.2.1/lyriks/
+-rw-r--r--   0 max       (1000) max       (1000)     1431 2024-05-25 17:06:51.000000 lyriks-0.2.1/lyriks/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1298 2024-05-25 17:07:44.000000 lyriks-0.2.1/lyriks/cli.py
+-rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.1/lyriks/genie_client.py
+-rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.1/lyriks/lyrics.py
+-rw-r--r--   0 max       (1000) max       (1000)     5443 2024-05-25 17:06:51.000000 lyriks-0.2.1/lyriks/lyrics_fetcher.py
+-rw-r--r--   0 max       (1000) max       (1000)     1973 2024-05-25 00:28:29.000000 lyriks-0.2.1/lyriks/mb_client.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 17:09:15.128557 lyriks-0.2.1/lyriks.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 17:07:44.000000 lyriks-0.2.1/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 17:09:15.128557 lyriks-0.2.1/setup.cfg
```

### Comparing `lyriks-0.2.0/PKG-INFO` & `lyriks-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.0
+Version: 0.2.1
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,15 +18,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.0-py3-none-any.whl
+pip install dist/lyriks-0.2.1-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.0/README.md` & `lyriks-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.0-py3-none-any.whl
+pip install dist/lyriks-0.2.1-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.0/lyriks/cli.py` & `lyriks-0.2.1/lyriks/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import argparse
+from pathlib import Path
 
 PROGNAME = 'lyriks'
-VERSION = '0.2.0'
+VERSION = '0.2.1'
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(prog=PROGNAME, description='A command line tool that fetches lyrics from Genie.')
     path_help = f"""
                 The path to the music collection.
                 {PROGNAME} will recursively search for music files in this directory.
                 """
-    parser.add_argument('path', type=str, help=path_help)
+    parser.add_argument('collection_path', type=Path, metavar='path', help=path_help)
     parser.add_argument('-n', '--dry-run', action='store_true', help='fetch lyrics without writing them to files')
     parser.add_argument('-f', '--force',
                         action='store_true',
                         help='force fetching lyrics for all tracks, even if they already have them'
                              ' - THIS WILL OVERWRITE EXISTING LYRICS FILES!')
     parser.add_argument('-R', '--report',
-                        nargs='?', const='report.html',
-                        help='write a HTML report of releases missing album URLs to a file (default: report.html)')
+                        type=Path, nargs='?', metavar='path', const='report.html',
+                        help='write a HTML report of releases missing album URLs to a file at [path]'
+                             ' (default: report.html in the current directory)')
     parser.add_argument('-v', '--version', action='version', version='%(prog)s ' + VERSION)
 
     return parser.parse_args()
```

### Comparing `lyriks-0.2.0/lyriks/genie_client.py` & `lyriks-0.2.1/lyriks/genie_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.0/lyriks/lyrics.py` & `lyriks-0.2.1/lyriks/lyrics.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.0/lyriks/lyrics_fetcher.py` & `lyriks-0.2.1/lyriks/lyrics_fetcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from os import PathLike
 from os import path
 
 import mutagen
 
 from .genie_client import fetch_genie_album_song_ids, GenieSong, fetch_lyrics
 from .mb_client import get_release_by_track, get_releases_by_release_group, Release
 
@@ -24,17 +25,16 @@
     def fetch_lyrics(self, filename: str) -> bool:
         basename = filename.rsplit('.', 1)[0]
         timed_lyrics_file = f'{basename}.lrc'
         static_lyrics_file = f'{basename}.txt'
 
         has_timed_lyrics = path.exists(timed_lyrics_file)
         has_static_lyrics = path.exists(static_lyrics_file)
-        has_nolyrics_file = path.exists(path.join(path.dirname(filename), '.nolyrics'))
 
-        if (has_timed_lyrics or has_static_lyrics or has_nolyrics_file) and not self.force:
+        if (has_timed_lyrics or has_static_lyrics) and not self.force:
             # Skip if lyrics already exist
             return True
 
         file = mutagen.File(filename, easy=True)
         if not file:
             return False
 
@@ -61,15 +61,15 @@
 
         print(f'Fetching lyrics for {title}', end='')
 
         # Fetch lyrics
         song = songs[track_number - 1]
         lyrics = fetch_lyrics(song.song_id)
         if not lyrics:
-            print(f' - no lyrics found')
+            print(' - no lyrics found')
             return False
 
         if self.dry_run:
             print(' - done [dry run]')
         else:
             # Write lyrics to file
             if lyrics.is_timed:
@@ -143,19 +143,19 @@
                 return album_id
 
         print(f'No Genie URL found for release {release.title} [{release.id}]')
         self.missing_releases.add(release)
 
         return None
 
-    def write_report(self, filename: str):
-        with open(filename, 'w') as file:
-            file.write('<html><head><title>lyriks report</title></head>')
-            file.write('<body>')
-            file.write('<h1>Releases missing Genie URLs</h1>')
-            file.write('<ul>')
+    def write_report(self, file: str | PathLike[str]):
+        with open(file, 'w') as f:
+            f.write('<html><head><title>lyriks report</title></head>')
+            f.write('<body>')
+            f.write('<h1>Releases missing Genie URLs</h1>')
+            f.write('<ul>')
             for release in self.missing_releases:
                 url = f'https://musicbrainz.org/release/{release.id}'
-                file.write(f'<li><a href="{url}">{release.title}</a></li>')
-            file.write('</ul>')
-            file.write('</body>')
-            file.write('</html>')
+                f.write(f'<li><a href="{url}">{release.title}</a></li>')
+            f.write('</ul>')
+            f.write('</body>')
+            f.write('</html>')
```

### Comparing `lyriks-0.2.0/lyriks/mb_client.py` & `lyriks-0.2.1/lyriks/mb_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.0/lyriks.egg-info/PKG-INFO` & `lyriks-0.2.1/lyriks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.0
+Version: 0.2.1
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,15 +18,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.0-py3-none-any.whl
+pip install dist/lyriks-0.2.1-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.0/pyproject.toml` & `lyriks-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lyriks"
-version = "0.2.0"
+version = "0.2.1"
 description = "A command line tool to fetch lyrics from Genie"
 authors = [
     { name = "Maxr1998", email = "max@maxr1998.de" },
 ]
 license = { text = "GPLv3" }
 readme = "README.md"
 classifiers = [
```

