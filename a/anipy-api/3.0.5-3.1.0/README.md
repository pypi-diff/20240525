# Comparing `tmp/anipy_api-3.0.5.tar.gz` & `tmp/anipy_api-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipy_api-3.0.5.tar", max compression
+gzip compressed data, was "anipy_api-3.1.0.tar", max compression
```

## Comparing `anipy_api-3.0.5.tar` & `anipy_api-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      227 2024-05-19 09:41:00.160333 anipy_api-3.0.5/README.md
--rw-r--r--   0        0        0      847 2024-05-19 09:41:00.160333 anipy_api-3.0.5/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/__init__.py
--rw-r--r--   0        0        0     5417 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/anime.py
--rw-r--r--   0        0        0    11550 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/download.py
--rw-r--r--   0        0        0     2765 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/error.py
--rw-r--r--   0        0        0     7953 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/locallist.py
--rw-r--r--   0        0        0    20790 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/mal.py
--rw-r--r--   0        0        0      132 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/__init__.py
--rw-r--r--   0        0        0     5499 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/base.py
--rw-r--r--   0        0        0     1692 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/player.py
--rw-r--r--   0        0        0      267 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/__init__.py
--rw-r--r--   0        0        0     1147 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/mpv.py
--rw-r--r--   0        0        0     2651 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/mpv_control.py
--rw-r--r--   0        0        0      941 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/syncplay.py
--rw-r--r--   0        0        0      918 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/player/players/vlc.py
--rw-r--r--   0        0        0      628 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/__init__.py
--rw-r--r--   0        0        0     5321 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/base.py
--rw-r--r--   0        0        0     3397 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/filter.py
--rw-r--r--   0        0        0     1543 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/provider.py
--rw-r--r--   0        0        0       96 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/providers/__init__.py
--rw-r--r--   0        0        0    12230 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/providers/gogo_provider.py
--rw-r--r--   0        0        0     1482 2024-05-19 09:41:00.160333 anipy_api-3.0.5/src/anipy_api/provider/utils.py
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0      227 2024-05-25 15:13:05.716186 anipy_api-3.1.0/README.md
+-rw-r--r--   0        0        0      847 2024-05-25 15:13:05.716186 anipy_api-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/__init__.py
+-rw-r--r--   0        0        0     5493 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/anime.py
+-rw-r--r--   0        0        0    11550 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/download.py
+-rw-r--r--   0        0        0     2765 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/error.py
+-rw-r--r--   0        0        0     7953 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/locallist.py
+-rw-r--r--   0        0        0    20790 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/mal.py
+-rw-r--r--   0        0        0      132 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/__init__.py
+-rw-r--r--   0        0        0     5499 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/base.py
+-rw-r--r--   0        0        0     1692 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/player.py
+-rw-r--r--   0        0        0      267 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/__init__.py
+-rw-r--r--   0        0        0     1147 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/mpv.py
+-rw-r--r--   0        0        0     2651 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/mpv_control.py
+-rw-r--r--   0        0        0      941 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/syncplay.py
+-rw-r--r--   0        0        0      918 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/player/players/vlc.py
+-rw-r--r--   0        0        0      628 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/__init__.py
+-rw-r--r--   0        0        0     5321 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/base.py
+-rw-r--r--   0        0        0     3397 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/filter.py
+-rw-r--r--   0        0        0     1543 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/provider.py
+-rw-r--r--   0        0        0      183 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/providers/__init__.py
+-rw-r--r--   0        0        0    12240 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/providers/gogo_provider.py
+-rw-r--r--   0        0        0     8521 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/providers/yugen_provider.py
+-rw-r--r--   0        0        0     1482 2024-05-25 15:13:05.716186 anipy_api-3.1.0/src/anipy_api/provider/utils.py
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 anipy_api-3.1.0/PKG-INFO
```

### Comparing `anipy_api-3.0.5/pyproject.toml` & `anipy_api-3.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anipy-api"
-version = "3.0.5"
+version = "3.1.0"
 description = "api for anipy-cli"
 authors = ["sdaqo <sdaqo.dev@protonmail.com>"]
 license = "GPL-3.0"
 repository = "https://github.com/sdaqo/anipy-cli"
 homepage = "https://sdaqo.github.io/anipy-cli"
 documentation = "https://sdaqo.github.io/anipy-cli/getting-started-api"
 keywords = ["anime", "api"]
