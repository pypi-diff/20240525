# Comparing `tmp/pandalibs-0.1.3.tar.gz` & `tmp/pandalibs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandalibs-0.1.3.tar", last modified: Sun Apr  7 18:45:02 2024, max compression
+gzip compressed data, was "pandalibs-0.1.4.tar", last modified: Sat May 25 15:41:04 2024, max compression
```

## Comparing `pandalibs-0.1.3.tar` & `pandalibs-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 18:45:02.633301 pandalibs-0.1.3/
--rw-rw-rw-   0        0        0      111 2024-04-07 18:45:02.633301 pandalibs-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       91 2024-04-07 14:31:37.000000 pandalibs-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 18:45:02.629274 pandalibs-0.1.3/pandalibs/
--rw-rw-rw-   0        0        0        0 2024-04-07 14:00:56.000000 pandalibs-0.1.3/pandalibs/__init__.py
--rw-rw-rw-   0        0        0      151 2024-04-07 17:47:23.000000 pandalibs-0.1.3/pandalibs/pprint_nosort.py
--rw-rw-rw-   0        0        0     2274 2024-04-07 15:37:26.000000 pandalibs-0.1.3/pandalibs/yaml_importer.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:45:02.632298 pandalibs-0.1.3/pandalibs.egg-info/
--rw-rw-rw-   0        0        0      111 2024-04-07 18:45:02.000000 pandalibs-0.1.3/pandalibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-04-07 18:45:02.000000 pandalibs-0.1.3/pandalibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 18:45:02.000000 pandalibs-0.1.3/pandalibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-07 18:45:02.000000 pandalibs-0.1.3/pandalibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-07 18:45:02.000000 pandalibs-0.1.3/pandalibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 18:45:02.633301 pandalibs-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      382 2024-04-07 17:47:58.000000 pandalibs-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:41:04.410258 pandalibs-0.1.4/
+-rw-rw-rw-   0        0        0      111 2024-05-25 15:41:04.410258 pandalibs-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2024-04-07 14:31:37.000000 pandalibs-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 15:41:04.406261 pandalibs-0.1.4/pandalibs/
+-rw-rw-rw-   0        0        0        0 2024-04-07 14:00:56.000000 pandalibs-0.1.4/pandalibs/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-07 17:47:23.000000 pandalibs-0.1.4/pandalibs/pprint_nosort.py
+-rw-rw-rw-   0        0        0     2271 2024-05-25 15:38:48.000000 pandalibs-0.1.4/pandalibs/yaml_importer.py
+drwxrwxrwx   0        0        0        0 2024-05-25 15:41:04.410258 pandalibs-0.1.4/pandalibs.egg-info/
+-rw-rw-rw-   0        0        0      111 2024-05-25 15:41:04.000000 pandalibs-0.1.4/pandalibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-25 15:41:04.000000 pandalibs-0.1.4/pandalibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 15:41:04.000000 pandalibs-0.1.4/pandalibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-25 15:41:04.000000 pandalibs-0.1.4/pandalibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 15:41:04.000000 pandalibs-0.1.4/pandalibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 15:41:04.410258 pandalibs-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      602 2024-05-25 15:38:55.000000 pandalibs-0.1.4/setup.py
```

### Comparing `pandalibs-0.1.3/pandalibs/yaml_importer.py` & `pandalibs-0.1.4/pandalibs/yaml_importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
     if getattr(sys, "frozen", False):
         # Frozen executable, path manipulation
         path = os.path.dirname(sys.executable)
         return path if not go_up_one_level else os.path.dirname(path)
     else:
         # Regular script, path manipulation
-        path = os.path.dirname(os.path.abspath(sys.argv[0]))
+        path = os.path.dirname(os.path.abspath(__file__))
         return path if not go_up_one_level else os.path.dirname(path)
 
 
 # Get configuration data as a dictionary
 def get_configuration_data(up_a_level=False, file_name=DEFAULT_CONFIG_FILE, subfolder="config"):
     """Load and convert configuration file into appropriate data.
     Accepts optional filename and subfolder, as well as option to go up a level.
```

