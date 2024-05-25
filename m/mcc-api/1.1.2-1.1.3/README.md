# Comparing `tmp/mcc_api-1.1.2.tar.gz` & `tmp/mcc_api-1.1.3.tar.gz`

## Comparing `mcc_api-1.1.2.tar` & `mcc_api-1.1.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/conf.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/event.rst
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/index.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mcc_api-1.1.2/docs/island.rst
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/__init__.py
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/__init__.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/enums.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/exceptions.py
--rw-r--r--   0        0        0    13133 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/event/responses.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/auth.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/directives.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/enums.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/scalars.py
--rw-r--r--   0        0        0    15196 2020-02-02 00:00:00.000000 mcc_api-1.1.2/mcc_api/island/types.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/run_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_event.py
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_halloffame.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_participants.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/test_rundown.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_event.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_halloffame.json
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_halloffame_game.json
--rw-r--r--   0        0        0     8123 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_participants.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_participants_team.json
--rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/200_rundown.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/404_halloffame_game.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/404_participants_team.json
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/404_rundown.json
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/event/mock_data/429_ratelimit.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/island/__init__.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 mcc_api-1.1.2/tests/island/test_schema.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.1.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mcc_api-1.1.2/LICENSE
--rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 mcc_api-1.1.2/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mcc_api-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mcc_api-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mcc_api-1.1.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mcc_api-1.1.3/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 mcc_api-1.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 mcc_api-1.1.3/docs/conf.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 mcc_api-1.1.3/docs/event.rst
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 mcc_api-1.1.3/docs/index.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mcc_api-1.1.3/docs/island.rst
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/__init__.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/event/__init__.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/event/enums.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/event/exceptions.py
+-rw-r--r--   0        0        0    13269 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/event/responses.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/island/__init__.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/island/auth.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/island/directives.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/island/enums.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/island/scalars.py
+-rw-r--r--   0        0        0    15196 2020-02-02 00:00:00.000000 mcc_api-1.1.3/mcc_api/island/types.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/run_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/__init__.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/test_event.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/test_halloffame.py
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/test_participants.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/test_rundown.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/200_event.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/200_halloffame.json
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/200_halloffame_game.json
+-rw-r--r--   0        0        0    13473 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/200_participants.json
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/200_participants_team.json
+-rw-r--r--   0        0        0    29967 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/200_rundown.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/404_halloffame_game.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/404_participants_team.json
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/404_rundown.json
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/event/mock_data/429_ratelimit.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/island/__init__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 mcc_api-1.1.3/tests/island/test_schema.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 mcc_api-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mcc_api-1.1.3/LICENSE
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 mcc_api-1.1.3/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 mcc_api-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5303 2020-02-02 00:00:00.000000 mcc_api-1.1.3/PKG-INFO
```

### Comparing `mcc_api-1.1.2/.github/workflows/docs.yml` & `mcc_api-1.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/.github/workflows/pypi_publish.yml` & `mcc_api-1.1.3/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/.github/workflows/tests.yml` & `mcc_api-1.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/docs/conf.py` & `mcc_api-1.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/docs/index.rst` & `mcc_api-1.1.3/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 python_mcc_api
 ==============
 
 .. image:: https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI
    :alt: 🐍 PyPI
    :target: https://pypi.org/project/mcc-api/
