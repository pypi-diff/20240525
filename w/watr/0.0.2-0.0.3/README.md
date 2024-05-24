# Comparing `tmp/watr-0.0.2.tar.gz` & `tmp/watr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watr-0.0.2.tar", last modified: Wed Apr 24 16:45:28 2024, max compression
+gzip compressed data, was "watr-0.0.3.tar", last modified: Fri May 24 21:33:05 2024, max compression
```

## Comparing `watr-0.0.2.tar` & `watr-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.847182 watr-0.0.2/
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1173 2024-04-24 16:45:28.846948 watr-0.0.2/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      736 2024-04-07 03:44:00.000000 watr-0.0.2/README.md
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)       84 2024-03-31 17:29:21.000000 watr-0.0.2/pyproject.toml
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      593 2024-04-24 16:45:28.848628 watr-0.0.2/setup.cfg
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)       68 2024-03-31 17:30:54.000000 watr-0.0.2/setup.py
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.807577 watr-0.0.2/src/
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.839892 watr-0.0.2/src/watr/
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      429 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/WatrEntity.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      240 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/__init__.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1169 2024-04-01 16:00:25.000000 watr-0.0.2/src/watr/entity.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      316 2024-03-31 21:51:05.000000 watr-0.0.2/src/watr/util.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)    10495 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/watrapi.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      292 2024-04-01 15:59:48.000000 watr-0.0.2/src/watr/watrexceptions.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     2977 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/watrsprinklersystem.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1531 2024-04-01 15:59:05.000000 watr-0.0.2/src/watr/watrsystem.py
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     3105 2024-04-07 03:40:25.000000 watr-0.0.2/src/watr/watrzone.py
-drwxr-xr-x   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        0 2024-04-24 16:45:28.846440 watr-0.0.2/src/watr.egg-info/
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)     1173 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)      374 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/SOURCES.txt
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        1 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/dependency_links.txt
--rw-r--r--   0 gcpease  (1709703766) GRANITESCHOOLS\Domain Users (1389146880)        5 2024-04-24 16:45:28.000000 watr-0.0.2/src/watr.egg-info/top_level.txt
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-05-24 21:33:05.298041 watr-0.0.3/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1173 2024-05-24 21:33:05.297832 watr-0.0.3/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      736 2024-04-07 03:44:00.000000 watr-0.0.3/README.md
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2024-03-31 17:29:21.000000 watr-0.0.3/pyproject.toml
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      593 2024-05-24 21:33:05.299730 watr-0.0.3/setup.cfg
+-rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2024-03-31 17:30:54.000000 watr-0.0.3/setup.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-05-24 21:33:05.284793 watr-0.0.3/src/
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-05-24 21:33:05.291944 watr-0.0.3/src/watr/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      240 2024-05-24 21:31:46.000000 watr-0.0.3/src/watr/__init__.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1269 2024-05-24 21:17:51.000000 watr-0.0.3/src/watr/entity.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      316 2024-03-31 21:51:05.000000 watr-0.0.3/src/watr/util.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880    10495 2024-04-07 03:40:25.000000 watr-0.0.3/src/watr/watrapi.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      429 2024-04-07 03:40:25.000000 watr-0.0.3/src/watr/watrentity.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      292 2024-04-01 15:59:48.000000 watr-0.0.3/src/watr/watrexceptions.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     3146 2024-05-24 21:32:39.000000 watr-0.0.3/src/watr/watrsprinklersystem.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1680 2024-05-24 21:14:45.000000 watr-0.0.3/src/watr/watrsystem.py
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     3105 2024-05-24 21:31:46.000000 watr-0.0.3/src/watr/watrzone.py
+drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2024-05-24 21:33:05.297370 watr-0.0.3/src/watr.egg-info/
+-rw-r--r--   0 gcpease  (1709703766) 1389146880     1173 2024-05-24 21:33:05.000000 watr-0.0.3/src/watr.egg-info/PKG-INFO
+-rw-r--r--   0 gcpease  (1709703766) 1389146880      397 2024-05-24 21:33:05.000000 watr-0.0.3/src/watr.egg-info/SOURCES.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2024-05-24 21:33:05.000000 watr-0.0.3/src/watr.egg-info/dependency_links.txt
+-rw-r--r--   0 gcpease  (1709703766) 1389146880        5 2024-05-24 21:33:05.000000 watr-0.0.3/src/watr.egg-info/top_level.txt
```

### Comparing `watr-0.0.2/PKG-INFO` & `watr-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watr
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library to control a Watr system
 Home-page: https://capstone-cs.eng.utah.edu/Watr
 Author: Watr
 Author-email: watr@peasenet.com.com
 Project-URL: Bug Tracker, https://capstone-cs.eng.utah.edu/Watr/Watr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `watr-0.0.2/README.md` & `watr-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `watr-0.0.2/setup.cfg` & `watr-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = watr
