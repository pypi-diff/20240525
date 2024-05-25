# Comparing `tmp/kub-0.1.0.tar.gz` & `tmp/kub-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kub-0.1.0.tar", max compression
+gzip compressed data, was "kub-0.1.1.tar", max compression
```

## Comparing `kub-0.1.0.tar` & `kub-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-08-26 02:01:01.716187 kub-0.1.0/LICENSE
--rw-r--r--   0        0        0       46 2023-08-26 02:01:01.716427 kub-0.1.0/README.md
--rw-r--r--   0        0        0      327 2024-04-28 17:41:41.705060 kub-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7642 2024-05-24 14:03:48.796275 kub-0.1.0/src/kub/KUB.py
--rw-r--r--   0        0        0        0 2023-08-26 12:23:34.125444 kub-0.1.0/src/kub/__init__.py
--rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 kub-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-26 02:01:01.716187 kub-0.1.1/LICENSE
+-rw-r--r--   0        0        0       46 2023-08-26 02:01:01.716427 kub-0.1.1/README.md
+-rw-r--r--   0        0        0      327 2024-05-24 14:24:52.667716 kub-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-26 12:23:34.125444 kub-0.1.1/src/kub/__init__.py
+-rw-r--r--   0        0        0     7642 2024-05-24 14:03:48.796275 kub-0.1.1/src/kub/kubUtilities.py
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 kub-0.1.1/PKG-INFO
```

### Comparing `kub-0.1.0/LICENSE` & `kub-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kub-0.1.0/src/kub/KUB.py` & `kub-0.1.1/src/kub/kubUtilities.py`

 * *Files identical despite different names*

