# Comparing `tmp/corderius_play-1.0.0.tar.gz` & `tmp/corderius_play-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corderius_play-1.0.0.tar", last modified: Fri May 24 10:54:14 2024, max compression
+gzip compressed data, was "corderius_play-1.0.1.tar", last modified: Sat May 25 09:28:26 2024, max compression
```

## Comparing `corderius_play-1.0.0.tar` & `corderius_play-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:54:14.362192 corderius_play-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-24 10:54:09.000000 corderius_play-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-24 10:54:09.000000 corderius_play-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-24 10:54:14.358192 corderius_play-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30269 2024-05-24 10:54:09.000000 corderius_play-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:54:14.358192 corderius_play-1.0.0/corderius_play.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-24 10:54:14.000000 corderius_play-1.0.0/corderius_play.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 10:54:14.000000 corderius_play-1.0.0/corderius_play.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:54:14.000000 corderius_play-1.0.0/corderius_play.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 10:54:14.000000 corderius_play-1.0.0/corderius_play.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-24 10:54:14.000000 corderius_play-1.0.0/corderius_play.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    76062 2024-05-24 10:54:09.000000 corderius_play-1.0.0/example.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:54:14.358192 corderius_play-1.0.0/play/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/all_sprites.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/async_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/blank_image.png
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/clamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/color.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/keypress.py
--rw-r--r--   0 runner    (1001) docker     (127)    18639 2024-05-24 10:54:09.000000 corderius_play-1.0.0/play/play.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-24 10:54:09.000000 corderius_play-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:54:14.362192 corderius_play-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-24 10:54:09.000000 corderius_play-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:28:26.537928 corderius_play-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-25 09:28:16.000000 corderius_play-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-25 09:28:16.000000 corderius_play-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-25 09:28:26.537928 corderius_play-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30269 2024-05-25 09:28:16.000000 corderius_play-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:28:26.537928 corderius_play-1.0.1/corderius_play.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30827 2024-05-25 09:28:26.000000 corderius_play-1.0.1/corderius_play.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-25 09:28:26.000000 corderius_play-1.0.1/corderius_play.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:28:26.000000 corderius_play-1.0.1/corderius_play.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-25 09:28:26.000000 corderius_play-1.0.1/corderius_play.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 09:28:26.000000 corderius_play-1.0.1/corderius_play.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76062 2024-05-25 09:28:16.000000 corderius_play-1.0.1/example.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:28:26.537928 corderius_play-1.0.1/play/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/all_sprites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/async_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/blank_image.png
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:28:26.537928 corderius_play-1.0.1/play/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/keypress.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:28:26.537928 corderius_play-1.0.1/play/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/objects/box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/objects/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/objects/sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/objects/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:28:26.537928 corderius_play-1.0.1/play/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18639 2024-05-25 09:28:16.000000 corderius_play-1.0.1/play/play.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-25 09:28:16.000000 corderius_play-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:28:26.537928 corderius_play-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-25 09:28:16.000000 corderius_play-1.0.1/setup.py
```

### Comparing `corderius_play-1.0.0/LICENSE` & `corderius_play-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/PKG-INFO` & `corderius_play-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corderius-play
-Version: 1.0.0
+Version: 1.0.1
 Summary: The easiest way to make games and media projects in Python.
 Home-page: https://github.com/Corderius-College-Amersfoort/play
 Author: koen1711
 Author-email: koenvurk1711@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `corderius_play-1.0.0/README.md` & `corderius_play-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/corderius_play.egg-info/PKG-INFO` & `corderius_play-1.0.1/corderius_play.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corderius-play
-Version: 1.0.0
+Version: 1.0.1
 Summary: The easiest way to make games and media projects in Python.
 Home-page: https://github.com/Corderius-College-Amersfoort/play
 Author: koen1711
 Author-email: koenvurk1711@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `corderius_play-1.0.0/example.gif` & `corderius_play-1.0.1/example.gif`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/play/async_helpers.py` & `corderius_play-1.0.1/play/async_helpers.py`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/play/blank_image.png` & `corderius_play-1.0.1/play/blank_image.png`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/play/color.py` & `corderius_play-1.0.1/play/color.py`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/play/keypress.py` & `corderius_play-1.0.1/play/keypress.py`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/play/play.py` & `corderius_play-1.0.1/play/play.py`

 * *Files identical despite different names*

### Comparing `corderius_play-1.0.0/setup.py` & `corderius_play-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pathlib
-from setuptools import setup
+from setuptools import setup, find_packages
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="corderius-play",
-    version="1.0.0",
+    version="1.0.1",
     description="The easiest way to make games and media projects in Python.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Corderius-College-Amersfoort/play",
     author="koen1711",
     author_email="koenvurk1711@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
     ],
     python_requires=">=3.5",
-    packages=["play"],
+    packages=find_packages(),
     include_package_data=True,
     install_requires=["pygame", "numpy", "pymunk"],
 )
```

