# Comparing `tmp/xingpyc-0.0.2.tar.gz` & `tmp/xingpyc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingpyc-0.0.2.tar", last modified: Sat May 25 03:22:29 2024, max compression
+gzip compressed data, was "xingpyc-0.0.3.tar", last modified: Sat May 25 03:40:56 2024, max compression
```

## Comparing `xingpyc-0.0.2.tar` & `xingpyc-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.892658 xingpyc-0.0.2/
--rw-r--r--   0 xiaolin    (501) staff       (20)      486 2024-05-25 03:22:29.892444 xingpyc-0.0.2/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.2/README.md
--rw-r--r--   0 xiaolin    (501) staff       (20)      474 2024-05-25 03:22:26.000000 xingpyc-0.0.2/pyproject.toml
--rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 03:22:29.892699 xingpyc-0.0.2/setup.cfg
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.890611 xingpyc-0.0.2/src/
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.891078 xingpyc-0.0.2/src/xingpyc/
--rw-r--r--   0 xiaolin    (501) staff       (20)        0 2024-05-25 02:33:23.000000 xingpyc-0.0.2/src/xingpyc/__init__.py
--rw-r--r--   0 xiaolin    (501) staff       (20)       42 2024-05-25 03:13:33.000000 xingpyc-0.0.2/src/xingpyc/example.py
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.892223 xingpyc-0.0.2/src/xingpyc.egg-info/
--rw-r--r--   0 xiaolin    (501) staff       (20)      486 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/PKG-INFO
--rw-r--r--   0 xiaolin    (501) staff       (20)      226 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/SOURCES.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/dependency_links.txt
--rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 03:22:29.000000 xingpyc-0.0.2/src/xingpyc.egg-info/top_level.txt
-drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:22:29.891945 xingpyc-0.0.2/tests/
--rw-r--r--   0 xiaolin    (501) staff       (20)       25 2024-05-25 03:18:16.000000 xingpyc-0.0.2/tests/test1.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:40:56.262681 xingpyc-0.0.3/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      486 2024-05-25 03:40:56.262466 xingpyc-0.0.3/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)       14 2024-05-25 03:21:31.000000 xingpyc-0.0.3/README.md
+-rw-r--r--   0 xiaolin    (501) staff       (20)      474 2024-05-25 03:40:49.000000 xingpyc-0.0.3/pyproject.toml
+-rw-r--r--   0 xiaolin    (501) staff       (20)       38 2024-05-25 03:40:56.262724 xingpyc-0.0.3/setup.cfg
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:40:56.260277 xingpyc-0.0.3/src/
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:40:56.261002 xingpyc-0.0.3/src/xingpyc/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      109 2024-05-25 03:39:14.000000 xingpyc-0.0.3/src/xingpyc/__init__.py
+-rw-r--r--   0 xiaolin    (501) staff       (20)       27 2024-05-25 03:31:48.000000 xingpyc-0.0.3/src/xingpyc/example.py
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:40:56.262252 xingpyc-0.0.3/src/xingpyc.egg-info/
+-rw-r--r--   0 xiaolin    (501) staff       (20)      486 2024-05-25 03:40:56.000000 xingpyc-0.0.3/src/xingpyc.egg-info/PKG-INFO
+-rw-r--r--   0 xiaolin    (501) staff       (20)      226 2024-05-25 03:40:56.000000 xingpyc-0.0.3/src/xingpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        1 2024-05-25 03:40:56.000000 xingpyc-0.0.3/src/xingpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaolin    (501) staff       (20)        8 2024-05-25 03:40:56.000000 xingpyc-0.0.3/src/xingpyc.egg-info/top_level.txt
+drwxr-xr-x   0 xiaolin    (501) staff       (20)        0 2024-05-25 03:40:56.261951 xingpyc-0.0.3/tests/
+-rw-r--r--   0 xiaolin    (501) staff       (20)       40 2024-05-25 03:39:07.000000 xingpyc-0.0.3/tests/test1.py
```

