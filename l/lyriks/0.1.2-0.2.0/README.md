# Comparing `tmp/lyriks-0.1.2.tar.gz` & `tmp/lyriks-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyriks-0.1.2.tar", last modified: Mon May 13 01:47:24 2024, max compression
+gzip compressed data, was "lyriks-0.2.0.tar", last modified: Sat May 25 01:13:45 2024, max compression
```

## Comparing `lyriks-0.1.2.tar` & `lyriks-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-13 01:47:24.680548 lyriks-0.1.2/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-13 01:47:24.680548 lyriks-0.1.2/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-13 01:46:38.000000 lyriks-0.1.2/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-13 01:47:24.680548 lyriks-0.1.2/lyriks/
--rw-r--r--   0 max       (1000) max       (1000)      536 2024-05-12 15:25:28.000000 lyriks-0.1.2/lyriks/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.1.2/lyriks/genie_client.py
--rw-r--r--   0 max       (1000) max       (1000)     1134 2024-05-12 20:20:30.000000 lyriks-0.1.2/lyriks/lyrics.py
--rw-r--r--   0 max       (1000) max       (1000)     3971 2024-05-12 21:46:34.000000 lyriks-0.1.2/lyriks/lyrics_fetcher.py
--rw-r--r--   0 max       (1000) max       (1000)     1942 2024-05-13 01:46:38.000000 lyriks-0.1.2/lyriks/mb_client.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-13 01:47:24.680548 lyriks-0.1.2/lyriks.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-13 01:47:24.000000 lyriks-0.1.2/lyriks.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      310 2024-05-13 01:47:24.000000 lyriks-0.1.2/lyriks.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-13 01:47:24.000000 lyriks-0.1.2/lyriks.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-13 01:47:24.000000 lyriks-0.1.2/lyriks.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-13 01:47:24.000000 lyriks-0.1.2/lyriks.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-13 01:47:24.000000 lyriks-0.1.2/lyriks.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-13 01:46:38.000000 lyriks-0.1.2/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-13 01:47:24.680548 lyriks-0.1.2/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 01:13:45.353452 lyriks-0.2.0/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 01:13:45.353452 lyriks-0.2.0/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 01:12:39.000000 lyriks-0.2.0/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 01:13:45.353452 lyriks-0.2.0/lyriks/
+-rw-r--r--   0 max       (1000) max       (1000)      603 2024-05-25 01:03:46.000000 lyriks-0.2.0/lyriks/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1151 2024-05-25 01:13:11.000000 lyriks-0.2.0/lyriks/cli.py
+-rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.0/lyriks/genie_client.py
+-rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.0/lyriks/lyrics.py
+-rw-r--r--   0 max       (1000) max       (1000)     5548 2024-05-25 01:10:13.000000 lyriks-0.2.0/lyriks/lyrics_fetcher.py
+-rw-r--r--   0 max       (1000) max       (1000)     1973 2024-05-25 00:28:29.000000 lyriks-0.2.0/lyriks/mb_client.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 01:13:45.353452 lyriks-0.2.0/lyriks.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 01:13:45.000000 lyriks-0.2.0/lyriks.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 01:13:19.000000 lyriks-0.2.0/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 01:13:45.353452 lyriks-0.2.0/setup.cfg
```

### Comparing `lyriks-0.1.2/PKG-INFO` & `lyriks-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.1.2
+Version: 0.2.0
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
-pip install dist/lyriks-0.1.2-py3-none-any.whl
+pip install dist/lyriks-0.2.0-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.1.2/README.md` & `lyriks-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.1.2-py3-none-any.whl
+pip install dist/lyriks-0.2.0-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.1.2/lyriks/genie_client.py` & `lyriks-0.2.0/lyriks/genie_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.1.2/lyriks/lyrics.py` & `lyriks-0.2.0/lyriks/lyrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+import os
 from dataclasses import dataclass
 
 
+def opener(path: str, flags: int) -> int:
+    return os.open(path, flags, 0o644)
+
+
 @dataclass
 class Lyrics:
     lines: list[str]
     is_timed: bool
 
     def write_to_file(self, path: str):
