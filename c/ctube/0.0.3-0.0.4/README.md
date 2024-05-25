# Comparing `tmp/ctube-0.0.3.tar.gz` & `tmp/ctube-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctube-0.0.3.tar", max compression
+gzip compressed data, was "ctube-0.0.4.tar", max compression
```

## Comparing `ctube-0.0.3.tar` & `ctube-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.3/LICENSE
--rw-r--r--   0        0        0       32 2024-05-25 10:03:30.952624 ctube-0.0.3/README.md
--rw-r--r--   0        0        0       22 2024-05-25 10:03:30.952624 ctube-0.0.3/ctube/__init__.py
--rw-r--r--   0        0        0     4575 2024-05-25 11:24:02.708999 ctube-0.0.3/ctube/app.py
--rw-r--r--   0        0        0     1655 2024-05-25 10:15:32.727491 ctube-0.0.3/ctube/callbacks.py
--rw-r--r--   0        0        0      511 2024-05-25 10:03:40.745849 ctube-0.0.3/ctube/cli.py
--rw-r--r--   0        0        0     2375 2024-05-25 11:23:50.259140 ctube-0.0.3/ctube/cmds.py
--rw-r--r--   0        0        0      658 2024-05-25 10:28:10.864792 ctube-0.0.3/ctube/colors.py
--rw-r--r--   0        0        0      354 2024-05-25 10:03:48.972425 ctube-0.0.3/ctube/containers.py
--rw-r--r--   0        0        0     4025 2024-05-25 11:18:12.416190 ctube-0.0.3/ctube/download.py
--rw-r--r--   0        0        0      184 2024-05-25 11:14:15.391963 ctube-0.0.3/ctube/errors.py
--rw-r--r--   0        0        0     2118 2024-05-25 10:51:12.461628 ctube-0.0.3/ctube/extractors.py
--rw-r--r--   0        0        0     1430 2024-05-25 11:18:34.919283 ctube-0.0.3/ctube/helpers.py
--rw-r--r--   0        0        0     1893 2024-05-25 11:16:41.380482 ctube-0.0.3/ctube/parser.py
--rw-r--r--   0        0        0      247 2024-05-25 10:03:30.955957 ctube-0.0.3/ctube/paths.py
--rw-r--r--   0        0        0     1684 2024-05-25 10:32:51.554622 ctube-0.0.3/ctube/printers.py
--rw-r--r--   0        0        0     2068 2024-05-25 10:05:03.171596 ctube-0.0.3/ctube/terminal.py
--rw-r--r--   0        0        0      622 2024-05-25 10:03:30.955957 ctube-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 ctube-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-25 10:03:30.952624 ctube-0.0.4/LICENSE
+-rw-r--r--   0        0        0      610 2024-05-25 13:44:20.828071 ctube-0.0.4/README.md
+-rw-r--r--   0        0        0       22 2024-05-25 13:45:20.440579 ctube-0.0.4/ctube/__init__.py
+-rw-r--r--   0        0        0     4575 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/app.py
+-rw-r--r--   0        0        0     1655 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/callbacks.py
+-rw-r--r--   0        0        0      511 2024-05-25 10:03:40.745849 ctube-0.0.4/ctube/cli.py
+-rw-r--r--   0        0        0     2428 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/cmds.py
+-rw-r--r--   0        0        0      664 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/colors.py
+-rw-r--r--   0        0        0      353 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/containers.py
+-rw-r--r--   0        0        0     4024 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/download.py
+-rw-r--r--   0        0        0      184 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/errors.py
+-rw-r--r--   0        0        0     2119 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/extractors.py
+-rw-r--r--   0        0        0     1430 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/helpers.py
+-rw-r--r--   0        0        0     1892 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/parser.py
+-rw-r--r--   0        0        0       79 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/paths.py
+-rw-r--r--   0        0        0     1682 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/printers.py
+-rw-r--r--   0        0        0     2072 2024-05-25 13:42:39.319492 ctube-0.0.4/ctube/terminal.py
+-rw-r--r--   0        0        0      622 2024-05-25 13:45:14.753991 ctube-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1539 1970-01-01 00:00:00.000000 ctube-0.0.4/PKG-INFO
```

### Comparing `ctube-0.0.3/LICENSE` & `ctube-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctube-0.0.3/ctube/app.py` & `ctube-0.0.4/ctube/app.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.3/ctube/callbacks.py` & `ctube-0.0.4/ctube/callbacks.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.3/ctube/cmds.py` & `ctube-0.0.4/ctube/cmds.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         name="download", 
         description=(
             "Starts downloading the specified media contents.\n"
             "The contents are specified through the respective indexes.\n"
             "If you intend to download only one content, simply provide\n"
             "its index as an argument to the command.\n"
             "Multiple contents can be specified as follows:\n"
+            "\u2022 'all': download all contents.\n"
             "\u2022 Indices separated by a comma, for example 0, 1, ...\n"
             "\u2022 A slice that respects the Python syntax, for example\n"
             " 0:3 to download contents with index 0, 1, and 2."
         )
     )
 
     EXIT = _Command(
```

### Comparing `ctube-0.0.3/ctube/colors.py` & `ctube-0.0.4/ctube/colors.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     WHITE = "\033[97m"
 
 
 def get_color_by_name(color_name: str) -> Color:
     return Color.__members__[color_name.upper()]
 
 
-def color(string: str, color: Color) -> str:
-    return f"{color.value}{string}{Color.RESET.value}"
+def color(string: str, col: Color) -> str:
+    return f"{col.value}{string}{Color.RESET.value}"
 
 
 def get_color_names() -> Set[str]:
     upper_color_names = set(Color.__members__.keys())
     upper_color_names.remove("RESET")
-    return {color.lower() for color in upper_color_names}
+    return {color_name.lower() for color_name in upper_color_names}
```

### Comparing `ctube-0.0.3/ctube/download.py` & `ctube-0.0.4/ctube/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         bytes_received = filesize - bytes_remaining
         self.on_progress_callback(data, filesize, bytes_received)
 
     def download(self, item: MusicItem, artist: str) -> List[YouTube]:
         playlist = Playlist(url=f"{BaseURL.PLAYLIST.value}{item.playlist_id}")
         failed_downloads: List[YouTube] = []
 
-        response = request.urlopen(item.thumbanail_url)
+        response = request.urlopen(item.thumbnail_url)
         image_data = response.read()
 
         final_destination = os.path.join(
             os.path.join(
                 self.output_path, sanitize_filename(artist)
             ), 
             sanitize_filename(item.title)
```

### Comparing `ctube-0.0.3/ctube/extractors.py` & `ctube-0.0.4/ctube/extractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,32 +9,32 @@
         "navigationEndpoint"]["browseEndpoint"]["browseId"]
 
 
 def extract_artist_music(data: Dict) -> Tuple[List[MusicItem], str]:
     music_items: List[MusicItem] = []
     for item in data["contents"]["singleColumnBrowseResultsRenderer"]["tabs"][0][
         "tabRenderer"]["content"]["sectionListRenderer"]["contents"][
-        0]["gridRenderer"]["items"]:
+            0]["gridRenderer"]["items"]:
 
         item_data = item["musicTwoRowItemRenderer"]
         item_type = item_data["subtitle"]["runs"][0]["text"]
         title = item_data["title"]["runs"][0]["text"]
         release_year = int(item_data["subtitle"]["runs"][-1]["text"])
