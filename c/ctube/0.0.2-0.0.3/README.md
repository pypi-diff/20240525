# Comparing `tmp/ctube-0.0.2.tar.gz` & `tmp/ctube-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctube-0.0.2.tar", max compression
+gzip compressed data, was "ctube-0.0.3.tar", max compression
```

## Comparing `ctube-0.0.2.tar` & `ctube-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1058 2024-05-21 18:00:19.544353 ctube-0.0.2/LICENSE
--rw-r--r--   0        0        0        8 2024-05-21 18:12:37.447875 ctube-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-21 18:10:22.007715 ctube-0.0.2/ctube/__init__.py
--rw-r--r--   0        0        0     6703 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/app.py
--rw-r--r--   0        0        0      511 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/cli.py
--rw-r--r--   0        0        0     2004 2024-05-21 20:56:10.230755 ctube-0.0.2/ctube/cmds.py
--rw-r--r--   0        0        0      658 2024-05-21 21:21:21.916025 ctube-0.0.2/ctube/colors.py
--rw-r--r--   0        0        0      397 2024-05-20 21:34:33.134572 ctube-0.0.2/ctube/containers.py
--rw-r--r--   0        0        0     1364 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/decorators.py
--rw-r--r--   0        0        0     4172 2024-05-21 21:47:45.472668 ctube-0.0.2/ctube/download.py
--rw-r--r--   0        0        0      325 2024-05-21 21:08:14.245466 ctube-0.0.2/ctube/errors.py
--rw-r--r--   0        0        0     1722 2024-05-21 18:08:57.179084 ctube-0.0.2/ctube/extractors.py
--rw-r--r--   0        0        0     2885 2024-05-21 22:00:49.146238 ctube-0.0.2/ctube/helpers.py
--rw-r--r--   0        0        0      247 2024-05-21 18:00:19.574354 ctube-0.0.2/ctube/paths.py
--rw-r--r--   0        0        0     1903 2024-05-21 22:28:30.102105 ctube-0.0.2/ctube/printers.py
--rw-r--r--   0        0        0     2068 2024-05-21 21:41:27.800799 ctube-0.0.2/ctube/terminal.py
--rw-r--r--   0        0        0      622 2024-05-23 07:36:38.694868 ctube-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      937 1970-01-01 00:00:00.000000 ctube-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.3/LICENSE
+-rw-r--r--   0        0        0       32 2024-05-25 10:03:30.952624 ctube-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-25 10:03:30.952624 ctube-0.0.3/ctube/__init__.py
+-rw-r--r--   0        0        0     4575 2024-05-25 11:24:02.708999 ctube-0.0.3/ctube/app.py
+-rw-r--r--   0        0        0     1655 2024-05-25 10:15:32.727491 ctube-0.0.3/ctube/callbacks.py
+-rw-r--r--   0        0        0      511 2024-05-25 10:03:40.745849 ctube-0.0.3/ctube/cli.py
+-rw-r--r--   0        0        0     2375 2024-05-25 11:23:50.259140 ctube-0.0.3/ctube/cmds.py
+-rw-r--r--   0        0        0      658 2024-05-25 10:28:10.864792 ctube-0.0.3/ctube/colors.py
+-rw-r--r--   0        0        0      354 2024-05-25 10:03:48.972425 ctube-0.0.3/ctube/containers.py
+-rw-r--r--   0        0        0     4025 2024-05-25 11:18:12.416190 ctube-0.0.3/ctube/download.py
+-rw-r--r--   0        0        0      184 2024-05-25 11:14:15.391963 ctube-0.0.3/ctube/errors.py
+-rw-r--r--   0        0        0     2118 2024-05-25 10:51:12.461628 ctube-0.0.3/ctube/extractors.py
+-rw-r--r--   0        0        0     1430 2024-05-25 11:18:34.919283 ctube-0.0.3/ctube/helpers.py
+-rw-r--r--   0        0        0     1893 2024-05-25 11:16:41.380482 ctube-0.0.3/ctube/parser.py
+-rw-r--r--   0        0        0      247 2024-05-25 10:03:30.955957 ctube-0.0.3/ctube/paths.py
+-rw-r--r--   0        0        0     1684 2024-05-25 10:32:51.554622 ctube-0.0.3/ctube/printers.py
+-rw-r--r--   0        0        0     2068 2024-05-25 10:05:03.171596 ctube-0.0.3/ctube/terminal.py
+-rw-r--r--   0        0        0      622 2024-05-25 10:03:30.955957 ctube-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 ctube-0.0.3/PKG-INFO
```

### Comparing `ctube-0.0.2/LICENSE` & `ctube-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctube-0.0.2/ctube/colors.py` & `ctube-0.0.3/ctube/colors.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.2/ctube/download.py` & `ctube-0.0.3/ctube/download.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,32 @@
 import os
 from pathvalidate import sanitize_filename
 from enum import Enum
 from urllib import request
 from typing import Callable, List
