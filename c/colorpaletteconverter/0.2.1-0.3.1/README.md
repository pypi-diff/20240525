# Comparing `tmp/colorpaletteconverter-0.2.1.tar.gz` & `tmp/colorpaletteconverter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colorpaletteconverter-0.2.1.tar", last modified: Fri Aug 20 11:20:56 2021, max compression
+gzip compressed data, was "colorpaletteconverter-0.3.1.tar", last modified: Sat May 25 13:48:02 2024, max compression
```

## Comparing `colorpaletteconverter-0.2.1.tar` & `colorpaletteconverter-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rutgerberns   (504) staff       (20)        0 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/
--rw-r--r--   0 rutgerberns   (504) staff       (20)     1069 2021-08-19 12:53:22.000000 colorpaletteconverter-0.2.1/LICENSE.txt
--rw-r--r--   0 rutgerberns   (504) staff       (20)       70 2021-08-19 14:10:40.000000 colorpaletteconverter-0.2.1/MANIFEST.in
--rw-r--r--   0 rutgerberns   (504) staff       (20)     2424 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/PKG-INFO
--rw-r--r--   0 rutgerberns   (504) staff       (20)     1421 2021-08-20 10:24:43.000000 colorpaletteconverter-0.2.1/README.md
--rw-r--r--   0 rutgerberns   (504) staff       (20)       38 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/setup.cfg
--rw-r--r--   0 rutgerberns   (504) staff       (20)     1061 2021-08-20 10:38:03.000000 colorpaletteconverter-0.2.1/setup.py
-drwxr-xr-x   0 rutgerberns   (504) staff       (20)        0 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/src/
-drwxr-xr-x   0 rutgerberns   (504) staff       (20)        0 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/src/colorpaletteconverter.egg-info/
--rw-r--r--   0 rutgerberns   (504) staff       (20)     2424 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/src/colorpaletteconverter.egg-info/PKG-INFO
--rw-r--r--   0 rutgerberns   (504) staff       (20)      351 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/src/colorpaletteconverter.egg-info/SOURCES.txt
--rw-r--r--   0 rutgerberns   (504) staff       (20)        1 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/src/colorpaletteconverter.egg-info/dependency_links.txt
--rw-r--r--   0 rutgerberns   (504) staff       (20)       64 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/src/colorpaletteconverter.egg-info/requires.txt
--rw-r--r--   0 rutgerberns   (504) staff       (20)       22 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/src/colorpaletteconverter.egg-info/top_level.txt
--rw-r--r--   0 rutgerberns   (504) staff       (20)     1381 2021-08-20 10:12:08.000000 colorpaletteconverter-0.2.1/src/colorpaletteconverter.py
-drwxr-xr-x   0 rutgerberns   (504) staff       (20)        0 2021-08-20 11:20:56.000000 colorpaletteconverter-0.2.1/tests/
--rw-r--r--   0 rutgerberns   (504) staff       (20)      410 2021-08-19 14:39:20.000000 colorpaletteconverter-0.2.1/tests/test_colorpaletteconverter.py
+drwxr-xr-x   0 rutgerberns   (501) staff       (20)        0 2024-05-25 13:48:02.383121 colorpaletteconverter-0.3.1/
+-rw-r--r--   0 rutgerberns   (501) staff       (20)     1069 2024-05-25 13:44:03.000000 colorpaletteconverter-0.3.1/LICENSE.txt
+-rw-r--r--   0 rutgerberns   (501) staff       (20)       70 2024-05-25 13:44:03.000000 colorpaletteconverter-0.3.1/MANIFEST.in
+-rw-r--r--   0 rutgerberns   (501) staff       (20)     2353 2024-05-25 13:48:02.382834 colorpaletteconverter-0.3.1/PKG-INFO
+-rw-r--r--   0 rutgerberns   (501) staff       (20)     1563 2024-05-25 13:44:03.000000 colorpaletteconverter-0.3.1/README.md
+-rw-r--r--   0 rutgerberns   (501) staff       (20)       38 2024-05-25 13:48:02.383185 colorpaletteconverter-0.3.1/setup.cfg
+-rw-r--r--   0 rutgerberns   (501) staff       (20)     1063 2024-05-25 13:44:44.000000 colorpaletteconverter-0.3.1/setup.py
+drwxr-xr-x   0 rutgerberns   (501) staff       (20)        0 2024-05-25 13:48:02.380974 colorpaletteconverter-0.3.1/src/
+drwxr-xr-x   0 rutgerberns   (501) staff       (20)        0 2024-05-25 13:48:02.382328 colorpaletteconverter-0.3.1/src/colorpaletteconverter.egg-info/
+-rw-r--r--   0 rutgerberns   (501) staff       (20)     2353 2024-05-25 13:48:02.000000 colorpaletteconverter-0.3.1/src/colorpaletteconverter.egg-info/PKG-INFO
+-rw-r--r--   0 rutgerberns   (501) staff       (20)      351 2024-05-25 13:48:02.000000 colorpaletteconverter-0.3.1/src/colorpaletteconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 rutgerberns   (501) staff       (20)        1 2024-05-25 13:48:02.000000 colorpaletteconverter-0.3.1/src/colorpaletteconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 rutgerberns   (501) staff       (20)       66 2024-05-25 13:48:02.000000 colorpaletteconverter-0.3.1/src/colorpaletteconverter.egg-info/requires.txt
+-rw-r--r--   0 rutgerberns   (501) staff       (20)       22 2024-05-25 13:48:02.000000 colorpaletteconverter-0.3.1/src/colorpaletteconverter.egg-info/top_level.txt
+-rw-r--r--   0 rutgerberns   (501) staff       (20)     1381 2024-05-25 13:44:03.000000 colorpaletteconverter-0.3.1/src/colorpaletteconverter.py
+drwxr-xr-x   0 rutgerberns   (501) staff       (20)        0 2024-05-25 13:48:02.381806 colorpaletteconverter-0.3.1/tests/
+-rw-r--r--   0 rutgerberns   (501) staff       (20)      410 2024-05-25 13:44:03.000000 colorpaletteconverter-0.3.1/tests/test_colorpaletteconverter.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `colorpaletteconverter-0.2.1/LICENSE.txt` & `colorpaletteconverter-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colorpaletteconverter-0.2.1/README.md` & `colorpaletteconverter-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # ColorpaletteConverter
 
 Export colorpalettes in Python to the MacOS color helper. 
 
 ![MacOS color helper](assets/output.png)
 
+## Install
+
+```
+pip install colorpaletteconverter
+```
+Note: MacOS only
 ## Usage
 
 ```python
 import colorpaletteconverter as cv
 
 # Create the palette, named "MyPythonPalette"
 mypalette = cv.Palette("MyPythonPalette")
