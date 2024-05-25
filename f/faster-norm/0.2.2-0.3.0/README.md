# Comparing `tmp/faster_norm-0.2.2.tar.gz` & `tmp/faster_norm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_norm-0.2.2.tar", last modified: Thu May  9 15:39:16 2024, max compression
+gzip compressed data, was "faster_norm-0.3.0.tar", last modified: Sat May 25 07:32:46 2024, max compression
```

## Comparing `faster_norm-0.2.2.tar` & `faster_norm-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:39:16.913591 faster_norm-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-05-05 15:03:52.000000 faster_norm-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-09 14:38:06.000000 faster_norm-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1052 2024-05-09 15:39:16.913591 faster_norm-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2024-05-09 15:37:29.000000 faster_norm-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:39:16.913591 faster_norm-0.2.2/faster_norm/
--rw-r--r--   0 root         (0) root         (0)       41 2024-05-09 14:38:49.000000 faster_norm-0.2.2/faster_norm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3913 2024-05-09 15:32:11.000000 faster_norm-0.2.2/faster_norm/faster_norm.cpp
--rw-r--r--   0 root         (0) root         (0)      469 2024-05-09 15:34:25.000000 faster_norm-0.2.2/faster_norm/faster_norm.hpp
--rw-r--r--   0 root         (0) root         (0)     1356 2024-05-09 14:40:09.000000 faster_norm-0.2.2/faster_norm/faster_norm.py
--rw-r--r--   0 root         (0) root         (0)    12604 2024-05-09 15:35:21.000000 faster_norm-0.2.2/faster_norm/faster_norm_cuda.cu
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 15:39:16.913591 faster_norm-0.2.2/faster_norm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1052 2024-05-09 15:39:16.000000 faster_norm-0.2.2/faster_norm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      317 2024-05-09 15:39:16.000000 faster_norm-0.2.2/faster_norm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 15:39:16.000000 faster_norm-0.2.2/faster_norm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-09 15:39:16.000000 faster_norm-0.2.2/faster_norm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 15:39:16.913591 faster_norm-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      860 2024-05-09 15:37:40.000000 faster_norm-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:32:46.044390 faster_norm-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-05-05 15:03:52.000000 faster_norm-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-09 14:38:06.000000 faster_norm-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-25 07:32:46.044390 faster_norm-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      486 2024-05-14 17:40:39.000000 faster_norm-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:32:46.044390 faster_norm-0.3.0/faster_norm/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-14 17:40:39.000000 faster_norm-0.3.0/faster_norm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8467 2024-05-14 17:40:39.000000 faster_norm-0.3.0/faster_norm/faster_norm.cpp
+-rw-r--r--   0 root         (0) root         (0)      858 2024-05-14 18:13:41.000000 faster_norm-0.3.0/faster_norm/faster_norm.hpp
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-05-14 17:42:48.000000 faster_norm-0.3.0/faster_norm/faster_norm.py
+-rw-r--r--   0 root         (0) root         (0)    23555 2024-05-25 07:31:14.000000 faster_norm-0.3.0/faster_norm/faster_norm_cuda.cu
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 07:32:46.044390 faster_norm-0.3.0/faster_norm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-25 07:32:45.000000 faster_norm-0.3.0/faster_norm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      317 2024-05-25 07:32:46.000000 faster_norm-0.3.0/faster_norm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 07:32:45.000000 faster_norm-0.3.0/faster_norm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-25 07:32:45.000000 faster_norm-0.3.0/faster_norm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 07:32:46.044390 faster_norm-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      860 2024-05-14 19:08:48.000000 faster_norm-0.3.0/setup.py
```

### Comparing `faster_norm-0.2.2/LICENSE` & `faster_norm-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_norm-0.2.2/setup.py` & `faster_norm-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 
 setup(name="faster_norm",
-      version="0.2.2",
+      version="0.3.0",
       author="Tailing Yuan",
       author_email="yuantailing@gmail.com",
       url="https://github.com/yuantailing/faster-norm",
       tests_require=["pytest", "torch"],
       description="A fast, yet specialized, RMSNorm/LayerNorm implementation",
       long_description=long_description,
       license="MIT",
```

