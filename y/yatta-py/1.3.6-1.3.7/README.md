# Comparing `tmp/yatta_py-1.3.6.tar.gz` & `tmp/yatta_py-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatta_py-1.3.6.tar", max compression
+gzip compressed data, was "yatta_py-1.3.7.tar", max compression
```

## Comparing `yatta_py-1.3.6.tar` & `yatta_py-1.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35803 2024-01-14 04:26:04.823894 yatta_py-1.3.6/LICENSE
--rw-r--r--   0        0        0     1454 2024-05-15 01:02:23.742621 yatta_py-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     2120 2024-05-15 01:01:47.122575 yatta_py-1.3.6/README.md
--rw-r--r--   0        0        0       95 2024-03-22 02:44:08.196644 yatta_py-1.3.6/yatta/__init__.py
--rw-r--r--   0        0        0    13680 2024-04-05 00:09:28.638364 yatta_py-1.3.6/yatta/client.py
--rw-r--r--   0        0        0      596 2024-04-05 00:09:28.638364 yatta_py-1.3.6/yatta/enums.py
--rw-r--r--   0        0        0      664 2024-04-05 00:09:28.638364 yatta_py-1.3.6/yatta/exceptions.py
--rw-r--r--   0        0        0      168 2024-01-14 04:26:04.825416 yatta_py-1.3.6/yatta/models/__init__.py
--rw-r--r--   0        0        0      862 2024-04-04 23:38:17.654235 yatta_py-1.3.6/yatta/models/base.py
--rw-r--r--   0        0        0     1388 2024-04-05 00:09:28.638364 yatta_py-1.3.6/yatta/models/book.py
--rw-r--r--   0        0        0      731 2024-04-04 23:38:17.655237 yatta_py-1.3.6/yatta/models/change_log.py
--rw-r--r--   0        0        0    12524 2024-04-05 00:32:54.719733 yatta_py-1.3.6/yatta/models/character.py
--rw-r--r--   0        0        0     2938 2024-04-05 00:09:28.638364 yatta_py-1.3.6/yatta/models/item.py
--rw-r--r--   0        0        0     3967 2024-04-05 00:09:28.639369 yatta_py-1.3.6/yatta/models/light_cone.py
--rw-r--r--   0        0        0      565 2024-04-04 23:38:17.656244 yatta_py-1.3.6/yatta/models/message.py
--rw-r--r--   0        0        0     2014 2024-04-04 23:46:45.749929 yatta_py-1.3.6/yatta/models/relic.py
--rw-r--r--   0        0        0     2120 2024-04-05 00:32:19.587547 yatta_py-1.3.6/yatta/utils.py
--rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 yatta_py-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    35803 2024-01-14 04:26:04.823894 yatta_py-1.3.7/LICENSE
+-rw-r--r--   0        0        0     1586 2024-05-25 08:09:11.899152 yatta_py-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2123 2024-05-25 05:24:37.488891 yatta_py-1.3.7/README.md
+-rw-r--r--   0        0        0       95 2024-03-22 02:44:08.196644 yatta_py-1.3.7/yatta/__init__.py
+-rw-r--r--   0        0        0    14038 2024-05-25 08:08:20.811168 yatta_py-1.3.7/yatta/client.py
+-rw-r--r--   0        0        0      596 2024-04-05 00:09:28.638364 yatta_py-1.3.7/yatta/enums.py
+-rw-r--r--   0        0        0      664 2024-04-05 00:09:28.638364 yatta_py-1.3.7/yatta/exceptions.py
+-rw-r--r--   0        0        0      168 2024-01-14 04:26:04.825416 yatta_py-1.3.7/yatta/models/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-04 23:38:17.654235 yatta_py-1.3.7/yatta/models/base.py
+-rw-r--r--   0        0        0     2431 2024-05-15 01:09:49.929359 yatta_py-1.3.7/yatta/models/book.py
+-rw-r--r--   0        0        0      731 2024-04-04 23:38:17.655237 yatta_py-1.3.7/yatta/models/change_log.py
+-rw-r--r--   0        0        0    12524 2024-04-05 00:32:54.719733 yatta_py-1.3.7/yatta/models/character.py
+-rw-r--r--   0        0        0     2938 2024-04-05 00:09:28.638364 yatta_py-1.3.7/yatta/models/item.py
+-rw-r--r--   0        0        0     3967 2024-04-05 00:09:28.639369 yatta_py-1.3.7/yatta/models/light_cone.py
+-rw-r--r--   0        0        0      565 2024-04-04 23:38:17.656244 yatta_py-1.3.7/yatta/models/message.py
+-rw-r--r--   0        0        0     2014 2024-04-04 23:46:45.749929 yatta_py-1.3.7/yatta/models/relic.py
+-rw-r--r--   0        0        0     2120 2024-04-05 00:32:19.587547 yatta_py-1.3.7/yatta/utils.py
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 yatta_py-1.3.7/PKG-INFO
```

### Comparing `yatta_py-1.3.6/LICENSE` & `yatta_py-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/pyproject.toml` & `yatta_py-1.3.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [project]
 name = "yatta-py"
 requires-python = ">=3.11"
 
