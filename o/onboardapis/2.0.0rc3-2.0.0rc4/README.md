# Comparing `tmp/onboardapis-2.0.0rc3.tar.gz` & `tmp/onboardapis-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onboardapis-2.0.0rc3.tar", last modified: Tue May 14 19:06:49 2024, max compression
+gzip compressed data, was "onboardapis-2.0.0rc4.tar", last modified: Sat May 25 12:00:41 2024, max compression
```

## Comparing `onboardapis-2.0.0rc3.tar` & `onboardapis-2.0.0rc4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.219254 onboardapis-2.0.0rc3/onboardapis/
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.219254 onboardapis-2.0.0rc3/onboardapis/bus/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/bus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.219254 onboardapis-2.0.0rc3/onboardapis/other/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/other/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/plane/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/ship/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/ship/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/at/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/at/obb/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/obb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/obb/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/at/obb/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/bth/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/bth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/db/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11454 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/db/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/flix/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/flix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/flix/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/flix/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/me/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/me/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/me/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/me/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/de/tdh/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/tdh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/de/tdh/apis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.223254 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/it/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/it/ti/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/ti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/ti/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/it/ti/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/icomera/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/onboardapis/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/onboardapis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 19:06:49.000000 onboardapis-2.0.0rc3/onboardapis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-14 19:06:44.000000 onboardapis-2.0.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:06:49.227254 onboardapis-2.0.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.976149 onboardapis-2.0.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.964149 onboardapis-2.0.0rc4/onboardapis/
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/bus/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/bus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/other/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/other/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/ship/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/ship/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/at/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/at/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/at/obb/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/at/obb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/at/obb/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/at/obb/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/de/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/de/bth/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/bth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/de/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/db/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/db/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/db/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/de/flix/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/flix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/flix/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/flix/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/de/me/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/me/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/me/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/me/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.968149 onboardapis-2.0.0rc4/onboardapis/train/de/tdh/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/tdh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/de/tdh/apis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis/train/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis/train/fr/sncf/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/fr/sncf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/fr/sncf/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/fr/sncf/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis/train/it/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/it/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis/train/it/ti/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/it/ti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/it/ti/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/it/ti/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis/train/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis/train/third_party/icomera/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/icomera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/icomera/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/icomera/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/onboardapis/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 12:00:41.972149 onboardapis-2.0.0rc4/onboardapis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-25 12:00:41.000000 onboardapis-2.0.0rc4/onboardapis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-25 12:00:41.000000 onboardapis-2.0.0rc4/onboardapis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 12:00:41.000000 onboardapis-2.0.0rc4/onboardapis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-25 12:00:41.000000 onboardapis-2.0.0rc4/onboardapis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-25 12:00:41.000000 onboardapis-2.0.0rc4/onboardapis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-25 12:00:35.000000 onboardapis-2.0.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 12:00:41.976149 onboardapis-2.0.0rc4/setup.cfg
```

### Comparing `onboardapis-2.0.0rc3/LICENSE` & `onboardapis-2.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/PKG-INFO` & `onboardapis-2.0.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardapis
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: A pure Python wrapper for the on-board APIs of many different transportation providers.
 Author-email: Felix Zenk <felix.zenk@web.de>
 License: MIT
 Project-URL: Homepage, https://felix-zenk.github.io/onboardapis
 Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/
 Project-URL: Repository, https://github.com/felix-zenk/onboardapis
 Project-URL: Issues, https://github.com/felix-zenk/onboardapis/issues
@@ -115,32 +115,30 @@
 > ```
 
 Every vehicle has an ``init``-method that needs to be called to initialize the connection to the API.
 When using a vehicle as a context manager the ``init``-method will automatically be called.
 
 ```python
 from onboardapis.train.de.db import ICEPortal
-from onboardapis.units import kilometers, kmh
-
+from onboardapis.units import kilometers, kilometers_per_hour
 
 # init is automatically called
 with ICEPortal() as train:
     print(
         f"Distance to {train.current_station.name}:",
         f"{kilometers(meters=train.calculate_distance(train.current_station)):.1f} km"
     )
 
-
 # init has to be explicitly called
 train = ICEPortal()
 train.init()  # Explicit call to init method to initialize API connection
 
 print(
     f"Travelling at {train.speed} m/s",
-    f"({kmh(ms=train.speed):.2f} km/h)",
+    f"({kilometers_per_hour(meters_per_second=train.speed):.2f} km/h)",
     f"with a delay of {train.delay.total_seconds():.0f} seconds"
 )
 ```
 
 And there you go!  
 You can read more information about available attributes in the ``onboardapis.train.Train`` and ``onboardapis.mixins`` documentation
 and the respective train's documentation.
```

### Comparing `onboardapis-2.0.0rc3/README.md` & `onboardapis-2.0.0rc4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,32 +73,30 @@
 > ```
 
 Every vehicle has an ``init``-method that needs to be called to initialize the connection to the API.
 When using a vehicle as a context manager the ``init``-method will automatically be called.
 
 ```python
 from onboardapis.train.de.db import ICEPortal
