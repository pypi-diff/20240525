# Comparing `tmp/squice-0.2.tar.gz` & `tmp/squice-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squice-0.2.tar", last modified: Sun May 19 14:38:31 2024, max compression
+gzip compressed data, was "squice-0.3.tar", last modified: Sat May 25 17:08:11 2024, max compression
```

## Comparing `squice-0.2.tar` & `squice-0.3.tar`

### file list

```diff
@@ -1,53 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.289654 squice-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.293654 squice-0.2/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-19 14:38:25.000000 squice-0.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-19 14:38:25.000000 squice-0.2/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-19 14:38:25.000000 squice-0.2/.github/workflows/lint_style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 14:38:25.000000 squice-0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-19 14:38:25.000000 squice-0.2/.github/workflows/pydoctor.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-19 14:38:25.000000 squice-0.2/.github/workflows/pytest_app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-19 14:38:25.000000 squice-0.2/.github/workflows/pytest_lib.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-19 14:38:25.000000 squice-0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-19 14:38:25.000000 squice-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-19 14:38:25.000000 squice-0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-19 14:38:25.000000 squice-0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-19 14:38:25.000000 squice-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-19 14:38:31.297654 squice-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-19 14:38:25.000000 squice-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/app/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-19 14:38:25.000000 squice-0.2/app/home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/app/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-19 14:38:25.000000 squice-0.2/app/pages/2_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-19 14:38:25.000000 squice-0.2/app/pages/3_use_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-19 14:38:25.000000 squice-0.2/app/pages/4_about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)   183520 2024-05-19 14:38:25.000000 squice-0.2/app/static/squice.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.289654 squice-0.2/app/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/app/tests/use_cases/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-19 14:38:25.000000 squice-0.2/app/tests/use_cases/test_add_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-19 14:38:25.000000 squice-0.2/citation.cff
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-19 14:38:25.000000 squice-0.2/dev.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-19 14:38:25.000000 squice-0.2/docs/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 14:38:25.000000 squice-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-19 14:38:25.000000 squice-0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 14:38:25.000000 squice-0.2/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-19 14:38:31.301654 squice-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-19 14:38:25.000000 squice-0.2/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/src/squice/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-19 14:38:25.000000 squice-0.2/src/squice/ClassCurves.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:25.000000 squice-0.2/src/squice/ModulePredict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:25.000000 squice-0.2/src/squice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/src/squice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-19 14:38:31.000000 squice-0.2/src/squice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-19 14:38:31.000000 squice-0.2/src/squice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 14:38:31.000000 squice-0.2/src/squice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-19 14:38:31.000000 squice-0.2/src/squice.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.293654 squice-0.2/src/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/src/tests/speed/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-19 14:38:25.000000 squice-0.2/src/tests/speed/speed_log.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 14:38:31.297654 squice-0.2/src/tests/utility/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-19 14:38:25.000000 squice-0.2/src/tests/utility/test_curves.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.250116 squice-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.238116 squice-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.242116 squice-0.3/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-25 17:08:05.000000 squice-0.3/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-25 17:08:05.000000 squice-0.3/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-25 17:08:05.000000 squice-0.3/.github/workflows/lint_style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-25 17:08:05.000000 squice-0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-25 17:08:05.000000 squice-0.3/.github/workflows/pydoctor.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-25 17:08:05.000000 squice-0.3/.github/workflows/pytest_app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-25 17:08:05.000000 squice-0.3/.github/workflows/pytest_lib.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-25 17:08:05.000000 squice-0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-25 17:08:05.000000 squice-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-25 17:08:05.000000 squice-0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-25 17:08:05.000000 squice-0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-05-25 17:08:05.000000 squice-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-25 17:08:11.250116 squice-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-25 17:08:05.000000 squice-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-25 17:08:05.000000 squice-0.3/app/home.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/app/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-25 17:08:05.000000 squice-0.3/app/pages/2_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-25 17:08:05.000000 squice-0.3/app/pages/3_use_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-25 17:08:05.000000 squice-0.3/app/pages/4_about.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   183520 2024-05-25 17:08:05.000000 squice-0.3/app/static/squice.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.238116 squice-0.3/app/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/app/tests/use_cases/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 17:08:05.000000 squice-0.3/app/tests/use_cases/test_add_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-25 17:08:05.000000 squice-0.3/citation.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-25 17:08:05.000000 squice-0.3/dev.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-25 17:08:05.000000 squice-0.3/docs/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-25 17:08:05.000000 squice-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-25 17:08:05.000000 squice-0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-25 17:08:05.000000 squice-0.3/requirements_lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-25 17:08:11.250116 squice-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-25 17:08:05.000000 squice-0.3/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/src/squice/
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-25 17:08:05.000000 squice-0.3/src/squice/DataLoaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:05.000000 squice-0.3/src/squice/ModulePredict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-25 17:08:05.000000 squice-0.3/src/squice/MtxDisplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-25 17:08:05.000000 squice-0.3/src/squice/MtxInterpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:05.000000 squice-0.3/src/squice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.250116 squice-0.3/src/squice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-25 17:08:11.000000 squice-0.3/src/squice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-25 17:08:11.000000 squice-0.3/src/squice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 17:08:11.000000 squice-0.3/src/squice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 17:08:11.000000 squice-0.3/src/squice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:05.000000 squice-0.3/src/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.246116 squice-0.3/src/tests/speed/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:05.000000 squice-0.3/src/tests/speed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.250116 squice-0.3/src/tests/speed/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-25 17:08:05.000000 squice-0.3/src/tests/speed/data/speed_data.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-25 17:08:05.000000 squice-0.3/src/tests/speed/data/speed_log.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-25 17:08:05.000000 squice-0.3/src/tests/speed/help_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-25 17:08:05.000000 squice-0.3/src/tests/speed/test_dataloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.250116 squice-0.3/src/tests/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:05.000000 squice-0.3/src/tests/utility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 17:08:11.250116 squice-0.3/src/tests/utility/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-25 17:08:05.000000 squice-0.3/src/tests/utility/data/data1.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-25 17:08:05.000000 squice-0.3/src/tests/utility/data/data3d.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-25 17:08:05.000000 squice-0.3/src/tests/utility/test_loader.py
```

### Comparing `squice-0.2/.github/scripts/release.py` & `squice-0.3/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `squice-0.2/.github/workflows/docker.yml` & `squice-0.3/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `squice-0.2/.github/workflows/lint_style.yml` & `squice-0.3/.github/workflows/lint_style.yml`

 * *Files identical despite different names*

### Comparing `squice-0.2/.github/workflows/pydoctor.yml` & `squice-0.3/.github/workflows/pydoctor.yml`

 * *Files identical despite different names*

### Comparing `squice-0.2/.github/workflows/pytest_app.yml` & `squice-0.3/.github/workflows/pytest_app.yml`

 * *Files identical despite different names*

### Comparing `squice-0.2/.github/workflows/pytest_lib.yml` & `squice-0.3/.github/workflows/pytest_lib.yml`

 * *Files identical despite different names*

### Comparing `squice-0.2/.gitignore` & `squice-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `squice-0.2/Dockerfile` & `squice-0.3/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ######################################################################################################
 ### Correctly set up the .github/workflows/docker.yml will update this to docker automatically. ###
 #######################################################################################################
 ### To build this manually ###
 # docker build -f Dockerfile -t raea/squice .
-# 
+#
 ### To run it manually ###
 # docker run --rm --name squice -p 8001:8501 raea/squice
 #
 # I can then be found at http://localhost:8201/
-# 
+#
 ### To push it manually ###
 # docker push raea/squice
 ######################################################################################################
 
 FROM python:3.10
 WORKDIR /app
 COPY requirements.txt ./requirements.txt
```

