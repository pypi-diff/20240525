# Comparing `tmp/fortnitepy-edit-1.0.8.tar.gz` & `tmp/fortnitepy-edit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortnitepy-edit-1.0.8.tar", last modified: Wed Feb 14 19:19:39 2024, max compression
+gzip compressed data, was "fortnitepy-edit-1.0.9.tar", last modified: Sat May 25 14:50:59 2024, max compression
```

## Comparing `fortnitepy-edit-1.0.8.tar` & `fortnitepy-edit-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 19:19:39.149483 fortnitepy-edit-1.0.8/
--rw-r--r--   0 runner    (1000) runner    (1000)     4348 2024-02-14 19:19:39.145483 fortnitepy-edit-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     3298 2023-12-30 14:38:03.000000 fortnitepy-edit-1.0.8/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 19:19:39.137482 fortnitepy-edit-1.0.8/fortnitepy/
--rw-rw----   0 runner    (1000) runner    (1000)     2293 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/__init__.py
--rw-rw----   0 runner    (1000) runner    (1000)    40932 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/auth.py
--rw-rw----   0 runner    (1000) runner    (1000)   117774 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/client.py
--rw-rw----   0 runner    (1000) runner    (1000)     8250 2024-01-04 12:16:12.000000 fortnitepy-edit-1.0.8/fortnitepy/enums.py
--rw-rw----   0 runner    (1000) runner    (1000)     7760 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/errors.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 19:19:39.061474 fortnitepy-edit-1.0.8/fortnitepy/ext/
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 19:19:39.145483 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/
--rw-rw----   0 runner    (1000) runner    (1000)      195 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/__init__.py
--rw-rw----   0 runner    (1000) runner    (1000)     1130 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/_types.py
--rw-rw----   0 runner    (1000) runner    (1000)    32192 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/bot.py
--rw-rw----   0 runner    (1000) runner    (1000)    15374 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/cog.py
--rw-rw----   0 runner    (1000) runner    (1000)    11690 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/context.py
--rw-rw----   0 runner    (1000) runner    (1000)     6113 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/converter.py
--rw-rw----   0 runner    (1000) runner    (1000)     8382 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/cooldown.py
--rw-rw----   0 runner    (1000) runner    (1000)    60255 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/core.py
--rw-rw----   0 runner    (1000) runner    (1000)    14407 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/errors.py
--rw-rw----   0 runner    (1000) runner    (1000)    50693 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/help.py
--rw-rw----   0 runner    (1000) runner    (1000)     1214 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/typedefs.py
--rw-rw----   0 runner    (1000) runner    (1000)     6204 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/ext/commands/view.py
--rw-rw----   0 runner    (1000) runner    (1000)    18535 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/friend.py
--rw-rw----   0 runner    (1000) runner    (1000)    61318 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/http.py
--rw-rw----   0 runner    (1000) runner    (1000)     3674 2024-02-01 09:11:29.000000 fortnitepy-edit-1.0.8/fortnitepy/kairos.py
--rw-rw----   0 runner    (1000) runner    (1000)     3852 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/message.py
--rw-rw----   0 runner    (1000) runner    (1000)     2670 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/news.py
--rw-r--r--   0 runner    (1000) runner    (1000)   152023 2024-02-14 19:14:19.000000 fortnitepy-edit-1.0.8/fortnitepy/party.py
--rw-rw----   0 runner    (1000) runner    (1000)     3748 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/playlist.py
--rw-rw----   0 runner    (1000) runner    (1000)    13918 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/presence.py
--rw-rw----   0 runner    (1000) runner    (1000)    10143 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/stats.py
--rw-rw----   0 runner    (1000) runner    (1000)    10533 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/store.py
--rw-rw----   0 runner    (1000) runner    (1000)     1361 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/typedefs.py
--rw-rw----   0 runner    (1000) runner    (1000)    22715 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/user.py
--rw-rw----   0 runner    (1000) runner    (1000)     2556 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/utils.py
--rw-rw----   0 runner    (1000) runner    (1000)    58476 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.8/fortnitepy/xmpp.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-02-14 19:19:39.145483 fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     4348 2024-02-14 19:19:38.000000 fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1026 2024-02-14 19:19:38.000000 fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-02-14 19:19:38.000000 fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       87 2024-02-14 19:19:38.000000 fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-02-14 19:19:38.000000 fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      567 2024-02-01 09:17:33.000000 fortnitepy-edit-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-02-14 19:19:39.149483 fortnitepy-edit-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1846 2024-02-14 19:15:56.000000 fortnitepy-edit-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 14:50:59.704959 fortnitepy-edit-1.0.9/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4519 2024-05-25 14:50:59.704959 fortnitepy-edit-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     3298 2023-12-30 14:38:03.000000 fortnitepy-edit-1.0.9/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 14:50:59.684957 fortnitepy-edit-1.0.9/fortnitepy/
+-rw-rw----   0 runner    (1000) runner    (1000)     2286 2024-05-25 14:49:52.000000 fortnitepy-edit-1.0.9/fortnitepy/__init__.py
+-rw-rw----   0 runner    (1000) runner    (1000)    40932 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/auth.py
+-rw-rw----   0 runner    (1000) runner    (1000)   117769 2024-05-25 14:48:09.000000 fortnitepy-edit-1.0.9/fortnitepy/client.py
+-rw-rw----   0 runner    (1000) runner    (1000)     8287 2024-05-25 14:48:22.000000 fortnitepy-edit-1.0.9/fortnitepy/enums.py
+-rw-rw----   0 runner    (1000) runner    (1000)     7760 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/errors.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 14:50:59.672956 fortnitepy-edit-1.0.9/fortnitepy/ext/
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 14:50:59.700958 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/
+-rw-rw----   0 runner    (1000) runner    (1000)      195 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/__init__.py
+-rw-rw----   0 runner    (1000) runner    (1000)     1130 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/_types.py
+-rw-rw----   0 runner    (1000) runner    (1000)    32192 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/bot.py
+-rw-rw----   0 runner    (1000) runner    (1000)    15374 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/cog.py
+-rw-rw----   0 runner    (1000) runner    (1000)    11690 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/context.py
+-rw-rw----   0 runner    (1000) runner    (1000)     6113 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/converter.py
+-rw-rw----   0 runner    (1000) runner    (1000)     8382 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/cooldown.py
+-rw-rw----   0 runner    (1000) runner    (1000)    60255 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/core.py
+-rw-rw----   0 runner    (1000) runner    (1000)    14407 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/errors.py
+-rw-rw----   0 runner    (1000) runner    (1000)    50693 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/help.py
+-rw-rw----   0 runner    (1000) runner    (1000)     1214 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/typedefs.py
+-rw-rw----   0 runner    (1000) runner    (1000)     6204 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/ext/commands/view.py
+-rw-rw----   0 runner    (1000) runner    (1000)    18535 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/friend.py
+-rw-rw----   0 runner    (1000) runner    (1000)    61318 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/http.py
+-rw-rw----   0 runner    (1000) runner    (1000)     3674 2024-02-01 09:11:29.000000 fortnitepy-edit-1.0.9/fortnitepy/kairos.py
+-rw-rw----   0 runner    (1000) runner    (1000)     3852 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/message.py
+-rw-rw----   0 runner    (1000) runner    (1000)     2670 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/news.py
+-rw-r--r--   0 runner    (1000) runner    (1000)   152282 2024-05-25 14:46:22.000000 fortnitepy-edit-1.0.9/fortnitepy/party.py
+-rw-rw----   0 runner    (1000) runner    (1000)     3748 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/playlist.py
+-rw-rw----   0 runner    (1000) runner    (1000)    13918 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/presence.py
+-rw-rw----   0 runner    (1000) runner    (1000)    10143 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/stats.py
+-rw-rw----   0 runner    (1000) runner    (1000)    10533 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/store.py
+-rw-rw----   0 runner    (1000) runner    (1000)     1361 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/typedefs.py
+-rw-rw----   0 runner    (1000) runner    (1000)    22715 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/user.py
+-rw-rw----   0 runner    (1000) runner    (1000)     2556 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/utils.py
+-rw-rw----   0 runner    (1000) runner    (1000)    58476 2023-12-31 17:25:55.000000 fortnitepy-edit-1.0.9/fortnitepy/xmpp.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-25 14:50:59.704959 fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     4519 2024-05-25 14:50:59.000000 fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1026 2024-05-25 14:50:59.000000 fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-25 14:50:59.000000 fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       87 2024-05-25 14:50:59.000000 fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       11 2024-05-25 14:50:59.000000 fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      567 2024-02-01 09:17:33.000000 fortnitepy-edit-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-25 14:50:59.704959 fortnitepy-edit-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1846 2024-05-25 14:45:45.000000 fortnitepy-edit-1.0.9/setup.py
```

### Comparing `fortnitepy-edit-1.0.8/PKG-INFO` & `fortnitepy-edit-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortnitepy-edit
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for interacting with fortnite services
 Author: klld
 License: MIT
 Project-URL: Documentation, https://fortnitepy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/klldme/fortnitepy-edit/Issue
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5.3
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp>=3.3
+Requires-Dist: aioxmpp>=0.10.4
+Requires-Dist: aioconsole>=0.1.15
+Requires-Dist: pytz
 Provides-Extra: docs
