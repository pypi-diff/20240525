# Comparing `tmp/pandalibs-0.1.3.tar.gz` & `tmp/pandalibs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandalibs-0.1.3.tar", last modified: Sun Apr  7 18:45:02 2024, max compression
+gzip compressed data, was "pandalibs-0.1.6.tar", last modified: Sat May 25 21:42:40 2024, max compression
```

## Comparing `pandalibs-0.1.3.tar` & `pandalibs-0.1.6.tar`

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
+drwxrwxrwx   0        0        0        0 2024-05-25 21:42:40.679463 pandalibs-0.1.6/
+-rw-rw-rw-   0        0        0      111 2024-05-25 21:42:40.679463 pandalibs-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2024-04-07 14:31:37.000000 pandalibs-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 21:42:40.675462 pandalibs-0.1.6/pandalibs/
+-rw-rw-rw-   0        0        0        0 2024-04-07 14:00:56.000000 pandalibs-0.1.6/pandalibs/__init__.py
+-rw-rw-rw-   0        0        0      151 2024-04-07 17:47:23.000000 pandalibs-0.1.6/pandalibs/pprint_nosort.py
+-rw-rw-rw-   0        0        0     2463 2024-05-25 21:27:30.000000 pandalibs-0.1.6/pandalibs/yaml_importer.py
+drwxrwxrwx   0        0        0        0 2024-05-25 21:42:40.678464 pandalibs-0.1.6/pandalibs.egg-info/
+-rw-rw-rw-   0        0        0      111 2024-05-25 21:42:40.000000 pandalibs-0.1.6/pandalibs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-25 21:42:40.000000 pandalibs-0.1.6/pandalibs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 21:42:40.000000 pandalibs-0.1.6/pandalibs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-25 21:42:40.000000 pandalibs-0.1.6/pandalibs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 21:42:40.000000 pandalibs-0.1.6/pandalibs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 21:42:40.679463 pandalibs-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-05-25 16:14:36.000000 pandalibs-0.1.6/setup.py
```

### Comparing `pandalibs-0.1.3/pandalibs/yaml_importer.py` & `pandalibs-0.1.6/pandalibs/yaml_importer.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,19 +36,23 @@
 # Get configuration data as a dictionary
 def get_configuration_data(up_a_level=False, file_name=DEFAULT_CONFIG_FILE, subfolder="config"):
     """Load and convert configuration file into appropriate data.
     Accepts optional filename and subfolder, as well as option to go up a level.
     Defaults to config.yaml within config subfolder.
     """
     try:
-        exe_dir = get_application_path(up_a_level)
-        if subfolder:
-            config_path = os.path.join(exe_dir, subfolder, file_name)
-        else:
-            config_path = os.path.join(exe_dir, file_name)
+        # Get the current working directory (which should be the executable's directory)
+        script_dir = os.getcwd()
+
+        # If you need to go up a level, adjust the path accordingly
+        if up_a_level:
+            script_dir = os.path.dirname(script_dir)
+
+        # Construct the complete path to the configuration file
+        config_path = os.path.join(script_dir, subfolder, file_name)
 
         if not os.path.exists(config_path):
             raise ConfigurationError(f"Configuration file '{file_name}' not found at '{config_path}'")
 
         with open(config_path, "r") as f:
             userinfo = yaml.safe_load(f)
```