-version = 0.0.2
+version = 0.0.3
 author = Watr
 author_email = watr@peasenet.com.com
 description = A python library to control a Watr system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://capstone-cs.eng.utah.edu/Watr
 project_urls =
```

### Comparing `watr-0.0.2/src/watr/entity.py` & `watr-0.0.3/src/watr/entity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from collections.abc import Callable
+import logging
 
 #
 # This class is borrowed from: https://github.com/natekspencer/vivintpy/blob/main/vivintpy/entity.py
 #
 UPDATE = "update"
+_LOGGER = logging.getLogger(__name__)
 
 
 class Entity:
     """
     A class representing an entity.
     """
 
@@ -21,14 +23,15 @@
         Returns the raw data of the entity.
         :return: The raw data of the entity.
         """
         return self.__data
 
     def update_data(self, data: dict, override: bool = False):
         self.__data = data
+        _LOGGER.debug(f"Updated data: {data}")
         self.emit(UPDATE, {"data": data})
 
     def on(self, event_name: str, callback: Callable) -> Callable:
         listeners = self._listeners.get(event_name, [])
         listeners.append(callback)
 
         def unsubscribe():
```

### Comparing `watr-0.0.2/src/watr/watrapi.py` & `watr-0.0.3/src/watr/watrapi.py`

 * *Files identical despite different names*

### Comparing `watr-0.0.2/src/watr/watrsprinklersystem.py` & `watr-0.0.3/src/watr/watrsprinklersystem.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from .WatrEntity import WatrEntity
+from .watrentity import WatrEntity
 from .watrapi import WatrApi
 from .watrzone import WatrZone
 from .util import first_or_none
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -82,16 +82,19 @@
 
     async def refresh(self) -> None:
         """
         Refreshes the system data.
         :return: None
         """
         system_data = await self.__api.get_system(self.id)
+        _LOGGER.debug(f"System data: {system_data}")
         if system_data is None:
+            _LOGGER.error("No system data returned.")
             return
+        _LOGGER.debug(f"Updating system data: {system_data}")
         self.update_data(system_data)
         for z in system_data["zones"]:
             # if the zone is not in the list of zones, add it
             _zone = first_or_none(self.zones, lambda _zz: _zz.id == z["id"])
             if not _zone:
                 self.__zones.append(WatrZone(self.__api, z, self))
             else:
```

### Comparing `watr-0.0.2/src/watr/watrzone.py` & `watr-0.0.3/src/watr/watrzone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from .WatrEntity import WatrEntity
+from .watrentity import WatrEntity
 from .watrapi import WatrApi
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class WatrZone(WatrEntity):
     """
```

### Comparing `watr-0.0.2/src/watr.egg-info/PKG-INFO` & `watr-0.0.3/src/watr.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watr
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python library to control a Watr system
 Home-page: https://capstone-cs.eng.utah.edu/Watr
 Author: Watr
 Author-email: watr@peasenet.com.com
 Project-URL: Bug Tracker, https://capstone-cs.eng.utah.edu/Watr/Watr/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