-from onboardapis.units import kilometers, kmh
-
+from onboardapis.units import kilometers, kilometers_per_hour
 
 # init is automatically called
 with ICEPortal() as train:
     print(
         f"Distance to {train.current_station.name}:",
         f"{kilometers(meters=train.calculate_distance(train.current_station)):.1f} km"
     )
 
-
 # init has to be explicitly called
 train = ICEPortal()
 train.init()  # Explicit call to init method to initialize API connection
 
 print(
     f"Travelling at {train.speed} m/s",
-    f"({kmh(ms=train.speed):.2f} km/h)",
+    f"({kilometers_per_hour(meters_per_second=train.speed):.2f} km/h)",
     f"with a delay of {train.delay.total_seconds():.0f} seconds"
 )
 ```
 
 And there you go!  
 You can read more information about available attributes in the ``onboardapis.train.Train`` and ``onboardapis.mixins`` documentation
 and the respective train's documentation.
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/__init__.py` & `onboardapis-2.0.0rc4/onboardapis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,14 @@
     "units",
     "Vehicle",
     "Station",
     "ConnectingVehicle",
 ]
 
 
-def _package_version() -> str:
-    from importlib.metadata import version
-    return version('onboardapis')
-
-
 class Vehicle(metaclass=ABCMeta):
     """
     Base class for all vehicles
     """
 
     _api: API
     """The :class:`API` that supplies the data for this vehicle."""
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/data.py` & `onboardapis-2.0.0rc4/onboardapis/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import logging
 import time
 
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from functools import wraps
 from json import JSONDecodeError
-from typing import TypeVar, Generic, ClassVar, Any
+from typing import TypeVar, Generic, ClassVar, Callable
 from threading import Thread
 
 from geopy.point import Point
 from geopy.distance import geodesic
 from gql import Client
 from gql.transport.requests import RequestsHTTPTransport
 from restfly import APISession
@@ -49,27 +49,24 @@
 
 ID = TypeVar("ID", str, int)
 """A TypeVar indicating the return type of Vehicle.id"""
 
 StationType = TypeVar("StationType", bound="Station")
 """A TypeVar indicating the Station type"""
 
-ApiType = TypeVar("ApiType", bound="API")
-"""A TypeVar indicating the API type"""
-
 
 def get_package_version() -> str:
     """Return the version of the ``onboardapis`` package."""
     try:
         return importlib.metadata.version('onboardapis')
     except importlib.metadata.PackageNotFoundError:
         return 'unknown'
 
 
-def default(arg: Any, default: Any = None, *, boolean: bool = True) -> Any:  # noqa: F402
+def default(arg: any, default: any = None, *, boolean: bool = True) -> any:  # noqa: F402
     """Return ``arg`` if it evaluates to ``True``, else return ``default``.
 
     Set ``boolean`` to ``False`` to only test for ``arg is None``.
 
     Args:
         arg: The data to test.
         default: The default value to return if no data is present.
@@ -101,16 +98,16 @@
         Args:
             scheduled: The value that should happen.
             actual: The value that actually happens, will be the same as the scheduled value if passed as None.
         """
         self.scheduled = scheduled
         self.actual = actual or scheduled
 
-    def __str__(self):
-        return str(self.scheduled) if self.actual is None else str(self.actual)
+    def __str__(self) -> str:
+        return str(default(self.actual, self.scheduled))
 
 
 @dataclass
 class Position(object):
     """
     A position requires at least a latitude and longitude,
     but can also provide data on altitude and the current compass heading.
@@ -121,27 +118,27 @@
     longitude: float
     """The longitude in decimal degrees"""
     altitude: float = None
     """The altitude in meters"""
     heading: float = None
     """The compass heading in degrees"""
 
-    def __str__(self):
+    def __str__(self) -> str:
         (lat_deg, lat_min, lat_sec), (lon_deg, lon_min, lon_sec,) = coordinates_decimal_to_dms(
             (self.latitude, self.longitude)
         )
         coordinates = (
             f"{abs(lat_deg)}°{lat_min}'{lat_sec:.3f}\"{'N' if lat_deg >= 0 else 'S'}"
             + f" {abs(lon_deg)}°{lon_min}'{lon_sec:.3f}\"{'E' if lon_deg >= 0 else 'W'}"
             + (f" {self.altitude:.2f}m" if self.altitude is not None else "")
             + (f" {self.heading:.2f}°" if self.heading is not None else "")
         )
         return coordinates
 
-    def __getitem__(self, item):
+    def __getitem__(self, item) -> float:
         return (self.latitude, self.longitude)[item]
 
     def calculate_distance(self, other: Position | Point) -> float:
         """
         Calculate the distance (in meters) between this position and another position.
 
         :param other: The other position
@@ -158,59 +155,61 @@
 
 class API(metaclass=ABCMeta):
     """A class for retrieving data from an API."""
 
     API_URL: ClassVar[str]
     """The base URL for the API."""
 
-    def __init__(self):
+    _data: dict[str, any]
+
+    def __init__(self) -> None:
         """Initialize a new ``API``."""
         self._data = dict()
 
-    def load(self, key: str, default: Any = None) -> Any:  # noqa: F402
+    def load(self, key: str, default: any = None) -> any:  # noqa: F402
         """Load data from the cache.
 
         Args:
             key: The key to load.
             default: The default value to return if the key is not present.
 
         Returns:
             The data if present, else the default.
         """
         return self._data.get(key, default)
 
-    def store(self, key: str, value: Any) -> None:
+    def store(self, key: str, value: any) -> None:
         """Store data in the cache.
 
         Args:
             key: The key the data should be stored under.
             value: The data to store.
         """
         self._data[key] = value
 
-    def __getitem__(self, item):
+    def __getitem__(self, item: str) -> any:
         return self._data[item]
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: any) -> None:
         self._data[key] = value
 
     def init(self) -> None:
         """Initialize the API connection."""
         pass
 
 
-def store(name=None):
+def store(name: str | Callable[..., T] = None) -> Callable[..., T]:
     """
     Decorator / decorator factory to apply to an ``API`` method
     to immediately store the return value of the decorated method
     as the key ``name`` or the method name if left out.
     """
-    def decorator(method):
+    def decorator(method: Callable[..., T]) -> Callable[..., T]:
         @wraps(method)
-        def wrapper(self, *args, **kwargs):
+        def wrapper(self: API, args: tuple[any, ...], kwargs: dict[str, any]) -> T:
             if isinstance(self, API):
                 self[name or method.__name__] = method(self, *args, **kwargs)
                 return self[name or method.__name__]
             return method(self, *args, **kwargs)
 
         return wrapper
 
@@ -267,70 +266,68 @@
 
             try:
                 self.refresh()
                 self._is_connected = True
             except (APIConnectionError, JSONDecodeError) as e:
                 if not self._is_connected:
                     raise InitialConnectionError from e
-                logger.error(f"{e}")
+                logger.exception(str(e))
                 continue
 
             counter = (tps - int(max(0.0, (target - time.time_ns()) / 1e9) * tps)) % tps
 
     def stop(self) -> None:
         """Stop requesting data and shut down the separate thread."""
         self._is_running = False
         if self.is_alive():
             self.join()
 
     def reset(self) -> None:
         """Reset the thread and the cache so that they can be reused with ``start()``."""
         self.stop()
-        Thread.__init__(self)
-        API.__init__(self)
-        self._is_connected = False
+        self.__init__()
 
     @abstractmethod
     def refresh(self) -> None:
         """Method that collects data from the server and stores it in the cache."""
         raise NotImplementedError
 
 
 class BlockingRestAPI(APISession, API):
     """A RESTful ``API`` that uses an ``restfly.session.APISession`` to fetch data."""
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs: any) -> None:
         """Initialize a new ``BlockingRestAPI``.
 
         Args:
             kwargs: The kwargs to pass to the underlying ``restfly.session.APISession``.
         """
         kwargs['url'] = kwargs.pop('url', self.API_URL)
         APISession.__init__(self, **kwargs)
         API.__init__(self)
 
-    def _build_session(self, **kwargs: Any) -> None:
+    def _build_session(self, **kwargs: any) -> None:
         APISession._build_session(self, **kwargs)
         self._session.headers.update({"User-Agent": "Python/onboardapis (%s)" % get_package_version()})
 
 
 class ThreadedRestAPI(ThreadedAPI, BlockingRestAPI, metaclass=ABCMeta):
     """A threaded version of the ``BlockingRestAPI``."""
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs: any) -> None:
         """Initialize a new ``ThreadedRestAPI``."""
         kwargs['url'] = kwargs.pop('url', self.API_URL)
-        APISession.__init__(self, **kwargs)
         ThreadedAPI.__init__(self)
+        BlockingRestAPI.__init__(self, **kwargs)
 
 
 class BlockingGraphQlAPI(Client, API):
     """A GraphQL ``API`` that uses a ``gql.client.Client`` to fetch data."""
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs: any) -> None:
         """Initialize a new ``BlockingGraphQlAPI``.
 
         Args:
             kwargs: The kwargs to pass to the underlying ``gql.client.Client``.
         """
         kwargs.update({
             'transport': kwargs.pop('transport', RequestsHTTPTransport(
@@ -342,18 +339,18 @@
             )),
             'fetch_schema_from_transport': kwargs.pop('fetch_schema_from_transport', True),
         })
         Client.__init__(self, **kwargs)
         API.__init__(self)
 
 
-class ThreadedGraphQlAPI(BlockingGraphQlAPI, ThreadedAPI, metaclass=ABCMeta):
+class ThreadedGraphQlAPI(ThreadedAPI, BlockingGraphQlAPI, metaclass=ABCMeta):
     """A threaded version of the ``BlockingGraphQlAPI``."""
 
-    def __init__(self, **kwargs: Any) -> None:
+    def __init__(self, **kwargs: any) -> None:
         """Initialize a new ``ThreadedGraphQlAPI``.
 
         Args:
             kwargs: The kwargs to pass to the underlying ``gql.client.Client``.
         """
-        BlockingGraphQlAPI.__init__(self, **kwargs)
         ThreadedAPI.__init__(self)
+        BlockingGraphQlAPI.__init__(self, **kwargs)
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/exceptions.py` & `onboardapis-2.0.0rc4/onboardapis/exceptions.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/mixins.py` & `onboardapis-2.0.0rc4/onboardapis/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,14 +134,22 @@
             The current delay of the vehicle as a `datetime.timedelta` object.
         """
         return timedelta(seconds=(
             self.current_station.arrival.actual - self.current_station.arrival.scheduled
         ).total_seconds())
 
     @property
+    def is_delayed(self) -> bool:
+        """Whether the train is delayed.
+
+        Convenience function that tests if `delay > timedelta(0)`.
+        """
+        return self.delay > timedelta()
+
+    @property
     def distance(self) -> float:
         """
         The distance from the start in meters
 
         :return: The distance
         :rtype: float
         """
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/protocols.py` & `onboardapis-2.0.0rc4/onboardapis/protocols.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/__init__.py` & `onboardapis-2.0.0rc4/onboardapis/train/__init__.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/at/obb/apis.py` & `onboardapis-2.0.0rc4/onboardapis/train/at/obb/apis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 
-from ....units import ms
+from ....units import meters_per_second
 from ....data import Position
 from ... import Train
 from .interfaces import RailnetRegioAPI
 
 logger = logging.getLogger(__name__)
 
 
@@ -19,15 +19,15 @@
 
     def __init__(self):
         self._api = RailnetRegioAPI()
         Train.__init__(self)
 
     @property
     def speed(self) -> float:
-        return ms(kmh=self._api['gps']['JSON']['speed'])
+        return meters_per_second(kilometers_per_hour=self._api['gps']['JSON']['speed'])
 
     @property
     def position(self) -> Position:
         return Position(
             latitude=self._api['gps']['JSON']['lat'],
             longitude=self._api['gps']['JSON']['lon'],
             # these are only present in newer trains
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/at/obb/interfaces.py` & `onboardapis-2.0.0rc4/onboardapis/train/at/obb/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import time
 
 from functools import lru_cache
 from typing import TypedDict
 
 from deprecation import deprecated
 
-from .... import _package_version
-from ....data import ThreadedRestAPI, store
+from ....data import ThreadedRestAPI, store, get_package_version
 
 logger = logging.getLogger(__name__)
 
 Endpoints = TypedDict("Endpoints", {
     'api/train_info': int,
     'api/gps': dict,
     'api/speed': float,
@@ -36,15 +35,15 @@
     @store('speed')
     def speed(self) -> float:
         return float(self.get("api/speed").text)
 
     @deprecated(
         deprecated_in='2.0.0',
         removed_in='2.1.0',
-        current_version=_package_version(),
+        current_version=get_package_version(),
         details='combined has been removed from the API by ÖBB'
     )
     @store('combined')
     def combined(self) -> dict:
         return self.get("assets/modules/fis/combined.json", params={"_time": time.time()}).json()
 
     def refresh(self) -> None:
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/de/db/apis.py` & `onboardapis-2.0.0rc4/onboardapis/train/de/db/apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 import re
 
 from typing import Literal
 from datetime import datetime, timedelta
 
 from deprecation import deprecated
 
-from .... import _package_version
 from ....exceptions import DataInvalidError
-from ....data import ID, default, ScheduledEvent, Position
+from ....data import ID, default, ScheduledEvent, Position, get_package_version
 from ....mixins import SpeedMixin, PositionMixin, StationsMixin, InternetAccessMixin
-from ....units import ms
+from ....units import meters_per_second
 from ... import Train, TrainStation
 from .mappings import id_name_map
-from .interfaces import ICEPortalAPI, RegioGuideAPI, ICEPortalInternetInterface
+from .interfaces import ICEPortalAPI, RegioGuideAPI, ICEPortalInternetInterface, ICEPortalInternetAccessAPI
 
 logger = logging.getLogger(__name__)
 
 InternetStatus = Literal["NO_INFO", "NO_INTERNET", "UNSTABLE", "WEAK", "MIDDLE", "HIGH"]
 
 
 class ICEPortal(Train, SpeedMixin, PositionMixin, StationsMixin[TrainStation], InternetAccessMixin):
     """Wrapper for interacting with the DB ICE Portal API."""
 
     _api: ICEPortalAPI
     _internet_access: ICEPortalInternetInterface
 
     def __init__(self):
         self._api = ICEPortalAPI()
-        self._internet_access = ICEPortalInternetInterface(self._api)
+        self._internet_access = ICEPortalInternetInterface(ICEPortalInternetAccessAPI())
         Train.__init__(self)
 
     def now(self) -> datetime:
         return datetime.fromtimestamp(int(default(
             self._api["status"].get("serverTime", None), 0,
         )) / 1000)
 
@@ -116,15 +115,15 @@
         try:
             return self.stations_dict[station_id]
         except KeyError as e:
             raise DataInvalidError("No current station found") from e
 
     @property
     def speed(self) -> float:
-        return ms(kmh=self._api["status"].get("speed", 0))
+        return meters_per_second(kilometers_per_hour=self._api["status"].get("speed", 0))
 
     @property
     def distance(self) -> float:
         return (
             self._api["trip"].get("trip", {}).get("actualPosition", 0)
             + self._api["trip"].get("trip", {}).get("distanceFromLastStop", 0)
         )
@@ -205,15 +204,15 @@
 
         :return: The wagon class
         :rtype: Literal["FIRST", "SECOND"]
         """
         return default(self._api["status"].get("wagonClass"))
 
     @property
-    def current_internet_status(self) -> InternetStatus:
+    def internet_status(self) -> InternetStatus:
         """Returns the current internet connection status of the train."""
         return default(
             self._api["status"]
             .get("connectivity", {})
             .get("currentState"),
             "NO_INFO",
         )
@@ -226,15 +225,15 @@
             .get("connectivity", {})
             .get("nextState"),
             "NO_INFO",
         )
 
     @property
     def internet_status_change(self) -> timedelta | None:
-        """Returns the timedelta until ``internet_status`` changes to ``next_internet_status``."""
+        """Returns the time until ``internet_status`` changes to ``next_internet_status``."""
         remaining_seconds = (
             self._api["status"]
             .get("connectivity", {})
             .get("remainingTimeSeconds", "")
         )
         return None if default(remaining_seconds) is None else timedelta(seconds=int(remaining_seconds))
 
@@ -296,12 +295,12 @@
         ), None)
         return self.destination if station is None else station
 
 
 @deprecated(
     deprecated_in='2.0.0rc3',
     removed_in='2.0.0',
-    current_version=_package_version(),
+    current_version=get_package_version(),
     details='Renamed by DB. Use RegioGuide instead.'
 )
 class ZugPortal(RegioGuide):
     """Renamed by DB. Use RegioGuide instead."""
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/de/db/interfaces.py` & `onboardapis-2.0.0rc4/onboardapis/train/de/db/interfaces.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,45 +8,46 @@
 from http import HTTPStatus
 from typing import Generator
 
 from bs4 import BeautifulSoup
 from geopy import Point
 from geopy.distance import distance
 
+from ...third_party.icomera import GenericIcomeraInternetAccessInterface
 from ....data import (
     ID,
     ThreadedRestAPI,
     ScheduledEvent,
     default,
     store,
     BlockingRestAPI,
 )
-from ....mixins import InternetAccessInterface, InternetMetricsInterface
+from ....mixins import InternetMetricsInterface
 from ... import ConnectingTrain
 
 logger = logging.getLogger(__name__)
 
 
 class ICEPortalAPI(ThreadedRestAPI):
     API_URL = "https://iceportal.de"
 
     @store('bap')
     @lru_cache
-    def bap_service_status(self):
+    def bap_service_status(self) -> dict[str, any]:
         return self.get("bap/api/bap-service-status").json()
 
     @store('trip')
-    def trip_info(self):
+    def trip_info(self) -> dict[str, any]:
         return self.get("api1/rs/tripInfo/trip").json()
 
     @store('status')
-    def status(self):
+    def status(self) -> dict[str, any]:
         return self.get("api1/rs/status").json()
 
-    def refresh(self):
+    def refresh(self) -> None:
         self.status()
         self.trip_info()
         self.bap_service_status()
 
     def get_connections(
         self, station_id: str
     ) -> Generator[ConnectingTrain, None, None]:
@@ -95,72 +96,75 @@
             return
 
         self[f"connections_{station_id}"] = connections
         yield from connections
         return
 
 
-class ICEPortalInternetInterface(InternetAccessInterface, InternetMetricsInterface):
-    _api: ICEPortalAPI
+class ICEPortalInternetAccessAPI(BlockingRestAPI):
+    API_URL = 'https://login.wifionice.de'
 
-    def enable(self):
+
+class ICEPortalInternetInterface(GenericIcomeraInternetAccessInterface, InternetMetricsInterface):
+    _api: ICEPortalInternetAccessAPI
+
+    def enable(self) -> None:  # TODO needed?
         """WIP: DOES NOT WORK YET!"""
         response = self._api.get('de')
         soup = BeautifulSoup(response.text, 'html.parser')
 
         # Check if the user is already online
         if soup.find(id='accept') is None:
             return
 
         # User is offline
-        logger.info('Cookie: %s', response.cookies['csrf'])
-        response = self._api.post('de', json={
-            'CSRFToken': response.cookies['csrf'],
+        response = self._api.post('de/', json={
             'login': True,
+            'CSRFToken': response.cookies['csrf'],
         })
         response.raise_for_status()
 
         # Check if login was successful
         if not (response.is_redirect and response.url.startswith(ICEPortalAPI.API_URL)):
             raise ConnectionError('Login failed!')
 
-    def disable(self):
+    def disable(self):  # TODO needed?
         """WIP: DOES NOT WORK YET!"""
         response = self._api.get('de')
         soup = BeautifulSoup(response.text, 'html.parser')
 
         # Check if user is already offline
         if soup.find(id='accept') is not None:
             return
 
         # User is online
-        response = self._api.post('de', json={
-            'CSRFToken': response.cookies['csrf'],
+        response = self._api.post('de/', json={
             'logout': True,
+            'CSRFToken': response.cookies['csrf'],
         })
         response.raise_for_status()
 
         # Check if logout was successful
         if BeautifulSoup(response.text, 'html.parser').find(id='accept', recursive=True) is None:
             raise ConnectionError('Logout failed!')
 
     @property
-    def is_enabled(self) -> bool:
+    def is_enabled(self) -> bool:  # TODO needed?
         return BeautifulSoup(
             self._api.get('de').text, 'html.parser'
         ).find(id='accept') is None
 
     def limit(self) -> float | None:
         usage_info = self._api.get('usage_info')
         if usage_info.status_code == HTTPStatus.NOT_IMPLEMENTED:
             return None
         return usage_info.json()['limit']  # TODO min api version = 14?
 
 
-class ModeOfTransport(Enum):
+class ModeOfTransport(str, Enum):
     UNKNOWN = 'UNKNOWN'
     BUS = 'BUS'
     TRAM = 'TRAM'
     SUBWAY = 'SUBWAY'
     CITY_TRAIN = 'CITY_TRAIN'
     REGIONAL_TRAIN = 'REGIONAL_TRAIN'
     INTER_REGIONAL_TRAIN = 'INTER_REGIONAL_TRAIN'
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/de/db/mappings.py` & `onboardapis-2.0.0rc4/onboardapis/train/de/db/mappings.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/de/flix/apis.py` & `onboardapis-2.0.0rc4/onboardapis/train/de/flix/apis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import logging
 
-from ....units import ms
+from ....units import meters_per_second
 from ....data import Position
 from ....mixins import PositionMixin, SpeedMixin
 from ... import Train
 from .interfaces import FlixTainmentAPI
 
 logger = logging.getLogger(__name__)
 
@@ -26,12 +26,12 @@
         return Position(
             latitude=self._api["position"].get("latitude", None),
             longitude=self._api["position"].get("longitude", None),
         )
 
     @property
     def speed(self) -> float:
-        return ms(kmh=float(self._api["position"].get("speed", 0.0)))
+        return meters_per_second(kilometers_per_hour=float(self._api["position"].get("speed", 0.0)))
 
     @property
     def type(self) -> str:
         return 'FLX'
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/de/me/apis.py` & `onboardapis-2.0.0rc4/onboardapis/train/de/me/apis.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 from ...third_party.icomera import GenericIcomeraTrain
 from ....mixins import InternetAccessMixin
 from .interfaces import MetronomAPI, MetronomInternetAccessInterface
 
 logger = logging.getLogger(__name__)
 
 
-class MetronomCaptivePortal(GenericIcomeraTrain, InternetAccessMixin):
+class MetronomCaptivePortal(GenericIcomeraTrain):
     _api: MetronomAPI
     _internet_access: MetronomInternetAccessInterface
 
     def __init__(self) -> None:
         self._api = MetronomAPI()
-        self._internet_access = MetronomInternetAccessInterface()
+        self._internet_access = MetronomInternetAccessInterface(self._api)
         GenericIcomeraTrain.__init__(self)
-        InternetAccessMixin.__init__(self)
 
     @property
     def type(self) -> str:
         return 'ME'
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/de/me/interfaces.py` & `onboardapis-2.0.0rc4/onboardapis/train/third_party/icomera/interfaces.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 from __future__ import annotations
 
 import logging
 
+from abc import ABCMeta
+
 from bs4 import BeautifulSoup
 
-from ....exceptions import APIConnectionError
 from ....data import BlockingRestAPI
+from ....exceptions import APIConnectionError
 from ....mixins import InternetAccessInterface
 
 logger = logging.getLogger(__name__)
 
 
-class MetronomAPI(BlockingRestAPI):
+class GenericIcomeraAPI(BlockingRestAPI, metaclass=ABCMeta):
     # noinspection HttpUrlsUsage
-    API_URL = 'http://wifi.metronom.de'
+    API_URL = 'http://omboard.info'
 
 
-class MetronomInternetAccessInterface(BlockingRestAPI, InternetAccessInterface):
-    # noinspection HttpUrlsUsage
-    API_URL = 'http://wifi.metronom.de'
+class GenericIcomeraInternetAccessInterface(InternetAccessInterface):
+    _api: BlockingRestAPI
 
-    def enable(self):
-        response = self.get('de')
-        soup = BeautifulSoup(response.text, 'html.parser')
-        if soup.find(class_='user-offline') is None:
+    def __init__(self, api: BlockingRestAPI) -> None:
+        InternetAccessInterface.__init__(self, api)
+
+    def enable(self) -> None:
+        response = self._api.get('de')
+        if BeautifulSoup(response.text, 'html.parser').find(class_='user-offline') is None:
             return  # Already online
 
-        # csrf_token = soup.find('input', {'name': 'CSRFToken'})['value']
-        csrf_token = response.cookies['csrf']
-        response = self.post('de', data={
+        response = self._api.post('de/', data={
             'login': True,
-            'CSRFToken': csrf_token,
+            'CSRFToken': response.cookies['csrf'],
         })
         response.raise_for_status()
         if BeautifulSoup(response.text, 'html.parser').find(class_='user-online') is None:
             raise APIConnectionError('Login failed!')
 
-    def disable(self):
-        response = self.get('de')
-        soup = BeautifulSoup(response.text, 'html.parser')
-        if soup.find(class_='user-online') is None:
+    def disable(self) -> None:
+        response = self._api.get('de')
+        if BeautifulSoup(response.text, 'html.parser').find(class_='user-online') is None:
             return  # Already offline
 
-        # csrf_token = soup.find('input', {'name': 'CSRFToken'})['value']
-        csrf_token = response.cookies['csrf']
-        response = self.post('de', data={
+        response = self._api.post('de/', data={
             'logout': True,
-            'CSRFToken': csrf_token,
+            'CSRFToken': response.cookies['csrf'],
         })
         response.raise_for_status()
         if BeautifulSoup(response.text, 'html.parser').find(class_='user-offline') is None:
             raise APIConnectionError('Logout failed!')
 
     @property
     def is_enabled(self) -> bool:
         return BeautifulSoup(
-            self.get('de').text, 'html.parser'
-        ).find(class_='user-offline') is None
+            self._api.get('de').text, 'html.parser'
+        ).find(class_='user-online') is not None
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/apis.py` & `onboardapis-2.0.0rc4/onboardapis/train/fr/sncf/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/fr/sncf/interfaces.py` & `onboardapis-2.0.0rc4/onboardapis/train/fr/sncf/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/it/ti/apis.py` & `onboardapis-2.0.0rc4/onboardapis/train/it/ti/apis.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 from datetime import datetime, timedelta
 
 from ....data import ID
 from ....exceptions import DataInvalidError
-from ....units import ms
+from ....units import meters_per_second
 from ... import Train, TrainStation
 from .interfaces import PortaleRegionaleConnector
 
 logger = logging.getLogger(__name__)
 
 
 class PortaleRegionale(Train):
@@ -42,15 +42,15 @@
     def delay(self) -> timedelta:
         delay_minutes = self._api['infovaggio']['infos'].get('delay', '')
         return timedelta() if delay_minutes in ('0', '') else timedelta(minutes=int(delay_minutes))
 
     @property
     def speed(self) -> float:
         if self._api['infovaggio'].get('isGpsValid', 'false').lower() == 'true':
-            return ms(kmh=(float(self._api['infovaggio']['infos']['speed'])))
+            return meters_per_second(kilometers_per_hour=(float(self._api['infovaggio']['infos']['speed'])))
         raise DataInvalidError('GPS data invalid.')
 
     @property
     def stations_dict(self) -> dict[ID, TrainStation]:
         first = self._api['infovaggio']['infos']['stazionePartenza']
         current = self._api['infovaggio']['nextStation']
         last = self._api['infovaggio']['infos']['stazioneArrivo']
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/it/ti/interfaces.py` & `onboardapis-2.0.0rc4/onboardapis/train/it/ti/interfaces.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/apis.py` & `onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/apis.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/interfaces.py` & `onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import json
 import logging
-import requests
 
 from typing import ClassVar
 from urllib.parse import parse_qs, urlparse
 
+import requests
+
 from gql import gql
+from requests.exceptions import ConnectionError
 
 from ....exceptions import InitialConnectionError
 from ....data import ThreadedGraphQlAPI, get_package_version
 from ....mixins import InternetAccessInterface
 
 logger = logging.getLogger(__name__)
```

