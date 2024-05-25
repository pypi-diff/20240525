# Comparing `tmp/swc_utils-0.1.2.tar.gz` & `tmp/swc_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swc_utils-0.1.2.tar", last modified: Mon May 20 16:56:34 2024, max compression
+gzip compressed data, was "swc_utils-0.2.0.tar", last modified: Sat May 25 20:35:39 2024, max compression
```

## Comparing `swc_utils-0.1.2.tar` & `swc_utils-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.281915 swc_utils-0.1.2/
--rw-rw-rw-   0        0        0     1090 2024-05-18 12:05:04.000000 swc_utils-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      711 2024-05-20 16:56:34.280916 swc_utils-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       85 2024-05-18 12:04:37.000000 swc_utils-0.1.2/README.md
--rw-rw-rw-   0        0        0      704 2024-05-20 15:45:12.000000 swc_utils-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 16:56:34.281915 swc_utils-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.255913 swc_utils-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.262914 swc_utils-0.1.2/src/swc_utils/
--rw-rw-rw-   0        0        0        0 2024-05-18 12:00:49.000000 swc_utils-0.1.2/src/swc_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.272913 swc_utils-0.1.2/src/swc_utils/database/
--rw-rw-rw-   0        0        0      105 2024-05-18 12:15:55.000000 swc_utils-0.1.2/src/swc_utils/database/__init__.py
--rw-rw-rw-   0        0        0     1068 2024-04-27 15:30:53.000000 swc_utils-0.1.2/src/swc_utils/database/connection_profile.py
--rw-rw-rw-   0        0        0      493 2024-05-18 12:01:51.000000 swc_utils-0.1.2/src/swc_utils/database/database_connection.py
--rw-rw-rw-   0        0        0     3500 2024-05-20 16:55:40.000000 swc_utils-0.1.2/src/swc_utils/database/db_table_care.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.273916 swc_utils-0.1.2/src/swc_utils/other/
--rw-rw-rw-   0        0        0       63 2024-05-18 12:34:45.000000 swc_utils-0.1.2/src/swc_utils/other/__init__.py
--rw-rw-rw-   0        0        0      619 2024-04-25 14:33:38.000000 swc_utils-0.1.2/src/swc_utils/other/generator_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.275915 swc_utils-0.1.2/src/swc_utils/tools/
--rw-rw-rw-   0        0        0       67 2024-05-18 12:34:45.000000 swc_utils-0.1.2/src/swc_utils/tools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-06-03 18:25:42.000000 swc_utils-0.1.2/src/swc_utils/tools/config.py
--rw-rw-rw-   0        0        0      512 2024-04-25 14:07:54.000000 swc_utils-0.1.2/src/swc_utils/tools/route_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.277915 swc_utils-0.1.2/src/swc_utils/web/
--rw-rw-rw-   0        0        0      186 2024-05-18 12:34:45.000000 swc_utils-0.1.2/src/swc_utils/web/__init__.py
--rw-rw-rw-   0        0        0      542 2024-05-18 12:34:45.000000 swc_utils-0.1.2/src/swc_utils/web/adv_responses.py
--rw-rw-rw-   0        0        0     1044 2024-05-18 12:34:45.000000 swc_utils-0.1.2/src/swc_utils/web/auth_manager.py
--rw-rw-rw-   0        0        0     2524 2023-02-28 00:29:50.000000 swc_utils-0.1.2/src/swc_utils/web/request_codes.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.279917 swc_utils-0.1.2/src/swc_utils/wsl/
--rw-rw-rw-   0        0        0       87 2024-05-18 12:34:45.000000 swc_utils-0.1.2/src/swc_utils/wsl/__init__.py
--rw-rw-rw-   0        0        0      663 2024-05-18 12:34:45.000000 swc_utils-0.1.2/src/swc_utils/wsl/wsl_compatability.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:56:34.280916 swc_utils-0.1.2/src/swc_utils.egg-info/
--rw-rw-rw-   0        0        0      711 2024-05-20 16:56:34.000000 swc_utils-0.1.2/src/swc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      780 2024-05-20 16:56:34.000000 swc_utils-0.1.2/src/swc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 16:56:34.000000 swc_utils-0.1.2/src/swc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-20 16:56:34.000000 swc_utils-0.1.2/src/swc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-20 16:56:34.000000 swc_utils-0.1.2/src/swc_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.625033 swc_utils-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-18 12:05:04.000000 swc_utils-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      711 2024-05-25 20:35:39.624031 swc_utils-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2024-05-18 12:04:37.000000 swc_utils-0.2.0/README.md
+-rw-rw-rw-   0        0        0      704 2024-05-23 16:46:40.000000 swc_utils-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-25 20:35:39.625033 swc_utils-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.599032 swc_utils-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.607033 swc_utils-0.2.0/src/swc_utils/
+-rw-rw-rw-   0        0        0        0 2024-05-18 12:00:49.000000 swc_utils-0.2.0/src/swc_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.614031 swc_utils-0.2.0/src/swc_utils/database/
+-rw-rw-rw-   0        0        0      105 2024-05-18 12:15:55.000000 swc_utils-0.2.0/src/swc_utils/database/__init__.py
+-rw-rw-rw-   0        0        0     1068 2024-04-27 15:30:53.000000 swc_utils-0.2.0/src/swc_utils/database/connection_profile.py
+-rw-rw-rw-   0        0        0      493 2024-05-18 12:01:51.000000 swc_utils-0.2.0/src/swc_utils/database/database_connection.py
+-rw-rw-rw-   0        0        0     3500 2024-05-20 16:55:40.000000 swc_utils-0.2.0/src/swc_utils/database/db_table_care.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.616032 swc_utils-0.2.0/src/swc_utils/other/
+-rw-rw-rw-   0        0        0       63 2024-05-18 12:34:45.000000 swc_utils-0.2.0/src/swc_utils/other/__init__.py
+-rw-rw-rw-   0        0        0      619 2024-04-25 14:33:38.000000 swc_utils-0.2.0/src/swc_utils/other/generator_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.617031 swc_utils-0.2.0/src/swc_utils/routing/
+-rw-rw-rw-   0        0        0        0 2024-05-23 16:26:40.000000 swc_utils-0.2.0/src/swc_utils/routing/__init__.py
+-rw-rw-rw-   0        0        0     1671 2024-05-23 17:29:27.000000 swc_utils-0.2.0/src/swc_utils/routing/auth_routes.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.619032 swc_utils-0.2.0/src/swc_utils/tools/
+-rw-rw-rw-   0        0        0       67 2024-05-18 12:34:45.000000 swc_utils-0.2.0/src/swc_utils/tools/__init__.py
+-rw-rw-rw-   0        0        0      974 2024-05-23 16:57:16.000000 swc_utils-0.2.0/src/swc_utils/tools/config.py
+-rw-rw-rw-   0        0        0      512 2024-04-25 14:07:54.000000 swc_utils-0.2.0/src/swc_utils/tools/route_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.621031 swc_utils-0.2.0/src/swc_utils/web/
+-rw-rw-rw-   0        0        0      186 2024-05-18 12:34:45.000000 swc_utils-0.2.0/src/swc_utils/web/__init__.py
+-rw-rw-rw-   0        0        0      542 2024-05-18 12:34:45.000000 swc_utils-0.2.0/src/swc_utils/web/adv_responses.py
+-rw-rw-rw-   0        0        0     1708 2024-05-25 20:35:03.000000 swc_utils-0.2.0/src/swc_utils/web/auth_manager.py
+-rw-rw-rw-   0        0        0     2524 2023-02-28 00:29:50.000000 swc_utils-0.2.0/src/swc_utils/web/request_codes.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.622032 swc_utils-0.2.0/src/swc_utils/wsl/
+-rw-rw-rw-   0        0        0       87 2024-05-18 12:34:45.000000 swc_utils-0.2.0/src/swc_utils/wsl/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-05-18 12:34:45.000000 swc_utils-0.2.0/src/swc_utils/wsl/wsl_compatability.py
+drwxrwxrwx   0        0        0        0 2024-05-25 20:35:39.623032 swc_utils-0.2.0/src/swc_utils.egg-info/
+-rw-rw-rw-   0        0        0      711 2024-05-25 20:35:39.000000 swc_utils-0.2.0/src/swc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-05-25 20:35:39.000000 swc_utils-0.2.0/src/swc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 20:35:39.000000 swc_utils-0.2.0/src/swc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-25 20:35:39.000000 swc_utils-0.2.0/src/swc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 20:35:39.000000 swc_utils-0.2.0/src/swc_utils.egg-info/top_level.txt
```

### Comparing `swc_utils-0.1.2/LICENSE` & `swc_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/PKG-INFO` & `swc_utils-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swc_utils
-Version: 0.1.2
+Version: 0.2.0
 Summary: Provides utility functions for SWC projects
 Author-email: Davis_Software <davissoftware6@gmail.com>
 Project-URL: Homepage, https://gitlab.software-city.org/root/swc_utils
 Project-URL: Issues, https://gitlab.software-city.org/root/swc_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swc_utils-0.1.2/pyproject.toml` & `swc_utils-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "swc_utils"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="Davis_Software", email="davissoftware6@gmail.com" },
 ]
 description = "Provides utility functions for SWC projects"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `swc_utils-0.1.2/src/swc_utils/database/connection_profile.py` & `swc_utils-0.2.0/src/swc_utils/database/connection_profile.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/src/swc_utils/database/db_table_care.py` & `swc_utils-0.2.0/src/swc_utils/database/db_table_care.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/src/swc_utils/other/generator_utils.py` & `swc_utils-0.2.0/src/swc_utils/other/generator_utils.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/src/swc_utils/tools/config.py` & `swc_utils-0.2.0/src/swc_utils/tools/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 class Config:
-    def __init__(self, config_file):
+    def __init__(self, config_file: str):
         self.config_file = config_file
         self.__config = self.__read_config()
 
     def __read_config(self):
         config = {}
         with open(self.config_file, 'r', encoding="utf-8") as f:
             for line in f:
@@ -12,18 +12,18 @@
                     key, value = line.split('=')
                     config[key] = value
         return config
 
     def __getitem__(self, item):
         return self.get(item)
 
-    def get(self, key, default=None):
+    def get(self, key: str, default: str = None):
         return self.__config.get(key, default)
 
-    def get_bool(self, key, default=None):
+    def get_bool(self, key: str, default: bool = None):
         return self.get(key, default) in ['True', 'true', '1']
 
-    def get_list(self, key, default=None):
+    def get_list(self, key: str, default: list[str] = None):
         return self.get(key, default).split(',')
 
-    def get_int(self, key, default=None):
+    def get_int(self, key: str, default: int = None):
         return int(self.get(key, default))
```

