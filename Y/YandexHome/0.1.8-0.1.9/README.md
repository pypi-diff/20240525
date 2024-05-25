# Comparing `tmp/YandexHome-0.1.8.tar.gz` & `tmp/YandexHome-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YandexHome-0.1.8.tar", last modified: Sun Aug  6 15:52:16 2023, max compression
+gzip compressed data, was "YandexHome-0.1.9.tar", last modified: Sun Aug  6 15:58:42 2023, max compression
```

## Comparing `YandexHome-0.1.8.tar` & `YandexHome-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.185297 YandexHome-0.1.8/
--rw-rw-rw-   0        0        0      132 2023-08-06 15:52:16.185297 YandexHome-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-08-06 15:47:45.000000 YandexHome-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-06 15:52:16.186344 YandexHome-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.168673 YandexHome-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.175689 YandexHome-0.1.8/src/YandexHome/
--rw-rw-rw-   0        0        0     8436 2023-08-06 15:50:22.000000 YandexHome-0.1.8/src/YandexHome/__init__.py
--rw-rw-rw-   0        0        0     6245 2023-08-06 15:12:11.000000 YandexHome-0.1.8/src/YandexHome/device.py
--rw-rw-rw-   0        0        0     3459 2023-08-06 15:51:56.000000 YandexHome-0.1.8/src/YandexHome/group.py
--rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.8/src/YandexHome/scenario.py
-drwxrwxrwx   0        0        0        0 2023-08-06 15:52:16.183298 YandexHome-0.1.8/src/YandexHome.egg-info/
--rw-rw-rw-   0        0        0      132 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-06 15:52:16.000000 YandexHome-0.1.8/src/YandexHome.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-06 15:58:42.720568 YandexHome-0.1.9/
+-rw-rw-rw-   0        0        0      132 2023-08-06 15:58:42.719565 YandexHome-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-06 15:56:02.000000 YandexHome-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-06 15:58:42.720568 YandexHome-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-06 15:58:42.701159 YandexHome-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2023-08-06 15:58:42.709553 YandexHome-0.1.9/src/YandexHome/
+-rw-rw-rw-   0        0        0     8385 2023-08-06 15:57:17.000000 YandexHome-0.1.9/src/YandexHome/__init__.py
+-rw-rw-rw-   0        0        0     6245 2023-08-06 15:12:11.000000 YandexHome-0.1.9/src/YandexHome/device.py
+-rw-rw-rw-   0        0        0     3459 2023-08-06 15:51:56.000000 YandexHome-0.1.9/src/YandexHome/group.py
+-rw-rw-rw-   0        0        0      730 2023-08-06 12:52:06.000000 YandexHome-0.1.9/src/YandexHome/scenario.py
+drwxrwxrwx   0        0        0        0 2023-08-06 15:58:42.717567 YandexHome-0.1.9/src/YandexHome.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-08-06 15:58:42.000000 YandexHome-0.1.9/src/YandexHome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-06 15:58:42.000000 YandexHome-0.1.9/src/YandexHome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 15:58:42.000000 YandexHome-0.1.9/src/YandexHome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-08-06 15:58:42.000000 YandexHome-0.1.9/src/YandexHome.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-06 15:58:42.000000 YandexHome-0.1.9/src/YandexHome.egg-info/top_level.txt
```

### Comparing `YandexHome-0.1.8/src/YandexHome/__init__.py` & `YandexHome-0.1.9/src/YandexHome/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -64,30 +64,32 @@
             devices.append(device)
         return devices
                 
     async def get_groups(self):
         user_data = await self.get_user()
         groups = []
         for group in user_data['groups']:
-            group = Group(group['id'], group['name'], group['aliases'], group['type'], group['state'], group['devices'], self.token)
-            groups.append(group)
+            async with ClientSession() as session:
+                async with session.get(f'https://api.iot.yandex.net/v1.0/groups/{group["id"]}') as req:
+                    group = await req.json()
+                    group = Group(group['id'], group['name'], group['aliases'], group['type'], group['state'], group['devices'], self.token)
+                    groups.append(group)
         return groups
     
     async def get_group(self, id: str = None, *, name: str = None):
-        user_data = await self.get_user()
+        user_data = await self.get_groups()
         if name or id:
             groups = []
-            for group in user_data['groups']:
+            for group in user_data:
                 if id != None:
-                    if group['id'] == id:
-                        group = Group(group['id'], group['name'], group['aliases'], group['type'], group['state'], group['devices'], self.token)
+                    if group.id == id:
                         return group
                 if name != None:
-                    if group['name'].lower() == name.lower() or name.lower() in [alias.lower() for alias in group['aliases']]:
-                        groups.append(Group(group['id'], group['name'], group['aliases'], group['type'], group['state'], group['devices'], self.token))
+                    if group.name.lower() == name.lower() or name.lower() in [alias.lower() for alias in group.aliases]:
+                        groups.append(group)
             if len(groups) > 0:
                 if len(groups) == 1:
                     return groups[0]
                 else:
                     return groups
             else:
                 raise YandexHomeError("Группы с таким именем не найдены!")
```

### Comparing `YandexHome-0.1.8/src/YandexHome/device.py` & `YandexHome-0.1.9/src/YandexHome/device.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.8/src/YandexHome/group.py` & `YandexHome-0.1.9/src/YandexHome/group.py`

 * *Files identical despite different names*

### Comparing `YandexHome-0.1.8/src/YandexHome/scenario.py` & `YandexHome-0.1.9/src/YandexHome/scenario.py`

 * *Files identical despite different names*

