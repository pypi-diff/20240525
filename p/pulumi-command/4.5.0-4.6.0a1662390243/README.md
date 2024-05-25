# Comparing `tmp/pulumi_command-4.5.0.tar.gz` & `tmp/pulumi_command-4.6.0a1662390243.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_command-4.5.0.tar", last modified: Mon Sep  5 14:48:31 2022, max compression
+gzip compressed data, was "dist/pulumi_command-4.6.0a1662390243.tar", last modified: Mon Sep  5 15:07:17 2022, max compression
```

## Comparing `pulumi_command-4.5.0.tar` & `pulumi_command-4.6.0a1662390243.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)    18083 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14637 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8050 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/local/
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25930 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/local/command.py
--rw-r--r--   0 runner    (1001) docker     (121)    13550 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/local/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/remote/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/remote/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12371 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/remote/command.py
--rw-r--r--   0 runner    (1001) docker     (121)     8413 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/remote/copy_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command/remote/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18083 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/pulumi_command.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-09-05 14:48:31.000000 pulumi_command-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:07:17.000000 pulumi_command-4.6.0a1662390243/
+-rw-r--r--   0 runner    (1001) docker     (121)    18094 2022-09-05 15:07:17.000000 pulumi_command-4.6.0a1662390243/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14637 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:07:17.000000 pulumi_command-4.6.0a1662390243/pulumi_command/
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8050 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:07:17.000000 pulumi_command-4.6.0a1662390243/pulumi_command/local/
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25930 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/local/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13550 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/local/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:07:17.000000 pulumi_command-4.6.0a1662390243/pulumi_command/remote/
+-rw-r--r--   0 runner    (1001) docker     (121)      331 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3439 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/remote/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12371 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/remote/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8413 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/remote/copy_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3257 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command/remote/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 15:07:17.000000 pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    18094 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 15:07:17.000000 pulumi_command-4.6.0a1662390243/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-09-05 15:07:16.000000 pulumi_command-4.6.0a1662390243/setup.py
```

### Comparing `pulumi_command-4.5.0/PKG-INFO` & `pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_command
-Version: 4.5.0
+Name: pulumi-command
+Version: 4.6.0a1662390243
 Summary: The Pulumi Command Provider enables you to execute commands and scripts either locally or remotely as part of the Pulumi resource model.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-command
 Description: [![Actions Status](https://github.com/pulumi/pulumi-command/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-command/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fcommand.svg)](https://www.npmjs.com/package/@pulumi/command)
```

### Comparing `pulumi_command-4.5.0/README.md` & `pulumi_command-4.6.0a1662390243/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/__init__.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/_utilities.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/local/command.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/local/command.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/local/run.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/local/run.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/provider.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/remote/_inputs.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/remote/command.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/remote/command.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/remote/copy_file.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/remote/copy_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command/remote/outputs.py` & `pulumi_command-4.6.0a1662390243/pulumi_command/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/pulumi_command.egg-info/PKG-INFO` & `pulumi_command-4.6.0a1662390243/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-command
-Version: 4.5.0
+Name: pulumi_command
+Version: 4.6.0a1662390243
 Summary: The Pulumi Command Provider enables you to execute commands and scripts either locally or remotely as part of the Pulumi resource model.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-command
 Description: [![Actions Status](https://github.com/pulumi/pulumi-command/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-command/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fcommand.svg)](https://www.npmjs.com/package/@pulumi/command)
```

### Comparing `pulumi_command-4.5.0/pulumi_command.egg-info/SOURCES.txt` & `pulumi_command-4.6.0a1662390243/pulumi_command.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_command-4.5.0/setup.py` & `pulumi_command-4.6.0a1662390243/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.5.0"
-PLUGIN_VERSION = "4.5.0"
+VERSION = "4.6.0a1662390243"
+PLUGIN_VERSION = "4.6.0-alpha.1662390243+5c22c9dd"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'command', PLUGIN_VERSION])
         except OSError as error:
```

