# Comparing `tmp/vbinsta-0.1.4.tar.gz` & `tmp/vbinsta-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbinsta-0.1.4.tar", max compression
+gzip compressed data, was "vbinsta-0.1.5.tar", max compression
```

## Comparing `vbinsta-0.1.4.tar` & `vbinsta-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.4/README.md
--rw-r--r--   0        0        0      368 2024-05-25 14:45:34.478044 vbinsta-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.4/vbinsta/__init__.py
--rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.4/vbinsta/__main__.py
--rw-r--r--   0        0        0     2725 2024-05-25 14:45:29.075769 vbinsta-0.1.4/vbinsta/functions.py
--rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.4/vbinsta/main.py
--rw-r--r--   0        0        0      973 2024-05-25 14:33:42.283724 vbinsta-0.1.4/vbinsta/upload.py
--rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.662078 vbinsta-0.1.5/README.md
+-rw-r--r--   0        0        0      368 2024-05-25 17:25:19.654738 vbinsta-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 06:30:54.661978 vbinsta-0.1.5/vbinsta/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-23 07:38:03.656860 vbinsta-0.1.5/vbinsta/__main__.py
+-rw-r--r--   0        0        0     1236 2024-05-25 15:57:02.621318 vbinsta-0.1.5/vbinsta/choice_option.py
+-rw-r--r--   0        0        0     3605 2024-05-25 17:25:23.183185 vbinsta-0.1.5/vbinsta/function_gpt.py
+-rw-r--r--   0        0        0     2725 2024-05-25 17:25:26.416875 vbinsta-0.1.5/vbinsta/functions.py
+-rw-r--r--   0        0        0      261 2024-05-23 08:10:25.061042 vbinsta-0.1.5/vbinsta/main.py
+-rw-r--r--   0        0        0     4178 2024-05-25 17:25:25.115487 vbinsta-0.1.5/vbinsta/token_cost_calculations.py
+-rw-r--r--   0        0        0     2302 2024-05-25 16:07:03.530032 vbinsta-0.1.5/vbinsta/upload.py
+-rw-r--r--   0        0        0      372 1970-01-01 00:00:00.000000 vbinsta-0.1.5/PKG-INFO
```

### Comparing `vbinsta-0.1.4/vbinsta/functions.py` & `vbinsta-0.1.5/vbinsta/functions.py`

 * *Files identical despite different names*

