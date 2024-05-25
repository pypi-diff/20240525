# Comparing `tmp/openai_commands-3.8.1.tar.gz` & `tmp/openai_commands-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_commands-3.8.1.tar", last modified: Sat May 25 01:11:56 2024, max compression
+gzip compressed data, was "openai_commands-3.9.1.tar", last modified: Sat May 25 01:51:37 2024, max compression
```

## Comparing `openai_commands-3.8.1.tar` & `openai_commands-3.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:11:56.603003 openai_commands-3.8.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-24 02:29:00.000000 openai_commands-3.8.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:29:00.000000 openai_commands-3.8.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     8444 2024-05-25 01:11:56.601671 openai_commands-3.8.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     6727 2024-05-24 02:53:20.000000 openai_commands-3.8.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:11:56.596336 openai_commands-3.8.1/openai_commands/
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-25 01:11:48.000000 openai_commands-3.8.1/openai_commands/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     1249 2024-05-24 02:38:45.000000 openai_commands-3.8.1/openai_commands/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      481 2024-05-24 02:50:14.000000 openai_commands-3.8.1/openai_commands/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-24 02:38:46.000000 openai_commands-3.8.1/openai_commands/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-24 02:29:00.000000 openai_commands-3.8.1/openai_commands/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:11:56.600249 openai_commands-3.8.1/openai_commands.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     8444 2024-05-25 01:11:56.000000 openai_commands-3.8.1/openai_commands.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      393 2024-05-25 01:11:56.000000 openai_commands-3.8.1/openai_commands.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:11:56.000000 openai_commands-3.8.1/openai_commands.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-25 01:11:56.000000 openai_commands-3.8.1/openai_commands.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       16 2024-05-25 01:11:56.000000 openai_commands-3.8.1/openai_commands.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:29:00.000000 openai_commands-3.8.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-05-24 02:29:00.000000 openai_commands-3.8.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:11:56.603281 openai_commands-3.8.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-24 02:30:24.000000 openai_commands-3.8.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:51:37.367912 openai_commands-3.9.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2024-05-24 02:29:00.000000 openai_commands-3.9.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-24 02:29:00.000000 openai_commands-3.9.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     8444 2024-05-25 01:51:37.366661 openai_commands-3.9.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     6727 2024-05-24 02:53:20.000000 openai_commands-3.9.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:51:37.360692 openai_commands-3.9.1/openai_commands/
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-25 01:51:29.000000 openai_commands-3.9.1/openai_commands/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     1249 2024-05-24 02:38:45.000000 openai_commands-3.9.1/openai_commands/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      481 2024-05-24 02:50:14.000000 openai_commands-3.9.1/openai_commands/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       96 2024-05-24 02:38:46.000000 openai_commands-3.9.1/openai_commands/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2024-05-24 02:29:00.000000 openai_commands-3.9.1/openai_commands/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-25 01:51:37.365479 openai_commands-3.9.1/openai_commands.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     8444 2024-05-25 01:51:37.000000 openai_commands-3.9.1/openai_commands.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      393 2024-05-25 01:51:37.000000 openai_commands-3.9.1/openai_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-25 01:51:37.000000 openai_commands-3.9.1/openai_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      204 2024-05-25 01:51:37.000000 openai_commands-3.9.1/openai_commands.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       16 2024-05-25 01:51:37.000000 openai_commands-3.9.1/openai_commands.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-24 02:29:00.000000 openai_commands-3.9.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      264 2024-05-24 02:29:00.000000 openai_commands-3.9.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-25 01:51:37.368153 openai_commands-3.9.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      239 2024-05-24 02:30:24.000000 openai_commands-3.9.1/setup.py
```

### Comparing `openai_commands-3.8.1/LICENSE` & `openai_commands-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_commands-3.8.1/PKG-INFO` & `openai_commands-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_commands
-Version: 3.8.1
+Version: 3.9.1
 Summary: 🛠️ a command interface to the OpenAI API
 Home-page: https://github.com/kamangir/openai-commands
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `openai_commands-3.8.1/README.md` & `openai_commands-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_commands-3.8.1/openai_commands/__main__.py` & `openai_commands-3.9.1/openai_commands/__main__.py`

 * *Files identical despite different names*

### Comparing `openai_commands-3.8.1/openai_commands.egg-info/PKG-INFO` & `openai_commands-3.9.1/openai_commands.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_commands
-Version: 3.8.1
+Version: 3.9.1
 Summary: 🛠️ a command interface to the OpenAI API
 Home-page: https://github.com/kamangir/openai-commands
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

