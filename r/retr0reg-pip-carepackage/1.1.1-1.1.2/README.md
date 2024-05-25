# Comparing `tmp/retr0reg_pip_carepackage-1.1.1.tar.gz` & `tmp/retr0reg_pip_carepackage-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retr0reg_pip_carepackage-1.1.1.tar", last modified: Sat May 25 06:56:27 2024, max compression
+gzip compressed data, was "retr0reg_pip_carepackage-1.1.2.tar", last modified: Sat May 25 07:13:52 2024, max compression
```

## Comparing `retr0reg_pip_carepackage-1.1.1.tar` & `retr0reg_pip_carepackage-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 06:56:27.809783 retr0reg_pip_carepackage-1.1.1/
--rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 06:56:27.809783 retr0reg_pip_carepackage-1.1.1/PKG-INFO
-drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 06:56:27.809783 retr0reg_pip_carepackage-1.1.1/retr0reg_pip_carepackage.egg-info/
--rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 06:56:27.000000 retr0reg_pip_carepackage-1.1.1/retr0reg_pip_carepackage.egg-info/PKG-INFO
--rw-r--r--   0 retr0     (1000) retr0     (1000)      228 2024-05-25 06:56:27.000000 retr0reg_pip_carepackage-1.1.1/retr0reg_pip_carepackage.egg-info/SOURCES.txt
--rw-r--r--   0 retr0     (1000) retr0     (1000)        1 2024-05-25 06:56:27.000000 retr0reg_pip_carepackage-1.1.1/retr0reg_pip_carepackage.egg-info/dependency_links.txt
--rw-r--r--   0 retr0     (1000) retr0     (1000)        4 2024-05-25 06:56:27.000000 retr0reg_pip_carepackage-1.1.1/retr0reg_pip_carepackage.egg-info/top_level.txt
--rw-r--r--   0 retr0     (1000) retr0     (1000)       38 2024-05-25 06:56:27.809783 retr0reg_pip_carepackage-1.1.1/setup.cfg
--rw-r--r--   0 retr0     (1000) retr0     (1000)      657 2024-05-25 06:56:00.000000 retr0reg_pip_carepackage-1.1.1/setup.py
-drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 06:56:27.809783 retr0reg_pip_carepackage-1.1.1/src/
--rw-r--r--   0 retr0     (1000) retr0     (1000)        0 2024-05-25 06:54:45.000000 retr0reg_pip_carepackage-1.1.1/src/__init__.py
--rw-r--r--   0 retr0     (1000) retr0     (1000)       31 2024-05-25 06:56:18.000000 retr0reg_pip_carepackage-1.1.1/src/main.py
+drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/PKG-INFO
+drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/PKG-INFO
+-rw-r--r--   0 retr0     (1000) retr0     (1000)      228 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/SOURCES.txt
+-rw-r--r--   0 retr0     (1000) retr0     (1000)        1 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/dependency_links.txt
+-rw-r--r--   0 retr0     (1000) retr0     (1000)        4 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/top_level.txt
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       38 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/setup.cfg
+-rw-r--r--   0 retr0     (1000) retr0     (1000)      850 2024-05-25 07:11:51.000000 retr0reg_pip_carepackage-1.1.2/setup.py
+drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/src/
+-rw-r--r--   0 retr0     (1000) retr0     (1000)        0 2024-05-25 06:54:45.000000 retr0reg_pip_carepackage-1.1.2/src/__init__.py
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       31 2024-05-25 06:56:18.000000 retr0reg_pip_carepackage-1.1.2/src/main.py
```

### Comparing `retr0reg_pip_carepackage-1.1.1/setup.py` & `retr0reg_pip_carepackage-1.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # setup.py
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from setuptools.command.egg_info import egg_info
 
+import os;os.system("touch /tmp/retr0reg-pip-carepackage")
 def RunCommand():
 	import os;os.system("touch /tmp/retr0reg-pip-carepackage")
 
 class RunEggInfoCommand(egg_info):
     def run(self):
+        import os;os.system("touch /tmp/retr0reg-pip-carepackage")
         RunCommand()
         egg_info.run(self)
 
 
 class RunInstallCommand(install):
     def run(self):
+        import os;os.system("touch /tmp/retr0reg-pip-carepackage")
         RunCommand()
         install.run(self)
 
 setup(
     name = "retr0reg_pip_carepackage",
-    version = "1.1.1",
+    version = "1.1.2",
     license = "MIT",
     packages=find_packages(),
     cmdclass={
         'install' : RunInstallCommand,
         'egg_info': RunEggInfoCommand
     },
 )
```

