# Comparing `tmp/lbt-grasshopper-1.8.8.tar.gz` & `tmp/lbt-grasshopper-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lbt-grasshopper-1.8.8.tar", last modified: Thu Apr 11 23:09:02 2024, max compression
+gzip compressed data, was "dist/lbt-grasshopper-1.8.9.tar", last modified: Fri Apr 12 14:57:00 2024, max compression
```

## Comparing `lbt-grasshopper-1.8.8.tar` & `lbt-grasshopper-1.8.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/CI_STATUS.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/ci-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   730519 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/gradients.png
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/installer.gh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/lbt_grasshopper/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/lbt_grasshopper/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/lbt_grasshopper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/lbt_grasshopper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/lbt_grasshopper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/lbt_grasshopper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/lbt_grasshopper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/lbt_grasshopper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/pass_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/ruby-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 23:09:02.000000 lbt-grasshopper-1.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-11 23:07:55.000000 lbt-grasshopper-1.8.8/uninstaller.gh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12892 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/CI_STATUS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/ci-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   730519 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/gradients.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/installer.gh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/lbt_grasshopper/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/lbt_grasshopper/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/lbt_grasshopper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/lbt_grasshopper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/lbt_grasshopper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/lbt_grasshopper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/lbt_grasshopper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/lbt_grasshopper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/pass_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/ruby-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 14:57:00.000000 lbt-grasshopper-1.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7445 2024-04-12 14:55:54.000000 lbt-grasshopper-1.8.9/uninstaller.gh
```

### Comparing `lbt-grasshopper-1.8.8/.github/workflows/ci.yaml` & `lbt-grasshopper-1.8.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/.github/workflows/dependency-release.yaml` & `lbt-grasshopper-1.8.9/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/CI_STATUS.md` & `lbt-grasshopper-1.8.9/CI_STATUS.md`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/LICENSE` & `lbt-grasshopper-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/PKG-INFO` & `lbt-grasshopper-1.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.8.8
+Version: 1.8.9
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.8.8/README.md` & `lbt-grasshopper-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/gradients.png` & `lbt-grasshopper-1.8.9/gradients.png`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/installer.gh` & `lbt-grasshopper-1.8.9/installer.gh`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/lbt_grasshopper.egg-info/PKG-INFO` & `lbt-grasshopper-1.8.9/lbt_grasshopper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbt-grasshopper
-Version: 1.8.8
+Version: 1.8.9
 Summary: Collection of all Ladybug Tools plugins for Grasshopper
 Home-page: https://github.com/ladybug-tools/lbt-grasshopper
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: Implementation :: IronPython
```

### Comparing `lbt-grasshopper-1.8.8/setup.py` & `lbt-grasshopper-1.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `lbt-grasshopper-1.8.8/uninstaller.gh` & `lbt-grasshopper-1.8.9/uninstaller.gh`

 * *Files identical despite different names*

