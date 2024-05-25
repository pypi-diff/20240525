# Comparing `tmp/investimentpy-1.0.0.tar.gz` & `tmp/investimentpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investimentpy-1.0.0.tar", last modified: Sat May 25 13:30:31 2024, max compression
+gzip compressed data, was "investimentpy-1.0.1.tar", last modified: Sat May 25 13:56:38 2024, max compression
```

## Comparing `investimentpy-1.0.0.tar` & `investimentpy-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-05-25 13:30:31.782618 investimentpy-1.0.0/
--rw-r--r--   0 thiagoadriano   (501) staff       (20)     1937 2024-05-25 13:30:31.782388 investimentpy-1.0.0/PKG-INFO
--rw-r--r--   0 thiagoadriano   (501) staff       (20)     1643 2024-05-25 11:36:47.000000 investimentpy-1.0.0/README.md
-drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-05-25 13:30:31.782101 investimentpy-1.0.0/investimentpy.egg-info/
--rw-r--r--   0 thiagoadriano   (501) staff       (20)     1937 2024-05-25 13:30:31.000000 investimentpy-1.0.0/investimentpy.egg-info/PKG-INFO
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      274 2024-05-25 13:30:31.000000 investimentpy-1.0.0/investimentpy.egg-info/SOURCES.txt
--rw-r--r--   0 thiagoadriano   (501) staff       (20)        1 2024-05-25 13:30:31.000000 investimentpy-1.0.0/investimentpy.egg-info/dependency_links.txt
--rw-r--r--   0 thiagoadriano   (501) staff       (20)        9 2024-05-25 13:30:31.000000 investimentpy-1.0.0/investimentpy.egg-info/top_level.txt
-drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-05-25 13:30:31.781406 investimentpy-1.0.0/investpy/
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      126 2024-05-25 11:12:40.000000 investimentpy-1.0.0/investpy/__init__.py
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      122 2024-05-25 11:13:10.000000 investimentpy-1.0.0/investpy/calculos.py
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      847 2024-05-25 11:12:46.000000 investimentpy-1.0.0/investpy/dados.py
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      306 2024-05-25 11:13:22.000000 investimentpy-1.0.0/investpy/visualizacao.py
--rw-r--r--   0 thiagoadriano   (501) staff       (20)       38 2024-05-25 13:30:31.782668 investimentpy-1.0.0/setup.cfg
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      534 2024-05-25 13:20:28.000000 investimentpy-1.0.0/setup.py
-drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-05-25 13:30:31.781747 investimentpy-1.0.0/tests/
--rw-r--r--   0 thiagoadriano   (501) staff       (20)      886 2024-05-25 11:29:26.000000 investimentpy-1.0.0/tests/test_investpy.py
+drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-05-25 13:56:38.118231 investimentpy-1.0.1/
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)     1713 2024-05-25 13:56:38.118114 investimentpy-1.0.1/PKG-INFO
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)     1478 2024-05-25 13:55:09.000000 investimentpy-1.0.1/README.md
+drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-05-25 13:56:38.116768 investimentpy-1.0.1/investimentpy.egg-info/
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)     1713 2024-05-25 13:56:38.000000 investimentpy-1.0.1/investimentpy.egg-info/PKG-INFO
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      251 2024-05-25 13:56:38.000000 investimentpy-1.0.1/investimentpy.egg-info/SOURCES.txt
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)        1 2024-05-25 13:56:38.000000 investimentpy-1.0.1/investimentpy.egg-info/dependency_links.txt
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)        9 2024-05-25 13:56:38.000000 investimentpy-1.0.1/investimentpy.egg-info/top_level.txt
+drwxr-xr-x   0 thiagoadriano   (501) staff       (20)        0 2024-05-25 13:56:38.117770 investimentpy-1.0.1/investpy/
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      126 2024-05-25 11:12:40.000000 investimentpy-1.0.1/investpy/__init__.py
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      122 2024-05-25 11:13:10.000000 investimentpy-1.0.1/investpy/calculos.py
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      847 2024-05-25 11:12:46.000000 investimentpy-1.0.1/investpy/dados.py
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      306 2024-05-25 11:13:22.000000 investimentpy-1.0.1/investpy/visualizacao.py
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)       38 2024-05-25 13:56:38.118291 investimentpy-1.0.1/setup.cfg
+-rw-r--r--   0 thiagoadriano   (501) staff       (20)      477 2024-05-25 13:55:52.000000 investimentpy-1.0.1/setup.py
```

### Comparing `investimentpy-1.0.0/investpy/dados.py` & `investimentpy-1.0.1/investpy/dados.py`

 * *Files identical despite different names*

