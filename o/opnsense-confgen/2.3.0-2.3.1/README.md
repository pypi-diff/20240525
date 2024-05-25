# Comparing `tmp/opnsense-confgen-2.3.0.tar.gz` & `tmp/opnsense_confgen-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opnsense-confgen-2.3.0.tar", last modified: Mon Oct 10 23:46:28 2022, max compression
+gzip compressed data, was "opnsense_confgen-2.3.1.tar", last modified: Sat May 25 18:42:00 2024, max compression
```

## Comparing `opnsense-confgen-2.3.0.tar` & `opnsense_confgen-2.3.1.tar`

### file list

```diff
@@ -1,31 +1,37 @@
-drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2022-10-10 23:46:28.398807 opnsense-confgen-2.3.0/
--rw-r--r--   0 utkonos    (502) staff       (20)     1072 2022-05-15 00:44:45.000000 opnsense-confgen-2.3.0/LICENSE.txt
--rw-r--r--   0 utkonos    (502) staff       (20)     8731 2022-10-10 23:46:28.399097 opnsense-confgen-2.3.0/PKG-INFO
--rw-r--r--   0 utkonos    (502) staff       (20)     7607 2022-10-10 23:16:04.000000 opnsense-confgen-2.3.0/README.md
--rw-r--r--   0 utkonos    (502) staff       (20)       87 2022-10-09 04:58:21.000000 opnsense-confgen-2.3.0/pyproject.toml
--rw-r--r--   0 utkonos    (502) staff       (20)     1428 2022-10-10 23:46:28.400233 opnsense-confgen-2.3.0/setup.cfg
-drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2022-10-10 23:46:28.388642 opnsense-confgen-2.3.0/src/
-drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2022-10-10 23:46:28.392077 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/
--rw-r--r--   0 utkonos    (502) staff       (20)     8731 2022-10-10 23:46:28.000000 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/PKG-INFO
--rw-r--r--   0 utkonos    (502) staff       (20)      716 2022-10-10 23:46:28.000000 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/SOURCES.txt
--rw-r--r--   0 utkonos    (502) staff       (20)        1 2022-10-10 23:46:28.000000 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/dependency_links.txt
--rw-r--r--   0 utkonos    (502) staff       (20)       39 2022-10-10 23:46:28.000000 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/entry_points.txt
--rw-r--r--   0 utkonos    (502) staff       (20)       15 2022-10-10 23:46:28.000000 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/requires.txt
--rw-r--r--   0 utkonos    (502) staff       (20)        5 2022-10-10 23:46:28.000000 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/top_level.txt
--rw-r--r--   0 utkonos    (502) staff       (20)        1 2022-10-10 23:46:28.000000 opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/zip-safe
-drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2022-10-10 23:46:28.394353 opnsense-confgen-2.3.0/src/oscg/
--rw-r--r--   0 utkonos    (502) staff       (20)        0 2022-05-15 20:23:20.000000 opnsense-confgen-2.3.0/src/oscg/__init__.py
--rw-r--r--   0 utkonos    (502) staff       (20)     5504 2022-07-08 01:37:37.000000 opnsense-confgen-2.3.0/src/oscg/cli.py
--rw-r--r--   0 utkonos    (502) staff       (20)    13250 2022-10-10 23:29:59.000000 opnsense-confgen-2.3.0/src/oscg/core.py
--rw-r--r--   0 utkonos    (502) staff       (20)     1709 2022-10-10 23:19:52.000000 opnsense-confgen-2.3.0/src/oscg/example.py
-drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2022-10-10 23:46:28.398440 opnsense-confgen-2.3.0/src/oscg/templates/
--rw-r--r--   0 utkonos    (502) staff       (20)      100 2022-10-10 05:04:57.000000 opnsense-confgen-2.3.0/src/oscg/templates/apikey.xml
--rw-r--r--   0 utkonos    (502) staff       (20)    12854 2022-10-09 04:09:54.000000 opnsense-confgen-2.3.0/src/oscg/templates/config.xml
--rw-r--r--   0 utkonos    (502) staff       (20)      364 2022-05-15 00:35:43.000000 opnsense-confgen-2.3.0/src/oscg/templates/fw_admin.xml
--rw-r--r--   0 utkonos    (502) staff       (20)      348 2022-10-09 04:05:14.000000 opnsense-confgen-2.3.0/src/oscg/templates/fw_wg.xml
--rw-r--r--   0 utkonos    (502) staff       (20)      304 2022-10-09 04:26:28.000000 opnsense-confgen-2.3.0/src/oscg/templates/opt_dhcp.xml
--rw-r--r--   0 utkonos    (502) staff       (20)      159 2022-10-09 04:26:36.000000 opnsense-confgen-2.3.0/src/oscg/templates/opt_if.xml
--rw-r--r--   0 utkonos    (502) staff       (20)      942 2022-10-09 04:44:32.000000 opnsense-confgen-2.3.0/src/oscg/templates/wg_conf.xml
--rw-r--r--   0 utkonos    (502) staff       (20)      209 2022-05-15 00:33:58.000000 opnsense-confgen-2.3.0/src/oscg/templates/wg_grp.xml
--rw-r--r--   0 utkonos    (502) staff       (20)      125 2022-05-15 00:34:27.000000 opnsense-confgen-2.3.0/src/oscg/templates/wg_if.xml
--rw-r--r--   0 utkonos    (502) staff       (20)     1210 2022-05-29 00:56:29.000000 opnsense-confgen-2.3.0/src/oscg/utils.py
+drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2024-05-25 18:41:59.999864 opnsense_confgen-2.3.1/
+-rw-r--r--   0 utkonos    (502) staff       (20)     1072 2024-03-05 00:50:01.000000 opnsense_confgen-2.3.1/LICENSE.txt
+-rw-r--r--   0 utkonos    (502) staff       (20)     8776 2024-05-25 18:41:59.999637 opnsense_confgen-2.3.1/PKG-INFO
+-rw-r--r--   0 utkonos    (502) staff       (20)     7607 2022-10-10 23:16:04.000000 opnsense_confgen-2.3.1/README.md
+-rw-r--r--   0 utkonos    (502) staff       (20)       85 2024-05-25 15:07:22.000000 opnsense_confgen-2.3.1/pyproject.toml
+-rw-r--r--   0 utkonos    (502) staff       (20)     1428 2024-05-25 18:42:00.000516 opnsense_confgen-2.3.1/setup.cfg
+drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2024-05-25 18:41:59.981904 opnsense_confgen-2.3.1/src/
+drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2024-05-25 18:41:59.999091 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/
+-rw-r--r--   0 utkonos    (502) staff       (20)     8776 2024-05-25 18:41:59.000000 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/PKG-INFO
+-rw-r--r--   0 utkonos    (502) staff       (20)      817 2024-05-25 18:41:59.000000 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkonos    (502) staff       (20)        1 2024-05-25 18:41:59.000000 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkonos    (502) staff       (20)       39 2024-05-25 18:41:59.000000 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/entry_points.txt
+-rw-r--r--   0 utkonos    (502) staff       (20)       15 2024-05-25 18:41:59.000000 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/requires.txt
+-rw-r--r--   0 utkonos    (502) staff       (20)        5 2024-05-25 18:41:59.000000 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/top_level.txt
+-rw-r--r--   0 utkonos    (502) staff       (20)        1 2022-10-10 23:46:28.000000 opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/zip-safe
+drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2024-05-25 18:41:59.989548 opnsense_confgen-2.3.1/src/oscg/
+-rw-r--r--   0 utkonos    (502) staff       (20)        0 2022-05-15 20:23:20.000000 opnsense_confgen-2.3.1/src/oscg/__init__.py
+-rw-r--r--   0 utkonos    (502) staff       (20)     5303 2024-03-05 00:51:33.000000 opnsense_confgen-2.3.1/src/oscg/cli.py
+-rw-r--r--   0 utkonos    (502) staff       (20)    13547 2024-03-05 00:51:27.000000 opnsense_confgen-2.3.1/src/oscg/core.py
+-rw-r--r--   0 utkonos    (502) staff       (20)     1709 2024-03-05 00:51:24.000000 opnsense_confgen-2.3.1/src/oscg/example.py
+drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2024-05-25 18:41:59.994901 opnsense_confgen-2.3.1/src/oscg/templates/
+-rw-r--r--   0 utkonos    (502) staff       (20)      100 2022-10-10 05:04:57.000000 opnsense_confgen-2.3.1/src/oscg/templates/apikey.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)    12854 2022-10-09 04:09:54.000000 opnsense_confgen-2.3.1/src/oscg/templates/config.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)      364 2022-05-15 00:35:43.000000 opnsense_confgen-2.3.1/src/oscg/templates/fw_admin.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)      348 2022-10-09 04:05:14.000000 opnsense_confgen-2.3.1/src/oscg/templates/fw_wg.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)      304 2022-10-09 04:26:28.000000 opnsense_confgen-2.3.1/src/oscg/templates/opt_dhcp.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)      159 2022-10-09 04:26:36.000000 opnsense_confgen-2.3.1/src/oscg/templates/opt_if.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)      942 2022-10-09 04:44:32.000000 opnsense_confgen-2.3.1/src/oscg/templates/wg_conf.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)      209 2022-05-15 00:33:58.000000 opnsense_confgen-2.3.1/src/oscg/templates/wg_grp.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)      125 2022-05-15 00:34:27.000000 opnsense_confgen-2.3.1/src/oscg/templates/wg_if.xml
+-rw-r--r--   0 utkonos    (502) staff       (20)     1210 2024-03-05 00:51:19.000000 opnsense_confgen-2.3.1/src/oscg/utils.py
+drwxr-xr-x   0 utkonos    (502) staff       (20)        0 2024-05-25 18:41:59.998491 opnsense_confgen-2.3.1/tests/
+-rw-r--r--   0 utkonos    (502) staff       (20)    31984 2024-03-05 01:49:09.000000 opnsense_confgen-2.3.1/tests/test_cli.py
+-rw-r--r--   0 utkonos    (502) staff       (20)    24234 2024-03-05 00:50:53.000000 opnsense_confgen-2.3.1/tests/test_core.py
+-rw-r--r--   0 utkonos    (502) staff       (20)     2245 2024-03-05 00:50:48.000000 opnsense_confgen-2.3.1/tests/test_example.py
+-rw-r--r--   0 utkonos    (502) staff       (20)     3296 2024-03-05 00:50:42.000000 opnsense_confgen-2.3.1/tests/test_linters.py
+-rw-r--r--   0 utkonos    (502) staff       (20)     3139 2024-03-05 00:50:37.000000 opnsense_confgen-2.3.1/tests/test_utils.py
```

### Comparing `opnsense-confgen-2.3.0/LICENSE.txt` & `opnsense_confgen-2.3.1/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Malwarology LLC
+Copyright (c) 2024 Malwarology LLC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `opnsense-confgen-2.3.0/PKG-INFO` & `opnsense_confgen-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: opnsense-confgen
-Version: 2.3.0
+Version: 2.3.1
 Summary: Generate OPNsense configuration XML
 Home-page: https://github.com/malwarology/opnsense-confgen
 Author: Malwarology LLC
 Project-URL: Bug Tracker, https://github.com/malwarology/opnsense-confgen/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10.7
+Requires-Python: >=3.12.3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pynacl
+Requires-Dist: pycdlib
 
 # OPNsense Configuration Generator
 
 This package takes a Python ConfigParser formatted INI file and generates a ready to use config.xml file for OPNsense. The intent is for the file to be used during the installation process by the OPNsense Importer. The end result is a minimal working configuraion with interfaces fully configured. Included in this package are a command line interface and a class which is importable into Python scripts and other applications.
 
 More information about the OPNsense importer can be found [here](https://docs.opnsense.org/manual/install.html#opnsense-importer).
```