-        with open(path, 'w') as f:
+        with open(path, 'w', opener=opener) as f:
             f.writelines(self.lines)
 
     @staticmethod
     def timed(lyrics_dict: dict[str, str]) -> 'Lyrics':
         return Lyrics(_convert_to_lrc(lyrics_dict), is_timed=True)
 
     @staticmethod
```

### Comparing `lyriks-0.1.2/lyriks/lyrics_fetcher.py` & `lyriks-0.2.0/lyriks/lyrics_fetcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,113 @@
+import os
 from os import path
 
 import mutagen
 
 from .genie_client import fetch_genie_album_song_ids, GenieSong, fetch_lyrics
 from .mb_client import get_release_by_track, get_releases_by_release_group, Release
 
 TITLE_TAG = 'title'
+ALBUM_TAG = 'album'
 TRACKNUMBER_TAG = 'tracknumber'
 MB_RGID_TAG = 'musicbrainz_releasegroupid'
 MB_RTID_TAG = 'musicbrainz_releasetrackid'
 
 
 class LyricsFetcher:
-    def __init__(self):
+    def __init__(self, dry_run: bool = False, force: bool = False):
+        self.dry_run = dry_run
+        self.force = force
         self.release_cache = {}
         self.genie_cache = {}
+        self.missing_releases = set()
 
     def fetch_lyrics(self, filename: str) -> bool:
         basename = filename.rsplit('.', 1)[0]
         timed_lyrics_file = f'{basename}.lrc'
         static_lyrics_file = f'{basename}.txt'
 
-        if path.exists(timed_lyrics_file) or path.exists(static_lyrics_file):
+        has_timed_lyrics = path.exists(timed_lyrics_file)
+        has_static_lyrics = path.exists(static_lyrics_file)
+        has_nolyrics_file = path.exists(path.join(path.dirname(filename), '.nolyrics'))
+
+        if (has_timed_lyrics or has_static_lyrics or has_nolyrics_file) and not self.force:
             # Skip if lyrics already exist
             return True
 
         file = mutagen.File(filename, easy=True)
         if not file:
             return False
 
         tags = file.tags