+Requires-Dist: sphinxcontrib_trio==1.1.0; extra == "docs"
 
  # fortnitepy-edit
 
 [![Supported py versions](https://img.shields.io/pypi/pyversions/fortnitepy-edit.svg)](https://pypi.org/project/fortnitepy-edit/)
 [![Current pypi version](https://img.shields.io/pypi/v/fortnitepy-edit.svg)](https://pypi.org/project/fortnitepy-edit/)
```

### Comparing `fortnitepy-edit-1.0.8/README.md` & `fortnitepy-edit-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/__init__.py` & `fortnitepy-edit-1.0.9/fortnitepy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa
 
 """
 MIT License
 
-Copyright (c) 2019-2021 Terbau
+Copyright (c) 2024 klld
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -21,15 +21,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = '3.6.9'
+__version__ = '1.0.9'
 
 from .client import Client, run_multiple, start_multiple, close_multiple
 from .auth import (Auth, EmailAndPasswordAuth, ExchangeCodeAuth,
                    AuthorizationCodeAuth, DeviceAuth, RefreshTokenAuth,
                    AdvancedAuth)
 from .friend import Friend, IncomingPendingFriend, OutgoingPendingFriend
 from .message import FriendMessage, PartyMessage
```

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/auth.py` & `fortnitepy-edit-1.0.9/fortnitepy/auth.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/client.py` & `fortnitepy-edit-1.0.9/fortnitepy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 """
 MIT License
 
-Copyright (c) 2019-2021 Terbau
+Copyright (c) 2024 klld
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -557,21 +557,21 @@
                  **kwargs: Any) -> None:
 
         self.loop = loop or asyncio.get_event_loop()
 
         self.status = kwargs.get('status', 'Battle Royale Lobby - {party_size} / {party_max_size}')  # noqa
         self.away = kwargs.get('away', AwayStatus.ONLINE)
         self.avatar = kwargs.get('avatar', get_random_default_avatar())  # noqa
-        self.platform = kwargs.get('platform', Platform.WINDOWS)
+        self.platform = kwargs.get('platform', Platform.EPIC_GAMES)
         self.net_cl = kwargs.get('net_cl', '')
         self.party_version = kwargs.get('party_version', 3)
         self.party_build_id = '1:{0.party_version}:{0.net_cl}'.format(self)
         self.default_party_config = kwargs.get('default_party_config', DefaultPartyConfig())  # noqa
         self.default_party_member_config = kwargs.get('default_party_member_config', DefaultPartyMemberConfig())  # noqa
-        self.build = kwargs.get('build', '++Fortnite+Release-14.10-CL-14288110')  # noqa
+        self.build = kwargs.get('build', '++Fortnite+Release-29.00-CL-31978752')  # noqa
         self.os = kwargs.get('os', 'Windows/10.0.17134.1.768.64bit')
         self.service_host = kwargs.get('xmpp_host', 'prod.ol.epicgames.com')
         self.service_domain = kwargs.get('xmpp_domain', 'xmpp-service-prod.ol.epicgames.com')  # noqa
         self.service_port = kwargs.get('xmpp_port', 5222)
         self.cache_users = kwargs.get('cache_users', True)
         self.fetch_user_data_in_events = kwargs.get('fetch_user_data_in_events', True)  # noqa
         self.wait_for_member_meta_in_events = kwargs.get('wait_for_member_meta_in_events', True)  # noqa
@@ -3353,8 +3353,8 @@
             LTMs are for the specified region.
         """
         data = await self.http.fortnite_get_timeline()
 
         states = data['channels']['client-matchmaking']['states']
         region_data = states[len(states) - 1]['state']['region'].get(
             region.value, {})
-        return region_data.get('eventFlagsForcedOn', [])
+        return region_data.get('eventFlagsForcedOn', [])
```

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/enums.py` & `fortnitepy-edit-1.0.9/fortnitepy/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # flake8: noqa
 
 """
 MIT License
 
-Copyright (c) 2019-2021 Terbau
+Copyright (c) 2024 klld
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -136,15 +136,14 @@
     CID_A_278_Athena_Commando_F_Prime_G = 5
     CID_A_279_Athena_Commando_M_Prime = 6
     CID_A_280_Athena_Commando_M_Prime_B = 7
     CID_A_282_Athena_Commando_M_Prime_D = 8
     CID_A_283_Athena_Commando_M_Prime_E = 9
     CID_A_284_Athena_Commando_M_Prime_F = 10
 
-
 class V1Gamemode(Enum):
     SOLO  = 'p2'
     DUO   = 'p10'
     SQUAD = 'p9'
 
 
 class V1Platform(Enum):
@@ -257,14 +256,15 @@
     SEASON_11 = ('s11_social_bp_level', SeasonEndTimestamp.SEASON_11.value)
     SEASON_12 = ('s11_social_bp_level', SeasonEndTimestamp.SEASON_12.value)
     SEASON_13 = (('s13_social_bp_level', 's11_social_bp_level'), SeasonEndTimestamp.SEASON_13.value)
     SEASON_14 = ('s14_social_bp_level', SeasonEndTimestamp.SEASON_14.value)
     SEASON_15 = ('s15_social_bp_level', SeasonEndTimestamp.SEASON_15.value)
     SEASON_16 = ('s16_social_bp_level', SeasonEndTimestamp.SEASON_16.value)
     SEASON_17 = ('s17_social_bp_level', None)
+    SEASON_29 = ('s29_social_bp_level', None)
 
 
 class KairosBackgroundColorPreset(Enum):
     TEAL         = ["#8EFDE5","#1CBA9E","#034D3F"]
     SWEET_RED    = ["#FF81AE","#D8033C","#790625"]
     LIGHT_ORANGE = ["#FFDF00","#FBA000","#975B04"]
     GREEN        = ["#CCF95A","#30C11B","#194D12"]
@@ -276,8 +276,8 @@
     ORANGE       = ["#FFAF5D","#FF6D32","#852A05"]
     DARK_PURPLE  = ["#E93FEB","#7B009C","#500066"]
     LIME         = ["#DFFF73","#86CF13","#404B07"]
     INDIGO       = ["#B35EEF","#4D1397","#2E0A5D"]
 
 
 class StatsCollectionType(Enum):
-    FISH = 'collection_fish'
+    FISH = 'collection_fish'
```

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/errors.py` & `fortnitepy-edit-1.0.9/fortnitepy/errors.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/_types.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/bot.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/cog.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/context.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/converter.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/cooldown.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/cooldown.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/core.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/errors.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/help.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/typedefs.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/typedefs.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/ext/commands/view.py` & `fortnitepy-edit-1.0.9/fortnitepy/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/friend.py` & `fortnitepy-edit-1.0.9/fortnitepy/friend.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/http.py` & `fortnitepy-edit-1.0.9/fortnitepy/http.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/kairos.py` & `fortnitepy-edit-1.0.9/fortnitepy/kairos.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/message.py` & `fortnitepy-edit-1.0.9/fortnitepy/message.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/news.py` & `fortnitepy-edit-1.0.9/fortnitepy/news.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/party.py` & `fortnitepy-edit-1.0.9/fortnitepy/party.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,15 +636,15 @@
             }),
             'Default:AthenaCosmeticLoadout_j': json.dumps({
                 'AthenaCosmeticLoadout': {
                     'characterPrimaryAssetId': ("AthenaCharacter:{0}".format(self.def_character)),
                     'characterEKey': '',
                     'backpackDef': 'None',
                     'backpackEKey': '',
-                    'pickaxeDef': ("/Game/Athena/Items/Cosmetics/Pickaxes/DefaultPickaxe.DefaultPickaxe"),
+                    'pickaxeDef': 'None',
                     'pickaxeEKey': '',
                     'contrailDef': '/Game/Athena/Items/Cosmetics/Contrails/DefaultContrail.DefaultContrail',
                     'contrailEKey': '',
                     'scratchpad': [],
                     "cosmeticStats": [
                               {
                                 "statName": "HabaneroProgression", 
@@ -1427,17 +1427,18 @@
     @property
     def backpack(self) -> str:
         """:class:`str`: The BID of the backpack this member currently has equipped.
         ``None`` if no backpack is equipped.
         """
         asset = self.meta.backpack
         if '/petcarriers/' not in asset.lower():
-          return asset
-        else:
-          return None
+            result = re.search(r".*\.([^\'\"]*)", asset.strip("'"))
+
+            if result is not None and result.group(1) != 'None':
+                return result.group(1)
 
     @property
     def pet(self) -> str:
         """:class:`str`: The ID of the pet this member currently has equipped.
         ``None`` if no pet is equipped.
         """
         asset = self.meta.backpack
@@ -1448,15 +1449,18 @@
 
     @property
     def pickaxe(self) -> str:
         """:class:`str`: The pickaxe id of the pickaxe this member currently
         has equipped.
         """
         asset = self.meta.pickaxe
-        return asset
+        result = re.search(r".*\.([^\'\"]*)", asset.strip("'"))
+
+        if result is not None and result.group(1) != 'None':
+            return result.group(1)
 
     @property
     def contrail(self) -> str:
         """:class:`str`: The contrail id of the pickaxe this member currently
         has equipped.
         """
         asset = self.meta.contrail
@@ -2276,15 +2280,15 @@
         Raises
         ------
         HTTPException
             An error occured while requesting.
         """
         if asset is not None:
             if asset != '' and '.' not in asset:
-                asset = ("AthenaBackpack:{0}".format(asset))
+                asset = ("/BRCosmetics/Athena/Items/Cosmetics/Backpacks/{0}.{0}".format(asset))
         else:
             prop = self.meta.get_prop('Default:AthenaCosmeticLoadout_j')
             asset = prop['AthenaCosmeticLoadout']['backpackDef']
 
         if enlightenment is not None:
             if len(enlightenment) != 2:
                 raise ValueError('enlightenment has to be a list/tuple with '
@@ -2437,15 +2441,15 @@
         Raises
         ------
         HTTPException
             An error occured while requesting.
         """
         if asset is not None:
             if asset != '' and '.' not in asset:
-                asset = ("AthenaPickaxe:{0}".format(asset))
+                asset = ("/BRCosmetics/Athena/Items/Cosmetics/Pickaxes/{0}.{0}".format(asset))
         else:
             prop = self.meta.get_prop('Default:AthenaCosmeticLoadout_j')
             asset = prop['AthenaCosmeticLoadout']['pickaxeDef']
 
         new = self.meta.variants
         if variants is not None:
             new['AthenaPickaxe'] = {'i': variants}
```

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/playlist.py` & `fortnitepy-edit-1.0.9/fortnitepy/playlist.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/presence.py` & `fortnitepy-edit-1.0.9/fortnitepy/presence.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/stats.py` & `fortnitepy-edit-1.0.9/fortnitepy/stats.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/store.py` & `fortnitepy-edit-1.0.9/fortnitepy/store.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/typedefs.py` & `fortnitepy-edit-1.0.9/fortnitepy/typedefs.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/user.py` & `fortnitepy-edit-1.0.9/fortnitepy/user.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/utils.py` & `fortnitepy-edit-1.0.9/fortnitepy/utils.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy/xmpp.py` & `fortnitepy-edit-1.0.9/fortnitepy/xmpp.py`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/PKG-INFO` & `fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortnitepy-edit
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for interacting with fortnite services
 Author: klld
 License: MIT
 Project-URL: Documentation, https://fortnitepy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/klldme/fortnitepy-edit/Issue
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5.3
 Description-Content-Type: text/markdown
+Requires-Dist: aiohttp>=3.3
+Requires-Dist: aioxmpp>=0.10.4
+Requires-Dist: aioconsole>=0.1.15
+Requires-Dist: pytz
 Provides-Extra: docs
+Requires-Dist: sphinxcontrib_trio==1.1.0; extra == "docs"
 
  # fortnitepy-edit
 
 [![Supported py versions](https://img.shields.io/pypi/pyversions/fortnitepy-edit.svg)](https://pypi.org/project/fortnitepy-edit/)
 [![Current pypi version](https://img.shields.io/pypi/v/fortnitepy-edit.svg)](https://pypi.org/project/fortnitepy-edit/)
```

### Comparing `fortnitepy-edit-1.0.8/fortnitepy_edit.egg-info/SOURCES.txt` & `fortnitepy-edit-1.0.9/fortnitepy_edit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/pyproject.toml` & `fortnitepy-edit-1.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fortnitepy-edit-1.0.8/setup.py` & `fortnitepy-edit-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setuptools.setup(
     name="fortnitepy-edit",
     project_urls={
       "Documentation": "https://fortnitepy.readthedocs.io/en/latest/",
       "Issue tracker": "https://github.com/klldme/fortnitepy-edit/Issue",
     },
-    version="1.0.8",
+    version="1.0.9",
     author="klld",
     description="Library for interacting with fortnite services",
     long_description=long_description,
     license='MIT',
     long_description_content_type="text/markdown",
     install_requires=requirements,
     extras_require=extras_require,
```

