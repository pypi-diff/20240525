# Comparing `tmp/mcanvil-0.7.3.tar.gz` & `tmp/mcanvil-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcanvil-0.7.3.tar", last modified: Wed Apr 24 20:27:15 2024, max compression
+gzip compressed data, was "mcanvil-0.8.0.tar", last modified: Sat May 25 14:25:59 2024, max compression
```

## Comparing `mcanvil-0.7.3.tar` & `mcanvil-0.8.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-24 20:27:11.000000 mcanvil-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-24 20:27:15.532363 mcanvil-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-24 20:27:11.000000 mcanvil-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 20:27:11.000000 mcanvil-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 20:27:15.532363 mcanvil-0.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.524363 mcanvil-0.7.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.524363 mcanvil-0.7.3/src/anvil/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.528363 mcanvil-0.7.3/src/anvil/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89516 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/actors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/blockbench.py
--rw-r--r--   0 runner    (1001) docker     (127)    27515 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32083 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)   249766 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    31125 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    40436 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    34447 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/items.py
--rw-r--r--   0 runner    (1001) docker     (127)    96987 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/molang.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/texture_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    54579 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)   258421 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/api/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (127)    18415 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/src/anvil/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    31965 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/format_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    15532 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/materials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)    21533 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/sounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/lib/textures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/src/anvil/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22412 2024-04-24 20:27:11.000000 mcanvil-0.7.3/src/anvil/tools/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:27:15.532363 mcanvil-0.7.3/src/mcanvil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:27:15.000000 mcanvil-0.7.3/src/mcanvil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:59.975623 mcanvil-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 14:25:51.000000 mcanvil-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-25 14:25:59.975623 mcanvil-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-25 14:25:51.000000 mcanvil-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-25 14:25:51.000000 mcanvil-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-25 14:25:59.975623 mcanvil-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:59.967623 mcanvil-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:59.967623 mcanvil-0.8.0/src/anvil/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:59.971623 mcanvil-0.8.0/src/anvil/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86012 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/actors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/blockbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26068 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32083 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249793 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34214 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41246 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34513 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96987 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/molang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/texture_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54520 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)   258421 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/api/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17331 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:59.975623 mcanvil-0.8.0/src/anvil/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31979 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/format_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17464 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22614 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10009 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/sounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/lib/textures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:59.975623 mcanvil-0.8.0/src/anvil/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22412 2024-05-25 14:25:51.000000 mcanvil-0.8.0/src/anvil/tools/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 14:25:59.975623 mcanvil-0.8.0/src/mcanvil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-25 14:25:59.000000 mcanvil-0.8.0/src/mcanvil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-25 14:25:59.000000 mcanvil-0.8.0/src/mcanvil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:25:59.000000 mcanvil-0.8.0/src/mcanvil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 14:25:59.000000 mcanvil-0.8.0/src/mcanvil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 14:25:59.000000 mcanvil-0.8.0/src/mcanvil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-25 14:25:59.000000 mcanvil-0.8.0/src/mcanvil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 14:25:59.000000 mcanvil-0.8.0/src/mcanvil.egg-info/top_level.txt
```

### Comparing `mcanvil-0.7.3/LICENSE` & `mcanvil-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/PKG-INFO` & `mcanvil-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcanvil
-Version: 0.7.3
+Version: 0.8.0
 Summary: A Minecraft bedrock content development framework.
 Home-page: https://anvil.starktma.net/
 Author: Yasser A. Benfoughal
 Author-email: yasser@starktma.net
 License: GNU GPLv3
 Project-URL: Github, https://github.com/StarkTMA/Anvil
 Project-URL: Website, https://starktma.net