### Comparing `onboardapis-2.0.0rc3/onboardapis/train/third_party/unwired/mixins.py` & `onboardapis-2.0.0rc4/onboardapis/train/third_party/unwired/mixins.py`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/onboardapis/units.py` & `onboardapis-2.0.0rc4/onboardapis/units.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     'ft',
     'nm',
     'seconds',
     'minutes',
     'hours',
     'coordinates_decimal_to_dms',
     'coordinates_dms_to_decimal',
-    'kmh',
-    'ms',
+    'kilometers_per_hour',
+    'kilometers_per_hour',
+    'meters_per_second',
+    'meters_per_second',
 ]
 
 
 def coordinates_decimal_to_dms(
         coordinates: tuple[float, float]
 ) -> tuple[tuple[int, int, float], tuple[int, int, float]]:
     """
@@ -41,18 +43,17 @@
     lat, lon = coordinates
     lat_deg = int(abs(lat))
     lat_min = int((abs(lat) - lat_deg) * 60)
     lat_sec = ((abs(lat) - lat_deg) * 60 - lat_min) * 60
     lon_deg = int(abs(lon))
     lon_min = int((abs(lon) - lon_deg) * 60)
     lon_sec = ((abs(lon) - lon_deg) * 60 - lon_min) * 60
-    return (-lat_deg if lat < 0 else lat_deg, lat_min, lat_sec), (
-        -lon_deg if lon < 0 else lon_deg,
-        lon_min,
-        lon_sec,
+    return (
+        (-lat_deg if lat < 0 else lat_deg, lat_min, lat_sec),
+        (-lon_deg if lon < 0 else lon_deg, lon_min, lon_sec)
     )
 
 
 def coordinates_dms_to_decimal(
         coordinates: tuple[tuple[int, int, float], tuple[int, int, float]]
 ) -> tuple[float, float]:
     """