+[project.urls]
+"Bug Tracker" = "https://github.com/seriaati/yatta/issues"
+Repository = "https://github.com/seriaati/yatta.git"
+
 [tool.poetry]
 authors = ["seriaati <seria.ati@gmail.com>"]
 description = "Python async API wrapper for hsr.yatta.top"
 license = "GPL-3.0"
 name = "yatta-py"
 packages = [{include = "yatta"}]
 readme = "README.md"
-version = "1.3.6"
+version = "1.3.7"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.9.1"
 aiohttp-client-cache = {extras = ["sqlite"], version = "^0.11.0"}
 pydantic = "^2.5.2"
 python = "^3.11"
```

### Comparing `yatta_py-1.3.6/README.md` & `yatta_py-1.3.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Quick links
 
 Developing something for Hoyoverse games? Here's a collection of Python async API wrappers for Hoyoverse games made by me:
 
 - [enka.py](https://github.com/seriaati/enka-py) is an Enka Network API wrapper for fetching in-game showcase.
 - [yatta.py](https://github.com/seriaati/yatta) is a Project Yatta API wrapper for fetching Honkai Star Rail game data.
 - [ambr.py](https://github.com/seriaati/ambr) is a Project Ambr API wrapper for fetching Genshin Impact game data.
-- [hakushin.py](https://github.com/seriaati/hakushin) is a Hakushin API wrapper for fetching Genshin Impact and Honkai Star Rail beta game data.
+- [hakushin.py](https://github.com/seriaati/hakushin-py) is a Hakushin API wrapper for fetching Genshin Impact and Honkai Star Rail beta game data.
 
 ## Introduction
 
 yatta-py is an async API wrapper for [Project Yatta](https://hsr.yatta.top/) written in Python.  
 Project Yatta is a beautiful website that displays Honkai: Star Rail game data.
 
 > Note: I am not the developer of Project Yatta.
```

### Comparing `yatta_py-1.3.6/yatta/client.py` & `yatta_py-1.3.7/yatta/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from __future__ import annotations
+
 import logging
 from enum import Enum
-from typing import Any, Final
+from typing import TYPE_CHECKING, Any, Final, Self
 
 from aiohttp_client_cache.backends.sqlite import SQLiteBackend
 from aiohttp_client_cache.session import CachedSession
 
 from .exceptions import ConnectionTimeoutError, DataNotFoundError, YattaAPIError
 from .models import (
     Book,
@@ -17,14 +19,17 @@
     LightCone,
     LightConeDetail,
     Message,
     RelicSet,
     RelicSetDetail,
 )
 
+if TYPE_CHECKING:
+    import aiohttp
+
 __all__ = ("Language", "YattaAPI")
 
 LOGGER_ = logging.getLogger("yatta.py")
 
 
 class Language(Enum):
     CHT = "cht"
@@ -42,45 +47,39 @@
     VI = "vi"
 
 
 class YattaAPI:
     """
     The main class that is used to interact with the API.
 
-    Parameters
-    ----------
-    lang : Language, optional
-        The language to use for the API. Defaults to Language.EN.
-    cache_ttl : int, optional
-        The time to live for the cache. Defaults to 3600.
-
-    Attributes
-    ----------
-    BASE_URL : str
-        The base URL for the API. This is used internally.
-    lang : Language
-        The language that is used for the API.
+    Parameters:
+        lang: The language to use for the API. Defaults to Language.EN.
+        cache_ttl: The time-to-live for the cache in seconds. Defaults to 3600.
+        headers: A dictionary of headers to use for the requests. Defaults to None.
+        session: An aiohttp.ClientSession to use for the requests. Defaults to None.
     """
 
     BASE_URL: Final[str] = "https://api.yatta.top/hsr/v2"
 
     def __init__(
         self,
         *,
         lang: Language = Language.EN,
         cache_ttl: int = 3600,
         headers: dict[str, Any] | None = None,
+        session: aiohttp.ClientSession | None = None,
     ) -> None:
         self.lang = lang
         self.cache_ttl = cache_ttl
 
+        self._session = session
         self._cache = SQLiteBackend("./.cache/yatta/aiohttp-cache.db", expire_after=cache_ttl)
         self._headers = headers or {"User-Agent": "yatta-py"}
 
-    async def __aenter__(self) -> "YattaAPI":
+    async def __aenter__(self) -> Self:
         await self.start()
         return self
 
     async def __aexit__(self, exc_type, exc, tb) -> None:  # noqa: ANN001
         await self.close()
 
     async def _request(
@@ -104,22 +103,26 @@
             The response from the API.
 
         Raises
         ------
         DataNotFound
             If the requested data is not found.
         """
+        if self._session is None:
+            msg = "Call `start` before making requests."
+            raise RuntimeError(msg)
+
         if static:
             url = f"{self.BASE_URL}/static/{endpoint}"
         else:
             url = f"{self.BASE_URL}/{self.lang.value}/{endpoint}"
 
         LOGGER_.debug("Requesting %s...", url)
 
-        if not use_cache:
+        if not use_cache and isinstance(self._session, CachedSession):
             async with self._session.disabled(), self._session.get(url) as resp:
                 if resp.status != 200:
                     self._handle_error(resp.status)
                 data: dict[str, Any] = await resp.json()
         else:
             async with self._session.get(url) as resp:
                 if resp.status != 200:
@@ -140,21 +143,22 @@
             case _:
                 raise YattaAPIError(code)
 
     async def start(self) -> None:
         """
         Starts the client session.
         """
-        self._session = CachedSession(headers=self._headers, cache=self._cache)
+        self._session = self._session or CachedSession(headers=self._headers, cache=self._cache)
 
     async def close(self) -> None:
         """
         Closes the client session and cache.
         """
-        await self._session.close()
+        if self._session is not None:
+            await self._session.close()
 
     async def fetch_books(self, use_cache: bool = True) -> list[Book]:
         """
         Fetch all books from the API.
 
         Parameters
         ----------
```

### Comparing `yatta_py-1.3.6/yatta/enums.py` & `yatta_py-1.3.7/yatta/enums.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/exceptions.py` & `yatta_py-1.3.7/yatta/exceptions.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/models/base.py` & `yatta_py-1.3.7/yatta/models/base.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/models/change_log.py` & `yatta_py-1.3.7/yatta/models/change_log.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/models/character.py` & `yatta_py-1.3.7/yatta/models/character.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/models/item.py` & `yatta_py-1.3.7/yatta/models/item.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/models/light_cone.py` & `yatta_py-1.3.7/yatta/models/light_cone.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/models/message.py` & `yatta_py-1.3.7/yatta/models/message.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/models/relic.py` & `yatta_py-1.3.7/yatta/models/relic.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/yatta/utils.py` & `yatta_py-1.3.7/yatta/utils.py`

 * *Files identical despite different names*

### Comparing `yatta_py-1.3.6/PKG-INFO` & `yatta_py-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatta-py
-Version: 1.3.6
+Version: 1.3.7
 Summary: Python async API wrapper for hsr.yatta.top
 License: GPL-3.0
 Author: seriaati
 Author-email: seria.ati@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 ## Quick links
 
 Developing something for Hoyoverse games? Here's a collection of Python async API wrappers for Hoyoverse games made by me:
 
 - [enka.py](https://github.com/seriaati/enka-py) is an Enka Network API wrapper for fetching in-game showcase.
 - [yatta.py](https://github.com/seriaati/yatta) is a Project Yatta API wrapper for fetching Honkai Star Rail game data.
 - [ambr.py](https://github.com/seriaati/ambr) is a Project Ambr API wrapper for fetching Genshin Impact game data.
-- [hakushin.py](https://github.com/seriaati/hakushin) is a Hakushin API wrapper for fetching Genshin Impact and Honkai Star Rail beta game data.
+- [hakushin.py](https://github.com/seriaati/hakushin-py) is a Hakushin API wrapper for fetching Genshin Impact and Honkai Star Rail beta game data.
 
 ## Introduction
 
 yatta-py is an async API wrapper for [Project Yatta](https://hsr.yatta.top/) written in Python.  
 Project Yatta is a beautiful website that displays Honkai: Star Rail game data.
 
 > Note: I am not the developer of Project Yatta.
```