### Comparing `squice-0.2/LICENSE` & `squice-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `squice-0.2/PKG-INFO` & `squice-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squice
-Version: 0.2
+Version: 0.3
 Summary: Example library for scientific software.
 Home-page: https://github.com/RachelAlcraft/squice
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/RachelAlcraft/squice/issues
 Project-URL: Documentation, https://rachelalcraft.github.io/squice
 Project-URL: Application demo, https://squice.streamlit.app
@@ -17,22 +17,26 @@
 
 # SQUICE
 
 *Slicing through squares: visualise and interpolate numerical matrix data.*
 
 This is a python library with accompanying demonstration streamlit web application, to visualise and interpolate numerical matrix data.
 
-This github site, streamlit application and pypi library has been created from the scientific application template [app-lib-py](https://github.com/RachelAlcraft/app-lib-py). 
+This github site, streamlit application and pypi library has been created from the scientific application template [app-lib-py](https://github.com/RachelAlcraft/app-lib-py).
 
 ### Use as an application
 To use the application simply go to the open source publicly hosted for free application [squice@streamlit](https://squice.streamlit.app/)
 
 ### Use as a python library
 ```
 pip install squice
 ```
-The documentation for the library is here: [squice docs](https://rachelalcraft.github.io/squice/index.html).  
+The documentation for the library is here: [squice docs](https://rachelalcraft.github.io/squice/index.html).
 Note the application [squice@streamlit](https://squice.streamlit.app/) also shows demonstrations of how to use the library.
 
 
 ### Use as a self-hosted web app
-This can also be downloaded from docker and self-hosted.
+This can also be [downloaded from docker](https://hub.docker.com/repository/docker/raea/squice/general) and self-hosted.
+```
+# docker pull raea/squice
+docker run --rm --name temp-name-p 8001:8501 raea/squice
+```
```

### Comparing `squice-0.2/README.md` & `squice-0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # SQUICE
 
 *Slicing through squares: visualise and interpolate numerical matrix data.*
 
 This is a python library with accompanying demonstration streamlit web application, to visualise and interpolate numerical matrix data.
 
-This github site, streamlit application and pypi library has been created from the scientific application template [app-lib-py](https://github.com/RachelAlcraft/app-lib-py). 
+This github site, streamlit application and pypi library has been created from the scientific application template [app-lib-py](https://github.com/RachelAlcraft/app-lib-py).
 
 ### Use as an application
 To use the application simply go to the open source publicly hosted for free application [squice@streamlit](https://squice.streamlit.app/)
 
 ### Use as a python library
 ```
 pip install squice
 ```
-The documentation for the library is here: [squice docs](https://rachelalcraft.github.io/squice/index.html).  
+The documentation for the library is here: [squice docs](https://rachelalcraft.github.io/squice/index.html).
 Note the application [squice@streamlit](https://squice.streamlit.app/) also shows demonstrations of how to use the library.
 
 
 ### Use as a self-hosted web app
-This can also be downloaded from docker and self-hosted.
+This can also be [downloaded from docker](https://hub.docker.com/repository/docker/raea/squice/general) and self-hosted.
+```
+# docker pull raea/squice
+docker run --rm --name temp-name-p 8001:8501 raea/squice
+```
```

### Comparing `squice-0.2/app/static/squice.png` & `squice-0.3/app/static/squice.png`

 * *Files identical despite different names*

### Comparing `squice-0.2/dev.md` & `squice-0.3/dev.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 **Use the appropriate one for the dev work. Keep a seperation in your mind between the scientific library (lib) and the demonstration of it (app).**
 
 # Virtual environments
 
 ## STREAMLIT APP
 ```
-python -m venv .env-sq-app
+/bin/python3.12 -m venv .env-sq-app
 ## Load dev environment
 source .env-sq-app/bin/activate
 (deactivate to exit venv)
 pip install --upgrade pip
 pip install -r requirements.txt --upgrade
 ```
 
@@ -19,22 +19,30 @@
 
 ## distribute to streamlit
 This will be automatically distributed to streamlit on push to main
 https://share.streamlit.io/
 
 ## Pypi library
 ```
-python -m venv .env-sq-lib
+/bin/python3.12 -m venv .env-sq-lib
 ## Load dev environment
 source .env-sq-lib/bin/activate
 (deactivate to exit venv)
 pip install --upgrade pip
 pip install -r requirements_lib.txt --upgrade
 ```
 
+## Pre-commit
+
+The pre-commit hook shyuld run on check in to format files as per standards.
+```
+pre-commit run --all-files
+black ./ --check --line-length 88 --diff
+black ./ --line-length 88
+```
 ---
 
 # Debugging
 
 ## A python file
 
 ## The streamlit app
```

### Comparing `squice-0.2/setup.cfg` & `squice-0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `squice-0.2/src/squice.egg-info/PKG-INFO` & `squice-0.3/src/squice.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: squice
-Version: 0.2
+Version: 0.3
 Summary: Example library for scientific software.
 Home-page: https://github.com/RachelAlcraft/squice
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/RachelAlcraft/squice/issues
 Project-URL: Documentation, https://rachelalcraft.github.io/squice
 Project-URL: Application demo, https://squice.streamlit.app
@@ -17,22 +17,26 @@
 
 # SQUICE
 
 *Slicing through squares: visualise and interpolate numerical matrix data.*
 
 This is a python library with accompanying demonstration streamlit web application, to visualise and interpolate numerical matrix data.
 
-This github site, streamlit application and pypi library has been created from the scientific application template [app-lib-py](https://github.com/RachelAlcraft/app-lib-py). 
+This github site, streamlit application and pypi library has been created from the scientific application template [app-lib-py](https://github.com/RachelAlcraft/app-lib-py).
 
 ### Use as an application
 To use the application simply go to the open source publicly hosted for free application [squice@streamlit](https://squice.streamlit.app/)
 
 ### Use as a python library
 ```
 pip install squice
 ```
-The documentation for the library is here: [squice docs](https://rachelalcraft.github.io/squice/index.html).  
+The documentation for the library is here: [squice docs](https://rachelalcraft.github.io/squice/index.html).
 Note the application [squice@streamlit](https://squice.streamlit.app/) also shows demonstrations of how to use the library.
 
 
 ### Use as a self-hosted web app
-This can also be downloaded from docker and self-hosted.
+This can also be [downloaded from docker](https://hub.docker.com/repository/docker/raea/squice/general) and self-hosted.
+```
+# docker pull raea/squice
+docker run --rm --name temp-name-p 8001:8501 raea/squice
+```
```

