# Comparing `tmp/kamangir-3.59.1.tar.gz` & `tmp/kamangir-3.60.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kamangir-3.59.1.tar", last modified: Sat May 25 01:52:51 2024, max compression
+gzip compressed data, was "kamangir-3.60.1.tar", last modified: Sat May 25 17:42:39 2024, max compression
```

## Comparing `kamangir-3.59.1.tar` & `kamangir-3.60.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:52:51.726327 kamangir-3.59.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.59.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:43.000000 kamangir-3.59.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4179 2024-05-25 01:52:51.725717 kamangir-3.59.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3281 2024-05-25 01:33:31.000000 kamangir-3.59.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:52:51.722524 kamangir-3.59.1/kamangir/
--rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-25 01:52:43.000000 kamangir-3.59.1/kamangir/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-05-21 02:51:14.000000 kamangir-3.59.1/kamangir/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     4725 2024-05-25 01:28:19.000000 kamangir-3.59.1/kamangir/content.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-05-21 02:51:14.000000 kamangir-3.59.1/kamangir/functions.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-21 02:51:14.000000 kamangir-3.59.1/kamangir/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-21 02:51:14.000000 kamangir-3.59.1/kamangir/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:52:51.724950 kamangir-3.59.1/kamangir.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4179 2024-05-25 01:52:51.000000 kamangir-3.59.1/kamangir.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      349 2024-05-25 01:52:51.000000 kamangir-3.59.1/kamangir.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:52:51.000000 kamangir-3.59.1/kamangir.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      180 2024-05-25 01:52:51.000000 kamangir-3.59.1/kamangir.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-25 01:52:51.000000 kamangir-3.59.1/kamangir.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-22 02:19:52.000000 kamangir-3.59.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      180 2024-05-25 01:29:17.000000 kamangir-3.59.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:52:51.726444 kamangir-3.59.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-22 02:20:30.000000 kamangir-3.59.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:42:39.075891 kamangir-3.60.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-12 02:58:40.000000 kamangir-3.60.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:43.000000 kamangir-3.60.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4179 2024-05-25 17:42:39.075294 kamangir-3.60.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3281 2024-05-25 17:42:34.000000 kamangir-3.60.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:42:39.071489 kamangir-3.60.1/kamangir/
+-rw-r--r--   0 kamangir   (502) staff       (20)       94 2024-05-25 17:42:33.000000 kamangir-3.60.1/kamangir/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      581 2024-05-21 02:51:14.000000 kamangir-3.60.1/kamangir/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     4725 2024-05-25 01:28:19.000000 kamangir-3.60.1/kamangir/content.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1943 2024-05-21 02:51:14.000000 kamangir-3.60.1/kamangir/functions.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-05-21 02:51:14.000000 kamangir-3.60.1/kamangir/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-21 02:51:14.000000 kamangir-3.60.1/kamangir/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 17:42:39.074583 kamangir-3.60.1/kamangir.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4179 2024-05-25 17:42:39.000000 kamangir-3.60.1/kamangir.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      349 2024-05-25 17:42:39.000000 kamangir-3.60.1/kamangir.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 17:42:39.000000 kamangir-3.60.1/kamangir.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      180 2024-05-25 17:42:39.000000 kamangir-3.60.1/kamangir.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-25 17:42:39.000000 kamangir-3.60.1/kamangir.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-22 02:19:52.000000 kamangir-3.60.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      180 2024-05-25 01:29:17.000000 kamangir-3.60.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 17:42:39.076007 kamangir-3.60.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-22 02:20:30.000000 kamangir-3.60.1/setup.py
```

### Comparing `kamangir-3.59.1/LICENSE` & `kamangir-3.60.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kamangir-3.59.1/PKG-INFO` & `kamangir-3.60.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kamangir
-Version: 3.59.1
+Version: 3.60.1
 Summary: 📜 github/kamangir
 Home-page: https://github.com/kamangir/kamangir
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -36,8 +36,8 @@
 | [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks and scripts for ai experiments and aws batch jobs. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 a recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
 | --- | --- | --- | --- |
 | [![image](https://github.com/kamangir/openai-commands/raw/main/assets/carrot.png)](https://github.com/kamangir/openai-commands) 🛠️ a command interface to the OpenAI API | [![image](https://github.com/kamangir/hubble/raw/main/assets/hst/u4ge0106r_c0m.gif)](https://github.com/kamangir/hubble) 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry. | [![image](https://github.com/kamangir/AI-ART/raw/main/blue-stability/blue_stability.gif)](https://github.com/kamangir/blue-stability) bash cli for stability.ai API's stable diffusion inference | [![image](https://github.com/kamangir/openai-commands/raw/main/assets/DALL-E.png?raw=1)](https://github.com/kamangir/aiart) 🎨 tools for ai artists. |
 | [![image](https://github.com/kamangir/awesome-bash-cli/raw/main/assets/marquee.png)](https://github.com/kamangir/awesome-bash-cli) 🚀 a language to speak AI. | [![image](https://user-images.githubusercontent.com/1007567/221448494-d57e08c1-625b-499e-a576-81894f112d6a.jpg)](https://github.com/kamangir/ferfereh) 3d-printed graffiti | [![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/Canadians_v11.gif)](https://github.com/kamangir/Kanata) a multi-screen video feed that is comprised of a matrix of animated faces that slide to the right. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/dec82-6.jpg)](https://github.com/kamangir/dec82) A wearable Raspberry Pi + Grove / Qwiic + Camera. |
 | [![image](https://github.com/kamangir/blue-rvr/raw/master/abcli/assets/marquee.jpeg)](https://github.com/kamangir/blue-rvr) a bash cli for Sphero RVR SDK - runs deep learning vision models on a Raspberry Pi using Python and TensorFlow. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/marquee.jpg)](https://github.com/kamangir/blue-bracket) a parametric 3d-printed bracket to build hardware for machine vision & ai on raspberry pi and jetson nano on the edge. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/blue3-1.jpg)](https://github.com/kamangir/blue-sbc) python + bash bootstrap for edge computing on single board computers. |  |
 
 ---
-built by [`abcli-8.214.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.57.1`](https://github.com/kamangir/kamangir).
+built by [`abcli-8.223.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.60.1`](https://github.com/kamangir/kamangir).
```

### Comparing `kamangir-3.59.1/README.md` & `kamangir-3.60.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 | [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks and scripts for ai experiments and aws batch jobs. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 a recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
 | --- | --- | --- | --- |
 | [![image](https://github.com/kamangir/openai-commands/raw/main/assets/carrot.png)](https://github.com/kamangir/openai-commands) 🛠️ a command interface to the OpenAI API | [![image](https://github.com/kamangir/hubble/raw/main/assets/hst/u4ge0106r_c0m.gif)](https://github.com/kamangir/hubble) 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry. | [![image](https://github.com/kamangir/AI-ART/raw/main/blue-stability/blue_stability.gif)](https://github.com/kamangir/blue-stability) bash cli for stability.ai API's stable diffusion inference | [![image](https://github.com/kamangir/openai-commands/raw/main/assets/DALL-E.png?raw=1)](https://github.com/kamangir/aiart) 🎨 tools for ai artists. |
 | [![image](https://github.com/kamangir/awesome-bash-cli/raw/main/assets/marquee.png)](https://github.com/kamangir/awesome-bash-cli) 🚀 a language to speak AI. | [![image](https://user-images.githubusercontent.com/1007567/221448494-d57e08c1-625b-499e-a576-81894f112d6a.jpg)](https://github.com/kamangir/ferfereh) 3d-printed graffiti | [![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/Canadians_v11.gif)](https://github.com/kamangir/Kanata) a multi-screen video feed that is comprised of a matrix of animated faces that slide to the right. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/dec82-6.jpg)](https://github.com/kamangir/dec82) A wearable Raspberry Pi + Grove / Qwiic + Camera. |
 | [![image](https://github.com/kamangir/blue-rvr/raw/master/abcli/assets/marquee.jpeg)](https://github.com/kamangir/blue-rvr) a bash cli for Sphero RVR SDK - runs deep learning vision models on a Raspberry Pi using Python and TensorFlow. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/marquee.jpg)](https://github.com/kamangir/blue-bracket) a parametric 3d-printed bracket to build hardware for machine vision & ai on raspberry pi and jetson nano on the edge. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/blue3-1.jpg)](https://github.com/kamangir/blue-sbc) python + bash bootstrap for edge computing on single board computers. |  |
 
 ---
-built by [`abcli-8.214.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.57.1`](https://github.com/kamangir/kamangir).
+built by [`abcli-8.223.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.60.1`](https://github.com/kamangir/kamangir).
```

### Comparing `kamangir-3.59.1/kamangir/__main__.py` & `kamangir-3.60.1/kamangir/__main__.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.59.1/kamangir/content.py` & `kamangir-3.60.1/kamangir/content.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.59.1/kamangir/functions.py` & `kamangir-3.60.1/kamangir/functions.py`

 * *Files identical despite different names*

### Comparing `kamangir-3.59.1/kamangir.egg-info/PKG-INFO` & `kamangir-3.60.1/kamangir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kamangir
-Version: 3.59.1
+Version: 3.60.1
 Summary: 📜 github/kamangir
 Home-page: https://github.com/kamangir/kamangir
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
@@ -36,8 +36,8 @@
 | [![image](https://github.com/kamangir/assets/raw/main/nbs/3x4.jpg?raw=true)](https://github.com/kamangir/notebooks-and-scripts) 📜 notebooks and scripts for ai experiments and aws batch jobs. | [![image](https://user-images.githubusercontent.com/1007567/196573547-b1c71b3b-7fac-4d2c-bba0-a87b063830da.png)](https://github.com/kamangir/Vancouver-Watching) 🌈 Vancouver Watching with AI. | [![image](https://github.com/kamangir/giza/raw/main/assets/giza.png)](https://github.com/kamangir/giza) 🔻 a recipe for AI languages. | [![image](https://github.com/kamangir/assets/blob/main/2023-10-28-16-28-36-88493-predict.gif?raw=true)](https://github.com/kamangir/roofAI) 🏛️ everything AI about roofs. |
 | --- | --- | --- | --- |
 | [![image](https://github.com/kamangir/openai-commands/raw/main/assets/carrot.png)](https://github.com/kamangir/openai-commands) 🛠️ a command interface to the OpenAI API | [![image](https://github.com/kamangir/hubble/raw/main/assets/hst/u4ge0106r_c0m.gif)](https://github.com/kamangir/hubble) 🔭 tools to access and process Hubble Space Telescope imagery and other datasets on AWS Open Data Registry. | [![image](https://github.com/kamangir/AI-ART/raw/main/blue-stability/blue_stability.gif)](https://github.com/kamangir/blue-stability) bash cli for stability.ai API's stable diffusion inference | [![image](https://github.com/kamangir/openai-commands/raw/main/assets/DALL-E.png?raw=1)](https://github.com/kamangir/aiart) 🎨 tools for ai artists. |
 | [![image](https://github.com/kamangir/awesome-bash-cli/raw/main/assets/marquee.png)](https://github.com/kamangir/awesome-bash-cli) 🚀 a language to speak AI. | [![image](https://user-images.githubusercontent.com/1007567/221448494-d57e08c1-625b-499e-a576-81894f112d6a.jpg)](https://github.com/kamangir/ferfereh) 3d-printed graffiti | [![image](https://kamangir-public.s3.ca-central-1.amazonaws.com/Canadians_v11.gif)](https://github.com/kamangir/Kanata) a multi-screen video feed that is comprised of a matrix of animated faces that slide to the right. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/dec82-6.jpg)](https://github.com/kamangir/dec82) A wearable Raspberry Pi + Grove / Qwiic + Camera. |
 | [![image](https://github.com/kamangir/blue-rvr/raw/master/abcli/assets/marquee.jpeg)](https://github.com/kamangir/blue-rvr) a bash cli for Sphero RVR SDK - runs deep learning vision models on a Raspberry Pi using Python and TensorFlow. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/marquee.jpg)](https://github.com/kamangir/blue-bracket) a parametric 3d-printed bracket to build hardware for machine vision & ai on raspberry pi and jetson nano on the edge. | [![image](https://github.com/kamangir/blue-bracket/raw/main/images/blue3-1.jpg)](https://github.com/kamangir/blue-sbc) python + bash bootstrap for edge computing on single board computers. |  |
 
 ---
-built by [`abcli-8.214.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.57.1`](https://github.com/kamangir/kamangir).
+built by [`abcli-8.223.1-current`](https://github.com/kamangir/awesome-bash-cli), based on [`kamangir-3.60.1`](https://github.com/kamangir/kamangir).
```

