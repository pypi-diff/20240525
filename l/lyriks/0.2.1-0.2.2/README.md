# Comparing `tmp/lyriks-0.2.1.tar.gz` & `tmp/lyriks-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyriks-0.2.1.tar", last modified: Sat May 25 17:09:15 2024, max compression
+gzip compressed data, was "lyriks-0.2.2.tar", last modified: Sat May 25 21:09:37 2024, max compression
```

## Comparing `lyriks-0.2.1.tar` & `lyriks-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 17:09:15.128557 lyriks-0.2.1/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 17:09:15.128557 lyriks-0.2.1/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 17:07:44.000000 lyriks-0.2.1/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 17:09:15.128557 lyriks-0.2.1/lyriks/
--rw-r--r--   0 max       (1000) max       (1000)     1431 2024-05-25 17:06:51.000000 lyriks-0.2.1/lyriks/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     1298 2024-05-25 17:07:44.000000 lyriks-0.2.1/lyriks/cli.py
--rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.1/lyriks/genie_client.py
--rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.1/lyriks/lyrics.py
--rw-r--r--   0 max       (1000) max       (1000)     5443 2024-05-25 17:06:51.000000 lyriks-0.2.1/lyriks/lyrics_fetcher.py
--rw-r--r--   0 max       (1000) max       (1000)     1973 2024-05-25 00:28:29.000000 lyriks-0.2.1/lyriks/mb_client.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 17:09:15.128557 lyriks-0.2.1/lyriks.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 17:09:15.000000 lyriks-0.2.1/lyriks.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 17:07:44.000000 lyriks-0.2.1/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 17:09:15.128557 lyriks-0.2.1/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:09:37.966672 lyriks-0.2.2/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:09:37.966672 lyriks-0.2.2/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-25 21:07:48.000000 lyriks-0.2.2/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:09:37.963339 lyriks-0.2.2/lyriks/
+-rw-r--r--   0 max       (1000) max       (1000)     1450 2024-05-25 18:57:10.000000 lyriks-0.2.2/lyriks/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     1476 2024-05-25 21:07:48.000000 lyriks-0.2.2/lyriks/cli.py
+-rw-r--r--   0 max       (1000) max       (1000)     2940 2024-05-13 01:42:38.000000 lyriks-0.2.2/lyriks/genie_client.py
+-rw-r--r--   0 max       (1000) max       (1000)     1242 2024-05-25 00:28:29.000000 lyriks-0.2.2/lyriks/lyrics.py
+-rw-r--r--   0 max       (1000) max       (1000)     7123 2024-05-25 21:06:54.000000 lyriks-0.2.2/lyriks/lyrics_fetcher.py
+-rw-r--r--   0 max       (1000) max       (1000)     3010 2024-05-25 20:47:16.000000 lyriks-0.2.2/lyriks/mb_client.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-25 21:09:37.966672 lyriks-0.2.2/lyriks.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      324 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-25 21:09:37.000000 lyriks-0.2.2/lyriks.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-25 21:07:48.000000 lyriks-0.2.2/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-25 21:09:37.966672 lyriks-0.2.2/setup.cfg
```

### Comparing `lyriks-0.2.1/PKG-INFO` & `lyriks-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.1
+Version: 0.2.2
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
-pip install dist/lyriks-0.2.1-py3-none-any.whl
+pip install dist/lyriks-0.2.2-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.1/README.md` & `lyriks-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.2.1-py3-none-any.whl
+pip install dist/lyriks-0.2.2-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.1/lyriks/__init__.py` & `lyriks-0.2.2/lyriks/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         report_path = report_path.expanduser().absolute()
         if report_path.is_dir():
             report_path = report_path / 'report.html'
         if not report_path.parent.exists():
             print(f'Error: directory \'{report_path.parent}\' does not exist', file=stderr)
             exit(2)
 
-    fetcher = LyricsFetcher(args.dry_run, args.force)
+    fetcher = LyricsFetcher(args.check_artist, args.dry_run, args.force)
 
     for root_dir, dirs, files in os.walk(collection_path, topdown=True):
         if path.exists(path.join(root_dir, '.nolyrics')):
             dirs.clear()
             continue
 
         for file in files:
```

### Comparing `lyriks-0.2.1/lyriks/cli.py` & `lyriks-0.2.2/lyriks/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import argparse
 from pathlib import Path
 
 PROGNAME = 'lyriks'
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 
 
 def parse_arguments():
     parser = argparse.ArgumentParser(prog=PROGNAME, description='A command line tool that fetches lyrics from Genie.')
     path_help = f"""
                 The path to the music collection.
                 {PROGNAME} will recursively search for music files in this directory.
                 """
     parser.add_argument('collection_path', type=Path, metavar='path', help=path_help)