@@ -32,15 +32,15 @@
 Requires-Dist: reportlab
 
 <img src="https://starktma.net/wp-content/uploads/2022/04/logo.png" width="300" alt="Anvil Logo">
 
 # Anvil
 
 ![Python 10](https://img.shields.io/badge/python-3.10%20%20|%20%203.11%20%20|%20%203.12-g.svg)
-![Anvil Version](https://img.shields.io/badge/beta-0.7.3-yellow.svg)
+![Anvil Version](https://img.shields.io/badge/beta-0.8.0-yellow.svg)
 ![OS](https://img.shields.io/badge/OS-Windows-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
 ## What is Anvil?
```

### Comparing `mcanvil-0.7.3/README.md` & `mcanvil-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <img src="https://starktma.net/wp-content/uploads/2022/04/logo.png" width="300" alt="Anvil Logo">
 
 # Anvil
 
 ![Python 10](https://img.shields.io/badge/python-3.10%20%20|%20%203.11%20%20|%20%203.12-g.svg)
-![Anvil Version](https://img.shields.io/badge/beta-0.7.3-yellow.svg)
+![Anvil Version](https://img.shields.io/badge/beta-0.8.0-yellow.svg)
 ![OS](https://img.shields.io/badge/OS-Windows-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
 ## What is Anvil?
```

### Comparing `mcanvil-0.7.3/setup.cfg` & `mcanvil-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/api/actors.py` & `mcanvil-0.8.0/src/anvil/api/actors.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,74 @@
 
 import requests
 from halo import Halo
 from PIL import Image
 
 from anvil import ANVIL, CONFIG
 from anvil.api import vanilla
-from anvil.api.blockbench import Animation, Geometry
+from anvil.api.blockbench import _Blockbench
 from anvil.api.components import Filter, InstantDespawn, Rideable, _component
 from anvil.api.enums import Difficulty, Population, Target, Vibrations
 from anvil.api.molang import Query, Variable
 from anvil.api.types import Identifier, Molang, event
 from anvil.api.vanilla import ENTITY_LIST, ITEMS_LIST, Entities
 from anvil.lib.lib import MOLANG_PREFIXES, CopyFiles, File, FileExists
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
 from anvil.lib.sounds import EntitySoundEvent, SoundCategory, SoundDescription
 
 __all__ = ["Entity", "Attachable"]
 
 
+class _ActorReuseAssets:
+    def __init__(self, client: "_ActorClientDescription") -> None:
+        self.client = client
+
+    def animation(self, shortname: str, animation_name: str, animate: bool = False, condition: str | Molang = None):
+        if animate is True:
+            if condition is None:
+                self.client._animate_append(shortname)
+            else:
+                self.client._animate_append({shortname: condition})
+
+        self.client._description["description"]["animations"].update({shortname: animation_name})
+
+    def animation_controller(
+        self, shortname: str, animation_controller_name: str, animate: bool = False, condition: str | Molang = None
+    ):
+        if animate is True:
+            if condition is None:
+                self.client._animate_append(shortname)
+            else:
+                self.client._animate_append({shortname: condition})
+
+        self.client._description["description"]["animations"].update({shortname: animation_controller_name})
+
+    def texture(self, shortname: str, texture_name: str):
+        self.client._description["description"]["textures"].update({shortname: texture_name})
+
+    def geometry(self, shortname: str, geometry_name: str):
+        self.client._description["description"]["geometry"].update({shortname: geometry_name})
+
+    def particle_effect(self, shortname: str, particle_name: str):
+        self.client["description"]["particle_effects"].update({shortname: particle_name})
+
+    def sound_effect(self, shortname: str, sound_name: str):
+        self.client._description["description"]["sound_effects"].update({shortname: sound_name})
+
+    def spawn_egg(self, item_sprite: str, texture_index: int = 0):
+        self.client._description["description"]["spawn_egg"] = {"texture": item_sprite, "texture_index": texture_index}
+
+    def render_controller(self, controller_name: str, condition: str = None):
+        if condition is None:
+            self.client._description["description"]["render_controllers"].append(controller_name)
+        else:
+            self.client._description["description"]["render_controllers"].append({controller_name: condition})
+
+
 class _ActorDescription(MinecraftDescription):
     """Base class for all actor descriptions."""
 
     def __init__(self, name: str, is_vanilla: bool = False) -> None:
         """Base class for all actor descriptions.
 
         Args:
@@ -84,84 +130,19 @@
         if animate is True:
             if condition is None:
                 self._animate_append(animation_shortname)
             else:
                 self._animate_append({animation_shortname: condition})
 
         self._description["description"]["animations"].update(
-            {
-                animation_shortname: f"animation.{CONFIG.NAMESPACE}.{geometry_name}.{animation_shortname}"
-            }
-        )
-
-
-class _ActorReuseAssets:
-    def __init__(self, client: "_ActorClientDescription") -> None:
-        self.client = client
-
-    def animation(self, shortname: str, animation_name: str, animate: bool = False, condition: str | Molang = None):
-        if animate is True:
-            if condition is None:
-                self.client._animate_append(shortname)
-            else:
-                self.client._animate_append({shortname: condition})
-
-        self.client._description["description"]["animations"].update(
-            {
-                shortname: animation_name
-            }
-        )
-    
-    def animation_controller(self, shortname: str, animation_controller_name: str, animate: bool = False, condition: str | Molang = None):
-        if animate is True:
-            if condition is None:
-                self.client._animate_append(shortname)
-            else:
-                self.client._animate_append({shortname: condition})
-
-        self.client._description["description"]["animations"].update(
-            {
-                shortname: animation_controller_name
-            }
-        )
-
-    def texture(self, shortname: str, texture_name: str):
-        self.client._description["description"]["textures"].update(
-            {shortname: texture_name}
-        )
-    
-    def geometry(self, shortname: str, geometry_name: str):
-        self.client._description["description"]["geometry"].update(
-            {shortname: geometry_name}
-        )
-    
-    def particle_effect(self, shortname: str, particle_name: str):
-        self.client._description["description"]["particle_effects"].update(
-            {shortname: particle_name}
+            {animation_shortname: f"animation.{CONFIG.NAMESPACE}.{geometry_name}.{animation_shortname}"}
         )
 
-    def sound_effect(self, shortname: str, sound_name: str):
-        self.client._description["description"]["sound_effects"].update(
-            {shortname: sound_name}
-        )
-    
-    def spawn_egg(self, item_sprite: str, texture_index: int = 0):
-        self.client._description["description"]["spawn_egg"] = {"texture": item_sprite, "texture_index": texture_index}
-
-    def render_controller(self, controller_name: str, condition: str = None):
-        if condition is None:
-            self.client._description["description"]["render_controllers"].append(controller_name)
-        else:
-            self.client._description["description"]["render_controllers"].append({controller_name: condition})
-
 
 class _ActorClientDescription(_ActorDescription):
-    _queued_models = set()
-    _queued_textures = set()
-    _queued_animations = set()
     _queued_animation_controllers = set()
     _type = "entity"
 
     def _render_append(self, key):
         if key not in self._description["description"]["render_controllers"]:
             self._description["description"]["render_controllers"].append(key)
 
@@ -172,173 +153,116 @@
             name (str): The name of the actor.
             is_vanilla (bool, optional): Whether or not the actor is a vanilla actor. Defaults to False.
             type (str, optional): The type of the actor. Defaults to "entity".
         """
         super().__init__(name, is_vanilla)
         if self._type not in ["entity", "attachables"]:
             CONFIG.Logger.client_type_unsupported(self._type, self.identifier)
-        
+
         if is_vanilla and ENTITY_LIST.get(self.name) is None:
             CONFIG.Logger.entity_not_valid_vanilla(self.name)
 
         self._is_vanilla = is_vanilla
+        self._is_dummy = False
         self._animation_controllers = _RP_AnimationControllers(self._name, self._is_vanilla)
         self._render_controllers = _RenderControllers(self._name, self._is_vanilla)
-        self._description["description"].update(JsonSchemes.client_description())
-
         self._sounds: list[SoundDescription] = []
 
-    @property
-    def dummy(self):
-        """Whether or not the actor is a dummy actor. If True, Anvil will create a dummy geometry and texture for the actor."""
-        dummy = Geometry("dummy")
-        dummy.add_geo("dummy", (8, 8)).set_visible_bounds((2, 1.5), (0, 0.25, 0)).add_bone("root", (0, 0, 0)).add_cube(
-            (0, 0, 0), (0, 0, 0), (0, 0)
-        )
-        dummy.queue("actors")
-        CopyFiles(
-            os.path.join("assets", "models", "actors"),
-            os.path.join(
-                "resource_packs",
-                f"RP_{CONFIG._PASCAL_PROJECT_NAME}",
-                "models",
-                "entity",
-                "actors",
-            ),
-            "dummy.geo.json",
-        )
-
-        self._description["description"]["geometry"].update({"dummy": f"geometry.{CONFIG.NAMESPACE}.dummy"})
-
-        img = Image.new("RGBA", (8, 8), color=(0, 0, 0, 0))
-        img.save(os.path.join("assets", "textures", "actors", "dummy.png"))
-        CopyFiles(
-            os.path.join("assets", "textures", "actors"),
-            os.path.join(
-                CONFIG.RP_PATH,
-                "textures",
-                CONFIG.NAMESPACE,
-                CONFIG.PROJECT_NAME,
-                "actors",
-            ),
-            "dummy.png",
-        )
-        self._description["description"]["textures"].update(
-            {"dummy": os.path.join("textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "actors", "dummy")}
-        )
-
-        self.render_controller("dummy").geometry("dummy").textures("dummy")
+        self._description["description"].update(JsonSchemes.client_description())
 
     def animation_controller(self, controller_shortname: str, animate: bool = False, condition: str | Molang = None):
         """Sets the mapping of internal animation controller references to actual animations.
 
         Args:
             controller_shortname (str): The name of the animation controller.
             animate (bool, optional): Whether or not to animate the animation controller. Defaults to False.
             condition (str| Molang, optional): The condition to animate the animation controller. Defaults to None.
 
         """
         self._animation_controller(controller_shortname, animate, condition)
         return self._animation_controllers.add_controller(controller_shortname)
 
-    def animation(self, geometry_name: str, animation_name: str, animate: bool = False, condition: str | Molang = None):
+    def animation(self, blockbench_name: str, animation_name: str, animate: bool = False, condition: str | Molang = None):
         """Sets the mapping of internal animation references to actual animations.
 
         Args:
             animation_name (str): The name of the animation.
             animate (bool, optional): Whether or not to animate the animation. Defaults to False.
             condition (str | Molang, optional): The condition to animate the animation. Defaults to None.
 
         """
-        
-        anim_namespace = f"animation.{CONFIG.NAMESPACE}.{geometry_name}.{animation_name}"
 
-        if not anim_namespace in _ActorClientDescription._queued_animations:
-            try: 
-                with open(os.path.join("assets", "animations", f"{geometry_name}{Animation._extension}")) as file:
-                    if anim_namespace not in file.read():
-                        CONFIG.Logger.missing_animation(
-                            os.path.join("assets", "animations", f"{geometry_name}{Animation._extension}"), anim_namespace
-                        )
-            except:
-                CONFIG.Logger.file_exist_error(f"{geometry_name}{Animation._extension}", os.path.join("assets", "animations"))
+        anim_namespace = f"animation.{CONFIG.NAMESPACE}.{blockbench_name}.{animation_name}"
 
-            _ActorClientDescription._queued_animations.add(anim_namespace)
+        bb = _Blockbench(blockbench_name, "actors")
+        bb.animations.queue_animation(animation_name)
 
-        self._animations(geometry_name, animation_name, animate, condition)
+        self._animations(blockbench_name, animation_name, animate, condition)
 
         return self
 
     def material(self, material_id: str, material_name: str):
         """This method manages the materials for an entity.
 
         Args:
             material_id (str): The id of the material.
             material_name (str): The name of the material.
 
         """
         self._description["description"]["materials"].update({material_id: material_name})
         return self
 
-    def geometry(self, geometry_shortname: str, geometry_name: str):
+    def geometry(self, geometry_name: str):
         """
         This method manages the geometry for an entity.
 
         Args:
-            geometry_shortname (str): The shortname of the geometry.
             geometry_name (str): The name of the geometry.
 
         Returns:
             self: Returns an instance of the class.
         """
 
-        geo_namespace = f"geometry.{CONFIG.NAMESPACE}.{geometry_name}"
-        if not geo_namespace in _ActorClientDescription._queued_models:
-            try:
-                with open(os.path.join("assets", "models", "actors", f"{geometry_name}.geo.json")) as file:
-                    data = file.read()
-                    if geo_namespace not in data:
-                        CONFIG.Logger.namespace_not_in_geo(
-                            os.path.join("assets", "models", "actors", f"{geometry_name}.geo.json"), geo_namespace
-                        )
-            except:
-                CONFIG.Logger.file_exist_error(f"{geometry_name}.geo.json", os.path.join("assets", "models", "actors"))
+        bb = _Blockbench(geometry_name, "actors")
+        bb.model.queue_model()
 
-            _ActorClientDescription._queued_models.add(geometry_name)
+        self._description["description"]["geometry"].update({geometry_name: f"geometry.{CONFIG.NAMESPACE}.{geometry_name}"})
 
-        self._description["description"]["geometry"].update({geometry_shortname: geo_namespace})
+        return self
 
+    def dummy(self):
+        """This method manages the dummy for an entity."""
+        self._is_dummy = True
         return self
 
     def queryable_geometry(self, geometry_shortname: str):
         """This method manages the queryable geometry for an entity.
 
         Args:
             geometry_shortname (str): The shortname of the geometry.
 
         """
-        self._description["description"]["queryable_geometry"] = f"geometry.{CONFIG.NAMESPACE}.{geometry_shortname}"
+        if not geometry_shortname in self._description["description"]["geometry"]:
+            CONFIG.Logger.queryable_missing_geometry(geometry_shortname, self.identifier)
+        self._description["description"]["queryable_geometry"] = geometry_shortname
         return self
-    
-    def texture(self, texture_id: str, texture_name: str):
+
+    def texture(self, blockbench_name: str, texture_name: str):
         """This method manages the textures for an entity.
 
         Args:
-            texture_id (str): The id of the texture.
+            blockbench_name (str): The name of the texture.
             texture_name (str): The name of the texture.
 
         """
-        if not texture_name in _ActorClientDescription._queued_textures:
-            if not FileExists(os.path.join("assets", "textures", "actors", f"{texture_name}.png")):
-                CONFIG.Logger.file_exist_error(f"{texture_name}.png", os.path.join("assets", "textures", "actors"))
-
-            self._queued_textures.add(texture_name)
+        bb = _Blockbench(blockbench_name, "actors")
+        bb.textures.queue_texture(texture_name)
 
         self._description["description"]["textures"].update(
-            {texture_id: os.path.join("textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "actors", texture_name)}
+            {texture_name: os.path.join("textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "actors", blockbench_name, texture_name)}
         )
 
         return self
 
     def script(self, variable: Variable | str, script: Molang | str):
         """This method manages the scripts for an entity."""
         self._description["description"]["scripts"]["pre_animation"].append(f"{variable}={script};".replace(";;", ";"))
@@ -366,24 +290,23 @@
 
     def should_update_bones_and_effects_offscreen(self, bool: bool = False):
         """Sets whether or not the entity should update bones and effects offscreen.
 
         Args:
             bool (bool, optional): Whether or not the entity should update bones and effects offscreen. Defaults to False.
         """
-        self._description["description"]["scripts"]["update_bones_and_effects_offscreen"] = str(int(bool))
+        self._description["description"]["scripts"]["should_update_bones_and_effects_offscreen"] = str(int(bool))
 
     def should_update_effects_offscreen(self, bool: bool = False):
         """Sets whether or not the entity should update effects offscreen.
 
         Args:
             bool (bool, optional): Whether or not the entity should update effects offscreen. Defaults to False.
         """
-        self._description["description"]["scripts"]["update_effects_offscreen"] = str(int(bool))
-
+        self._description["description"]["scripts"]["should_update_effects_offscreen"] = str(int(bool))
 
     def scaleXYZ(self, x: Molang | str = "1", y: Molang | str = "1", z: Molang | str = "1"):
         """Sets the scale of the entity.
 
         Args:
             x (str | Molang, optional): The x scale of the entity. Defaults to "1".
             y (str | Molang, optional): The y scale of the entity. Defaults to "1".
@@ -413,14 +336,15 @@
         """This method manages the particle effects for an entity.
 
         Args:
             particle_name (str): The name of the particle effect.
 
         """
         from anvil.api.features import Particle
+
         self._particle_name = particle_name
         self._description["description"]["particle_effects"].update(
             {self._particle_name: f"{CONFIG.NAMESPACE}:{self._particle_name}"}
         )
         Particle(self._particle_name).queue()
         return self
 
@@ -488,77 +412,43 @@
             directory (str, optional): The directory to export the entity to. Defaults to None.
 
         Raises:
             RuntimeError: If the entity does not have a geometry, texture, or render controller.
             Exception: If a geometry is reused but the entity it is reused from has not been queued yet.
 
         """
+        if not self._is_dummy:
+            if len(self._description["description"]["geometry"]) == 0:
+                CONFIG.Logger.missing_geometry(self.identifier)
+
+            if len(self._description["description"]["textures"]) == 0:
+                CONFIG.Logger.missing_texture(self.identifier)
+
+            if len(self._description["description"]["render_controllers"]) == 0:
+                CONFIG.Logger.missing_render_controller(self.identifier)
+
+            for controller in self._render_controllers._controllers:
+                controller._validate(
+                    self._description["description"]["textures"].keys(),
+                    self._description["description"]["geometry"].keys(),
+                    self._description["description"]["materials"].keys(),
+                )
 
-        if len(self._description["description"]["geometry"]) == 0:
-            CONFIG.Logger.missing_geometry(self.identifier)
-
-        if len(self._description["description"]["textures"]) == 0:
-            CONFIG.Logger.missing_texture(self.identifier)
-
-        if len(self._description["description"]["render_controllers"]) == 0:
-            CONFIG.Logger.missing_render_controller(self.identifier)
+            self._render_controllers.queue(directory)
+            self._animation_controllers.queue(directory)
 
         for sound in self._sounds:
             sound._export
 
-        self._render_controllers.queue(directory)
-        self._animation_controllers.queue(directory)
-
         return super().to_dict
 
-    @staticmethod
-    def _export():
-        for model in _ActorClientDescription._queued_models:
-            CopyFiles(
-                os.path.join("assets", "models", "actors"),
-                os.path.join(
-                    CONFIG.RP_PATH,
-                    "models",
-                    "entity",
-                    "actors"
-                ),
-                f"{model}.geo.json",
-            )
-        
-        for texture in _ActorClientDescription._queued_textures:
-            CopyFiles(
-                os.path.join("assets", "textures", "actors"),
-                os.path.join(
-                    CONFIG.RP_PATH,
-                    "textures",
-                    CONFIG.NAMESPACE,
-                    CONFIG.PROJECT_NAME,
-                    "actors"
-                ),
-                f"{texture}.png",
-            )
-        
-        for animation in _ActorClientDescription._queued_animations:
-            CopyFiles(
-                os.path.join("assets", "animations"),
-                os.path.join(
-                    CONFIG.RP_PATH,
-                    "animations",
-                    #CONFIG.NAMESPACE,
-                    #CONFIG.PROJECT_NAME,
-                    "actors"
-                ),
-                f"{animation.split(".")[2]}.animation.json",
-            )
-
 
 class _EntityServerDescription(_ActorDescription):
     """Base class for all server entity descriptions."""
 
-
     def __init__(self, name: str, is_vanilla: bool = False) -> None:
         """Base class for all server entity descriptions.
 
         Args:
             name (str): The name of the entity.
             is_vanilla (bool, optional): Whether or not the entity is a vanilla entity. Defaults to False.
         """
@@ -679,70 +569,48 @@
     def spawn_egg(self, item_sprite: str, texture_index: int = 0):
         """This method adds a spawn egg texture to the entity.
 
         Args:
             item_sprite (str): The name of the item sprite.
         """
         ANVIL.definitions.register_item_textures(item_sprite, "spawn_eggs", item_sprite)
-        self._description["description"]["spawn_egg"] = {"texture": f"{CONFIG.NAMESPACE}:{item_sprite}", "texture_index": texture_index if texture_index == 0 else {}}
+        self._description["description"]["spawn_egg"] = {
+            "texture": f"{CONFIG.NAMESPACE}:{item_sprite}",
+            "texture_index": texture_index if texture_index == 0 else {},
+        }
 
     def spawn_egg_color(self, base_color: str, overlay_color: str):
         """This method adds a spawn egg color to the entity.
 
         Args:
             base_color (str): The base color of the spawn egg.
             overlay_color (str): The overlay color of the spawn egg.
         """
         self._description["description"]["spawn_egg"] = {"base_color": base_color, "overlay_color": overlay_color}
-        
+
     def to_dict(self, directory: str):
         """Queues the entity for export.
 
         Args:
             directory (str): The directory to export the entity to.
 
         """
         super().to_dict(directory)
         if "spawn_egg" not in self._description["description"] and not self._is_vanilla:
-            self._spawn_egg_texture = list(self._description["description"]["textures"].values())[0].split("\\")[-1]
-            reduced_image = Image.open(
-                os.path.join(
-                    "assets",
-                    "textures",
-                    "actors",
-                    f'{self._spawn_egg_texture}.png',
-                )
-            ).convert("P", palette=Image.WEB)
-            palette = reduced_image.getpalette()
-            color_counts = (
-                (
-                    count,
-                    "#{0:02x}{1:02x}{2:02x}".format(*palette[3 * index : 3 * index + 3]),
-                )
-                for count, index in reduced_image.getcolors()
-            )
-            most_dominant = max(color_counts, key=lambda x: x[0])[1]
-            color_counts = (
-                (
-                    count,
-                    "#{0:02x}{1:02x}{2:02x}".format(*palette[3 * index : 3 * index + 3]),
-                )
-                for count, index in reduced_image.getcolors()
-            )
-            least_dominant = min(color_counts, key=lambda x: x[0])[1]
-
             self._description["description"]["spawn_egg"] = {
-                "base_color": most_dominant,
-                "overlay_color": least_dominant,
+                "base_color": "#FFFFFF",
+                "overlay_color": "#000000",
             }
+
         return self._description
 
 
 class _AttachableClientDescription(_ActorClientDescription):
     """Base class for all client attachable descriptions."""
+
     _type = "attachables"
 
     def __init__(self, name: str, is_vanilla: bool = False) -> None:
         """Base class for all client attachable descriptions.
 
         Args:
             name (str): The name of the attachable.
@@ -889,18 +757,18 @@
         self.content(self._server_entity)
 
         controllers = list(self._animation_controllers._animation_controllers["animation_controllers"].keys())
         cleared_items = []
         for key, controller in self._description._description["description"]["animations"].items():
             if controller.startswith("controller.") and controller not in controllers:
                 cleared_items.append(key)
-        
+
         for item in cleared_items:
             self._description._description["description"]["animations"].pop(item)
-            
+
         if Rideable.component_namespace in json.dumps(self._server_entity):
             ANVIL.definitions.register_lang(f"action.hint.exit.{self.identifier}", "Sneak to exit")
 
         super().queue(directory=directory)
 
 
 class _EntityClient(AddonObject):
@@ -926,15 +794,15 @@
         """Returns the entity description."""
         return self._description
 
     @property
     def reuse_assets(self):
         """Whether or not the actor should reuse assets from another actor."""
         return _ActorReuseAssets(self._description)
-    
+
     @property
     def identifier(self) -> str:
         return self.description.identifier
 
     def queue(self, directory: str = None):
         """Queues the entity for export.
 
@@ -945,14 +813,45 @@
 
         self.content(self._client_entity)
         super().queue(directory=directory)
 
 
 # Render Controllers
 class _RenderController:
+    def _validate(self, textures: list[str], geometries: list[str], materials: list[str]):
+        controller = self._controller[self.controller_identifier]
+        controller_textures = controller.get("textures", [])
+        controller_arrays = controller.get("arrays", {}).get("textures", {})
+
+        def log_invalid_texture(texture):
+            texture_ext = texture.split(".")[-1]
+            if texture_ext not in textures:
+                CONFIG.Logger.rc_referenced_texture_not_in_entity(texture_ext, self._identifier)
+
+        for texture in controller_textures:
+            if texture.startswith("Texture."):
+                log_invalid_texture(texture)
+
+        for array in controller_arrays:
+            for texture in controller_arrays.get(array.split("[")[0], []):
+                log_invalid_texture(texture)
+
+        for geometry in self._controller[self.controller_identifier]["geometry"]:
+            if geometry.startswith("Geometry.") and geometry.split(".")[-1] not in geometries:
+                CONFIG.Logger.rc_referenced_geometry_not_in_entity(geometry.split(".")[-1], self._identifier)
+            elif (
+                geometry.startswith("Array.")
+                and geometry.split(".")[-1] not in self._controller[self.controller_identifier]["arrays"]["geometries"][geometry]
+            ):
+                CONFIG.Logger.rc_referenced_geometry_not_in_entity(geometry.split(".")[-1], self._identifier)
+
+        for material in self._controller[self.controller_identifier]["materials"]:
+            if list(material.values())[0].split(".")[-1] not in materials:
+                CONFIG.Logger.rc_referenced_material_not_in_entity(material, self._identifier)
+
     def __init__(self, identifier, controller_name, is_vanilla):
         self._identifier = identifier
         self._is_vanilla = is_vanilla
         self._namespace_format = CONFIG.NAMESPACE
         if is_vanilla:
             self._namespace_format = "minecraft"
         self._controller_name = controller_name
@@ -973,23 +872,23 @@
 
     def geometry_array(self, array_name: str, *geometries_short_names: str):
         self._controller[self.controller_identifier]["arrays"]["geometries"].update(
             {f"Array.{array_name}": [f"Geometry.{geometry}" for geometry in geometries_short_names]}
         )
         return self
 
-    def geometry(self, short_name: str = "default"):
+    def geometry(self, short_name):
         if "Array" not in short_name:
             name = f"Geometry.{short_name}"
         else:
             name = short_name
         self._controller[self.controller_identifier]["geometry"] = name
         return self
 
-    def textures(self, short_name: str = "default"):
+    def textures(self, short_name):
         if "Array" not in short_name:
             name = f"Texture.{short_name}"
         else:
             name = short_name
 
         self._controller[self.controller_identifier]["textures"].append(name)
         return self
@@ -1386,15 +1285,15 @@
                     if "transitions" in tr:
                         for st in tr["transitions"]:
                             collected_states.extend(st.keys())
 
         for state in set(collected_states):
             if state not in self._states_names:
                 CONFIG.Logger.missing_state(self._side, self._controller_namespace, state)
-        
+
         if len(self._controllers[self._controller_namespace]["states"].items()) > 0:
             return self._controllers
         return {}
 
 
 class _RP_Controller(_BP_Controller):
     def __init__(self, name, controller_shortname, is_vanilla):
@@ -2127,15 +2026,15 @@
         self._event_name = event_name
         self._event = {
             self._event_name: {
                 "add": {"component_groups": []},
                 "remove": {"component_groups": []},
                 "queue_command": {"command": []},
                 "set_property": {},
-                "emit_vibration":{}
+                "emit_vibration": {},
             }
         }
 
     def add(self, *component_groups: str):
         self._event[self._event_name]["add"]["component_groups"].extend(component_groups)
         return self
 
@@ -2154,15 +2053,15 @@
     def queue_command(self, *commands: str):
         self._event[self._event_name]["queue_command"]["command"].extend(str(cmd) for cmd in commands)
         return self
 
     def emit_vibration(self, vibration: Vibrations):
         self._event[self._event_name]["vibration"] = vibration
         return self
-    
+
     @property
     def _export(self):
         return self._event
 
 
 class _Randomize(_BaseEvent):
     def __init__(self, parent):
@@ -2189,15 +2088,15 @@
     def set_property(self, property, value):
         self._event["set_property"].update({f"{CONFIG.NAMESPACE}:{property}": value})
         return self
 
     def queue_command(self, *commands: str):
         self._event.update({"queue_command": {"command": [str(cmd) for cmd in commands]}})
         return self
-    
+
     def emit_vibration(self, vibration: Vibrations):
         self._event.update({"vibration": vibration})
         return self
 
     @property
     def randomize(self):
         return self._parent_class.randomize
@@ -2242,19 +2141,19 @@
     def set_property(self, property, value):
         self._event["set_property"].update({f"{CONFIG.NAMESPACE}:{property}": value})
         return self
 
     def queue_command(self, *commands: str):
         self._event.update({"queue_command": {"command": [str(cmd) for cmd in commands]}})
         return self
-    
+
     def emit_vibration(self, vibration: Vibrations):
         self._event.update({"vibration": vibration})
         return self
-    
+
     @property
     def sequence(self):
         return self._parent_class.sequence
 
     @property
     def randomize(self):
         randomize = _Randomize(self)
@@ -2408,20 +2307,20 @@
 
 
 # ========================================================================================================
 class Entity:
     def _validate_name(self, name: str):
         if ":" in name:
             CONFIG.Logger.namespaces_not_allowed(name)
-        if not name[0].isalpha():
+        if not str(name)[0].isalpha():
             CONFIG.Logger.digits_not_allowed(name)
 
     def __init__(self, name: str, is_vanilla: bool = False) -> None:
         self._is_vanilla = is_vanilla
-        self._name = name if not is_vanilla else str(name)
+        self._name = str(name)
         self._namespace_format = "minecraft" if is_vanilla else CONFIG.NAMESPACE
         self._validate_name(self._name)
 
         if CONFIG._TARGET == "addon" and is_vanilla:
             CONFIG.Logger.vanilla_override_error(self._name)
 
         self._server = _EntityServer(self._name, self._is_vanilla)
```

### Comparing `mcanvil-0.7.3/src/anvil/api/blocks.py` & `mcanvil-0.8.0/src/anvil/api/blocks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 from enum import StrEnum
 
 from anvil import ANVIL, CONFIG
 from anvil.api.actors import _Components
+from anvil.api.blockbench import _Blockbench
 from anvil.api.components import _component
-from anvil.api.enums import (BlockFaces, BlockMaterial, ItemCategory,
-                             ItemGroups, PlacementDirectionTrait,
+from anvil.api.enums import (BlockFaces, BlockMaterial, BlockVanillaTags,
+                             ItemCategory, ItemGroups, PlacementDirectionTrait,
                              PlacementPositionTrait)
 from anvil.api.types import Molang, coordinates, position
 from anvil.lib.lib import CopyFiles, FileExists, clamp
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
 
 __all__ = [
@@ -35,14 +36,15 @@
     "PlacementPositionTrait",
     "CardinalDirectionsTrait",
     "FacingDirectionsTrait",
     "BlockFacesTrait",
     "VerticalHalfTrait",
 ]
 
+
 class BlockDescriptor(dict):
     """
     A class that inherits from Python's built-in dict class. It is used to create a descriptor for a block in Minecraft
     with its name, tags, and states.
     """
 
     def __init__(self, name: str, tags: Molang, **states):
@@ -85,18 +87,30 @@
 
     def textures(self, **kwargs: dict[str, BlockFaces]):
         """The textures of the block."""
         for k in kwargs.keys():
             if not FileExists(os.path.join("assets", "textures", "blocks", f"{k}.png")):
                 CONFIG.Logger.file_exist_error(f"{k}.png", os.path.join("assets", "textures", "blocks"))
 
+            CopyFiles(
+                os.path.join("assets", "textures", "blocks"),
+                os.path.join(CONFIG.RP_PATH, "textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "blocks").replace("\\", "/"),
+                f"{k}.png",
+            )
+            ANVIL.definitions.register_terrain_texture(k, "", k)
+
         if BlockFaces.All in kwargs.values():
-            self._component_add_field("textures", [f"{CONFIG.NAMESPACE}:{k}" for k, v in kwargs.items() if v == BlockFaces.All][0])
+            self._component_add_field(
+                "textures", [f"{CONFIG.NAMESPACE}:{k}" for k, v in kwargs.items() if v == BlockFaces.All][0]
+            )
         else:
             self._component_add_field("textures", {v: f"{CONFIG.NAMESPACE}:{k}" for k, v in kwargs.items()})
+            
+
+
         return self
 
     def carried_textures(self, **kwargs: dict[str, BlockFaces]):
         """The carried textures of the block."""
         if BlockFaces.All in kwargs.values():
             self._component_set_value(
                 "carried_textures", [f"{CONFIG.NAMESPACE}:{k}" for k, v in kwargs.items() if v == BlockFaces.All][0]
@@ -217,14 +231,15 @@
 
     def __init__(self) -> None:
         """Maps face or material_instance names in a geometry file to an actual material instance."""
         super().__init__("material_instances")
 
     def add_instance(
         self,
+        blockbench_name: str,
         texture_name: str,
         block_face: BlockFaces = BlockFaces.All,
         render_method: BlockMaterial = BlockMaterial.Opaque,
         ambient_occlusion: bool = True,
         face_dimming: bool = True,
     ):
         """Maps face or material_instance names in a geometry file to an actual material instance.
@@ -233,29 +248,30 @@
             texture_name (str): The name of the texture to use for this block.
             block_face (BlockFaces, optional): The face of the block to apply the texture to. Defaults to BlockFaces.All.
             render_method (BlockMaterial, optional): The render method to use for this block. Defaults to BlockMaterial.Opaque.
             ambient_occlusion (bool, optional): Whether or not to use ambient occlusion for this block. Defaults to True.
             face_dimming (bool, optional): Whether or not to use face dimming for this block. Defaults to True.
 
         """
-        if FileExists(os.path.join("assets", "textures", "blocks", f"{texture_name}.png")):
-            self[self.component_namespace].update(
-                {
-                    "*"
-                    if block_face == BlockFaces.All
-                    else block_face: {
-                        "texture": f"{CONFIG.NAMESPACE}:{texture_name}",
-                        "render_method": render_method if not render_method == BlockMaterial.Opaque else {},
-                        "ambient_occlusion": ambient_occlusion if ambient_occlusion is False else {},
-                        "face_dimming": face_dimming if face_dimming is False else {},
-                    }
+        bb = _Blockbench(blockbench_name, "blocks")
+        bb.textures.queue_texture(texture_name)
+
+        ANVIL.definitions.register_terrain_texture(texture_name, blockbench_name, texture_name)
+
+        self[self.component_namespace].update(
+            {
+                "*" if block_face == BlockFaces.All else block_face: {
+                    "texture": f"{CONFIG.NAMESPACE}:{texture_name}",
+                    "render_method": render_method if not render_method == BlockMaterial.Opaque else {},
+                    "ambient_occlusion": ambient_occlusion if ambient_occlusion is False else {},
+                    "face_dimming": face_dimming if face_dimming is False else {},
                 }
-            )
-        else:
-            CONFIG.Logger.file_exist_error(f"{texture_name}.png", os.path.join("assets", "textures", "blocks"))
+            }
+        )
+
         return self
 
 
 class BlockGeometry(_component):
     component_namespace = "minecraft:geometry"
 
     def __init__(self, geometry_name: str) -> None:
@@ -263,14 +279,17 @@
 
         Args:
             geometry_name (str): The name of the geometry to use to render this block.
         """
         super().__init__("geometry")
         self._component_set_value(f"geometry.{CONFIG.NAMESPACE}.{geometry_name}")
 
+        bb = _Blockbench(geometry_name, "blocks")
+        bb.model.queue_model()
+
     def bone_visibility(self, **bone: dict[str, bool | str | Molang]):
         """Specifies the visibility of bones in the geometry file.
 
         Example:
             >>> BlockGeometry('block').bone_visibility(bone0=True, bone1=False)
 
         """
@@ -426,29 +445,43 @@
 
         self._component_add_field("crafting_tags", crafting_tags)
 
 
 # Core
 class _PermutationComponents(_Components):
     _count = 0
-    
-    def __init__(self, condition: str | Molang):
+
+    def __init__(self, condition: str | Molang = None):
         """The permutation components.
 
         Args:
             condition (str | Molang): The condition for the permutation.
         """
         super().__init__()
         _PermutationComponents._count += 1
         self._component_group_name = "components"
         self._condition = condition
 
+    def tag(self, *tags: BlockVanillaTags):
+        """The tags for the block.
+
+        Args:
+            tags (BlockVanillaTags): The tags for the block.
+
+        [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/blockreference/examples/blocktags
+        """
+        for tag in tags:
+            self._set(f"tag:{tag}", {f"tag:{tag}": {"do_not_shorten": True}})
+
+        return self
+
     def _export(self):
         cmp = super()._export()
-        cmp["condition"] = self._condition
+        if self._condition:
+            cmp["condition"] = self._condition
         return cmp
 
 
 class _BlockTraits:
     def __init__(self) -> None:
         self._traits = {}
 
@@ -508,15 +541,19 @@
 
         """
         if len(range) > 16:
             CONFIG.Logger.block_state_values_out_of_range(self._name, name, len(range))
         self._description["description"]["states"][f"{CONFIG.NAMESPACE}:{name}"] = range
         return self
 
-    def menu_category(self, category: ItemCategory = ItemCategory.none, group: ItemGroups | str = ItemGroups.none, ):
+    def menu_category(
+        self,
+        category: ItemCategory = ItemCategory.none,
+        group: ItemGroups | str = ItemGroups.none,
+    ):
         """Sets the menu category for the block.
 
         Args:
             category (ItemCategory, optional): The category of the block. Defaults to ItemCategory.none.
             group (str, optional): The group of the block. Defaults to None.
 
         """
@@ -526,15 +563,15 @@
         }
         return self
 
     @property
     def is_hidden_in_commands(self):
         self._description["description"]["is_hidden_in_commands"] = True
         return self
-    
+
     @property
     def traits(self):
         """Sets the traits for the block.
 
         [Documentation reference]: https://learn.microsoft.com/en-gb/minecraft/creator/reference/content/blockreference/examples/blocktraits
         """
         return self._traits
@@ -547,36 +584,25 @@
 
 class _BlockServer(AddonObject):
     """The block server object."""
 
     _extension = ".block.json"
     _path = os.path.join(CONFIG.BP_PATH, "blocks")
 
-    def _check_model(self, block_name):
-        if FileExists(os.path.join("assets", "models", "blocks", f"{block_name}.geo.json")):
-            geo_namespace = f"geometry.{CONFIG.NAMESPACE}.{block_name}"
-            with open(os.path.join("assets", "models", "blocks", f"{block_name}.geo.json")) as file:
-                data = file.read()
-                if geo_namespace not in data:
-                    CONFIG.Logger.namespace_not_in_geo(block_name, geo_namespace)
-
-        else:
-            CONFIG.Logger.file_exist_error(f"{block_name}.geo.json", os.path.join("assets", "models", "blocks"))
-
     def __init__(self, name: str, is_vanilla: bool = False) -> None:
         """The block server object.
 
         Args:
             name (str): The name of the block.
             is_vanilla (bool, optional): Whether or not the block is a vanilla block. Defaults to False.
         """
         super().__init__(name)
         self._server_block = JsonSchemes.server_block()
         self._description = _BlockServerDescription(name, is_vanilla)
-        self._components = _Components()
+        self._components = _PermutationComponents(None)
         self._permutations: list[_PermutationComponents] = []
 
     @property
     def description(self):
         """The block description."""
         return self._description
 
@@ -599,58 +625,23 @@
     def queue(self):
         """Queues the block to be exported."""
         self._server_block["minecraft:block"].update(self.description.to_dict)
         self._server_block["minecraft:block"].update(self._components._export())
         comps: dict = self._server_block["minecraft:block"]["components"]
         self._server_block["minecraft:block"]["permutations"] = [permutation._export() for permutation in self._permutations]
 
-        target_models = set()
-        target_textures = set()
-
         if not BlockDefault.component_namespace in comps:
             if not BlockMaterialInstance.component_namespace in comps:
                 CONFIG.Logger.block_missing_texture(self._name)
-            else:
-                for i, m in comps[BlockMaterialInstance.component_namespace].items():
-                    target_textures.add(m["texture"].removeprefix(f"{CONFIG.NAMESPACE}:"))
-
             if not BlockGeometry.component_namespace in comps:
                 CONFIG.Logger.block_missing_geometry(self._name)
-            else:
-                target_models.add(
-                    self._server_block["minecraft:block"]["components"][BlockGeometry.component_namespace].split(".")[-1]
-                )
         else:
-            if type(comps[BlockDefault.component_namespace]["textures"]) is str:
-                target_textures.add(comps[BlockDefault.component_namespace]["textures"].removeprefix(f"{CONFIG.NAMESPACE}:"))
-            elif type(comps[BlockDefault.component_namespace]["textures"]) is dict:
-                for j in comps[BlockDefault.component_namespace]["textures"].values():
-                    target_textures.add(j.removeprefix(f"{CONFIG.NAMESPACE}:"))
-
             ANVIL.definitions.register_block(self.description.identifier, comps[BlockDefault.component_namespace])
             comps.pop(BlockDefault.component_namespace)
 
-        for p in self._server_block["minecraft:block"]["permutations"]:
-            if BlockGeometry.component_namespace in p["components"]:
-                target_models.append(p["components"][BlockGeometry.component_namespace].split(".")[-1])
-            if BlockMaterialInstance.component_namespace in p["components"]:
-                for i, m in p["components"][BlockMaterialInstance.component_namespace].items():
-                    target_textures.add(m["texture"].removeprefix(f"{CONFIG.NAMESPACE}:"))
-
-        for model in target_models:
-            self._check_model(model)
-            CopyFiles(
-                os.path.join("assets", "models", "blocks"),
-                os.path.join(CONFIG.RP_PATH, "models", "blocks"),
-                f"{model}.geo.json",
-            )
-
-        for texture in target_textures:
-            ANVIL.definitions.register_terrain_texture(texture, "", texture)
-
         if not BlockDisplayName.component_namespace in self._server_block["minecraft:block"]["components"]:
             display_name = self._name.replace("_", " ").title()
             self._server_block["minecraft:block"]["components"][BlockDisplayName.component_namespace] = display_name
 
         self.content(self._server_block)
         super().queue()
 
@@ -681,21 +672,22 @@
         """The block identifier."""
         return f"{self._namespace_format}:{self._name}"
 
     @property
     def name(self):
         return self._name
 
-    @property
     def queue(self):
         """Queues the block to be exported."""
         self.Server.queue
 
         if self.Server._server_block["minecraft:block"]["components"][BlockDisplayName.component_namespace].startswith("tile."):
-            display_name = ANVIL.definitions._language[self.Server._server_block["minecraft:block"]["components"][BlockDisplayName.component_namespace]]
+            display_name = ANVIL.definitions._language[
+                self.Server._server_block["minecraft:block"]["components"][BlockDisplayName.component_namespace]
+            ]
         else:
             display_name = self.Server._server_block["minecraft:block"]["components"][BlockDisplayName.component_namespace]
 
         CONFIG.Report.add_report(
             ReportType.BLOCK,
             vanilla=self._is_vanilla,
             col0=display_name,
```

### Comparing `mcanvil-0.7.3/src/anvil/api/commands.py` & `mcanvil-0.8.0/src/anvil/api/commands.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/api/components.py` & `mcanvil-0.8.0/src/anvil/api/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from typing import Union
+from typing import List, Tuple, Union
 
 from anvil import ANVIL, CONFIG
 from anvil.api.enums import (Biomes, ContainerType, ControlFlags, DamageCause,
                              Difficulty, Effects, FilterEquipmentDomain,
                              FilterOperation, FilterSubject,
                              RawTextConstructor, Selector, Slots, Target,
                              Vibrations)
@@ -466,15 +466,15 @@
         operator: FilterOperation = FilterOperation.Equals,
     ):
         return self._construct_filter("is_sprinting", subject, operator, None, value)
 
     @classmethod
     def was_last_hurt_by(
         self,
-        value: str,
+        value: bool,
         *,
         subject: FilterSubject = FilterSubject.Self,
         operator: FilterOperation = FilterOperation.Equals,
     ):
         return self._construct_filter("was_last_hurt_by", subject, operator, None, value)
 
     @classmethod
@@ -3308,15 +3308,15 @@
         if maximum_count != -1:
             sensor["maximum_count"] = maximum_count
         if minimum_count != -1:
             sensor["minimum_count"] = minimum_count
         if require_all:
             sensor["require_all"] = require_all
         if range != (10, 10):
-            sensor["range"] = range if type(range) is list else [range, range]
+            sensor["range"] = range if isinstance(range, (tuple, list)) else (range, range)
         if cooldown != -1:
             sensor["cooldown"] = cooldown
 
         self[self.component_namespace]["subsensors"].append(sensor)
 
         return self
```

### Comparing `mcanvil-0.7.3/src/anvil/api/enums.py` & `mcanvil-0.8.0/src/anvil/api/enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -1176,7 +1176,93 @@
     StatusEffects = "status_effects"
     ItemText = "item_text"
 
 
 class HudVisibility(StrEnum):
     Hide = "hide"
     Reset = "reset"
+
+
+class ItemVanillaTags(StrEnum):
+    Arrow = "minecraft:arrow"
+    Banner = "minecraft:banner"
+    Boat = "minecraft:boat"
+    Boats = "minecraft:boats"
+    BookshelfBooks = "minecraft:bookshelf_books"
+    ChainmailTier = "minecraft:chainmail_tier"
+    Coals = "minecraft:coals"
+    CrimsonStems = "minecraft:crimson_stems"
+    DecoratedPotSherds = "minecraft:decorated_pot_sherds"
+    DiamondTier = "minecraft:diamond_tier"
+    Digger = "minecraft:digger"
+    Door = "minecraft:door"
+    GoldenTier = "minecraft:golden_tier"
+    HangingActor = "minecraft:hanging_actor"
+    HangingSign = "minecraft:hanging_sign"
+    HorseArmor = "minecraft:horse_armor"
+    IronTier = "minecraft:iron_tier"
+    IsArmor = "minecraft:is_armor"
+    IsAxe = "minecraft:is_axe"
+    IsCooked = "minecraft:is_cooked"
+    IsFish = "minecraft:is_fish"
+    IsFood = "minecraft:is_food"
+    IsHoe = "minecraft:is_hoe"
+    IsMeat = "minecraft:is_meat"
+    IsMinecart = "minecraft:is_minecart"
+    IsPickaxe = "minecraft:is_pickaxe"
+    IsShovel = "minecraft:is_shovel"
+    IsSword = "minecraft:is_sword"
+    IsTool = "minecraft:is_tool"
+    IsTrident = "minecraft:is_trident"
+    LeatherTier = "minecraft:leather_tier"
+    LecternBooks = "minecraft:lectern_books"
+    Logs = "minecraft:logs"
+    LogsThatBurn = "minecraft:logs_that_burn"
+    MangroveLogs = "minecraft:mangrove_logs"
+    MusicDisc = "minecraft:music_disc"
+    NetheriteTier = "minecraft:netherite_tier"
+    Planks = "minecraft:planks"
+    Sand = "minecraft:sand"
+    Sign = "minecraft:sign"
+    SoulFireBaseBlocks = "minecraft:soul_fire_base_blocks"
+    SpawnEgg = "minecraft:spawn_egg"
+    StoneBricks = "minecraft:stone_bricks"
+    StoneCraftingMaterials = "minecraft:stone_crafting_materials"
+    StoneTier = "minecraft:stone_tier"
+    StoneToolMaterials = "minecraft:stone_tool_materials"
+    TransformMaterials = "minecraft:transform_materials"
+    TransformTemplates = "minecraft:transform_templates"
+    TransformableItems = "minecraft:transformable_items"
+    TrimTemplates = "minecraft:trim_templates"
+    TrimmableArmors = "minecraft:trimmable_armors"
+    VibrationDamper = "minecraft:vibration_damper"
+    WarpedStems = "minecraft:warped_stems"
+    WoodenSlabs = "minecraft:wooden_slabs"
+    WoodenTier = "minecraft:wooden_tier"
+    Wool = "minecraft:wool"
+
+
+class BlockVanillaTags(StrEnum):
+    Wood = "wood"
+    Pumpkin = "pumpkin"
+    Plant = "plant"
+    Stone = "stone"
+    Metal = "metal"
+    DiamondPickDiggable = "diamond_pick_diggable"
+    GoldPickDiggable = "gold_pick_diggable"
+    IronPickDiggable = "iron_pick_diggable"
+    StonePickDiggable = "stone_pick_diggable"
+    WoodPickDiggable = "wood_pick_diggable"
+    Dirt = "dirt"
+    Sand = "sand"
+    Gravel = "gravel"
+    Grass = "grass"
+    Snow = "snow"
+    Rail = "rail"
+    Water = "water"
+    MobSpawner = "mob_spawner"
+    LushPlantsReplaceable = "lush_plants_replaceable"
+    AzaleaLogReplaceable = "azalea_log_replaceable"
+    NotFeatureReplaceable = "not_feature_replaceable"
+    TextSign = "text_sign"
+    Crop = "minecraft:crop"
+    FertilizeArea = "fertilize_area"
```

### Comparing `mcanvil-0.7.3/src/anvil/api/features.py` & `mcanvil-0.8.0/src/anvil/api/features.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import json
 import os
 from enum import StrEnum
 
-from PIL import Image, ImageDraw, ImageFont
-
 from anvil import CONFIG
 from anvil.api.enums import (CameraPresets, FogCameraLocation, LootPoolType,
                              RawTextConstructor, RenderDistanceType,
                              SmeltingTags)
 from anvil.api.types import Identifier
 from anvil.lib.lib import CopyFiles, File, FileExists, clamp
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
+from PIL import Image, ImageDraw, ImageFont
 
 
 # Dialogue ------------------------------------------------
 class _DialogueButton:
     """Handles dialogue buttons.
 
     Attributes:
@@ -456,15 +455,15 @@
         return self._pool
 
 
 class LootTable(AddonObject):
     """A class representing a LootTable."""
 
     _extension = ".loot_table.json"
-    _path = os.path.join(CONFIG.BP_PATH, "loot_tables", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME)
+    _path = os.path.join(CONFIG.BP_PATH, "loot_tables", CONFIG.NAMESPACE)
 
     def __init__(self, name: str):
         """Initializes a LootTable instance.
 
         Args:
             name (str): The name of the LootTable.
         """
@@ -479,15 +478,15 @@
     ):
         pool = _LootPool(rolls, loot_type)
         self._pools.append(pool)
         return pool
 
     @property
     def path(self):
-        return os.path.join("loot_tables", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, self._directory, self._name + self._extension)
+        return os.path.join("loot_tables", CONFIG.NAMESPACE, self._directory, self._name + self._extension)
 
     def queue(self, directory: str = ""):
         for pool in self._pools:
             self._content["pools"].append(pool._export())
         self.content(self._content)
         self._directory = directory
         return super().queue(directory=directory)
@@ -522,15 +521,15 @@
 
 class SmithingRecipe(AddonObject):
     _extension = ".recipe.json"
     _path = os.path.join(CONFIG.BP_PATH, "recipes")
 
     def __init__(self, name: str):
         self._name = name
-        self.content(JsonSchemes.smithing_table_recipe(CONFIG.NAMESPACE, name))
+        self.content(JsonSchemes.smithing_table_recipe(CONFIG.NAMESPACE, name, ["smithing_table"]))
         super().__init__(name)
 
     def base(self, identifier: Identifier):
         self._content["minecraft:recipe_smithing_transform"]["base"] = identifier
         return self
 
     def addition(self, identifier: Identifier):
@@ -660,14 +659,39 @@
         self._content["minecraft:recipe_shaped"]["priority"] = priority
         return self
 
     def queue(self):
         return super().queue()
 
 
+class SmithingTrimRecipe(AddonObject):
+    _extension = ".recipe.json"
+    _path = os.path.join(CONFIG.BP_PATH, "recipes")
+
+    def __init__(self, name: str):
+        self._name = name
+        self.content(JsonSchemes.smithing_table_trim_recipe(CONFIG.NAMESPACE, name, ["smithing_table"]))
+        super().__init__(name)
+
+    def base(self, identifier: Identifier):
+        self._content["minecraft:recipe_smithing_transform"]["base"] = identifier
+        return self
+
+    def addition(self, identifier: Identifier):
+        self._content["minecraft:recipe_smithing_transform"]["addition"] = identifier
+        return self
+
+    def priority(self, priority: int):
+        self._content["minecraft:recipe_smithing_transform"]["priority"] = priority
+        return self
+
+    def queue(self):
+        return super().queue()
+
+
 # Function ------------------------------------------------
 class Function(AddonObject):
     _extension = ".mcfunction"
     _path = os.path.join(CONFIG.BP_PATH, "functions", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME)
 
     _ticking: list["Function"] = set()
     _setup: list["Function"] = set()
@@ -882,15 +906,16 @@
 
     def listener(self, value: bool):
         """Sets whether the listener is enabled.
 
         Args:
             value (bool): Whether the listener is enabled.
         """
-        self._camera_preset["minecraft:camera_preset"]["listener"] = value
+        if value:
+            self._camera_preset["minecraft:camera_preset"]["listener"] = "player"
         return self
 
     def extend_player_rendering(self, value: bool = True):
         """Sets whether the player rendering is extended.
 
         Args:
             value (bool): Whether the player rendering is extended.
@@ -898,15 +923,14 @@
         if self._inherit == CameraPresets.Free:
             if value == False:
                 self._camera_preset["minecraft:camera_preset"]["extend_player_rendering"] = False
         else:
             CONFIG.Logger.extend_player_rendering_not_free(self._name)
         return self
     
-    @property
     def queue(self):
         """Queues the camera preset to be exported."""
         self.content(self._camera_preset)
         return super().queue()
 
     def __str__(self) -> str:
         return f"{CONFIG.NAMESPACE}:{self._name}"
```

### Comparing `mcanvil-0.7.3/src/anvil/api/items.py` & `mcanvil-0.8.0/src/anvil/api/items.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 from anvil import ANVIL, CONFIG
 from anvil.api.actors import Attachable, _Components
 from anvil.api.commands import Effects, Slots
 from anvil.api.components import _component
-from anvil.api.enums import EnchantsSlots, ItemCategory, ItemGroups
+from anvil.api.enums import (EnchantsSlots, ItemCategory, ItemGroups,
+                             ItemVanillaTags)
 from anvil.api.types import Identifier, Seconds, inf
 from anvil.lib.format_versions import ITEM_SERVER_VERSION
 from anvil.lib.lib import clamp
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes, MinecraftDescription
 
 __all__ = [
@@ -44,15 +45,15 @@
 
 
 # Components
 # Require ITEM_SERVER_VERSION >= 1.20.50
 class ItemTags(_component):
     component_namespace = "minecraft:tags"
 
-    def __init__(self, *tags: str) -> None:
+    def __init__(self, *tags: ItemVanillaTags | str) -> None:
         super().__init__("tags")
         self._enforce_version(ITEM_SERVER_VERSION, "1.20.50")
         self._component_add_field("tags", tags)
 
 
 class ItemUseModifiers(_component):
     component_namespace = "minecraft:use_modifiers"
```

### Comparing `mcanvil-0.7.3/src/anvil/api/molang.py` & `mcanvil-0.8.0/src/anvil/api/molang.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/api/texture_pack.py` & `mcanvil-0.8.0/src/anvil/api/texture_pack.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/api/types.py` & `mcanvil-0.8.0/src/anvil/api/types.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/api/ui.py` & `mcanvil-0.8.0/src/anvil/api/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -548,16 +548,15 @@
 
     @property
     def queue(self):
         for texture in self._textures:
             CopyFiles(
                 os.path.join("assets", "textures", "ui"),
                 os.path.join(
-                    "resource_packs",
-                    f"RP_{CONFIG._PASCAL_PROJECT_NAME}",
+                    CONFIG.RP_PATH,
                     "textures",
                     "ui",
                 ),
                 f"{texture}.png",
             )
         for bind in self._bindings:
             self.element["bindings"].append(bind._content)
```

### Comparing `mcanvil-0.7.3/src/anvil/api/vanilla.py` & `mcanvil-0.8.0/src/anvil/api/vanilla.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/cli.py` & `mcanvil-0.8.0/src/anvil/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,41 +46,31 @@
 
     directories = find_key(tree, "", a=[])
     for directory in directories:
         CreateDirectory(directory)
 
 
 class JsonSchemes:
-
     @staticmethod
     def structure(project_name):
         return {
             project_name: {
-                "behavior_packs": {},
-                "resource_packs": {},
                 "assets": {
-                    "animations": {},
+                    "bbmodels": {},
                     "javascript": {},
                     "marketing": {},
-                    "models": {
-                        "actors": {},
-                        "blocks": {},
-                    },
                     "particles": {},
                     "python": {},
                     "skins": {},
                     "sounds": {},
                     "structures": {},
                     "textures": {
-                        "actors": {},
                         "environment": {},
-                        "blocks": {},
                         "items": {},
                         "ui": {},
-                        "particle": {},
                     },
                     "output": {},
                 },
             }
         }
 
     @staticmethod
@@ -237,18 +227,44 @@
         }
 
     @staticmethod
     def world_packs(pack_id, version):
         return [{"pack_id": i, "version": version} for i in pack_id]
 
     @staticmethod
-    def code_workspace(name, path1, path2):
+    def code_workspace(name, path1, path2, preview=False):
         return {
             "folders": [
                 {"name": name, "path": os.path.join(path1, path2)},
+                {
+                    "name": "Dev Resource Packs",
+                    "path": os.path.join(
+                        APPDATA,
+                        "Local",
+                        "Packages",
+                        f"Microsoft.Minecraft{'WindowsBeta' if preview else 'UWP'}_8wekyb3d8bbwe",
+                        "LocalState",
+                        "games",
+                        "com.mojang",
+                        "development_resource_packs",
+                    ),
+                },
+                {
+                    "name": "Dev Behaviour Packs",
+                    "path": os.path.join(
+                        APPDATA,
+                        "Local",
+                        "Packages",
+                        f"Microsoft.Minecraft{'WindowsBeta' if preview else 'UWP'}_8wekyb3d8bbwe",
+                        "LocalState",
+                        "games",
+                        "com.mojang",
+                        "development_behavior_packs",
+                    ),
+                },
             ]
         }
 
     @staticmethod
     def packagejson(project_name, version, description, author):
         return {
             "name": project_name,
@@ -281,24 +297,24 @@
                 ],
             },
             "include": ["assets/javascript/**/*"],
             "exclude": ["node_modules"],
         }
 
     @staticmethod
-    def vscode(pascal_project_name):
+    def vscode(path):
         return {
             "version": "0.3.0",
             "configurations": [
                 {
                     "type": "minecraft-js",
                     "request": "attach",
                     "name": "Wait for Minecraft Debug Connections",
                     "mode": "listen",
-                    "localRoot": f"${{workspaceFolder}}/behavior_packs/BP_{pascal_project_name}/scripts",
+                    "localRoot": path,
                     "port": 19144,
                 }
             ],
         }
 
     @staticmethod
     def tsconstants(namespace: str, project_name: str):
@@ -394,24 +410,46 @@
         latest_build = json.loads(
             requests.get(
                 f"https://raw.githubusercontent.com/Mojang/bedrock-samples/{'preview' if preview else 'main'}/version.json"
             ).text
         )["latest"]["version"]
     except:
         latest_build = MANIFEST_BUILD
+
     base_dir = os.path.join(
         APPDATA,
         "Local",
         "Packages",
         f"Microsoft.Minecraft{'WindowsBeta' if preview else 'UWP'}_8wekyb3d8bbwe",
         "LocalState",
         "games",
         "com.mojang",
         "minecraftWorlds",
     )
+    dev_res = os.path.join(
+        APPDATA,
+        "Local",
+        "Packages",
+        f"Microsoft.Minecraft{'WindowsBeta' if preview else 'UWP'}_8wekyb3d8bbwe",
+        "LocalState",
+        "games",
+        "com.mojang",
+        "development_resource_packs",
+    )
+    dev_beh = os.path.join(
+        APPDATA,
+        "Local",
+        "Packages",
+        f"Microsoft.Minecraft{'WindowsBeta' if preview else 'UWP'}_8wekyb3d8bbwe",
+        "LocalState",
+        "games",
+        "com.mojang",
+        "development_behavior_packs",
+    )
+
     os.chdir(base_dir)
 
     CreateDirectoriesFromTree(JsonSchemes.structure(project_name))
     os.chdir(project_name)
 
     # Init the config file
     config = Config()
@@ -433,138 +471,38 @@
     config.add_option(ConfigSection.BUILD, ConfigOption.PACK_UUID, str(uuid.uuid4()))
 
     config.add_option(ConfigSection.ANVIL, ConfigOption.DEBUG, False)
     config.add_option(ConfigSection.ANVIL, ConfigOption.SCRIPT_API, scriptapi)
     config.add_option(ConfigSection.ANVIL, ConfigOption.SCRIPT_UI, False)
     config.add_option(ConfigSection.ANVIL, ConfigOption.PBR, pbr)
     config.add_option(ConfigSection.ANVIL, ConfigOption.RANDOM_SEED, random_seed)
-    config.add_option(
-        ConfigSection.ANVIL, ConfigOption.PASCAL_PROJECT_NAME, "".join(x[0] for x in project_name.split("_")).upper()
-    )
+    config.add_option(ConfigSection.ANVIL, ConfigOption.PASCAL_PROJECT_NAME, "".join(x[0] for x in project_name.split("_")).upper())
     config.add_option(ConfigSection.ANVIL, ConfigOption.LAST_CHECK, datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
 
     config.add_section(namespace)
 
     config.save()
 
     File(f"{project_name}.anvil.py", JsonSchemes.script(), "", "w")
     File(".gitignore", JsonSchemes.gitignore(), "", "w")
     File("CHANGELOG.md", "", "", "w")
 
-    File(
-        "en_US.lang",
-        "\n".join(
-            JsonSchemes.pack_name_lang(
-                config.get_option("package", "display_name"),
-                config.get_option("package", "project_description"),
-            )
-        ),
-        os.path.join(
-            "behavior_packs",
-            "BP_" + config.get_option("anvil", "pascal_project_name"),
-            "texts",
-        ),
-        "w",
-    )
-    File(
-        "en_US.lang",
-        "\n".join(
-            JsonSchemes.pack_name_lang(
-                config.get_option("package", "display_name"),
-                config.get_option("package", "project_description"),
-            )
-        ),
-        os.path.join(
-            "resource_packs",
-            "RP_" + config.get_option("anvil", "pascal_project_name"),
-            "texts",
-        ),
-        "w",
-    )
-    File(
-        "manifest.json",
-        JsonSchemes.manifest_bp(
-            [1, 0, 0],
-            config.get_option(ConfigSection.BUILD, ConfigOption.BP_UUID)[0],
-            config.get_option(ConfigSection.BUILD, ConfigOption.RP_UUID)[0],
-            config.get_option(ConfigSection.PACKAGE, ConfigOption.COMPANY),
-            scriptapi,
-            False,
-        ),
-        os.path.join("behavior_packs", "BP_" + config.get_option(ConfigSection.ANVIL, ConfigOption.PASCAL_PROJECT_NAME)),
-        "w",
-    )
-    File(
-        "manifest.json",
-        JsonSchemes.manifest_rp(
-            [1, 0, 0],
-            config.get_option(ConfigSection.BUILD, ConfigOption.RP_UUID)[0],
-            config.get_option(ConfigSection.BUILD, ConfigOption.BP_UUID)[0],
-            config.get_option(ConfigSection.PACKAGE, ConfigOption.COMPANY),
-            pbr,
-            addon,
-        ),
-        os.path.join("resource_packs", "RP_" + config.get_option(ConfigSection.ANVIL, ConfigOption.PASCAL_PROJECT_NAME)),
-        "w",
-    )
-    File(
-        "manifest.json",
-        JsonSchemes.manifest_world(
-            [1, 0, 0],
-            config.get_option(ConfigSection.BUILD, ConfigOption.PACK_UUID),
-            config.get_option(ConfigSection.PACKAGE, ConfigOption.COMPANY),
-            random_seed,
-        ),
-        "",
-        "w",
-    )
+    File("manifest.json",JsonSchemes.manifest_world([1, 0, 0], config.get_option(ConfigSection.BUILD, ConfigOption.PACK_UUID), config.get_option(ConfigSection.PACKAGE, ConfigOption.COMPANY), random_seed), "", "w")
 
-    File(
-        "world_behavior_packs.json",
-        JsonSchemes.world_packs(config.get_option("build", "bp_uuid"), [1, 0, 0]),
-        "",
-        "w",
-    )
-    File(
-        "world_resource_packs.json",
-        JsonSchemes.world_packs(config.get_option("build", "rp_uuid"), [1, 0, 0]),
-        "",
-        "w",
-    )
+    File("world_behavior_packs.json", JsonSchemes.world_packs(config.get_option("build", "bp_uuid"), [1, 0, 0]), "", "w")
+    File("world_resource_packs.json", JsonSchemes.world_packs(config.get_option("build", "rp_uuid"), [1, 0, 0]), "", "w")
 
-    File(
-        f"{project_name}.code-workspace",
-        JsonSchemes.code_workspace(config.get_option("package", "company"), base_dir, project_name),
-        DESKTOP,
-        "w",
-    )
+    File(f"{project_name}.code-workspace", JsonSchemes.code_workspace(config.get_option("package", "company"), base_dir, project_name, preview), DESKTOP, "w")
 
     if scriptapi:
         click.echo("Initiating ScriptingAPI modules")
-        File(
-            "package.json",
-            JsonSchemes.packagejson(
-                project_name,
-                "1.0.0",
-                config.get_option("package", "display_name") + " Essentials",
-                config.get_option("package", "company"),
-            ),
-            "",
-            "w",
-            True,
-        )
+        File("package.json", JsonSchemes.packagejson(project_name, "1.0.0", config.get_option("package", "display_name") + " Essentials", config.get_option("package", "company")), "", "w", True)
         File("tsconfig.json", JsonSchemes.tsconfig(config.get_option("anvil", "pascal_project_name")), "", "w", False)
-        File("launch.json", JsonSchemes.vscode(config.get_option("anvil", "pascal_project_name")), ".vscode", "w", False)
-        File(
-            "anvilConstants.ts",
-            JsonSchemes.tsconstants(namespace, project_name),
-            os.path.join("assets", "javascript"),
-            "w",
-            False,
-        )
+        File("launch.json", JsonSchemes.vscode(os.path.join(dev_res, f"BP_{config.get_option("anvil", "pascal_project_name")}", "scripts")), ".vscode", "w", False)
+        File("anvilConstants.ts", JsonSchemes.tsconstants(namespace, project_name), os.path.join("assets", "javascript"), "w", False)
         File("main.ts", 'import * as mc from "@minecraft/server";\n', os.path.join("assets", "javascript"), "w", False)
 
     config.save()
 
     process_subcommand(
         f"start {os.path.join(DESKTOP, f'{project_name}.code-workspace')}", "Unable to start the project vscode workspace"
     )
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/config.py` & `mcanvil-0.8.0/src/anvil/lib/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import uuid
 from datetime import datetime
 from enum import StrEnum
 
 import requests
 
 from anvil.lib.format_versions import MANIFEST_BUILD
-from anvil.lib.lib import (FileExists, RemoveDirectory,
+from anvil.lib.lib import (APPDATA, FileExists, RemoveDirectory,
                            validate_namespace_project_name)
 from anvil.lib.logger import Logger
 from anvil.lib.reports import ReportCollector
 
 
 class ConfigSection(StrEnum):
     ANVIL = "anvil"
@@ -50,15 +50,15 @@
 class Config:
     """A class used to read and write to the config.ini file."""
 
     def __init__(self) -> None:
         """Initializes a Config object."""
         self._config = {}
         if FileExists("anvilconfig.json"):
-            with open("anvilconfig.json", "r", encoding='utf-8') as f:
+            with open("anvilconfig.json", "r", encoding="utf-8") as f:
                 self._config = json.loads(f.read())
 
     def save(self):
         """Saves the anvilconfig.json file."""
         with open("anvilconfig.json", "w") as f:
             f.write(json.dumps(self._config, indent=4))
 
@@ -165,26 +165,18 @@
 
     def _load_configs(self) -> None:
         """Loads the configs of the Anvil instance."""
         self.NAMESPACE = self._handle_config(ConfigSection.PACKAGE, ConfigOption.NAMESPACE, "input")
         self.PROJECT_NAME = self._handle_config(ConfigSection.PACKAGE, ConfigOption.PROJECT_NAME, "input")
 
         self.COMPANY = self._handle_config(ConfigSection.PACKAGE, ConfigOption.COMPANY, "input")
-        self.DISPLAY_NAME = self._handle_config(
-            ConfigSection.PACKAGE, ConfigOption.DISPLAY_NAME, "input"
-        )
-        self.PROJECT_DESCRIPTION = self._handle_config(
-            ConfigSection.PACKAGE, ConfigOption.PROJECT_DESCRIPTION, "input"
-        )
-        self.BEHAVIOR_DESCRIPTION = self._handle_config(
-            ConfigSection.PACKAGE, ConfigOption.BEHAVIOR_DESCRIPTION, "input"
-        )
-        self.RESOURCE_DESCRIPTION = self._handle_config(
-            ConfigSection.PACKAGE, ConfigOption.RESOURCE_DESCRIPTION, "input"
-        )
+        self.DISPLAY_NAME = self._handle_config(ConfigSection.PACKAGE, ConfigOption.DISPLAY_NAME, "input")
+        self.PROJECT_DESCRIPTION = self._handle_config(ConfigSection.PACKAGE, ConfigOption.PROJECT_DESCRIPTION, "input")
+        self.BEHAVIOR_DESCRIPTION = self._handle_config(ConfigSection.PACKAGE, ConfigOption.BEHAVIOR_DESCRIPTION, "input")
+        self.RESOURCE_DESCRIPTION = self._handle_config(ConfigSection.PACKAGE, ConfigOption.RESOURCE_DESCRIPTION, "input")
         self._DEBUG = self._handle_config(ConfigSection.ANVIL, ConfigOption.DEBUG, False)
         self._PASCAL_PROJECT_NAME = self._handle_config(
             ConfigSection.ANVIL, ConfigOption.PASCAL_PROJECT_NAME, "".join(x[0] for x in self.PROJECT_NAME.split("_")).upper()
         )
 
         self._VANILLA_VERSION = self._handle_config(ConfigSection.MINECRAFT, ConfigOption.VANILLA_VERSION, MANIFEST_BUILD)
         self._TARGET = self._handle_config(ConfigSection.PACKAGE, ConfigOption.TARGET, "world")
@@ -203,15 +195,15 @@
         self._PBR = self._handle_config(ConfigSection.ANVIL, ConfigOption.PBR, False)
         self._RANDOM_SEED = self._handle_config(ConfigSection.ANVIL, ConfigOption.RANDOM_SEED, False)
         self._EXPERIMENTAL = self._handle_config(ConfigSection.ANVIL, ConfigOption.EXPERIMENTAL, False)
 
         if self._TARGET not in ["world", "addon"]:
             self.Logger.invalid_target(self._TARGET)
 
-        validate_namespace_project_name(self.NAMESPACE, self.PROJECT_NAME, self._TARGET=="addon")
+        validate_namespace_project_name(self.NAMESPACE, self.PROJECT_NAME, self._TARGET == "addon")
 
     def _check_new_vanilla_version(self):
         self.Logger.check_update()
         try:
             j = requests.get("https://raw.githubusercontent.com/Mojang/bedrock-samples/main/version.json")
             latest_build = json.loads(j.text)["latest"]["version"]
             RemoveDirectory(os.path.join("assets", "cache"))
@@ -233,12 +225,22 @@
         self.Logger.header()
 
         self.Report = ReportCollector()
         self.Report.add_headers()
 
         self._load_configs()
 
-        self.RP_PATH = os.path.join("resource_packs", f"RP_{self._PASCAL_PROJECT_NAME}")
-        self.BP_PATH = os.path.join("behavior_packs", f"BP_{self._PASCAL_PROJECT_NAME}")
+        self._COM_MOJANG = os.path.join(
+            APPDATA,
+            "Local",
+            "Packages",
+            f"Microsoft.Minecraft{'WindowsBeta' if self._EXPERIMENTAL else 'UWP'}_8wekyb3d8bbwe",
+            "LocalState",
+            "games",
+            "com.mojang",
+        )
+
+        self.RP_PATH = os.path.join(self._COM_MOJANG, "development_resource_packs", f"RP_{self.PROJECT_NAME}")
+        self.BP_PATH = os.path.join(self._COM_MOJANG, "development_behavior_packs", f"BP_{self.PROJECT_NAME}")
 
         if int((datetime.now() - datetime.strptime(self._LAST_CHECK, "%Y-%m-%d %H:%M:%S")).total_seconds()) > 12 * 3600:
-            self._check_new_vanilla_version()
+            self._check_new_vanilla_version()
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/core.py` & `mcanvil-0.8.0/src/anvil/lib/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Provides the core functionality of the Anvil library."""
 
 import os
-from atexit import register
 from datetime import datetime
 
 import commentjson
-from bs4 import Stylesheet
 from halo import Halo
 from PIL import Image
 
+from anvil.api.blockbench import _Blockbench
 from anvil.api.types import Identifier
 from anvil.lib.config import _AnvilConfig
 from anvil.lib.lib import (CopyFiles, CreateDirectory, File, FileExists,
-                           RemoveDirectory, RemoveFile, process_subcommand,
+                           RemoveDirectory, process_subcommand,
                            validate_namespace_project_name, zipit)
 from anvil.lib.materials import MaterialsObject
 from anvil.lib.reports import ReportType
 from anvil.lib.schemas import AddonObject, JsonSchemes
 from anvil.lib.sounds import (EntitySoundEvent, MusicCategory, MusicDefinition,
                               SoundCategory, SoundDefinition, SoundEvent)
 from anvil.lib.textures import (BlocksJSONObject, ItemTexturesObject,
@@ -213,31 +212,34 @@
 
     def _export_language(self):
         default_langs = JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.RESOURCE_DESCRIPTION)
         langs = default_langs.copy()
         langs.extend([f"{k}={v}" for k, v in self._language.items()])
         langs.sort(reverse=True)
 
-        File("languages.json", JsonSchemes.languages(), os.path.join(self.config.BP_PATH, "texts"), "w")
-        File("languages.json", JsonSchemes.languages(), os.path.join(self.config.RP_PATH, "texts"), "w")
-        File("languages.json", JsonSchemes.languages(), "texts", "w")
+        File("languages.json", ["en_US"], os.path.join(self.config.BP_PATH, "texts"), "w")
+        File("languages.json", ["en_US"], os.path.join(self.config.RP_PATH, "texts"), "w")
+
 
         File("en_US.lang", "\n".join(langs), os.path.join(self.config.RP_PATH, "texts"), "w")
         File(
             "en_US.lang",
             "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.BEHAVIOR_DESCRIPTION)),
             os.path.join(self.config.BP_PATH, "texts"),
             "w",
         )
-        File(
-            "en_US.lang",
-            "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)),
-            "texts",
-            "w",
-        )
+
+        if self.config._TARGET == "world":
+            File("languages.json", ["en_US"], "texts", "w")
+            File(
+                "en_US.lang",
+                "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)),
+                "texts",
+                "w",
+            )
 
     def _export_scripts(self):
         File(
             "package.json",
             JsonSchemes.packagejson(
                 self.config.PROJECT_NAME, self.config._RELEASE, self.config.PROJECT_DESCRIPTION, self.config.COMPANY
             ),
@@ -383,14 +385,20 @@
         def _to_lang(translator: GoogleTranslator, langs: dict):
             lang = JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)
             translated = translator.translate_batch(langs.values())
             for k, v in zip(langs.keys(), translated):
                 lang.append(f"{k}={v}")
             return lang
 
+        File("languages.json", JsonSchemes.languages(), os.path.join(self.config.BP_PATH, "texts"), "w")
+        File("languages.json", JsonSchemes.languages(), os.path.join(self.config.RP_PATH, "texts"), "w")
+
+        if self.config._TARGET == "world":
+            File("languages.json", JsonSchemes.languages(), "texts", "w")
+
         for language in JsonSchemes.languages():
             destination_language = (
                 language.replace("zh_CN", "zh-CN").replace("zh_TW", "zh-TW").replace("nb_NO", "no").split("_")[0]
             )
             if not FileExists(
                 os.path.join(
                     self.config.RP_PATH,
@@ -408,33 +416,34 @@
                 )
                 File(
                     f"{language}.lang",
                     "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)),
                     os.path.join(self.config.BP_PATH, "texts"),
                     "w",
                 )
-                File(
-                    f"{language}.lang",
-                    "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)),
-                    os.path.join("texts"),
-                    "w",
-                )
+                if self.config._TARGET == "world":
+                    File(
+                        f"{language}.lang",
+                        "\n".join(JsonSchemes.pack_name_lang(self.config.DISPLAY_NAME, self.config.PROJECT_DESCRIPTION)),
+                        os.path.join("texts"),
+                        "w",
+                    )
 
     @Halo(text="Compiling", spinner="dots")
     def compile(self) -> None:
         """Compiles the project."""
 
         self._definitions.queue
+        _Blockbench._export()
 
         for object in self._objects_list:
-            object._export()
-
-        from anvil.api.actors import _ActorClientDescription
-
-        _ActorClientDescription._export()
+            try:
+                object._export()
+            except Exception as e:
+                self.config.Logger.object_export_error(object._name, e)
 
         from anvil.api.blocks import _PermutationComponents
 
         if _PermutationComponents._count > 10000:
             if self.config._TARGET == "addon":
                 self.config.Logger.too_many_permutations(_PermutationComponents._count)
             else:
@@ -483,126 +492,132 @@
         self._objects_list.append(object)
 
 
 class _Anvil(_AnvilCore):
     def __init__(self, config: _AnvilConfig):
         super().__init__(config)
 
-    def _process_art(self, apply_overlay: bool = False):
-        pack_icon_size = (256, 256)
-        store_screenshot_size = (800, 450)
-        marketing_screenshot_size = (1920, 1080)
-
-        source = os.path.join("assets", "marketing")
-        output_store = os.path.join("assets", "output", "Store Art")
-        output_marketing = os.path.join("assets", "output", "Marketing Art")
-
-        CreateDirectory(output_store)
-        CreateDirectory(output_marketing)
-
+    def _process_art(self, apply_overlay: bool = False, zip: bool = True):
         def resize(image: Image.Image, name: str, output: str, size, quality=95, dpi=72, overlay: Image.Image = None):
             resized = image.resize(size)
 
             if overlay:
                 overlay = overlay.resize(size)
                 resized.paste(overlay, mask=overlay.split()[3])
 
             resized.convert("RGB").save(
                 os.path.join(output, name),
                 dpi=(dpi, dpi),
                 quality=quality,
             )
 
+        pack_icon_size = (256, 256)
+        store_screenshot_size = (800, 450)
+        marketing_screenshot_size = (1920, 1080)
+
+        source = os.path.join("assets", "marketing")
+        output_store = os.path.join("assets", "output", "Store Art")
+        output_marketing = os.path.join("assets", "output", "Marketing Art")
+
         if FileExists(os.path.join(source, "pack_icon.png")):
             original = Image.open(os.path.join(source, "pack_icon.png"))
             resize(original, "pack_icon.png", self.config.BP_PATH, pack_icon_size)
             resize(original, "pack_icon.png", self.config.RP_PATH, pack_icon_size)
-            resize(original, f"{self.config.PROJECT_NAME}_packicon_0.jpg", output_store, pack_icon_size)
+
         else:
             self.config.Logger.file_exist_warning("pack_icon.png")
 
-        if FileExists(os.path.join(source, "keyart.png")):
-            original = Image.open(os.path.join(source, "keyart.png")).convert("RGB")
-            overlay = None
-
-            if apply_overlay:
-                overlay = Image.open(os.path.join(source, "keyart_overlay.png"))
-
-            resize(original, "world_icon.jpeg", "", store_screenshot_size, 95, 72, overlay)
-            resize(original, f"{self.config.PROJECT_NAME}_Thumbnail_0.jpg", output_store, store_screenshot_size, 95, 72, overlay)
-            resize(
-                original,
-                f"{self.config.PROJECT_NAME}_MarketingKeyArt.jpg",
-                output_marketing,
-                marketing_screenshot_size,
-                100,
-                300,
-                overlay,
-            )
-
-        else:
-            self.config.Logger.file_exist_warning("keyart.png")
+        if zip:
+            CreateDirectory(output_store)
+            CreateDirectory(output_marketing)
+
+            if FileExists(os.path.join(source, "keyart.png")):
+                original = Image.open(os.path.join(source, "keyart.png")).convert("RGB")
+                overlay = None
 
-        if FileExists(os.path.join(source, "panorama.png")):
-            original = Image.open(os.path.join(source, "panorama.png"))
-            scale_factor = 450 / original.size[1]
-
-            resize(
-                original,
-                f"{self.config.PROJECT_NAME}_panorama_0.jpg",
-                output_store,
-                (round(original.size[0] * scale_factor), 450),
-                95,
-                72,
-            )
+                if apply_overlay:
+                    overlay = Image.open(os.path.join(source, "keyart_overlay.png"))
 
-        else:
-            self.config.Logger.file_exist_info("panorama.png")
+                resize(original, "world_icon.jpeg", "", store_screenshot_size, 95, 72, overlay)
+                resize(
+                    original, f"{self.config.PROJECT_NAME}_Thumbnail_0.jpg", output_store, store_screenshot_size, 95, 72, overlay
+                )
+                resize(
+                    original,
+                    f"{self.config.PROJECT_NAME}_MarketingKeyArt.jpg",
+                    output_marketing,
+                    marketing_screenshot_size,
+                    100,
+                    300,
+                    overlay,
+                )
 
-        for i in range(999):
-            if not FileExists(os.path.join(source, f"{i}.png")):
-                if i < 5:
-                    self.config.Logger.file_exist_warning(f"{i}.png")
-                break
             else:
-                original = Image.open(os.path.join(source, f"{i}.png"))
+                self.config.Logger.file_exist_warning("keyart.png")
+
+            if FileExists(os.path.join(source, "panorama.png")):
+                original = Image.open(os.path.join(source, "panorama.png"))
+                scale_factor = 450 / original.size[1]
+
                 resize(
                     original,
-                    f"{self.config.PROJECT_NAME}_screenshot_{i}.jpg",
+                    f"{self.config.PROJECT_NAME}_panorama_0.jpg",
                     output_store,
-                    store_screenshot_size,
+                    (round(original.size[0] * scale_factor), 450),
                     95,
                     72,
-                    overlay,
                 )
+
+            else:
+                self.config.Logger.file_exist_info("panorama.png")
+
+            for i in range(999):
+                if not FileExists(os.path.join(source, f"{i}.png")):
+                    if i < 5:
+                        self.config.Logger.file_exist_warning(f"{i}.png")
+                    break
+                else:
+                    original = Image.open(os.path.join(source, f"{i}.png"))
+                    resize(
+                        original,
+                        f"{self.config.PROJECT_NAME}_screenshot_{i}.jpg",
+                        output_store,
+                        store_screenshot_size,
+                        95,
+                        72,
+                    )
+                    resize(
+                        original,
+                        f"{self.config.PROJECT_NAME}_MarketingScreenshot_{i}.jpg",
+                        output_marketing,
+                        marketing_screenshot_size,
+                        100,
+                        300,
+                    )
+
+            if FileExists(os.path.join(source, "partner_art.png")):
+                original = Image.open(os.path.join(source, "partner_art.png"))
+
                 resize(
                     original,
-                    f"{self.config.PROJECT_NAME}_MarketingScreenshot_{i}.jpg",
+                    f"{self.config.PROJECT_NAME}_PartnerArt.jpg",
                     output_marketing,
                     marketing_screenshot_size,
                     100,
                     300,
-                    overlay,
                 )
 
-        if FileExists(os.path.join(source, "partner_art.png")):
-            original = Image.open(os.path.join(source, "partner_art.png"))
-
-            resize(
-                original,
-                f"{self.config.PROJECT_NAME}_PartnerArt.jpg",
-                output_marketing,
-                marketing_screenshot_size,
-                100,
-                300,
-                overlay,
-            )
+            else:
+                self.config.Logger.file_exist_warning("partner_art.png")
 
-        else:
-            self.config.Logger.file_exist_warning("partner_art.png")
+            if FileExists(os.path.join(source, "pack_icon.png")):
+                original = Image.open(os.path.join(source, "pack_icon.png"))
+                resize(original, f"{self.config.PROJECT_NAME}_packicon_0.jpg", output_store, pack_icon_size)
+            else:
+                self.config.Logger.file_exist_warning("pack_icon.png")
 
     def package_zip(
         self,
         skip_translation: bool = False,
         apply_overlay: bool = False,
     ) -> None:
         if not self._compiled:
@@ -620,28 +635,34 @@
         }
 
         if self.config._TARGET == "addon":
             if len(self.config._RP_UUID) > 1:
                 self.config.Logger.multiple_rp_uuids()
             if len(self.config._BP_UUID) > 1:
                 self.config.Logger.multiple_bp_uuids()
-            
-            content_structure.update({
-                    "resource_packs": os.path.join("Content", "resource_packs"),
-                    "behavior_packs": os.path.join("Content", "behavior_packs"),
-                })
+
+            content_structure.update(
+                {
+                    self.config.RP_PATH: os.path.join("Content", "resource_packs", f"RP_{self.config._PASCAL_PROJECT_NAME}"),
+                    self.config.BP_PATH: os.path.join("Content", "behavior_packs", f"BP_{self.config._PASCAL_PROJECT_NAME}"),
+                }
+            )
 
         else:
             content_structure.update(
                 {
-                    "resource_packs": os.path.join("Content", "world_template", "resource_packs"),
-                    "behavior_packs": os.path.join("Content", "world_template", "behavior_packs"),
+                    self.config.RP_PATH: os.path.join(
+                        "Content", "world_template", "resource_packs", f"RP_{self.config._PASCAL_PROJECT_NAME}"
+                    ),
+                    self.config.BP_PATH: os.path.join(
+                        "Content", "world_template", "behavior_packs", f"BP_{self.config._PASCAL_PROJECT_NAME}"
+                    ),
                     "texts": os.path.join("Content", "world_template", "texts"),
                     "level.dat": os.path.join("Content", "world_template"),
-                    "levelname.txt": os.path.join("Content", "world_template"), 
+                    "levelname.txt": os.path.join("Content", "world_template"),
                     "manifest.json": os.path.join("Content", "world_template"),
                     "world_icon.jpeg": os.path.join("Content", "world_template"),
                     "world_behavior_packs.json": os.path.join("Content", "world_template"),
                     "world_resource_packs.json": os.path.join("Content", "world_template"),
                 }
             )
             if not self.config._RANDOM_SEED:
@@ -661,68 +682,41 @@
 
     def mcaddon(self):
         """Packages the project into a .mcaddon file."""
         if not self._compiled:
             self.config.Logger.not_compiled()
         self.config.Logger.packaging_mcaddon()
 
-        source = os.path.join("assets", "marketing")
-        output = os.path.join("assets", "output")
-        if FileExists(os.path.join(source, "pack_icon.png")):
-            CopyFiles(
-                source,
-                os.path.join("behavior_packs", f"BP_{self.config._PASCAL_PROJECT_NAME}"),
-                "pack_icon.png",
-            )
-            CopyFiles(
-                source,
-                os.path.join("resource_packs", f"RP_{self.config._PASCAL_PROJECT_NAME}"),
-                "pack_icon.png",
-            )
+        self._process_art(False, False)
 
-        resource_packs_structure = {
-            os.path.join("resource_packs", f"RP_{self.config._PASCAL_PROJECT_NAME}"): "",
-        }
-        behavior_packs_structure = {
-            os.path.join("behavior_packs", f"BP_{self.config._PASCAL_PROJECT_NAME}"): "",
-        }
         content_structure = {
-            os.path.join(output, f"{self.config.PROJECT_NAME}_RP.mcpack"): "",
-            os.path.join(output, f"{self.config.PROJECT_NAME}_BP.mcpack"): "",
+            self.config.RP_PATH: f"RP_{self.config.PROJECT_NAME}",
+            self.config.BP_PATH: f"BP_{self.config.PROJECT_NAME}",
         }
 
-        zipit(
-            os.path.join(output, f"{self.config.PROJECT_NAME}_RP.mcpack"),
-            resource_packs_structure,
-        )
-        zipit(
-            os.path.join(output, f"{self.config.PROJECT_NAME}_BP.mcpack"),
-            behavior_packs_structure,
-        )
-        zipit(os.path.join(output, f"{self.config.PROJECT_NAME}.mcaddon"), content_structure)
-        RemoveFile(os.path.join(output, f"{self.config.PROJECT_NAME}_RP.mcpack"))
-        RemoveFile(os.path.join(output, f"{self.config.PROJECT_NAME}_BP.mcpack"))
+        zipit(os.path.join("assets", "output", f"{self.config.PROJECT_NAME}.mcaddon"), content_structure)
 
     def mcworld(self):
         """Packages the project into a .mcworld file."""
         if not self._compiled:
             self.config.Logger.not_compiled()
         self.config.Logger.packaging_mcworld()
 
+        self._process_art(False, False)
+
         content_structure = {
-            "resource_packs": os.path.join("resource_packs"),
-            "behavior_packs": os.path.join("behavior_packs"),
-            "texts": os.path.join("texts"),
-            "db": os.path.join("db"),
-            "level.dat": os.path.join(""),
-            "levelname.txt": os.path.join(""),
-            "manifest.json": os.path.join(""),
-            "world_icon.jpeg": os.path.join(""),
-            "world_behavior_packs.json": os.path.join(""),
-            "world_resource_packs.json": os.path.join(""),
+            self.config.RP_PATH: os.path.join("resource_packs", f"RP_{self.config.PROJECT_NAME}"),
+            self.config.BP_PATH: os.path.join("behavior_packs", f"BP_{self.config.PROJECT_NAME}"),
+            "texts": "texts",
+            "level.dat": "",
+            "levelname.txt": "",
+            "manifest.json": "",
+            "world_icon.jpeg": "",
+            "world_behavior_packs.json": "",
+            "world_resource_packs.json": "",
         }
 
         zipit(
             os.path.join("assets", "output", f"{self.config.PROJECT_NAME}.mcworld"),
             content_structure,
         )
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/format_versions.py` & `mcanvil-0.8.0/src/anvil/lib/format_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 BLOCK_SERVER_VERSION: str = "1.20.30"  # The version of the block server.
 ENTITY_SERVER_VERSION: str = "1.20.80"  # The version of the entity server.
 ENTITY_CLIENT_VERSION: str = "1.10.0"  # The version of the entity client.
 BP_ANIMATION_VERSION: str = "1.10.0"  # The version of the behavior pack animation.
 RP_ANIMATION_VERSION: str = "1.8.0"  # The version of the resource pack animation.
 ANIMATION_CONTROLLERS_VERSION: str = "1.10.0"  # The version of the animation controllers.
 SPAWN_RULES_VERSION: str = "1.8.0"  # The version of the spawn rules.
-GEOMETRY_VERSION: str = "1.12.0"  # The version of the geometry.
+GEOMETRY_VERSION: str = "1.16.0"  # The version of the geometry.
 RENDER_CONTROLLER_VERSION: str = "1.10.0"  # The version of the render controller.
 SOUND_DEFINITIONS_VERSION: str = "1.20.20"  # The version of the sound definitions.
 DIALOGUE_VERSION: str = "1.18.0"  # The version of the dialogue.
 FOG_VERSION: str = "1.16.100"  # The version of the fog.
 MATERIALS_VERSION: str = "1.0.0"  # The version of the materials.
 ITEM_SERVER_VERSION: str = "1.20.70"  # The version of the item server.
 GLOBAL_LIGHTING = "1.0.0"
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/lib.py` & `mcanvil-0.8.0/src/anvil/lib/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,16 @@
 def RemoveDirectory(path: str) -> None:
     """
     Removes a directory and all its contents.
 
     Args:
         path (str): The path to the directory to be removed.
     """
+    
+    shutil.rmtree(path)
 
 
 def RemoveFile(path: str) -> None:
     """
     Removes a file.
 
     Args:
@@ -162,24 +164,18 @@
 
     def zipdir(ziph: zipfile.ZipFile, source, target):
         if os.path.isdir(source):
             for root, dirs, files in os.walk(source):
                 for file in files:
                     ziph.write(
                         os.path.join(root, file),
-                        os.path.join(
-                            target,
-                            os.path.relpath(os.path.join(root, file), os.path.join(source, ".")),
-                        ),
+                        os.path.join(target, os.path.relpath(os.path.join(root, file), os.path.join(source, "."))),
                     )
         else:
-            ziph.write(
-                source,
-                os.path.relpath(os.path.join(target, source), os.path.join(source, "..")),
-            )
+            ziph.write(source, os.path.relpath(os.path.join(target, source), os.path.join(source, "..")))
 
     zipf = zipfile.ZipFile(zip_name, "w", zipfile.ZIP_DEFLATED)
     for source, target in dir_list.items():
         zipdir(zipf, source, target)
     zipf.close()
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/logger.py` & `mcanvil-0.8.0/src/anvil/lib/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,7 +437,55 @@
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
 
     def extend_player_rendering_not_free(self, camera_preset: str):
         m = f"Extending player component is only supported with the Free preset. Error at {camera_preset}."
         self.logger.error(m)
         raise RuntimeError(self.Red("[ERROR]: " + m))
+
+    # Error
+    def rc_referenced_texture_not_in_entity(self, texture, entity):
+        m = f"Referenced texture [{texture}] is not in the entity {entity}."
+        self.logger.error(m)
+        raise RuntimeError(self.Red("[ERROR]: " + m))
+    
+    # Error
+    def rc_referenced_geometry_not_in_entity(self, geometry, entity):
+        m = f"Referenced geometry [{geometry}] is not in the entity {entity}."
+        self.logger.error(m)
+        raise RuntimeError(self.Red("[ERROR]: " + m))
+    
+    # Error
+    def rc_referenced_material_not_in_entity(self, material, entity):
+        m = f"Referenced material [{material}] is not in the entity {entity}."
+        self.logger.error(m)
+        raise RuntimeError(self.Red("[ERROR]: " + m))
+    
+    # Error
+    def queryable_missing_geometry(self, geometry, entity):
+        m = f"Queryable geometry {geometry} is missing from the entity {entity}."
+        self.logger.error(m)
+        raise RuntimeError(self.Red("[ERROR]: " + m))
+    
+    # Error
+    def blockbench_identifier_mismatch(self, identifier: str, expected: str):
+        m = f"Identifier {identifier} is not formatted correctly, expected {expected}."
+        self.logger.error(m)
+        raise ValueError(self.Red("[ERROR]: " + m))
+
+    # Error
+    def blockbench_animation_not_found(self, animation: str, filename:str):
+        m = f"Could not find the animation [{animation}] in {filename}.bbmodel"
+        self.logger.error(m)
+        raise FileNotFoundError(self.Red("[ERROR]: " + m))
+    
+    # Error
+    def blockbench_texture_not_found(self, texture: str, filename: str):
+        m = f"Could not find the texture [{texture}] in {filename}.bbmodel"
+        self.logger.error(m)
+        raise FileNotFoundError(self.Red("[ERROR]: " + m))
+    
+    # Error
+    def object_export_error(self, name: str, error: Exception):
+        m = f"Error exporting {name}: {error}"
+        self.logger.error(m)
+        raise error
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/materials.py` & `mcanvil-0.8.0/src/anvil/lib/materials.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/lib/reports.py` & `mcanvil-0.8.0/src/anvil/lib/reports.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/anvil/lib/schemas.py` & `mcanvil-0.8.0/src/anvil/lib/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,18 +310,30 @@
     def animation_controllers():
         return {
             "format_version": ANIMATION_CONTROLLERS_VERSION,
             "animation_controllers": {},
         }
 
     @staticmethod
-    def geometry():
+    def geometry(model_name: str, texture_size: list[int], visible_box: list[int], visible_offset: list[int]):
         return {
             "format_version": GEOMETRY_VERSION,
-            "minecraft:geometry": [],
+            "minecraft:geometry": [
+                {
+                    "description": {
+                        "identifier": f"geometry.{CONFIG.NAMESPACE}.{model_name}",
+                        "texture_width": texture_size[0],
+                        "texture_height": texture_size[1],
+                        "visible_bounds_width": visible_box[0],
+                        "visible_bounds_height": visible_box[1],
+                        "visible_bounds_offset": visible_offset,
+                    },
+                    "bones": [],
+                }
+            ],
         }
 
     @staticmethod
     def render_controller(controller_name, part, controller_type):
         return {
             f"controller.render.{controller_name}.{part}.{controller_type}": {
                 "arrays": {"textures": {}, "geometries": {}},
@@ -518,19 +530,30 @@
             "minecraft:recipe_furnace": {
                 "tags": tags,
                 "description": {"identifier": f"{namespace}:{name}"},
             },
         }
 
     @staticmethod
-    def smithing_table_recipe(namespace: str, name: str):
+    def smithing_table_recipe(namespace: str, name: str, tags: list[str]):
         return {
             "format_version": "1.17.0",
             "minecraft:recipe_smithing_transform": {
                 "description": {"identifier": f"{namespace}:{name}"},
+                "tags": tags,
+            },
+        }
+
+    @staticmethod
+    def smithing_table_trim_recipe(namespace: str, name: str, tags: list[str]):
+        return {
+            "format_version": "1.17.0",
+            "minecraft:recipe_smithing_trim": {
+                "description": {"identifier": f"{namespace}:{name}"},
+                "tags": tags,
             },
         }
 
     @staticmethod
     def shapeless_crafting_recipe(namespace: str, name: str, tags: list[str]):
         return {
             "format_version": "1.12",
@@ -631,17 +654,17 @@
         Exports the addon object after potentially shortening its content and replacing backslashes.
         Logs the event and writes the object to a file.
         """
 
         def _shorten_dict(d):
             if isinstance(d, dict):
                 return {
-                    k: v
+                    k: (v if v != {"do_not_shorten": True} else {})
                     for k, v in ((k, _shorten_dict(v)) for k, v in d.items())
-                    if v != {} and v != [] or str(k).startswith("minecraft:")
+                    if (v != {} and v != []) or str(k).startswith("minecraft:") or v == {"do_not_shorten": True}
                 }
 
             elif isinstance(d, list):
                 return [v for v in map(_shorten_dict, d) if v != []]
 
             return d
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/sounds.py` & `mcanvil-0.8.0/src/anvil/lib/sounds.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,15 @@
         """
         parent_dir = self._sound_reference.split(".")[0]
         for sound in self._sounds:
             s = sound["name"].split("\\")[-1]
             CopyFiles(
                 os.path.join("assets", "sounds", parent_dir),
                 os.path.join(
-                    "resource_packs",
-                    f"RP_{CONFIG._PASCAL_PROJECT_NAME}",
+                    CONFIG.RP_PATH,
                     "sounds",
                     self._path,
                 ),
                 f"{s}.ogg",
             )
         self._sound[self._sound_definition]["sounds"] = self._sounds
         return self._sound
```

### Comparing `mcanvil-0.7.3/src/anvil/lib/textures.py` & `mcanvil-0.8.0/src/anvil/lib/textures.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import os
 
 from anvil import CONFIG
+from anvil.api.types import Identifier
 from anvil.lib.lib import CopyFiles, FileExists
 from anvil.lib.schemas import AddonObject, JsonSchemes
-from anvil.api.types import Identifier
 
 
 class ItemTexturesObject(AddonObject):
     """Handles item textures for the addon."""
+
     _extension = ".json"
     _path = os.path.join(CONFIG.RP_PATH, "textures")
 
     def __init__(self) -> None:
         """Initializes a ItemTexturesObject instance."""
-        super().__init__(
-            "item_texture"
-        )
+        super().__init__("item_texture")
 
         self.content(JsonSchemes.item_texture(CONFIG.PROJECT_NAME))
 
     def add_item(self, item_name: str, directory, *item_sprites: str):
         """Adds item textures to the content.
 
         Args:
@@ -30,15 +29,17 @@
         for item in item_sprites:
             if not FileExists(os.path.join("assets", "textures", "items", f"{item}.png")):
                 CONFIG.Logger.file_exist_error(f"{item}.png", os.path.join("assets", "textures", "items"))
 
         self._content["texture_data"][f"{CONFIG.NAMESPACE}:{item_name}"] = {
             "textures": [
                 *[
-                    os.path.join("textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "items", directory, sprite).replace("\\", "/")
+                    os.path.join(
+                        "textures", CONFIG.NAMESPACE, CONFIG.PROJECT_NAME, "items", directory, sprite
+                    ).replace("\\", "/")
                     for sprite in item_sprites
                 ]
             ]
         }
 
     @property
     def queue(self):
@@ -57,33 +58,31 @@
         """
         if len(self._content["texture_data"]) > 0:
             for items in self._content["texture_data"].values():
                 for sprite in items["textures"]:
                     CopyFiles(
                         os.path.join("assets", "textures", "items"),
                         os.path.join(
-                            "resource_packs",
-                            f"RP_{CONFIG._PASCAL_PROJECT_NAME}",
+                            CONFIG.RP_PATH,
                             sprite.rstrip(sprite.split("/")[-1]),
                         ),
                         sprite.split("/")[-1] + ".png",
                     )
             return super()._export()
 
 
 class TerrainTexturesObject(AddonObject):
     """Handles terrain textures for the addon."""
+
     _extension = ".json"
     _path = os.path.join(CONFIG.RP_PATH, "textures")
 
     def __init__(self) -> None:
         """Initializes a TerrainTexturesObject instance."""
-        super().__init__(
-            "terrain_texture"
-        )
+        super().__init__("terrain_texture")
         self.content(JsonSchemes.terrain_texture(CONFIG.PROJECT_NAME))
 
     def add_block(self, block_name: str, directory: str, *block_textures: str):
         """Adds block textures to the content.
 
         Args:
             block_name (str): The name of the block.
@@ -111,24 +110,24 @@
     def _export(self):
         """Exports the block textures if at least one block texture was added.
 
         Returns:
             object: The parent's export method result.
         """
         if len(self._content["texture_data"]) > 0:
-            for items in self._content["texture_data"].values():
-                for sprite in items["textures"]:
-                    CopyFiles(
-                        os.path.join("assets", "textures", "blocks"),
-                        os.path.join(
-                            CONFIG.RP_PATH,
-                            sprite.rstrip(sprite.split("/")[-1]),
-                        ),
-                        sprite.split("/")[-1] + ".png",
-                    )
+            #for items in self._content["texture_data"].values():
+            #    for sprite in items["textures"]:
+            #        CopyFiles(
+            #            os.path.join("assets", "textures", "blocks"),
+            #            os.path.join(
+            #                CONFIG.RP_PATH,
+            #                sprite.rstrip(sprite.split("/")[-1]),
+            #            ),
+            #            sprite.split("/")[-1] + ".png",
+            #        )
             return super()._export()
 
 
 class BlocksJSONObject(AddonObject):
     _extension = ".json"
     _path = CONFIG.RP_PATH
```

### Comparing `mcanvil-0.7.3/src/anvil/tools/functions.py` & `mcanvil-0.8.0/src/anvil/tools/functions.py`

 * *Files identical despite different names*

### Comparing `mcanvil-0.7.3/src/mcanvil.egg-info/PKG-INFO` & `mcanvil-0.8.0/src/mcanvil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcanvil
-Version: 0.7.3
+Version: 0.8.0
 Summary: A Minecraft bedrock content development framework.
 Home-page: https://anvil.starktma.net/
 Author: Yasser A. Benfoughal
 Author-email: yasser@starktma.net
 License: GNU GPLv3
 Project-URL: Github, https://github.com/StarkTMA/Anvil
 Project-URL: Website, https://starktma.net
@@ -32,15 +32,15 @@
 Requires-Dist: reportlab
 
 <img src="https://starktma.net/wp-content/uploads/2022/04/logo.png" width="300" alt="Anvil Logo">
 
 # Anvil
 
 ![Python 10](https://img.shields.io/badge/python-3.10%20%20|%20%203.11%20%20|%20%203.12-g.svg)
-![Anvil Version](https://img.shields.io/badge/beta-0.7.3-yellow.svg)
+![Anvil Version](https://img.shields.io/badge/beta-0.8.0-yellow.svg)
 ![OS](https://img.shields.io/badge/OS-Windows-blue.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
 
 ## What is Anvil?
```

### Comparing `mcanvil-0.7.3/src/mcanvil.egg-info/SOURCES.txt` & `mcanvil-0.8.0/src/mcanvil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