@@ -13,15 +13,15 @@
   {include = "anipy_api", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-ffmpeg = "^2.0.11"
 pycryptodomex = "^3.20.0"
-requests = "^2.31.0"
+requests = "^2.32.0"
 pypresence = "^4.3.0"
 m3u8 = "^4.1.0"
 beautifulsoup4 = "^4.12.3"
 python-mpv = "^1.0.6"
 dataclasses-json = "^0.6.4"
 levenshtein = "^0.25.1"
```

### Comparing `anipy_api-3.0.5/src/anipy_api/anime.py` & `anipy_api-3.1.0/src/anipy_api/anime.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,11 +151,12 @@
 
         return streams
 
     def __repr__(self) -> str:
         available_langs = "/".join(
             [lang.value.capitalize()[0] for lang in self.languages]
         )
-        return f"{self.name} ({available_langs})"
+        provider_prefix = self.provider.NAME[:2].upper()
+        return f"{provider_prefix}: {self.name} ({available_langs})"
 
     def __hash__(self) -> int:
         return hash(self.provider.NAME + self.identifier)
```

### Comparing `anipy_api-3.0.5/src/anipy_api/download.py` & `anipy_api-3.1.0/src/anipy_api/download.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/error.py` & `anipy_api-3.1.0/src/anipy_api/error.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/locallist.py` & `anipy_api-3.1.0/src/anipy_api/locallist.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/mal.py` & `anipy_api-3.1.0/src/anipy_api/mal.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/player/base.py` & `anipy_api-3.1.0/src/anipy_api/player/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/player/player.py` & `anipy_api-3.1.0/src/anipy_api/player/player.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/player/players/mpv.py` & `anipy_api-3.1.0/src/anipy_api/player/players/mpv.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/player/players/mpv_control.py` & `anipy_api-3.1.0/src/anipy_api/player/players/mpv_control.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/player/players/syncplay.py` & `anipy_api-3.1.0/src/anipy_api/player/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/player/players/vlc.py` & `anipy_api-3.1.0/src/anipy_api/player/players/vlc.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/provider/__init__.py` & `anipy_api-3.1.0/src/anipy_api/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/provider/base.py` & `anipy_api-3.1.0/src/anipy_api/provider/base.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/provider/filter.py` & `anipy_api-3.1.0/src/anipy_api/provider/filter.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/provider/provider.py` & `anipy_api-3.1.0/src/anipy_api/provider/provider.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/src/anipy_api/provider/providers/gogo_provider.py` & `anipy_api-3.1.0/src/anipy_api/provider/providers/gogo_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 class GoGoProvider(BaseProvider):
     """For detailed documentation have a look
     at the [base class][anipy_api.provider.base.BaseProvider].
 
     Attributes:
         NAME: gogoanime
         BASE_URL: https://gogoanime3.co
-        FILTER_CAPS: YEAR, SEASON, STATUS
+        FILTER_CAPS: YEAR, SEASON, STATUS, NO_QUERY
     """
 
     NAME: str = "gogoanime"
     BASE_URL: str = "https://gogoanime3.co"
     FILTER_CAPS: FilterCapabilities = (
         FilterCapabilities.YEAR
         | FilterCapabilities.SEASON
```

### Comparing `anipy_api-3.0.5/src/anipy_api/provider/utils.py` & `anipy_api-3.1.0/src/anipy_api/provider/utils.py`

 * *Files identical despite different names*

### Comparing `anipy_api-3.0.5/PKG-INFO` & `anipy_api-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anipy-api
-Version: 3.0.5
+Version: 3.1.0
 Summary: api for anipy-cli
 Home-page: https://sdaqo.github.io/anipy-cli
 License: GPL-3.0
 Keywords: anime,api
 Author: sdaqo
 Author-email: sdaqo.dev@protonmail.com
 Requires-Python: >=3.9,<4.0
@@ -18,15 +18,15 @@
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Requires-Dist: levenshtein (>=0.25.1,<0.26.0)
 Requires-Dist: m3u8 (>=4.1.0,<5.0.0)
 Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
 Requires-Dist: pypresence (>=4.3.0,<5.0.0)
 Requires-Dist: python-ffmpeg (>=2.0.11,<3.0.0)
 Requires-Dist: python-mpv (>=1.0.6,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/sdaqo/anipy-cli/issues
 Project-URL: Documentation, https://sdaqo.github.io/anipy-cli/getting-started-api
 Project-URL: Repository, https://github.com/sdaqo/anipy-cli
 Description-Content-Type: text/markdown
 
 # anipy-api
 This is the api package for [anipy-cli](https://pypi.org/project/anipy-cli/).
```

