# Comparing `tmp/pyperclip_plus-0.1.7.tar.gz` & `tmp/pyperclip_plus-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperclip_plus-0.1.7.tar", last modified: Fri May 24 10:38:54 2024, max compression
+gzip compressed data, was "pyperclip_plus-0.1.8.tar", last modified: Sat May 25 13:23:59 2024, max compression
```

## Comparing `pyperclip_plus-0.1.7.tar` & `pyperclip_plus-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:38:54.242088 pyperclip_plus-0.1.7/
--rw-r--r--   0 akitashowhey   (501) staff       (20)     5418 2024-05-24 10:38:54.241975 pyperclip_plus-0.1.7/PKG-INFO
--rw-r--r--   0 akitashowhey   (501) staff       (20)     4684 2024-05-24 09:59:11.000000 pyperclip_plus-0.1.7/README.md
-drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:38:54.240814 pyperclip_plus-0.1.7/pyperclip_plus/
--rw-r--r--   0 akitashowhey   (501) staff       (20)       78 2024-05-24 10:10:16.000000 pyperclip_plus-0.1.7/pyperclip_plus/__init__.py
--rw-r--r--   0 akitashowhey   (501) staff       (20)     1422 2024-05-24 09:23:05.000000 pyperclip_plus-0.1.7/pyperclip_plus/clipboard_manager.py
-drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-24 10:38:54.241674 pyperclip_plus-0.1.7/pyperclip_plus.egg-info/
--rw-r--r--   0 akitashowhey   (501) staff       (20)     5418 2024-05-24 10:38:54.000000 pyperclip_plus-0.1.7/pyperclip_plus.egg-info/PKG-INFO
--rw-r--r--   0 akitashowhey   (501) staff       (20)      270 2024-05-24 10:38:54.000000 pyperclip_plus-0.1.7/pyperclip_plus.egg-info/SOURCES.txt
--rw-r--r--   0 akitashowhey   (501) staff       (20)        1 2024-05-24 10:38:54.000000 pyperclip_plus-0.1.7/pyperclip_plus.egg-info/dependency_links.txt
--rw-r--r--   0 akitashowhey   (501) staff       (20)       17 2024-05-24 10:38:54.000000 pyperclip_plus-0.1.7/pyperclip_plus.egg-info/requires.txt
--rw-r--r--   0 akitashowhey   (501) staff       (20)       15 2024-05-24 10:38:54.000000 pyperclip_plus-0.1.7/pyperclip_plus.egg-info/top_level.txt
--rw-r--r--   0 akitashowhey   (501) staff       (20)       38 2024-05-24 10:38:54.242135 pyperclip_plus-0.1.7/setup.cfg
--rw-r--r--   0 akitashowhey   (501) staff       (20)     1078 2024-05-24 10:38:43.000000 pyperclip_plus-0.1.7/setup.py
+drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-25 13:23:59.075622 pyperclip_plus-0.1.8/
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     2424 2024-05-25 13:23:59.075480 pyperclip_plus-0.1.8/PKG-INFO
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     1690 2024-05-25 13:20:36.000000 pyperclip_plus-0.1.8/README.md
+drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-25 13:23:59.074410 pyperclip_plus-0.1.8/pyperclip_plus/
+-rw-r--r--   0 akitashowhey   (501) staff       (20)       78 2024-05-24 10:10:16.000000 pyperclip_plus-0.1.8/pyperclip_plus/__init__.py
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     1422 2024-05-24 09:23:05.000000 pyperclip_plus-0.1.8/pyperclip_plus/clipboard_manager.py
+drwxr-xr-x   0 akitashowhey   (501) staff       (20)        0 2024-05-25 13:23:59.075278 pyperclip_plus-0.1.8/pyperclip_plus.egg-info/
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     2424 2024-05-25 13:23:59.000000 pyperclip_plus-0.1.8/pyperclip_plus.egg-info/PKG-INFO
+-rw-r--r--   0 akitashowhey   (501) staff       (20)      270 2024-05-25 13:23:59.000000 pyperclip_plus-0.1.8/pyperclip_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 akitashowhey   (501) staff       (20)        1 2024-05-25 13:23:59.000000 pyperclip_plus-0.1.8/pyperclip_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 akitashowhey   (501) staff       (20)       17 2024-05-25 13:23:59.000000 pyperclip_plus-0.1.8/pyperclip_plus.egg-info/requires.txt
+-rw-r--r--   0 akitashowhey   (501) staff       (20)       15 2024-05-25 13:23:59.000000 pyperclip_plus-0.1.8/pyperclip_plus.egg-info/top_level.txt
+-rw-r--r--   0 akitashowhey   (501) staff       (20)       38 2024-05-25 13:23:59.075675 pyperclip_plus-0.1.8/setup.cfg
+-rw-r--r--   0 akitashowhey   (501) staff       (20)     1078 2024-05-25 13:23:49.000000 pyperclip_plus-0.1.8/setup.py
```

### Comparing `pyperclip_plus-0.1.7/pyperclip_plus/clipboard_manager.py` & `pyperclip_plus-0.1.8/pyperclip_plus/clipboard_manager.py`

 * *Files identical despite different names*

### Comparing `pyperclip_plus-0.1.7/setup.py` & `pyperclip_plus-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # setup.py
 from setuptools import setup, find_packages
 import pathlib
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(
     name='pyperclip_plus',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     description='An enhanced clipboard management tool',
     author='Your Name',
     author_email='your.email@example.com',
     url='https://github.com/yourusername/pyperclip_plus',  # プロジェクトのURLを設定
     long_description=long_description,
     long_description_content_type="text/markdown",
```

