# Comparing `tmp/web-retriever-0.2.0.tar.gz` & `tmp/web-retriever-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-retriever-0.2.0.tar", last modified: Thu Oct 19 01:47:00 2023, max compression
+gzip compressed data, was "web-retriever-0.3.0.tar", last modified: Sat May 25 03:27:18 2024, max compression
```

## Comparing `web-retriever-0.2.0.tar` & `web-retriever-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 01:47:00.429408 web-retriever-0.2.0/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-05-15 19:32:34.000000 web-retriever-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7992 2023-10-19 01:47:00.429408 web-retriever-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7139 2023-10-19 01:19:15.000000 web-retriever-0.2.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      977 2023-10-16 17:26:18.000000 web-retriever-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       73 2023-10-19 01:47:00.429408 web-retriever-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2855 2023-10-16 17:26:18.000000 web-retriever-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 01:47:00.426075 web-retriever-0.2.0/web_retriever/
--rw-r--r--   0 root         (0) root         (0)     1526 2023-10-16 17:26:18.000000 web-retriever-0.2.0/web_retriever/conf.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-10-16 17:26:18.000000 web-retriever-0.2.0/web_retriever/scripts.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-10-19 01:39:41.000000 web-retriever-0.2.0/web_retriever/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 01:47:00.429408 web-retriever-0.2.0/web_retriever/web_retriever/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 01:47:00.429408 web-retriever-0.2.0/web_retriever/web_retriever/contracts/
--rw-r--r--   0 root         (0) root         (0)      161 2023-10-19 00:01:06.000000 web-retriever-0.2.0/web_retriever/web_retriever/contracts/fetch.py
--rw-r--r--   0 root         (0) root         (0)       76 2023-10-16 17:26:18.000000 web-retriever-0.2.0/web_retriever/web_retriever/contracts/throw.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-10-19 00:12:57.000000 web-retriever-0.2.0/web_retriever/web_retriever/fetch.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-10-19 00:01:38.000000 web-retriever-0.2.0/web_retriever/web_retriever/init.py
--rw-r--r--   0 root         (0) root         (0)     5524 2023-10-18 23:58:47.000000 web-retriever-0.2.0/web_retriever/web_retriever/ops.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-10-16 17:26:18.000000 web-retriever-0.2.0/web_retriever/web_retriever/rss.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-10-16 17:26:18.000000 web-retriever-0.2.0/web_retriever/web_retriever/throw.py
--rw-r--r--   0 root         (0) root         (0)     2391 2023-10-19 00:25:57.000000 web-retriever-0.2.0/web_retriever/web_retriever/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-19 01:47:00.429408 web-retriever-0.2.0/web_retriever.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7992 2023-10-19 01:47:00.000000 web-retriever-0.2.0/web_retriever.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      657 2023-10-19 01:47:00.000000 web-retriever-0.2.0/web_retriever.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-19 01:47:00.000000 web-retriever-0.2.0/web_retriever.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-10-19 01:47:00.000000 web-retriever-0.2.0/web_retriever.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-10-19 01:47:00.000000 web-retriever-0.2.0/web_retriever.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-10-19 01:47:00.000000 web-retriever-0.2.0/web_retriever.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-25 03:27:18.400245 web-retriever-0.3.0/
+-rw-rw-r--   0 root         (0) root         (0)    11345 2024-05-25 03:25:49.000000 web-retriever-0.3.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     8036 2024-05-25 03:27:18.400245 web-retriever-0.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7139 2024-05-25 03:25:49.000000 web-retriever-0.3.0/README.rst
+-rw-rw-r--   0 root         (0) root         (0)      977 2024-05-25 03:25:49.000000 web-retriever-0.3.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       73 2024-05-25 03:27:18.420249 web-retriever-0.3.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2855 2024-05-25 03:25:49.000000 web-retriever-0.3.0/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-25 03:27:18.400245 web-retriever-0.3.0/web_retriever/
+-rw-rw-r--   0 root         (0) root         (0)     1701 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/conf.py
+-rw-rw-r--   0 root         (0) root         (0)      184 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/scripts.py
+-rw-rw-r--   0 root         (0) root         (0)       18 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/version.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-25 03:27:18.400245 web-retriever-0.3.0/web_retriever/web_retriever/
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-25 03:27:18.400245 web-retriever-0.3.0/web_retriever/web_retriever/contracts/
+-rw-rw-r--   0 root         (0) root         (0)      161 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/contracts/fetch.py
+-rw-rw-r--   0 root         (0) root         (0)       76 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/contracts/throw.py
+-rw-rw-r--   0 root         (0) root         (0)     3865 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/fetch.py
+-rw-rw-r--   0 root         (0) root         (0)     2337 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/init.py
+-rw-rw-r--   0 root         (0) root         (0)     5524 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/ops.py
+-rw-rw-r--   0 root         (0) root         (0)     2332 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/rss.py
+-rw-rw-r--   0 root         (0) root         (0)     1648 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/throw.py
+-rw-rw-r--   0 root         (0) root         (0)     2391 2024-05-25 03:25:49.000000 web-retriever-0.3.0/web_retriever/web_retriever/web.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2024-05-25 03:27:18.400245 web-retriever-0.3.0/web_retriever.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     8036 2024-05-25 03:27:18.000000 web-retriever-0.3.0/web_retriever.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      657 2024-05-25 03:27:18.000000 web-retriever-0.3.0/web_retriever.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-05-25 03:27:18.000000 web-retriever-0.3.0/web_retriever.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       63 2024-05-25 03:27:18.000000 web-retriever-0.3.0/web_retriever.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)       81 2024-05-25 03:27:18.000000 web-retriever-0.3.0/web_retriever.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2024-05-25 03:27:18.000000 web-retriever-0.3.0/web_retriever.egg-info/top_level.txt
```

### Comparing `web-retriever-0.2.0/LICENSE` & `web-retriever-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/PKG-INFO` & `web-retriever-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: web-retriever
-Version: 0.2.0
-Home-page: 
+Version: 0.3.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: nicholasmhughes
 Author-email: nicholasmhughes@gmail.com
 License: Apache Software License 2.0
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -204,7 +206,9 @@
 proposed features (and known issues).
 
 ################
 Acknowledgements
 ################
 
 * `Img Shields <https://shields.io>`_ for making repository badges easy.
