# Comparing `tmp/ovos-tts-plugin-server-0.0.2a8.tar.gz` & `tmp/ovos-tts-plugin-server-0.0.2a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-plugin-server-0.0.2a8.tar", last modified: Sun Dec 31 05:36:13 2023, max compression
+gzip compressed data, was "ovos-tts-plugin-server-0.0.2a9.tar", last modified: Sun Dec 31 16:30:57 2023, max compression
```

## Comparing `ovos-tts-plugin-server-0.0.2a8.tar` & `ovos-tts-plugin-server-0.0.2a9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 05:36:13.651141 ovos-tts-plugin-server-0.0.2a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-12-31 05:36:13.651141 ovos-tts-plugin-server-0.0.2a8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 05:36:13.651141 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2023-12-31 05:36:09.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-31 05:36:09.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 05:36:13.651141 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2023-12-31 05:36:13.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-12-31 05:36:13.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 05:36:13.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-31 05:36:13.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-31 05:36:13.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-31 05:36:13.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 05:36:13.000000 ovos-tts-plugin-server-0.0.2a8/ovos_tts_plugin_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-31 05:36:13.651141 ovos-tts-plugin-server-0.0.2a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3279 2023-12-31 05:36:09.000000 ovos-tts-plugin-server-0.0.2a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 16:30:57.895913 ovos-tts-plugin-server-0.0.2a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-31 16:30:57.895913 ovos-tts-plugin-server-0.0.2a9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 16:30:57.891913 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2634 2023-12-31 16:30:50.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-31 16:30:50.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 16:30:57.895913 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-31 16:30:57.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2023-12-31 16:30:57.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 16:30:57.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-31 16:30:57.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-31 16:30:57.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-31 16:30:57.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 16:30:57.000000 ovos-tts-plugin-server-0.0.2a9/ovos_tts_plugin_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-31 16:30:57.895913 ovos-tts-plugin-server-0.0.2a9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3279 2023-12-31 16:30:50.000000 ovos-tts-plugin-server-0.0.2a9/setup.py
```

### Comparing `ovos-tts-plugin-server-0.0.2a8/setup.py` & `ovos-tts-plugin-server-0.0.2a9/setup.py`

 * *Files identical despite different names*

