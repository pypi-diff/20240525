# Comparing `tmp/xrvoyage-1.0.8.tar.gz` & `tmp/xrvoyage-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrvoyage-1.0.8.tar", max compression
+gzip compressed data, was "xrvoyage-1.0.9.tar", max compression
```

## Comparing `xrvoyage-1.0.8.tar` & `xrvoyage-1.0.9.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0     1065 2024-05-23 19:06:35.446691 xrvoyage-1.0.8/LICENSE
--rw-r--r--   0        0        0      483 2024-05-23 19:06:57.046855 xrvoyage-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      107 2024-05-23 19:06:35.446691 xrvoyage-1.0.8/xrvoyage/__init__.py
--rw-r--r--   0        0        0       18 2024-05-23 19:06:57.098855 xrvoyage-1.0.8/xrvoyage/_version.py
--rw-r--r--   0        0        0        0 2024-05-23 19:06:35.446691 xrvoyage-1.0.8/xrvoyage/handlers/__init__.py
--rw-r--r--   0        0        0      209 2024-05-23 19:06:35.446691 xrvoyage-1.0.8/xrvoyage/handlers/static.py
--rw-r--r--   0        0        0        0 2024-05-23 19:06:35.446691 xrvoyage-1.0.8/xrvoyage/models/__init__.py
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 xrvoyage-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/LICENSE
+-rw-r--r--   0        0        0      444 2024-05-23 19:09:58.113895 xrvoyage-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-23 19:09:58.161895 xrvoyage-1.0.9/xrvoyage/_version.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/config/__init__.py
+-rw-r--r--   0        0        0      711 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/config/config.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/handlers/__init__.py
+-rw-r--r--   0        0        0     4149 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/handlers/auth.py
+-rw-r--r--   0        0        0      107 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/handlers/exceptions.py
+-rw-r--r--   0        0        0     1008 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/handlers/models.py
+-rw-r--r--   0        0        0      209 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/handlers/static.py
+-rw-r--r--   0        0        0     1251 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/handlers/wss_client.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/models/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-23 19:09:42.321844 xrvoyage-1.0.9/xrvoyage/models/events.py
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 xrvoyage-1.0.9/PKG-INFO
```

### Comparing `xrvoyage-1.0.8/LICENSE` & `xrvoyage-1.0.9/LICENSE`

 * *Files identical despite different names*