@@ -65,17 +66,14 @@
     """
     (lat_deg, lat_min, lat_sec), (lon_deg, lon_min, lon_sec) = coordinates
     lat = lat_deg + lat_min / 60 + lat_sec / 3600
     lon = lon_deg + lon_min / 60 + lon_sec / 3600
     return lat, lon
 
 
-# Convert between different units
-
-
 def seconds(hours: float = 0, minutes: float = 0) -> float:  # noqa: F402
     """Convert to seconds"""
     ret = 0
     if hours:
         ret += hours * 3600
     if minutes:
         ret += minutes * 60
@@ -98,21 +96,25 @@
     if minutes:
         ret += minutes / 60
     if seconds:
         ret += seconds / 3600
     return ret
 
 
-def kmh(ms: float = None) -> float:  # noqa: F402
+def kilometers_per_hour(meters_per_second: float = None) -> float:  # noqa: F402
     """Convert to kilometers per hour"""
     ret = 0
-    if ms:
-        ret += kilometers(meters=ms) / hours(seconds=1)
+    if meters_per_second:
+        ret += kilometers(meters=meters_per_second) / hours(seconds=1)
     return ret
 
 
-def ms(kmh: float = None) -> float:  # noqa: F402
+def meters_per_second(kilometers_per_hour: float = None) -> float:  # noqa: F402
     """Convert to meters per second"""
     ret = 0
-    if kmh:
-        ret += meters(kilometers=kmh) / seconds(hours=1)
+    if kilometers_per_hour:
+        ret += meters(kilometers=kilometers_per_hour) / seconds(hours=1)
     return ret
+
+
+kmh = kilometers_per_hour
+ms = meters_per_second
```

### Comparing `onboardapis-2.0.0rc3/onboardapis.egg-info/PKG-INFO` & `onboardapis-2.0.0rc4/onboardapis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onboardapis
-Version: 2.0.0rc3
+Version: 2.0.0rc4
 Summary: A pure Python wrapper for the on-board APIs of many different transportation providers.
 Author-email: Felix Zenk <felix.zenk@web.de>
 License: MIT
 Project-URL: Homepage, https://felix-zenk.github.io/onboardapis
 Project-URL: Documentation, https://felix-zenk.github.io/onboardapis/
 Project-URL: Repository, https://github.com/felix-zenk/onboardapis
 Project-URL: Issues, https://github.com/felix-zenk/onboardapis/issues
@@ -115,32 +115,30 @@
 > ```
 
 Every vehicle has an ``init``-method that needs to be called to initialize the connection to the API.
 When using a vehicle as a context manager the ``init``-method will automatically be called.
 
 ```python
 from onboardapis.train.de.db import ICEPortal
-from onboardapis.units import kilometers, kmh
-
+from onboardapis.units import kilometers, kilometers_per_hour
 
 # init is automatically called
 with ICEPortal() as train:
     print(
         f"Distance to {train.current_station.name}:",
         f"{kilometers(meters=train.calculate_distance(train.current_station)):.1f} km"
     )
 
-
 # init has to be explicitly called
 train = ICEPortal()
 train.init()  # Explicit call to init method to initialize API connection
 
 print(
     f"Travelling at {train.speed} m/s",
-    f"({kmh(ms=train.speed):.2f} km/h)",
+    f"({kilometers_per_hour(meters_per_second=train.speed):.2f} km/h)",
     f"with a delay of {train.delay.total_seconds():.0f} seconds"
 )
 ```
 
 And there you go!  
 You can read more information about available attributes in the ``onboardapis.train.Train`` and ``onboardapis.mixins`` documentation
 and the respective train's documentation.
```

### Comparing `onboardapis-2.0.0rc3/onboardapis.egg-info/SOURCES.txt` & `onboardapis-2.0.0rc4/onboardapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onboardapis-2.0.0rc3/pyproject.toml` & `onboardapis-2.0.0rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onboardapis"
 description = "A pure Python wrapper for the on-board APIs of many different transportation providers."
-version = "2.0.0rc3"
+version = "2.0.0rc4"
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 keywords = [
     "public-transport",
     "train",
     "api",
 ]
```