-from dataclasses import dataclass
-from ctube.containers import MusicItem
+from ctube.containers import MusicItem, DownloadData
 from pytubefix import Playlist, Stream, YouTube
 from pytubefix.exceptions import (
         MembersOnly, 
         RecordingUnavailable, 
         VideoPrivate, 
         VideoUnavailable
 )
 
 
 class BaseURL(str, Enum):
     PLAYLIST = "https://music.youtube.com/playlist?list="
 
 
-@dataclass(kw_only=True)
-class Data:
-    title: str
-    album: str
-    artist: str
-    release_year: int
-    tracks_num: int
-    image_data: bytes
-    filepath: str
-
-
 class Downloader:
     def __init__(
             self,
             output_path: str,
-            on_complete_callback: Callable[[Data], None],
-            on_progress_callback: Callable[[Data, int, int], None],
+            on_complete_callback: Callable[[DownloadData], None],
+            on_progress_callback: Callable[[DownloadData, int, int], None],
             skip_existing: bool = False
     ):
         self.output_path = output_path
         self.on_complete_callback = on_complete_callback 
         self.on_progress_callback = on_progress_callback
         self.skip_existing = skip_existing
 
@@ -52,19 +40,19 @@
             os.makedirs(output_path, exist_ok=True)
         if not os.path.isdir(output_path):
             raise NotADirectoryError
         if not os.access(path=output_path, mode=os.W_OK):
             raise NotADirectoryError
         self._output_path = output_path
 
-    def _on_complete_callback(self, data: Data, filepath: str) -> None:
+    def _on_complete_callback(self, data: DownloadData, filepath: str) -> None:
         data.filepath = filepath
         self.on_complete_callback(data)
 
-    def _on_progress_callback(self, data: Data, bytes_remaining: int, stream: Stream) -> None:
+    def _on_progress_callback(self, data: DownloadData, bytes_remaining: int, stream: Stream) -> None:
         filesize = stream.filesize
         bytes_received = filesize - bytes_remaining
         self.on_progress_callback(data, filesize, bytes_received)
 
     def download(self, item: MusicItem, artist: str) -> List[YouTube]:
         playlist = Playlist(url=f"{BaseURL.PLAYLIST.value}{item.playlist_id}")
         failed_downloads: List[YouTube] = []
@@ -98,15 +86,15 @@
 
             audio_stream = stream.get_audio_only(subtype="mp4")
 
             if not audio_stream:
                 failed_downloads.append(youtube)
                 continue
 
-            data = Data(
+            data = DownloadData(
                 title=youtube.title,
                 artist=artist,
                 album=item.title,
                 tracks_num=i + 1,
                 release_year=item.release_year,
                 image_data=image_data,
                 filepath=""
```

### Comparing `ctube-0.0.2/ctube/extractors.py` & `ctube-0.0.3/ctube/extractors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from typing import Dict, Optional, List, Tuple
+from typing import Dict, List, Tuple
 from ctube.containers import MusicItem
-from ctube.decorators import handle_extraction
 
 
-@handle_extraction
-def extract_artist_id(data: Dict) -> Optional[str]:
+def extract_artist_id(data: Dict) -> str:
     return data["contents"]["tabbedSearchResultsRenderer"][
         "tabs"][0]["tabRenderer"]["content"]["sectionListRenderer"][
         "contents"][1]["musicCardShelfRenderer"]["title"]["runs"][0][
         "navigationEndpoint"]["browseEndpoint"]["browseId"]
 
 
-@handle_extraction
 def extract_artist_music(data: Dict) -> Tuple[List[MusicItem], str]:
     music_items: List[MusicItem] = []
     for item in data["contents"]["singleColumnBrowseResultsRenderer"]["tabs"][0][
         "tabRenderer"]["content"]["sectionListRenderer"]["contents"][
         0]["gridRenderer"]["items"]:
 
         item_data = item["musicTwoRowItemRenderer"]
@@ -35,7 +32,21 @@
                 release_year=release_year,
                 thumbanail_url=thumbanail_url,
                 playlist_id=playlist_id
             )
         )
     return music_items, data["header"][
         "musicHeaderRenderer"]["title"]["runs"][0]["text"]
