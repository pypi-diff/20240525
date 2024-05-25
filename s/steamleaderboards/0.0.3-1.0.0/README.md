# Comparing `tmp/steamleaderboards-0.0.3.tar.gz` & `tmp/steamleaderboards-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steamleaderboards-0.0.3.tar", last modified: Wed Feb  6 18:45:52 2019, max compression
+gzip compressed data, was "steamleaderboards-1.0.0.tar", max compression
```

## Comparing `steamleaderboards-0.0.3.tar` & `steamleaderboards-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,6 @@
-drwxrwxrwx   0        0        0        0 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/
--rw-rw-rw-   0        0        0     2094 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1226 2019-02-05 20:19:32.000000 steamleaderboards-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      895 2019-02-06 18:45:17.000000 steamleaderboards-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/steamleaderboards/
--rw-rw-rw-   0        0        0     5571 2019-02-06 18:44:25.000000 steamleaderboards-0.0.3/steamleaderboards/__init__.py
-drwxrwxrwx   0        0        0        0 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/steamleaderboards.egg-info/
--rw-rw-rw-   0        0        0     2094 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/steamleaderboards.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/steamleaderboards.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/steamleaderboards.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/steamleaderboards.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2019-02-06 18:45:52.000000 steamleaderboards-0.0.3/steamleaderboards.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1072 2024-05-24 23:19:06.948186 steamleaderboards-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1962 2024-05-25 01:52:35.242334 steamleaderboards-1.0.0/README.md
+-rw-r--r--   0        0        0      983 2024-05-25 01:11:24.553294 steamleaderboards-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5460 2024-05-25 01:05:23.296288 steamleaderboards-1.0.0/steamleaderboards/__init__.py
+-rw-r--r--   0        0        0     1728 2024-05-25 01:09:21.964292 steamleaderboards-1.0.0/steamleaderboards/__main__.py
+-rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 steamleaderboards-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `steamleaderboards-0.0.3/README.md` & `steamleaderboards-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,73 @@
-# `steamleaderboards`
-
-A package designed to help developers access the leaderboards of various Steam games.
-
-It was created with the Isaac Daily Run scoreboards in mind, but it can be used for other games as well.
-
-## Usage
-
-To use `steamleaderboards`, first create a `LeaderboardGroup` for the desired game.
-
-```python
-import steamleaderboards as sl
-lbgroup = sl.LeaderboardGroup(STEAM_APP_ID)
-```
-
-Once you have created the `LeaderboardGroup`, you can retrieve the desired leaderboards by using the `LeaderboardGroup.get` method.  
-You can specify the name, the display name or the id of the leaderboard to retrieve.
-
-```python
-leaderboard_a = lbgroup.get(name=LEADERBOARD_NAME)
-leaderboard_b = lbgroup.get(lbid=LEADERBOARD_ID)
-leaderboard_c = lbgroup.get(display_name=LEADERBOARD_DISPLAY_NAME)
-```
-
-When you have the `Leaderboard` object, you can find all the entries in the `Leaderboard.entries` field, or you can search for a specific one through the `Leaderboard.find_entry` method.
-
-```python
-all_scores = leaderboard_a.entries
-my_score = leaderboard_a.find_entry(MY_STEAMID_1)
-first_place_score = leaderboard_a.find_entry(rank=1)
-last_place_score = leaderboard_a.find_entry(rank=-1)
-```
+<div align="center">
+
+![](.media/icon-128x128_round.png)
+
+# `steamleaderboards`
+
+Retrieve and parse Steam leaderboards
+
+</div>
+
+## History
+
+It was created with the Isaac Daily Run scoreboards in mind, but it can be used for other games that have a public leaderboard as well.
+
+## Usage
+
+### In code
+
+To use `steamleaderboards`, first install it via PyPI:
+
+```console
+$ # If you're using pip in a venv on 
+$ .venv/bin/pip install steamleaderboards --upgrade
+```
+
+```console
+$ # If you're using poetry 
+$ poetry add steamleaderboards
+```
+
+Then, create a `LeaderboardGroup` for the desired game.
+
+```python
+import steamleaderboards as sl
+lbgroup = sl.LeaderboardGroup(STEAM_APP_ID)
+```
+
+Once you have created the `LeaderboardGroup`, you can retrieve the desired leaderboards by using the `LeaderboardGroup.get` method.  
+You can specify the name, the display name or the id of the leaderboard to retrieve.
+
+```python
+leaderboard_a = lbgroup.get(name=LEADERBOARD_NAME)
+leaderboard_b = lbgroup.get(lbid=LEADERBOARD_ID)
+leaderboard_c = lbgroup.get(display_name=LEADERBOARD_DISPLAY_NAME)
+```
+
+When you have the `Leaderboard` object, you can find all the entries in the `Leaderboard.entries` field, or you can search for a specific one through the `Leaderboard.find_entry` method.
+
+```python
+all_scores = leaderboard_a.entries
+my_score = leaderboard_a.find_entry(MY_STEAMID_1)
+first_place_score = leaderboard_a.find_entry(rank=1)
+last_place_score = leaderboard_a.find_entry(rank=-1)
+```
+
+### In the terminal
+
+To use `steamleaderboards`, first install it via PyPI:
+
+```console
+$ # Using pipx
+$ pipx install steamleaderboards
+```
+
+Then, you can use it to retrieve leaderboards for one or more Steam games via the terminal:
+
+```console
+$ steamleaderboards --output_dir="./data" 440
+```
+
+This will download all leaderboards for Team Fortress 2, the game with the app id `440`, to the `./data` directory.
+
+App ids for games can be found via [SteamDB](https://steamdb.info/).
```