@@ -33,7 +39,10 @@
 
 - Matplotlib color palettes: https://matplotlib.org/stable/tutorials/colors/colormaps.html
 - Seaborn color palettes: https://seaborn.pydata.org/tutorial/color_palettes.html
 
 The colors can be used in application like Apple Pages, Apple Keynote, Apple Numbers, Apple Final Cut Pro X, Microsoft Word, Microsoft Powerpoint and more.
 
 ![Example in Apple Pages](assets/PagesViridisExample.png)
+
+## Used packages
+- [PyObjC](https://github.com/ronaldoussoren/pyobjc)
```

### Comparing `colorpaletteconverter-0.2.1/setup.py` & `colorpaletteconverter-0.3.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup (
     name='colorpaletteconverter',
-    version='0.2.1',
+    version='0.3.1',
     description='Make a MacOS Color palette from Python',
     py_modules=["colorpaletteconverter"],
     package_dir={'': 'src'},
     author="Rutger Berns",
     author_email="rutgerb0000@gmail.com",
     url="https://github.com/Rutger0000/colorpalette-converter",
     classifiers=[
@@ -21,16 +21,16 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS",
         "Topic :: Multimedia"
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
-        "pyobjc-core ~= 7.3",
-        "pyobjc-framework-Cocoa ~= 7.3"
+        "pyobjc-core ~= 10.2",
+        "pyobjc-framework-Cocoa ~= 10.2"
     ],
     extras_require = {
         "dev": [
             "pytest>=5.2"
         ]
     }
 )
```

### Comparing `colorpaletteconverter-0.2.1/src/colorpaletteconverter.py` & `colorpaletteconverter-0.3.1/src/colorpaletteconverter.py`

 * *Files identical despite different names*

