# Comparing `tmp/roxbot-2.0.0.tar.gz` & `tmp/roxbot-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roxbot-2.0.0.tar", last modified: Wed May 15 15:55:55 2024, max compression
+gzip compressed data, was "roxbot-2.1.0.tar", last modified: Sat May 25 11:55:57 2024, max compression
```

## Comparing `roxbot-2.0.0.tar` & `roxbot-2.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 15:55:46.000000 roxbot-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-15 15:55:55.419286 roxbot-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-15 15:55:46.000000 roxbot-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-15 15:55:46.000000 roxbot-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 15:55:55.419286 roxbot-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.415286 roxbot-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.415286 roxbot-2.0.0/src/roxbot/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot/bridges/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/bridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/bridges/mqtt_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot/models/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/diff_drive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/linear_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/models/wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/utils/mock_robot.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/utils/runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-15 15:55:46.000000 roxbot-2.0.0/src/roxbot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/src/roxbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 15:55:55.000000 roxbot-2.0.0/src/roxbot.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 15:55:55.419286 roxbot-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_diffdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_mqtt_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-15 15:55:46.000000 roxbot-2.0.0/tests/test_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.638934 roxbot-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-25 11:55:49.000000 roxbot-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-25 11:55:57.638934 roxbot-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-25 11:55:49.000000 roxbot-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-25 11:55:49.000000 roxbot-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 11:55:57.638934 roxbot-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.630933 roxbot-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.634934 roxbot-2.1.0/src/roxbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.634934 roxbot-2.1.0/src/roxbot/bridges/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/bridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/bridges/mqtt_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.634934 roxbot-2.1.0/src/roxbot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/models/diff_drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/models/linear_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/models/wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.634934 roxbot-2.1.0/src/roxbot/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/utils/mock_robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/utils/runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-25 11:55:49.000000 roxbot-2.1.0/src/roxbot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.638934 roxbot-2.1.0/src/roxbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-25 11:55:57.000000 roxbot-2.1.0/src/roxbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-25 11:55:57.000000 roxbot-2.1.0/src/roxbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 11:55:57.000000 roxbot-2.1.0/src/roxbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-25 11:55:57.000000 roxbot-2.1.0/src/roxbot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-25 11:55:57.000000 roxbot-2.1.0/src/roxbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-25 11:55:57.000000 roxbot-2.1.0/src/roxbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 11:55:57.638934 roxbot-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-25 11:55:49.000000 roxbot-2.1.0/tests/test_diffdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-25 11:55:49.000000 roxbot-2.1.0/tests/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-25 11:55:49.000000 roxbot-2.1.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-25 11:55:49.000000 roxbot-2.1.0/tests/test_mqtt_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-25 11:55:49.000000 roxbot-2.1.0/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-25 11:55:49.000000 roxbot-2.1.0/tests/test_vectors.py
```

### Comparing `roxbot-2.0.0/LICENSE` & `roxbot-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/PKG-INFO` & `roxbot-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roxbot
-Version: 2.0.0
+Version: 2.1.0
 Summary: Pythonic robotics toolkit
 Author-email: ROX Automation <dev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://example.com/roxbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Dist: aiomqtt
 Requires-Dist: click
 Requires-Dist: coloredlogs
 Requires-Dist: numpy
 Requires-Dist: orjson
 Requires-Dist: pydantic-settings
 Requires-Dist: pydantic
+Requires-Dist: rox-vectors
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
```

### Comparing `roxbot-2.0.0/README.md` & `roxbot-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/pyproject.toml` & `roxbot-2.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #-----------------pyproject.toml configuration----------------
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "roxbot"
-version = "2.0.0"
+version = "2.1.0"
 description = "Pythonic robotics toolkit"
 authors = [
     {name = "ROX Automation", email = "dev@roxautomation.com"},
 ]
 license = {text = "MIT"}
 readme = "README.md"
 classifiers = [
@@ -25,14 +25,15 @@
     "aiomqtt",
     "click",
     "coloredlogs",
     "numpy",
     "orjson",
     "pydantic-settings",
     "pydantic",
+    "rox-vectors"
 ]
 requires-python = ">=3.11"
 
 [project.urls]
 Homepage = "https://example.com/roxbot"
 
 [project.scripts]
```

### Comparing `roxbot-2.0.0/src/roxbot/bridges/mqtt_bridge.py` & `roxbot-2.1.0/src/roxbot/bridges/mqtt_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/src/roxbot/interfaces.py` & `roxbot-2.1.0/src/roxbot/interfaces.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/src/roxbot/models/diff_drive.py` & `roxbot-2.1.0/src/roxbot/models/diff_drive.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/src/roxbot/models/linear_model.py` & `roxbot-2.1.0/src/roxbot/models/linear_model.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/src/roxbot/models/wheels.py` & `roxbot-2.1.0/src/roxbot/models/wheels.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/src/roxbot/utils/mock_robot.py` & `roxbot-2.1.0/src/roxbot/utils/mock_robot.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/src/roxbot/utils/runners.py` & `roxbot-2.1.0/src/roxbot/utils/runners.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/src/roxbot.egg-info/PKG-INFO` & `roxbot-2.1.0/src/roxbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roxbot
-Version: 2.0.0
+Version: 2.1.0
 Summary: Pythonic robotics toolkit
 Author-email: ROX Automation <dev@roxautomation.com>
 License: MIT
 Project-URL: Homepage, https://example.com/roxbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,14 +18,15 @@
 Requires-Dist: aiomqtt
 Requires-Dist: click
 Requires-Dist: coloredlogs
 Requires-Dist: numpy
 Requires-Dist: orjson
 Requires-Dist: pydantic-settings
 Requires-Dist: pydantic
+Requires-Dist: rox-vectors
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
```

### Comparing `roxbot-2.0.0/src/roxbot.egg-info/SOURCES.txt` & `roxbot-2.1.0/src/roxbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/tests/test_diffdrive.py` & `roxbot-2.1.0/tests/test_diffdrive.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/tests/test_interfaces.py` & `roxbot-2.1.0/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/tests/test_models.py` & `roxbot-2.1.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/tests/test_mqtt_bridge.py` & `roxbot-2.1.0/tests/test_mqtt_bridge.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/tests/test_smoke.py` & `roxbot-2.1.0/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `roxbot-2.0.0/tests/test_vectors.py` & `roxbot-2.1.0/tests/test_vectors.py`

 * *Files identical despite different names*