### Comparing `opnsense-confgen-2.3.0/README.md` & `opnsense_confgen-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `opnsense-confgen-2.3.0/setup.cfg` & `opnsense_confgen-2.3.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = opnsense-confgen
-version = 2.3.0
+version = 2.3.1
 author = Malwarology LLC
 description = Generate OPNsense configuration XML
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/malwarology/opnsense-confgen
 project_urls = 
 	Bug Tracker = https://github.com/malwarology/opnsense-confgen/issues
@@ -15,15 +15,15 @@
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.12
 	Topic :: Security
 	Topic :: System :: Networking :: Firewalls
 	Topic :: System :: Systems Administration
 	Topic :: Text Processing :: Markup :: XML
 	Topic :: Utilities
 
 [options]
@@ -31,15 +31,15 @@
 include_package_data = True
 package_dir = 
 	= src
 packages = find_namespace:
 install_requires = 
 	pynacl
 	pycdlib
-python_requires = >= 3.10.7
+python_requires = >= 3.12.3
 
 [options.package_data]
 oscg = templates/*.xml
 
 [options.packages.find]
 where = src
```

### Comparing `opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/PKG-INFO` & `opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: opnsense-confgen
-Version: 2.3.0
+Version: 2.3.1
 Summary: Generate OPNsense configuration XML
 Home-page: https://github.com/malwarology/opnsense-confgen
 Author: Malwarology LLC
 Project-URL: Bug Tracker, https://github.com/malwarology/opnsense-confgen/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking :: Firewalls
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10.7
+Requires-Python: >=3.12.3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: pynacl
+Requires-Dist: pycdlib
 
 # OPNsense Configuration Generator
 
 This package takes a Python ConfigParser formatted INI file and generates a ready to use config.xml file for OPNsense. The intent is for the file to be used during the installation process by the OPNsense Importer. The end result is a minimal working configuraion with interfaces fully configured. Included in this package are a command line interface and a class which is importable into Python scripts and other applications.
 
 More information about the OPNsense importer can be found [here](https://docs.opnsense.org/manual/install.html#opnsense-importer).
```

### Comparing `opnsense-confgen-2.3.0/src/opnsense_confgen.egg-info/SOURCES.txt` & `opnsense_confgen-2.3.1/src/opnsense_confgen.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,8 +18,13 @@
 src/oscg/templates/config.xml
 src/oscg/templates/fw_admin.xml
 src/oscg/templates/fw_wg.xml
 src/oscg/templates/opt_dhcp.xml
 src/oscg/templates/opt_if.xml
 src/oscg/templates/wg_conf.xml
 src/oscg/templates/wg_grp.xml
-src/oscg/templates/wg_if.xml
+src/oscg/templates/wg_if.xml
+tests/test_cli.py
+tests/test_core.py
+tests/test_example.py
+tests/test_linters.py
+tests/test_utils.py
```

### Comparing `opnsense-confgen-2.3.0/src/oscg/cli.py` & `opnsense_confgen-2.3.1/src/oscg/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# Copyright 2022 Malwarology LLC
+# Copyright 2024 Malwarology LLC
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 """Generate OPNsense configuration XML.
 
 The OPNsense Configuration Generator (oscg) is a command line tool for generating configuration XML files. The generator
 takes a simple INI file and emits a full config.xml file that is ready to use with the OPNsense importer during the
 install process. An optional WireGuard bootstrap can be included which allows immediate remote access to the new
 OPNsense instance. This bootstrap can use already existing keypairs, or can generate keypairs and a client config file
 if needed. The config.xml output can optionally be exported as an ISO.
 """
 import argparse
 import configparser
-import distutils
 import enum
 import pathlib
 import sys
 
 import oscg.core
 import oscg.example
 import oscg.utils
@@ -32,19 +31,15 @@
     URL = pathlib.Path('WGBootstrap.url')
     EX = pathlib.Path('opnsense_config_example.ini')
 
 
 def _cleanup():
     """Delete all output files."""
     delete = input('Delete all output files? (y/N): ')
-    try:
-        proceed = distutils.util.strtobool(delete)
-    except ValueError:
-        proceed = False
-    if not proceed:
+    if not delete.lower() in ['y', 'yes']:
         sys.exit()
     for path in list(_Output):
         path.value.unlink(missing_ok=True)
     sys.exit()
 
 
 def _write_example():
@@ -57,20 +52,16 @@
     sys.exit()
 
 
 def _check_path(path):
     """Check if path exists and ask if it should be overwritten."""
     if path.exists():
         overwrite = input('File "{}" exists, overwrite? (y/N): '.format(path.name))
-        try:
-            proceed = distutils.util.strtobool(overwrite)
-        except ValueError:
-            proceed = False
 
-        return proceed
+        return overwrite.lower() in ['y', 'yes']
 
     return True
 
 
 def _get_path(filename):
     """Check text string input path and return pathlib object if it exists."""
     path = pathlib.Path(filename)
```

### Comparing `opnsense-confgen-2.3.0/src/oscg/core.py` & `opnsense_confgen-2.3.1/src/oscg/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Malwarology LLC
+# Copyright 2024 Malwarology LLC
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 """Core functions for generating configs."""
 import configparser
 import importlib.metadata
@@ -17,15 +17,15 @@
 import oscg.utils
 
 
 class GenerateConfigs:
     """Class for generating an OPNsense config and optionally a WireGuard client config."""
 
     def __init__(self, config, testing=False):
-        with importlib.resources.open_text('oscg.templates', 'config.xml') as config_template:
+        with (importlib.resources.files('oscg.templates') / 'config.xml').open('r') as config_template:
             tree = xml.etree.ElementTree.parse(config_template)
         self._root = tree.getroot()
         if isinstance(config, dict):
             conf_parser = configparser.ConfigParser()
             conf_parser.read_dict(config)
             self._ini_config = conf_parser
         else:
@@ -141,41 +141,41 @@
         plugins = xml.etree.ElementTree.Element('plugins')
         plugins.text = 'os-wireguard'
         self._root.find('system').find('firmware').append(plugins)
 
     def _add_wg_if(self):
         """Append WireGuard interfaces to configuration."""
         # Append WireGuard interface group.
-        wg_grp_template = importlib.resources.read_text('oscg.templates', 'wg_grp.xml')
-        wg_grp = xml.etree.ElementTree.fromstring(wg_grp_template)
-        self._root.find('interfaces').append(wg_grp)
+        with (importlib.resources.files('oscg.templates') / 'wg_grp.xml').open('r') as wg_grp_template:
+            wg_grp = xml.etree.ElementTree.fromstring(wg_grp_template.read())
+            self._root.find('interfaces').append(wg_grp)
 
         # Append wg1 interface.
-        wg_if_template = importlib.resources.read_text('oscg.templates', 'wg_if.xml')
-        wg_if = xml.etree.ElementTree.fromstring(wg_if_template)
-        self._root.find('interfaces').append(wg_if)
+        with (importlib.resources.files('oscg.templates') / 'wg_if.xml').open('r') as wg_if_template:
+            wg_if = xml.etree.ElementTree.fromstring(wg_if_template.read())
+            self._root.find('interfaces').append(wg_if)
 
     def _add_wg_fw(self):
         """Add firewall rules relating to WireGuard."""
         # Insert firewall rule to allow WireGuard traffic on WAN interface at top of rule set.
-        fw_wg_template = importlib.resources.read_text('oscg.templates', 'fw_wg.xml')
-        fw_wg = xml.etree.ElementTree.fromstring(fw_wg_template)
-        fw_wg.find('destination').find('port').text = self._ini_config['WGB']['port']
-        self._root.find('filter').insert(0, fw_wg)
+        with (importlib.resources.files('oscg.templates') / 'fw_wg.xml').open('r') as fw_wg_template:
+            fw_wg = xml.etree.ElementTree.fromstring(fw_wg_template.read())
+            fw_wg.find('destination').find('port').text = self._ini_config['WGB']['port']
+            self._root.find('filter').insert(0, fw_wg)
 
         # Append firewall rule allowing access to OPNsense admin portal from WireGuard interface.
-        fw_admin_template = importlib.resources.read_text('oscg.templates', 'fw_admin.xml')
-        fw_admin = xml.etree.ElementTree.fromstring(fw_admin_template)
-        self._root.find('filter').append(fw_admin)
+        with (importlib.resources.files('oscg.templates') / 'fw_admin.xml').open('r') as fw_admin_template:
+            fw_admin = xml.etree.ElementTree.fromstring(fw_admin_template.read())
+            self._root.find('filter').append(fw_admin)
 
     def _add_wg_settings(self):
         """Append WireGuard settings to configuration."""
-        wg_conf_template = importlib.resources.read_text('oscg.templates', 'wg_conf.xml')
-        wg_conf = xml.etree.ElementTree.fromstring(wg_conf_template)
-        wgc = wg_conf.find('wireguard')
+        with (importlib.resources.files('oscg.templates') / 'wg_conf.xml').open('r') as wg_conf_template:
+            wg_conf = xml.etree.ElementTree.fromstring(wg_conf_template.read())
+            wgc = wg_conf.find('wireguard')
 
         # Add server endpoint settings.
         wg_server = wgc.find('server').find('servers').find('server')
         wg_server.set('uuid', str(uuid.uuid4()))
         wg_server.find('pubkey').text = self._ini_config['WGB']['server_pubkey']
         wg_server.find('privkey').text = self._ini_config['WGB']['server_privkey']
         wg_server.find('port').text = self._ini_config['WGB']['port']
@@ -201,44 +201,44 @@
 
         return opt_sections
 
     def _add_opt_if(self, match):
         """Append optional interface settings to configuration."""
         section = match.group(0)
 
-        opt_if_template = importlib.resources.read_text('oscg.templates', 'opt_if.xml')
-        opt_if = xml.etree.ElementTree.fromstring(opt_if_template)
+        with (importlib.resources.files('oscg.templates') / 'opt_if.xml').open('r') as opt_if_template:
+            opt_if = xml.etree.ElementTree.fromstring(opt_if_template.read())
 
-        opt_if.tag = 'opt{}'.format(match.group('number'))
-        opt_if.find('if').text = self._ini_config[section]['if']
-        opt_if.find('descr').text = self._ini_config[section]['description']
-        opt_if.find('ipaddr').text = self._ini_config[section]['ip']
-        opt_if.find('subnet').text = self._ini_config[section]['subnet']
+            opt_if.tag = 'opt{}'.format(match.group('number'))
+            opt_if.find('if').text = self._ini_config[section]['if']
+            opt_if.find('descr').text = self._ini_config[section]['description']
+            opt_if.find('ipaddr').text = self._ini_config[section]['ip']
+            opt_if.find('subnet').text = self._ini_config[section]['subnet']
 
-        self._root.find('interfaces').append(opt_if)
+            self._root.find('interfaces').append(opt_if)
 
     def _add_opt_dhcp(self, match):
         """Append optional interface DHCP settings to configuration."""
         section = match.group(0)
 
-        opt_dhcp_template = importlib.resources.read_text('oscg.templates', 'opt_dhcp.xml')
-        opt_dhcp = xml.etree.ElementTree.fromstring(opt_dhcp_template)
+        with (importlib.resources.files('oscg.templates') / 'opt_dhcp.xml').open('r') as opt_dhcp_template:
+            opt_dhcp = xml.etree.ElementTree.fromstring(opt_dhcp_template.read())
 
-        opt_dhcp.tag = 'opt{}'.format(match.group('number'))
-        opt_dhcp.find('gateway').text = self._ini_config[section]['ip']
-        opt_dhcp.find('range').find('from').text = self._ini_config[section].get('dhcp_start')
-        opt_dhcp.find('range').find('to').text = self._ini_config[section]['dhcp_end']
-        opt_dhcp.find('dnsserver').text = self._ini_config[section]['ip']
+            opt_dhcp.tag = 'opt{}'.format(match.group('number'))
+            opt_dhcp.find('gateway').text = self._ini_config[section]['ip']
+            opt_dhcp.find('range').find('from').text = self._ini_config[section].get('dhcp_start')
+            opt_dhcp.find('range').find('to').text = self._ini_config[section]['dhcp_end']
+            opt_dhcp.find('dnsserver').text = self._ini_config[section]['ip']
 
-        self._root.find('dhcpd').append(opt_dhcp)
+            self._root.find('dhcpd').append(opt_dhcp)
 
     def _add_apikey(self):
         """Add optional root API key."""
-        apikey_template = importlib.resources.read_text('oscg.templates', 'apikey.xml')
-        apikey = xml.etree.ElementTree.fromstring(apikey_template)
+        with (importlib.resources.files('oscg.templates') / 'apikey.xml').open('r') as apikey_template:
+            apikey = xml.etree.ElementTree.fromstring(apikey_template.read())
         apikey.find('item').find('key').text = self._ini_config['API']['key']
         apikey.find('item').find('secret').text = self._ini_config['API']['secret']
         self._root.find('system').find('user').append(apikey)
         expires = xml.etree.ElementTree.Element('expires')
         self._root.find('system').find('user').append(expires)
         authorizedkeys = xml.etree.ElementTree.Element('authorizedkeys')
         self._root.find('system').find('user').append(authorizedkeys)
```

### Comparing `opnsense-confgen-2.3.0/src/oscg/example.py` & `opnsense_confgen-2.3.1/src/oscg/example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Malwarology LLC
+# Copyright 2024 Malwarology LLC
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 """Generate an example configuration object."""
 import configparser
```

### Comparing `opnsense-confgen-2.3.0/src/oscg/templates/config.xml` & `opnsense_confgen-2.3.1/src/oscg/templates/config.xml`

 * *Files identical despite different names*

### Comparing `opnsense-confgen-2.3.0/src/oscg/templates/wg_conf.xml` & `opnsense_confgen-2.3.1/src/oscg/templates/wg_conf.xml`

 * *Files identical despite different names*

### Comparing `opnsense-confgen-2.3.0/src/oscg/utils.py` & `opnsense_confgen-2.3.1/src/oscg/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Malwarology LLC
+# Copyright 2024 Malwarology LLC
 #
 # Use of this source code is governed by an MIT-style
 # license that can be found in the LICENSE file or at
 # https://opensource.org/licenses/MIT.
 """Module for utility functions."""
 import base64
 import io
```

