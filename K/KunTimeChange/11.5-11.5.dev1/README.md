# Comparing `tmp/KunTimeChange-11.5.tar.gz` & `tmp/kuntimechange-11.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KunTimeChange-11.5.tar", last modified: Tue Jan 16 14:22:21 2024, max compression
+gzip compressed data, was "kuntimechange-11.5.dev1.tar", last modified: Sat May 25 12:55:54 2024, max compression
```

## Comparing `KunTimeChange-11.5.tar` & `kuntimechange-11.5.dev1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 14:22:21.005427 KunTimeChange-11.5/
-drwxrwxrwx   0        0        0        0 2024-01-16 14:22:21.003389 KunTimeChange-11.5/KunTimeChange.egg-info/
--rw-rw-rw-   0        0        0      259 2024-01-16 14:22:20.000000 KunTimeChange-11.5/KunTimeChange.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-01-16 14:22:20.000000 KunTimeChange-11.5/KunTimeChange.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-16 14:22:20.000000 KunTimeChange-11.5/KunTimeChange.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-16 14:22:20.000000 KunTimeChange-11.5/KunTimeChange.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      259 2024-01-16 14:22:21.004389 KunTimeChange-11.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-16 14:22:21.001389 KunTimeChange-11.5/ikuntime/
--rw-rw-rw-   0        0        0      298 2024-01-16 14:06:47.000000 KunTimeChange-11.5/ikuntime/__init__.py
--rw-rw-rw-   0        0        0       42 2024-01-16 14:22:21.005427 KunTimeChange-11.5/setup.cfg
--rw-rw-rw-   0        0        0      412 2024-01-16 14:11:59.000000 KunTimeChange-11.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:55:54.782169 kuntimechange-11.5.dev1/
+drwxrwxrwx   0        0        0        0 2024-05-25 12:55:54.773632 kuntimechange-11.5.dev1/KunTimeChange.egg-info/
+-rw-rw-rw-   0        0        0      259 2024-05-25 12:55:54.000000 kuntimechange-11.5.dev1/KunTimeChange.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-25 12:55:54.000000 kuntimechange-11.5.dev1/KunTimeChange.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 12:55:54.000000 kuntimechange-11.5.dev1/KunTimeChange.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-25 12:55:54.000000 kuntimechange-11.5.dev1/KunTimeChange.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      259 2024-05-25 12:55:54.777156 kuntimechange-11.5.dev1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-25 12:55:54.772127 kuntimechange-11.5.dev1/ikuntime/
+-rw-rw-rw-   0        0        0        0 2024-05-25 12:38:32.000000 kuntimechange-11.5.dev1/ikuntime/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-05-25 12:29:41.000000 kuntimechange-11.5.dev1/ikuntime/ikuntime.py
+-rw-rw-rw-   0        0        0       42 2024-05-25 12:55:54.782169 kuntimechange-11.5.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      412 2024-05-25 12:40:55.000000 kuntimechange-11.5.dev1/setup.py
```