+
+
```

### Comparing `web-retriever-0.2.0/README.rst` & `web-retriever-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/pyproject.toml` & `web-retriever-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/setup.py` & `web-retriever-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/web_retriever/conf.py` & `web-retriever-0.3.0/web_retriever/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,26 +10,31 @@
         "default": None,
         "help": "Load extra options from a configuration file onto hub.OPT.web_retriever",
     },
     "rules": {
         "default": None,
         "help": "Rule engine rules to load onto hub.OPT.web_retriever.rules",
     },
+    "port": {
+        "default": 8080,
+        "help": "The port number to run web-retriever on",
+    },
 }
 
 # The selected subcommand for your cli tool will show up under hub.SUBPARSER
 # The value for a subcommand is a dictionary that will be passed as kwargs to argparse.ArgumentParser.add_subparsers
 SUBCOMMANDS: Dict[str, Dict[str, Any]] = {
     # "my_sub_command": {}
 }
 
 # Include keys from the CONFIG dictionary that you want to expose on the cli
 # The values for these keys are a dictionaries that will be passed as kwargs to argparse.ArgumentParser.add_option
 CLI_CONFIG: Dict[str, Dict[str, Any]] = {
     "config": {"options": ["-c"]},
+    "port": {"os": "WEB_RETRIEVER_PORT", "subcommands": ["_global_"]}
     # "my_option1": {"subcommands": ["A list of subcommands that exclusively extend this option"]},
     # This option will be available under all subcommands and the root command
     # "my_option2": {"subcommands": ["_global_"]},
 }
 
 # These are the namespaces that your project extends
 # The hub will extend these keys with the modules listed in the values
```

### Comparing `web-retriever-0.2.0/web_retriever/web_retriever/fetch.py` & `web-retriever-0.3.0/web_retriever/web_retriever/fetch.py`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/web_retriever/web_retriever/init.py` & `web-retriever-0.3.0/web_retriever/web_retriever/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,24 @@
     for header in hub.web_retriever.init.HEADERS:
         headers += f' "%{{{header}}}i"'
 
     # Add routes for each endpoint
     hub.web_retriever.fetch.add_routes()
     hub.web_retriever.throw.add_routes()
 
+    # Make sure port can be converted to an int
+    try:
+        port_number = int(hub.OPT.web_retriever.port)
+    except ValueError:
+        hub.log.error(
+            f"ERROR - Could not convert port '{hub.OPT.web_retriever.port}' to int, using default port 8080"
+        )
+        port_number = 8080
+
     # Start the async code
     coroutine = hub.server.web.run(
+        port=port_number,
         loop=loop,
         routes=hub.web_retriever.init.ROUTES,
         access_log_format='%a %t "%r" %s %b "%{Referer}i" "%{User-Agent}i"' + headers,
     )
     hub.pop.Loop.run_until_complete(coroutine)
```

### Comparing `web-retriever-0.2.0/web_retriever/web_retriever/ops.py` & `web-retriever-0.3.0/web_retriever/web_retriever/ops.py`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/web_retriever/web_retriever/rss.py` & `web-retriever-0.3.0/web_retriever/web_retriever/rss.py`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/web_retriever/web_retriever/throw.py` & `web-retriever-0.3.0/web_retriever/web_retriever/throw.py`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/web_retriever/web_retriever/web.py` & `web-retriever-0.3.0/web_retriever/web_retriever/web.py`

 * *Files identical despite different names*

### Comparing `web-retriever-0.2.0/web_retriever.egg-info/PKG-INFO` & `web-retriever-0.3.0/web_retriever.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: web-retriever
-Version: 0.2.0
-Home-page: 
+Version: 0.3.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
 Author: nicholasmhughes
 Author-email: nicholasmhughes@gmail.com
 License: Apache Software License 2.0
+Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -204,7 +206,9 @@
 proposed features (and known issues).
 
 ################
 Acknowledgements
 ################
 
 * `Img Shields <https://shields.io>`_ for making repository badges easy.
+
+
```

### Comparing `web-retriever-0.2.0/web_retriever.egg-info/SOURCES.txt` & `web-retriever-0.3.0/web_retriever.egg-info/SOURCES.txt`

 * *Files identical despite different names*

