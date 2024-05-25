# Comparing `tmp/class4-0.0.5.tar.gz` & `tmp/class4-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class4/dist/tmpkf69ywmv/class4-0.0.5.tar", last modified: Sat May 25 16:43:08 2024, max compression
+gzip compressed data, was "/mnt/farrukh90/python-class/evolvecyber/class4/dist/tmpa59ixhi5/class4-0.1.0.tar", last modified: Sat May 25 17:06:06 2024, max compression
```

## Comparing `class4-0.0.5.tar` & `class4-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:43:08.000000 class4-0.0.5/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)     1218 2024-05-25 16:42:51.000000 class4-0.0.5/setup.py
-drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/top_level.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      138 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/SOURCES.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/dependency_links.txt
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:43:08.000000 class4-0.0.5/class4.egg-info/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      353 2024-05-25 15:58:27.000000 class4-0.0.5/README.md
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      722 2024-05-25 16:43:08.000000 class4-0.0.5/PKG-INFO
--rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-25 16:43:08.000000 class4-0.0.5/setup.cfg
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 17:06:06.000000 class4-0.1.0/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      634 2024-05-25 17:05:46.000000 class4-0.1.0/setup.py
+drwxrwxr-x   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 17:06:06.000000 class4-0.1.0/class4.egg-info/
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 17:06:06.000000 class4-0.1.0/class4.egg-info/top_level.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      146 2024-05-25 17:06:06.000000 class4-0.1.0/class4.egg-info/SOURCES.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        1 2024-05-25 17:06:06.000000 class4-0.1.0/class4.egg-info/dependency_links.txt
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      817 2024-05-25 17:06:06.000000 class4-0.1.0/class4.egg-info/PKG-INFO
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      353 2024-05-25 16:52:02.000000 class4-0.1.0/README.md
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)        0 2024-05-25 17:02:19.000000 class4-0.1.0/LICENSE
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)      817 2024-05-25 17:06:06.000000 class4-0.1.0/PKG-INFO
+-rw-rw-r--   0 farrukh90  (1402) farrukh90  (1404)       38 2024-05-25 17:06:06.000000 class4-0.1.0/setup.cfg
```