-        if (TITLE_TAG not in tags or TRACKNUMBER_TAG not in tags or
+        if (TITLE_TAG not in tags or ALBUM_TAG not in tags or TRACKNUMBER_TAG not in tags or
                 MB_RGID_TAG not in tags or MB_RTID_TAG not in tags):
             return False
 
-        print(f'Processing {filename}')
-
         title = tags[TITLE_TAG][0]
+        album = tags[ALBUM_TAG][0]
         track_number = int(tags[TRACKNUMBER_TAG][0].split('/')[0])
         rg_mbid = tags[MB_RGID_TAG][0]
         track_mbid = tags[MB_RTID_TAG][0]
 
         # Resolve release for the track
-        track_release = self.get_release(track_mbid)
+        track_release = self.get_release(track_mbid, album)
         if not track_release:
             return False
 
         # Resolve Genie album
         songs = self.get_genie_album(track_release, rg_mbid)
         if not songs or track_release.get_track_count() != len(songs):
             return False
 
+        print(f'Fetching lyrics for {title}', end='')
+
         # Fetch lyrics
         song = songs[track_number - 1]
         lyrics = fetch_lyrics(song.song_id)
         if not lyrics:
+            print(f' - no lyrics found')
             return False
 
-        print(f'Found lyrics for {title} / {song.name} [{song.song_id}], ', end='')
-
-        # Write lyrics to file
-        if lyrics.is_timed:
-            print(f'writing to {timed_lyrics_file}')
-            lyrics.write_to_file(timed_lyrics_file)
+        if self.dry_run:
+            print(' - done [dry run]')
         else:
-            print(f'writing to {static_lyrics_file}')
-            lyrics.write_to_file(static_lyrics_file)
+            # Write lyrics to file
+            if lyrics.is_timed:
+                print(f' - writing to {timed_lyrics_file}')
+                lyrics.write_to_file(timed_lyrics_file)
+
+                # Remove static lyrics file if necessary
+                if has_static_lyrics:
+                    os.unlink(static_lyrics_file)
+            elif has_timed_lyrics:
+                print(' - not writing static lyrics, timed lyrics already exist')
+            else:
+                print(f' - writing to {static_lyrics_file}')
+                lyrics.write_to_file(static_lyrics_file)
 
         return True
 
-    def get_release(self, track_mbid: str) -> Release | None:
+    def get_release(self, track_mbid: str, album_name: str) -> Release | None:
         if track_mbid in self.release_cache:
             return self.release_cache[track_mbid]
 
+        print(f'Fetching release info for {album_name}', end='')
+
         release = get_release_by_track(track_mbid)
         if not release:
+            print(' - no release found')
             return None
 
         for media in release.data['media']:
             for track in media['tracks']:
                 self.release_cache[track['id']] = release
 
+        print()  # terminate line
+
         return release
 
     def get_genie_album(self, release: Release, rg_mbid: str) -> list[GenieSong] | None:
         if release.id in self.genie_cache:
             return self.genie_cache[release.id]
 
         album_id = self.get_genie_album_id(release, rg_mbid)
@@ -97,16 +120,15 @@
             self.genie_cache[release.id] = None
             return None
 
         self.genie_cache[release.id] = songs
 
         return songs
 
-    @staticmethod
-    def get_genie_album_id(release: Release, rg_mbid: str) -> int | None:
+    def get_genie_album_id(self, release: Release, rg_mbid: str) -> int | None:
         # Try to get the album ID from the release itself first
         album_id = release.get_genie_album_id()
         if album_id is not None:
             return album_id
 
         # If that fails, check all releases from the release group
         rg_releases = get_releases_by_release_group(rg_mbid)
@@ -117,8 +139,23 @@
             if rg_release.get_track_count() != release.get_track_count():
                 continue
             album_id = rg_release.get_genie_album_id()
             if album_id is not None:
                 return album_id
 
         print(f'No Genie URL found for release {release.title} [{release.id}]')
+        self.missing_releases.add(release)
+
         return None
+
+    def write_report(self, filename: str):
+        with open(filename, 'w') as file:
+            file.write('<html><head><title>lyriks report</title></head>')
+            file.write('<body>')
+            file.write('<h1>Releases missing Genie URLs</h1>')
+            file.write('<ul>')
+            for release in self.missing_releases:
+                url = f'https://musicbrainz.org/release/{release.id}'
+                file.write(f'<li><a href="{url}">{release.title}</a></li>')
+            file.write('</ul>')
+            file.write('</body>')
+            file.write('</html>')
```

### Comparing `lyriks-0.1.2/lyriks/mb_client.py` & `lyriks-0.2.0/lyriks/mb_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import re
 import time
 
 import requests
 from requests import JSONDecodeError
 
+from .cli import VERSION
+
 API_URL = 'https://musicbrainz.org/ws/2'
-USER_AGENT = 'lyriks/0.1.2 ( max@maxr1998.de )'
+USER_AGENT = f'lyriks/{VERSION} ( max@maxr1998.de )'
 
 last_request_time = 0
 
 
 class Release:
     def __init__(self, data: dict):
         self.data = data
```

### Comparing `lyriks-0.1.2/lyriks.egg-info/PKG-INFO` & `lyriks-0.2.0/lyriks.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.1.2
+Version: 0.2.0
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
-pip install dist/lyriks-0.1.2-py3-none-any.whl
+pip install dist/lyriks-0.2.0-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.1.2/pyproject.toml` & `lyriks-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lyriks"
-version = "0.1.2"
+version = "0.2.0"
 description = "A command line tool to fetch lyrics from Genie"
 authors = [
     { name = "Maxr1998", email = "max@maxr1998.de" },
 ]
 license = { text = "GPLv3" }
 readme = "README.md"
 classifiers = [
```