-.. image:: https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red
-   :alt: 👑 Targeting Event API v1.3.2
-   :target: https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2
+.. image:: https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.3-red
+   :alt: 👑 Targeting Event API v1.3.3
+   :target: https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.3
 .. image:: https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.06-aqua
    :alt: 🏝️ Targeting Island API v24.05.06
    :target: https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.06
 
 A helper library for the `MC Championship <https://mcchampionship.com>`_ APIs
 (`Event <https://github.com/Noxcrew/mcchampionship-api>`_, inspired by `derNiklaas's <https://github.com/derNiklaas>`_
 `node-mcc-api <https://github.com/derNiklaas/node-mcc-api>`_ project, and
```

### Comparing `mcc_api-1.1.2/mcc_api/event/__init__.py` & `mcc_api-1.1.3/mcc_api/event/__init__.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/event/enums.py` & `mcc_api-1.1.3/mcc_api/event/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/event/exceptions.py` & `mcc_api-1.1.3/mcc_api/event/exceptions.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/event/responses.py` & `mcc_api-1.1.3/mcc_api/event/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,16 @@
 
     username: str
     """The Minecraft username of the participant."""
     uuid: str
     """The Minecraft UUID of the participant."""
     stream: str
     """The streaming URL of the participant."""
+    icon: str
+    """The URL of the icon of the participant."""
 
 
 class ParticipantsResponse(BaseResponse):
     """Response object representing all teams and their participants in the current event cycle."""
 
     data: dict[Team, list[Creator]]
     """Dictionary mapping from teams to lists of detailed participant data."""
@@ -315,15 +317,16 @@
     def __init__(self: "ParticipantsResponse", request: requests.Response | dict[str, t.Any]) -> None:
         data: dict[str, t.Any] = super()._extract_json_data(request)
         super().__init__(data)
 
         self.data = {Team[team]: [Creator(
             username=creator["username"],
             uuid=creator["uuid"],
-            stream=creator["stream"]
+            stream=creator["stream"],
+            icon=creator["icon"]
         ) for creator in participants] for team, participants in data["data"].items()}
 
 
 class ParticipantsTeamResponse(BaseResponse):
     """Response object representing a single team and its participants in the current event cycle."""
 
     data: list[Creator]
@@ -336,10 +339,11 @@
         if self.code == 404:
             raise InvalidTeamError(self.code, self.reason)
 
         self.data = [
             Creator(
                 username=creator["username"],
                 uuid=creator["uuid"],
-                stream=creator["stream"]
+                stream=creator["stream"],
+                icon=creator["icon"]
             ) for creator in data["data"]
         ]
```

### Comparing `mcc_api-1.1.2/mcc_api/island/__init__.py` & `mcc_api-1.1.3/mcc_api/island/__init__.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/island/auth.py` & `mcc_api-1.1.3/mcc_api/island/auth.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/island/directives.py` & `mcc_api-1.1.3/mcc_api/island/directives.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/island/enums.py` & `mcc_api-1.1.3/mcc_api/island/enums.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/island/scalars.py` & `mcc_api-1.1.3/mcc_api/island/scalars.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/mcc_api/island/types.py` & `mcc_api-1.1.3/mcc_api/island/types.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/run_tests.py` & `mcc_api-1.1.3/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/event/test_event.py` & `mcc_api-1.1.3/tests/event/test_event.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/event/test_halloffame.py` & `mcc_api-1.1.3/tests/event/test_halloffame.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/event/test_participants.py` & `mcc_api-1.1.3/tests/event/test_participants.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/event/test_rundown.py` & `mcc_api-1.1.3/tests/event/test_rundown.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/event/mock_data/200_halloffame.json` & `mcc_api-1.1.3/tests/event/mock_data/200_halloffame.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/event/mock_data/200_rundown.json` & `mcc_api-1.1.3/tests/event/mock_data/200_rundown.json`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/tests/island/test_schema.py` & `mcc_api-1.1.3/tests/island/test_schema.py`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/.gitignore` & `mcc_api-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/LICENSE` & `mcc_api-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/README.md` & `mcc_api-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Python MCC API
 
 [![🐍 PyPI](https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI)](https://pypi.org/project/mcc-api/)
-[![👑 Targeting Event API v1.3.2](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2)
+[![👑 Targeting Event API v1.3.3](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.3-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.3)
 [![🏝️ Targeting Island API v24.05.06](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.06-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.06)
 
 A helper library for the [MC Championship](https://mcchampionship.com) APIs
 ([Event](https://github.com/Noxcrew/mcchampionship-api), inspired by [derNiklaas's](https://github.com/derNiklaas)
 [node-mcc-api](https://github.com/derNiklaas/node-mcc-api) project, and
 [Island](https://github.com/Noxcrew/mccisland-api)).
```

### Comparing `mcc_api-1.1.2/pyproject.toml` & `mcc_api-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcc_api-1.1.2/PKG-INFO` & `mcc_api-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mcc-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: Wrapper for the MC Championship API
 Project-URL: Repository, https://github.com/JamesMCo/python_mcc_api
 Project-URL: Issues, https://github.com/JamesMCo/python_mcc_api/issues
 Project-URL: Documentation, https://mrjamesco.uk/python_mcc_api
 Author-email: "James C." <james@cordon.click>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,15 @@
 Requires-Dist: ratelimit
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Python MCC API
 
 [![🐍 PyPI](https://img.shields.io/pypi/v/mcc-api?label=🐍%20PyPI)](https://pypi.org/project/mcc-api/)
-[![👑 Targeting Event API v1.3.2](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.2-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.2)
+[![👑 Targeting Event API v1.3.3](https://img.shields.io/badge/👑_Targeting_Event_API-v1.3.3-red)](https://github.com/Noxcrew/mcchampionship-api/releases/tag/v1.3.3)
 [![🏝️ Targeting Island API v24.05.06](https://img.shields.io/badge/🏝️_Targeting_Island_API-v24.05.06-aqua)](https://github.com/Noxcrew/mccisland-api/releases/tag/v24.05.06)
 
 A helper library for the [MC Championship](https://mcchampionship.com) APIs
 ([Event](https://github.com/Noxcrew/mcchampionship-api), inspired by [derNiklaas's](https://github.com/derNiklaas)
 [node-mcc-api](https://github.com/derNiklaas/node-mcc-api) project, and
 [Island](https://github.com/Noxcrew/mccisland-api)).
```

