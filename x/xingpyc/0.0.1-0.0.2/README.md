# Comparing `tmp/xingpyc-0.0.1.tar.gz` & `tmp/xingpyc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.0.1.tar", last modified: Sat May 25 03:15:43 2024, max compression
+gzip compressed data, was "xingpyc-0.0.2.tar", last modified: Sat May 25 03:22:29 2024, max compression
```

## Comparing `xingpyc-0.0.1.tar` & `xingpyc-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:15:43.537891 xingpyc-0.0.1/
--rw-r--r--   0 xiaolin    (501) staff       (20)      527 2024-05-25 03:15:43.537723 xingpyc-0.0.1/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       55 2024-05-25 03:08:09.000000 xingpyc-0.0.1/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      474 2024-05-25 03:15:38.000000 xingpyc-0.0.1/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 03:15:43.537926 xingpyc-0.0.1/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:15:43.536268 xingpyc-0.0.1/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:15:43.536757 xingpyc-0.0.1/src/XingPyClient/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-25 02:33:23.000000 xingpyc-0.0.1/src/XingPyClient/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       42 2024-05-25 03:13:33.000000 xingpyc-0.0.1/src/XingPyClient/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:15:43.537550 xingpyc-0.0.1/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      527 2024-05-25 03:15:43.000000 xingpyc-0.0.1/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      221 2024-05-25 03:15:43.000000 xingpyc-0.0.1/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 03:15:43.000000 xingpyc-0.0.1/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)       13 2024-05-25 03:15:43.000000 xingpyc-0.0.1/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.892658 xingpyc-0.0.2/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      486 2024-05-25 03:22:29.892444 xingpyc-0.0.2/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.2/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      474 2024-05-25 03:22:26.000000 xingpyc-0.0.2/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 03:22:29.892699 xingpyc-0.0.2/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.890611 xingpyc-0.0.2/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.891078 xingpyc-0.0.2/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-25 02:33:23.000000 xingpyc-0.0.2/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       42 2024-05-25 03:13:33.000000 xingpyc-0.0.2/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.892223 xingpyc-0.0.2/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      486 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      226 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.891945 xingpyc-0.0.2/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)       25 2024-05-25 03:18:16.000000 xingpyc-0.0.2/tests/test1.py
```