+    parser.add_argument('-a', '--check-artist',
+                        action='store_true',
+                        help='ensure artist has a Genie URL when processing albums')
     parser.add_argument('-n', '--dry-run', action='store_true', help='fetch lyrics without writing them to files')
     parser.add_argument('-f', '--force',
                         action='store_true',
                         help='force fetching lyrics for all tracks, even if they already have them'
                              ' - THIS WILL OVERWRITE EXISTING LYRICS FILES!')
     parser.add_argument('-R', '--report',
                         type=Path, nargs='?', metavar='path', const='report.html',
```

### Comparing `lyriks-0.2.1/lyriks/genie_client.py` & `lyriks-0.2.2/lyriks/genie_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.1/lyriks/lyrics.py` & `lyriks-0.2.2/lyriks/lyrics.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.2.1/lyriks/mb_client.py` & `lyriks-0.2.2/lyriks/mb_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,23 +4,46 @@
 import requests
 from requests import JSONDecodeError
 
 from .cli import VERSION
 
 API_URL = 'https://musicbrainz.org/ws/2'
 USER_AGENT = f'lyriks/{VERSION} ( max@maxr1998.de )'
+_ARTIST_INC = 'url-rels'
+_RELEASE_INC = 'artist-credits+media+url-rels'
 
 last_request_time = 0
 
 
+def handle_rate_limit():
+    global last_request_time
+    time_since = time.time() - last_request_time
+    if time_since < 1:
+        time.sleep(1 - time_since)
+    last_request_time = time.time()
+
+
+class Artist:
+    def __init__(self, data: dict):
+        self.data = data
+        self.id: str = data['id']
+        self.name: str = data['name']
+        self.urls: set = {
+            relation['url']['resource'] for relation in data.get('relations', [])
+            if relation.get('target-type') == 'url'
+        }
+        self.has_genie_url: bool = any('genie.co.kr' in url for url in self.urls)
+
+
 class Release:
     def __init__(self, data: dict):
         self.data = data
         self.id: str = data['id']
         self.title: str = data['title']
+        self.artist_credit: dict = data['artist-credit']
 
     def get_track_count(self) -> int:
         return sum([media['track-count'] for media in self.data['media']])
 
     def get_genie_album_id(self) -> int | None:
         relations = self.data['relations']
         for relation in relations:
@@ -34,29 +57,39 @@
                     return int(album_id)
                 except ValueError:
                     print(f"Invalid album ID: {album_id}")
                     return None
         return None
 
 
+def get_artist(artist_mbid: str) -> Artist | None:
+    handle_rate_limit()
+
+    artist_url = f'{API_URL}/artist/{artist_mbid}?inc={_ARTIST_INC}'
+    response = requests.get(artist_url, headers={'User-Agent': USER_AGENT, 'Accept': 'application/json'})
+    try:
+        response_json = response.json()
+    except JSONDecodeError:
+        print(f'Error: could not fetch artist data for {artist_mbid}')
+        return None
+
+    return Artist(response_json)
+
+
 def get_releases(browse_url: str) -> list[Release]:
-    global last_request_time
-    time_since = time.time() - last_request_time
-    if time_since < 1:
-        time.sleep(1 - time_since)
-    response = requests.get(browse_url, headers={'User-Agent': USER_AGENT, 'Accept': 'application/json'})
-    last_request_time = time.time()
+    handle_rate_limit()
 
+    response = requests.get(browse_url, headers={'User-Agent': USER_AGENT, 'Accept': 'application/json'})
     try:
         response_json = response.json()
     except JSONDecodeError:
         return []
 
     return [Release(release) for release in response_json.get("releases", [])]
 
 
 def get_release_by_track(track_mbid: str) -> Release | None:
-    return next(iter(get_releases(f'{API_URL}/release?track={track_mbid}&status=official&inc=media+url-rels')), None)
+    return next(iter(get_releases(f'{API_URL}/release?track={track_mbid}&status=official&inc={_RELEASE_INC}')), None)
 
 
 def get_releases_by_release_group(rg_mbid: str) -> list[Release]:
-    return get_releases(f'{API_URL}/release?release-group={rg_mbid}&status=official&inc=media+url-rels')
+    return get_releases(f'{API_URL}/release?release-group={rg_mbid}&status=official&inc={_RELEASE_INC}')
```

### Comparing `lyriks-0.2.1/lyriks.egg-info/PKG-INFO` & `lyriks-0.2.2/lyriks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.2.1
+Version: 0.2.2
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
-pip install dist/lyriks-0.2.1-py3-none-any.whl
+pip install dist/lyriks-0.2.2-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.2.1/pyproject.toml` & `lyriks-0.2.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lyriks"
-version = "0.2.1"
+version = "0.2.2"
 description = "A command line tool to fetch lyrics from Genie"
 authors = [
     { name = "Maxr1998", email = "max@maxr1998.de" },
 ]
 license = { text = "GPLv3" }
 readme = "README.md"
 classifiers = [
```