### Comparing `swc_utils-0.1.2/src/swc_utils/tools/route_loader.py` & `swc_utils-0.2.0/src/swc_utils/tools/route_loader.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/src/swc_utils/web/adv_responses.py` & `swc_utils-0.2.0/src/swc_utils/web/adv_responses.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/src/swc_utils/web/request_codes.py` & `swc_utils-0.2.0/src/swc_utils/web/request_codes.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/src/swc_utils/wsl/wsl_compatability.py` & `swc_utils-0.2.0/src/swc_utils/wsl/wsl_compatability.py`

 * *Files identical despite different names*

### Comparing `swc_utils-0.1.2/src/swc_utils.egg-info/PKG-INFO` & `swc_utils-0.2.0/src/swc_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swc_utils
-Version: 0.1.2
+Version: 0.2.0
 Summary: Provides utility functions for SWC projects
 Author-email: Davis_Software <davissoftware6@gmail.com>
 Project-URL: Homepage, https://gitlab.software-city.org/root/swc_utils
 Project-URL: Issues, https://gitlab.software-city.org/root/swc_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `swc_utils-0.1.2/src/swc_utils.egg-info/SOURCES.txt` & `swc_utils-0.2.0/src/swc_utils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 src/swc_utils.egg-info/top_level.txt
 src/swc_utils/database/__init__.py
 src/swc_utils/database/connection_profile.py
 src/swc_utils/database/database_connection.py
 src/swc_utils/database/db_table_care.py
 src/swc_utils/other/__init__.py
 src/swc_utils/other/generator_utils.py
+src/swc_utils/routing/__init__.py
+src/swc_utils/routing/auth_routes.py
 src/swc_utils/tools/__init__.py
 src/swc_utils/tools/config.py
 src/swc_utils/tools/route_loader.py
 src/swc_utils/web/__init__.py
 src/swc_utils/web/adv_responses.py
 src/swc_utils/web/auth_manager.py
 src/swc_utils/web/request_codes.py
```