### Comparing `steamleaderboards-0.0.3/steamleaderboards/__init__.py` & `steamleaderboards-1.0.0/steamleaderboards/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-import requests
-from bs4 import BeautifulSoup
-import typing
-
-
-class LeaderboardGroup:
-    def __init__(self, app_id):
-        xml = requests.get(f"https://steamcommunity.com/stats/{app_id}/leaderboards/?xml=1")
-        _bs = BeautifulSoup(xml.content, features="lxml")
-        self.leaderboards = []
-        self.app_id = app_id
-        for leaderboard in _bs.find_all("leaderboard"):
-            self.leaderboards.append(ProtoLeaderboard(leaderboard, app_id))
-
-    def __repr__(self):
-        return f"<LeaderboardGroup for {self.app_id} with {len(self.leaderboards)} leaderboards>"
-
-    def get(self, name=None, *, lbid=None, display_name=None) -> typing.Optional["Leaderboard"]:
-        """Get the full leaderboard with the specified parameter."""
-        if bool(lbid) + bool(name) + bool(display_name) > 1:
-            raise ValueError("You can only find a leaderboard by 1 parameter.")
-        if lbid is not None:
-            if not isinstance(lbid, int):
-                raise ValueError("lbid must be an int")
-            for leaderboard in self.leaderboards:
-                if leaderboard.lbid == lbid:
-                    return leaderboard.full()
-        elif name is not None:
-            if not isinstance(name, str):
-                raise ValueError("name must be a str")
-            for leaderboard in self.leaderboards:
-                if leaderboard.name == name:
-                    return leaderboard.full()
-        elif display_name is not None:
-            if not isinstance(display_name, str):
-                raise ValueError("display_name must be a str")
-            for leaderboard in self.leaderboards:
-                if leaderboard.display_name == display_name:
-                    return leaderboard.full()
-        return None
-
-
-class ProtoLeaderboard:
-    """Information about a leaderboard retrieved through a leaderboard"""
-    def __init__(self, soup, app_id):
-        self.url = soup.url.text
-        self.lbid = int(soup.lbid.text)
-        self.name = soup.find("name").text
-        self.display_name = soup.display_name.text
-        self.entries = int(soup.entries.text)
-        self.sort_method = int(soup.sortmethod.text)
-        self.display_type = int(soup.displaytype.text)
-        self.app_id = app_id
-
-    def full(self) -> "Leaderboard":
-        return Leaderboard(protoleaderboard=self)
-
-
-class Leaderboard:
-    # noinspection PyMissingConstructor
-    def __init__(self, app_id=None, lbid=None, *, protoleaderboard=None):
-        if protoleaderboard:
-            self.url = protoleaderboard.url
-            self.lbid = protoleaderboard.lbid
-            self.name = protoleaderboard.name
-            self.display_name = protoleaderboard.display_name
-            self.entries = protoleaderboard.entries
-            self.sort_method = protoleaderboard.sort_method
-            self.display_type = protoleaderboard.display_type
-            self.app_id = protoleaderboard.app_id
-        elif app_id and lbid:
-            self.lbid = lbid
-            self.app_id = app_id
-            self.url = None
-            self.name = None
-            self.display_name = None
-            self.entries = None
-            self.sort_method = None
-            self.display_type = None
-        else:
-            raise ValueError("No app_id, lbid or protoleaderboard specified")
-        next_request_url = f"https://steamcommunity.com/stats/{self.app_id}/leaderboards/{self.lbid}/?xml=1"
-        self.entries = []
-        while next_request_url:
-            xml = requests.get(next_request_url)
-            _bs = BeautifulSoup(xml.content, features="lxml")
-            for entry in _bs.find_all("entry"):
-                self.entries.append(Entry(entry))
-            if _bs.response.entryend:
-                entry_end = int(_bs.response.entryend.text)
-                if entry_end < int(_bs.response.totalleaderboardentries.text):
-                    next_request_url = f"https://steamcommunity.com/stats/{app_id}/leaderboards/{lbid}/?xml=1&start={entry_end + 1}"
-                else:
-                    next_request_url = None
-            else:
-                next_request_url = None
-
-    def __repr__(self):
-        if self.name:
-            return f'<Leaderboard "{self.name}" for {self.app_id} with {len(self.entries)}>'
-        else:
-            return f'<Leaderboard [{self.lbid}] for {self.app_id} with {len(self.entries)}>'
-
-    def find_entry(self, steam_id=None, *, rank=None):
-        if bool(steam_id) + bool(rank) > 1:
-            raise ValueError("You can only find an entry by 1 parameter.")
-        if steam_id is not None:
-            if not isinstance(steam_id, str):
-                raise ValueError("steam_id must be a str")
-            for entry in self.entries:
-                if entry.steam_id == steam_id:
-                    return entry
-            else:
-                return None
-        elif rank is not None:
-            if not isinstance(rank, int):
-                raise ValueError("steam_id must be an int")
-            try:
-                return self.entries[rank - 1]
-            except IndexError:
-                return None
-
-
-class Entry:
-    def __init__(self, soup):
-        self.steam_id = soup.steamid.text
-        self.score = int(soup.score.text)
-        self.rank = int(soup.rank.text)
-        self.ugcid = soup.ugcid.text
-        self.details = soup.details.text
-
-    def __repr__(self):
-        return f"<Entry #{self.rank} {self.steam_id}: {self.score} pts>"
+import requests
+from bs4 import BeautifulSoup
+import typing
+
+
+class LeaderboardGroup:
+    def __init__(self, app_id):
+        xml = requests.get(f"https://steamcommunity.com/stats/{app_id}/leaderboards/?xml=1")
+        _bs = BeautifulSoup(xml.content, features="lxml-xml")
+        self.leaderboards = []
+        self.app_id = app_id
+        for leaderboard in _bs.find_all("leaderboard"):
+            self.leaderboards.append(ProtoLeaderboard(leaderboard, app_id))
+
+    def __repr__(self):
+        return f"<LeaderboardGroup for {self.app_id} with {len(self.leaderboards)} leaderboards>"
+
+    def get(self, name=None, *, lbid=None, display_name=None) -> typing.Optional["Leaderboard"]:
+        """Get the full leaderboard with the specified parameter."""
+        if bool(lbid) + bool(name) + bool(display_name) > 1:
+            raise ValueError("You can only find a leaderboard by 1 parameter.")
+        if lbid is not None:
+            if not isinstance(lbid, int):
+                raise ValueError("lbid must be an int")
+            for leaderboard in self.leaderboards:
+                if leaderboard.lbid == lbid:
+                    return leaderboard.full()
+        elif name is not None:
+            if not isinstance(name, str):
+                raise ValueError("name must be a str")
+            for leaderboard in self.leaderboards:
+                if leaderboard.name == name:
+                    return leaderboard.full()
+        elif display_name is not None:
+            if not isinstance(display_name, str):
+                raise ValueError("display_name must be a str")
+            for leaderboard in self.leaderboards:
+                if leaderboard.display_name == display_name:
+                    return leaderboard.full()
+        return None
+
+
+class ProtoLeaderboard:
+    """Information about a leaderboard retrieved through a leaderboard"""
+    def __init__(self, soup, app_id):
+        self.url = soup.url.text
+        self.lbid = int(soup.lbid.text)
+        self.name = soup.find("name").text
+        self.display_name = soup.display_name.text
+        self.entries = int(soup.entries.text)
+        self.sort_method = int(soup.sortmethod.text)
+        self.display_type = int(soup.displaytype.text)
+        self.app_id = app_id
+
+    def full(self) -> "Leaderboard":
+        return Leaderboard(protoleaderboard=self)
+
+
+class Leaderboard:
+    # noinspection PyMissingConstructor
+    def __init__(self, app_id=None, lbid=None, *, protoleaderboard=None):
+        if protoleaderboard:
+            self.url = protoleaderboard.url
+            self.lbid = protoleaderboard.lbid
+            self.name = protoleaderboard.name
+            self.display_name = protoleaderboard.display_name
+            self.entries = protoleaderboard.entries
+            self.sort_method = protoleaderboard.sort_method
+            self.display_type = protoleaderboard.display_type
+            self.app_id = protoleaderboard.app_id
+        elif app_id and lbid:
+            self.lbid = lbid
+            self.app_id = app_id
+            self.url = f"https://steamcommunity.com/stats/{self.app_id}/leaderboards/{self.lbid}/?xml=1"
+            self.name = None
+            self.display_name = None
+            self.entries = None
+            self.sort_method = None
+            self.display_type = None
+        else:
+            raise ValueError("No app_id, lbid or protoleaderboard specified")
+        next_request_url = self.url
+        self.entries = []
+        while next_request_url:
+            xml = requests.get(next_request_url)
+            _bs = BeautifulSoup(xml.content, features="lxml-xml")
+            for entry in _bs.find_all("entry"):
+                self.entries.append(Entry(entry))
+            if _bs.response.entryend:
+                entry_end = int(_bs.response.entryend.text)
+                if entry_end < int(_bs.response.totalleaderboardentries.text):
+                    next_request_url = f"https://steamcommunity.com/stats/{self.app_id}/leaderboards/{self.lbid}/?xml=1&start={entry_end + 1}"
+                else:
+                    next_request_url = None
+            else:
+                next_request_url = None
+
+    def __repr__(self):
+        if self.name:
+            return f'<Leaderboard "{self.name}" for {self.app_id} with {len(self.entries)}>'
+        else:
+            return f'<Leaderboard [{self.lbid}] for {self.app_id} with {len(self.entries)}>'
+
+    def find_entry(self, steam_id=None, *, rank=None):
+        if bool(steam_id) + bool(rank) > 1:
+            raise ValueError("You can only find an entry by 1 parameter.")
+        if steam_id is not None:
+            if not isinstance(steam_id, str):
+                raise ValueError("steam_id must be a str")
+            for entry in self.entries:
+                if entry.steam_id == steam_id:
+                    return entry
+            else:
+                return None
+        elif rank is not None:
+            if not isinstance(rank, int):
+                raise ValueError("steam_id must be an int")
+            try:
+                return self.entries[rank - 1]
+            except IndexError:
+                return None
+
+
+class Entry:
+    def __init__(self, soup):
+        self.steam_id = soup.steamid.text
+        self.score = int(soup.score.text)
+        self.rank = int(soup.rank.text)
+        self.ugcid = soup.ugcid.text
+        self.details = soup.details.text
+
+    def __repr__(self):
+        return f"<Entry #{self.rank} {self.steam_id}: {self.score} pts>"
```

