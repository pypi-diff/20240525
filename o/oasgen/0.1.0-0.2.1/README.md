# Comparing `tmp/oasgen-0.1.0.tar.gz` & `tmp/oasgen-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasgen-0.1.0.tar", max compression
+gzip compressed data, was "oasgen-0.2.1.tar", max compression
```

## Comparing `oasgen-0.1.0.tar` & `oasgen-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-25 13:55:28.857332 oasgen-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-25 13:55:28.857277 oasgen-0.1.0/oasgen/__init__.py
--rw-r--r--   0        0        0        0 2024-05-25 14:01:53.680009 oasgen-0.1.0/oasgen/main.py
--rw-r--r--   0        0        0      271 2024-05-25 13:55:28.858510 oasgen-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 oasgen-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-25 16:41:01.868339 oasgen-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-25 16:41:01.837339 oasgen-0.2.1/oasgen/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-25 16:41:01.869339 oasgen-0.2.1/oasgen/main.py
+-rw-r--r--   0        0        0     4734 2024-05-25 16:41:01.837339 oasgen-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      355 1970-01-01 00:00:00.000000 oasgen-0.2.1/PKG-INFO
```

