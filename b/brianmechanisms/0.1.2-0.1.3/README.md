# Comparing `tmp/brianmechanisms-0.1.2.tar.gz` & `tmp/brianmechanisms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brianmechanisms-0.1.2.tar", last modified: Fri May  3 11:13:01 2024, max compression
+gzip compressed data, was "brianmechanisms-0.1.3.tar", last modified: Sat May 25 20:59:31 2024, max compression
```

## Comparing `brianmechanisms-0.1.2.tar` & `brianmechanisms-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:01.684264 brianmechanisms-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-03 11:12:51.000000 brianmechanisms-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-03 11:13:01.684264 brianmechanisms-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-03 11:12:51.000000 brianmechanisms-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 11:12:51.000000 brianmechanisms-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 11:13:01.684264 brianmechanisms-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:01.680264 brianmechanisms-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:01.684264 brianmechanisms-0.1.2/src/brianmechanisms/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 11:12:51.000000 brianmechanisms-0.1.2/src/brianmechanisms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23911 2024-05-03 11:12:51.000000 brianmechanisms-0.1.2/src/brianmechanisms/appproximateStraightLineMechanisms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 11:13:01.684264 brianmechanisms-0.1.2/src/brianmechanisms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-03 11:13:01.000000 brianmechanisms-0.1.2/src/brianmechanisms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-03 11:13:01.000000 brianmechanisms-0.1.2/src/brianmechanisms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 11:13:01.000000 brianmechanisms-0.1.2/src/brianmechanisms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-03 11:13:01.000000 brianmechanisms-0.1.2/src/brianmechanisms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/src/brianmechanisms/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/appproximateStraightLineMechanisms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/locii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-25 20:59:20.000000 brianmechanisms-0.1.3/src/brianmechanisms/straightLineMechanisms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 20:59:31.471728 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 20:59:31.000000 brianmechanisms-0.1.3/src/brianmechanisms.egg-info/top_level.txt
```

### Comparing `brianmechanisms-0.1.2/LICENSE` & `brianmechanisms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brianmechanisms-0.1.2/src/brianmechanisms/appproximateStraightLineMechanisms.py` & `brianmechanisms-0.1.3/src/brianmechanisms/appproximateStraightLineMechanisms.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,8 +571,13 @@
         for animation in self.animes:
             animation_objects.append(animation.ani)
 
         # Concatenate all animation objects into a single animation object
         combined_animation = animation_objects[0] if animation_objects else None
         for anim in animation_objects[1:]:
             combined_animation += anim
-        return combined_animation
+        return combined_animation
+
+
+class parallelogram:
+    def __init__(self, vars=None):
+      pass
```