-        thumbanail_url = item_data["thumbnailRenderer"][
+        thumbnail_url = item_data["thumbnailRenderer"][
             "musicThumbnailRenderer"]["thumbnail"][
             "thumbnails"][-1]["url"]
         playlist_id = item_data["menu"]["menuRenderer"]["items"][
             0]["menuNavigationItemRenderer"]["navigationEndpoint"][
             "watchPlaylistEndpoint"]["playlistId"]
         music_items.append(
             MusicItem(
                 title=title, 
                 item_type=item_type,
                 release_year=release_year,
-                thumbanail_url=thumbanail_url,
+                thumbnail_url=thumbnail_url,
                 playlist_id=playlist_id
             )
         )
     return music_items, data["header"][
         "musicHeaderRenderer"]["title"]["runs"][0]["text"]
```

### Comparing `ctube-0.0.3/ctube/helpers.py` & `ctube-0.0.4/ctube/helpers.py`

 * *Files identical despite different names*

### Comparing `ctube-0.0.3/ctube/parser.py` & `ctube-0.0.4/ctube/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,7 @@
             for index in indexes:
                 if index < 0:
                     raise InvalidIndexSyntax("Indexes must be positive integers.")
                 if index not in filtered_indexes:
                     filtered_indexes.append(index)
             return filtered_indexes
         raise InvalidIndexSyntax(f"Invalid index syntax: {string}")
-
```

### Comparing `ctube-0.0.3/ctube/printers.py` & `ctube-0.0.4/ctube/printers.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,8 +39,8 @@
 
 
 def clear_screen() -> None:
     print("\033c", end="")
 
 
 def write(string: str, col: Color = Color.WHITE):
-    print(color(string, color=col))
+    print(color(string, col=col))
```

### Comparing `ctube-0.0.3/ctube/terminal.py` & `ctube-0.0.4/ctube/terminal.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-import sys, tty, termios
+import sys
+import tty
+import termios
 from typing import List, Optional
 from ctube.colors import Color, color
 
 
 class Prompt:
-    def __init__(self, char: str = "❯", color: Color = Color.GREEN):
+    def __init__(self, char: str = "❯", col: Color = Color.GREEN):
 
         self.char = char
-        self.color = color
+        self.col = col
 
     def get_input(self):
-        return input(f"{color(self.char, self.color)} ")
+        return input(f"{color(self.char, self.col)} ")
 
 
 class Buffer:
     def __init__(self, infinite_scroll: bool = True):
         self.infinite_scroll = infinite_scroll
         self._index = 0
         self._buffer: List[str] = []
```

### Comparing `ctube-0.0.3/pyproject.toml` & `ctube-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ctube"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 authors = ["Simone Gentili <gensydev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://pypi.org/project/ctube/"
 repository = "https://github.com/g3nsy/ctube"
 keywords = ["innertube", "youtube", "youtube-music", "python", "download", "music", "client"]
```