+
+
+def extract_search_suggestions(data: Dict) -> List[str]:
+    search_suggestions_section: Dict = data["contents"][0][
+        "searchSuggestionsSectionRenderer"]
+    if "contents" in search_suggestions_section:
+        contents = search_suggestions_section["contents"]
+    else:
+        contents: List[Dict] = search_suggestions_section["shelfDivider"]
+    return [
+        el["searchSuggestionRenderer"]["navigationEndpoint"][
+            "searchEndpoint"]["query"]
+        for el in contents
+    ]
```

### Comparing `ctube-0.0.2/ctube/printers.py` & `ctube-0.0.3/ctube/printers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 import shutil
 from typing import List
-from ctube.cmds import Commands, get_cmd_by_name
+import ctube
+from ctube.cmds import Command
 from ctube.colors import color, Color
 from ctube.containers import MusicItem
 
 
 def print_header() -> None:
-    print(color("░█▀▀░▀█▀░█░█░█▀▄░█▀▀░", Color.GREEN))
-    print(color("░█░░░░█░░█░█░█▀▄░█▀▀░", Color.GREEN))
-    print(color("░▀▀▀░░▀░░▀▀▀░▀▀░░▀▀▀░", Color.GREEN))
-    print(f"\u2022 {color('version', Color.BOLD)}: {color('0.0.2', Color.BLUE)}")
+    write("░█▀▀░▀█▀░█░█░█▀▄░█▀▀░", Color.GREEN)
+    write("░█░░░░█░░█░█░█▀▄░█▀▀░", Color.GREEN)
+    write("░▀▀▀░░▀░░▀▀▀░▀▀░░▀▀▀░", Color.GREEN)
+    print(f"\u2022 {color('version', Color.BOLD)}: {color(ctube.__version__, Color.BLUE)}")
     print("\u2022 source: https://github.com/g3nsy/ctube")
     print("\u2022 Type 'help' to list the available commands")
 
 
-def print_info(cmd_name: str) -> None:
-    try:
-        cmd_obj = get_cmd_by_name(cmd_name)
-        print(cmd_obj.value.description)
-    except KeyError:
-        print(color(f"Invalid argument for command 'info': {cmd_name}", Color.RED))
-        print(color(f"Valid arguments are {Commands.INFO.value.accepted_args}", Color.RED))
-
-
 def print_help() -> None:
-    print(color("Commands overview", Color.GREEN))
-    for cmd in Commands:
-        print(f"\u2022 {color(cmd.value.name, Color.BOLD)}", end=" ")
-        print(color(cmd.value.description, Color.BLUE))
+    write(":: Helper", Color.GREEN)
+    for cmd in Command:
+        print(f"\u2022 {color(cmd.value.name, Color.BOLD)}:")
+        write(cmd.value.description, Color.GREEN)
+        print()
 
 
 def print_music_items(music_items: List[MusicItem]) -> None:
     terminal_columns = shutil.get_terminal_size().columns
     max_index_len = len(str(len(music_items)))
     space_for_title = terminal_columns - max_index_len - 3  # [, ], ' '
     for i, music_item in enumerate(music_items):
@@ -41,7 +34,13 @@
             title = music_item.title
         lb = color("[", Color.BLUE)
         rb = color("]", Color.BLUE)
         ci = color(str(i), Color.GREEN)
         print(f"{lb}{ci}{rb}{' ' * (1 + max_index_len - len(str(i)))}{title}")
 
 
+def clear_screen() -> None:
+    print("\033c", end="")
+
+
+def write(string: str, col: Color = Color.WHITE):
+    print(color(string, color=col))
```

### Comparing `ctube-0.0.2/ctube/terminal.py` & `ctube-0.0.3/ctube/terminal.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.2/pyproject.toml` & `ctube-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctube"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Simone Gentili <gensydev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/ctube/"
 repository = "https://github.com/g3nsy/ctube"
 keywords = ["innertube", "youtube", "youtube-music", "python", "download", "music", "client"]
```

### Comparing `ctube-0.0.2/PKG-INFO` & `ctube-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctube
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Home-page: https://pypi.org/project/ctube/
 License: MIT
 Keywords: innertube,youtube,youtube-music,python,download,music,client
 Author: Simone Gentili
 Author-email: gensydev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -21,7 +21,9 @@
 Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytubefix (>=5.4.2,<6.0.0)
 Project-URL: Repository, https://github.com/g3nsy/ctube
 Description-Content-Type: text/markdown
 
 # ctube
 
+![](.github/video.gif)
+
```

