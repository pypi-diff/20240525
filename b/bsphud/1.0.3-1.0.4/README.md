# Comparing `tmp/bsphud-1.0.3.tar.gz` & `tmp/bsphud-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsphud-1.0.3.tar", last modified: Fri May 17 09:24:38 2024, max compression
+gzip compressed data, was "bsphud-1.0.4.tar", last modified: Sat May 25 07:48:47 2024, max compression
```

## Comparing `bsphud-1.0.3.tar` & `bsphud-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-17 09:24:38.466974 bsphud-1.0.3/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    11326 2024-05-16 23:09:48.000000 bsphud-1.0.3/LICENSE.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    16681 2024-05-17 09:24:38.466974 bsphud-1.0.3/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3453 2024-05-17 09:21:44.000000 bsphud-1.0.3/README.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      483 2024-05-17 09:24:06.000000 bsphud-1.0.3/pyproject.toml
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       38 2024-05-17 09:24:38.466974 bsphud-1.0.3/setup.cfg
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-17 09:24:38.462974 bsphud-1.0.3/src/
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-17 09:24:38.464974 bsphud-1.0.3/src/bsphud/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-16 20:10:27.000000 bsphud-1.0.3/src/bsphud/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       36 2024-05-16 20:11:13.000000 bsphud-1.0.3/src/bsphud/__main__.py
--rwxr-xr-x   0 maybetree  (1000) maybetree  (1000)     5565 2024-05-16 21:25:00.000000 bsphud-1.0.3/src/bsphud/bsphud.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-17 09:24:38.465974 bsphud-1.0.3/src/bsphud.egg-info/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    16681 2024-05-17 09:24:38.000000 bsphud-1.0.3/src/bsphud.egg-info/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      239 2024-05-17 09:24:38.000000 bsphud-1.0.3/src/bsphud.egg-info/SOURCES.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-17 09:24:38.000000 bsphud-1.0.3/src/bsphud.egg-info/dependency_links.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-17 09:24:38.000000 bsphud-1.0.3/src/bsphud.egg-info/top_level.txt
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:48:47.527387 bsphud-1.0.4/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    11326 2024-05-16 23:09:48.000000 bsphud-1.0.4/LICENSE.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    16681 2024-05-25 07:48:47.527387 bsphud-1.0.4/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3453 2024-05-17 09:21:44.000000 bsphud-1.0.4/README.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      483 2024-05-25 07:46:36.000000 bsphud-1.0.4/pyproject.toml
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       38 2024-05-25 07:48:47.528387 bsphud-1.0.4/setup.cfg
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:48:47.524387 bsphud-1.0.4/src/
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:48:47.526387 bsphud-1.0.4/src/bsphud/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-16 20:10:27.000000 bsphud-1.0.4/src/bsphud/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       36 2024-05-16 20:11:13.000000 bsphud-1.0.4/src/bsphud/__main__.py
+-rwxr-xr-x   0 maybetree  (1000) maybetree  (1000)     5590 2024-05-18 17:40:19.000000 bsphud-1.0.4/src/bsphud/bsphud.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-25 07:48:47.527387 bsphud-1.0.4/src/bsphud.egg-info/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    16681 2024-05-25 07:48:47.000000 bsphud-1.0.4/src/bsphud.egg-info/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      239 2024-05-25 07:48:47.000000 bsphud-1.0.4/src/bsphud.egg-info/SOURCES.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-25 07:48:47.000000 bsphud-1.0.4/src/bsphud.egg-info/dependency_links.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-25 07:48:47.000000 bsphud-1.0.4/src/bsphud.egg-info/top_level.txt
```

### Comparing `bsphud-1.0.3/LICENSE.txt` & `bsphud-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bsphud-1.0.3/PKG-INFO` & `bsphud-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bsphud
-Version: 1.0.3
+Version: 1.0.4
 Summary: Desktop switcher popup for BSPWM
-Author-email: maybetree <maybetree48@gmail.com>
+Author-email: maybetree <maybetree48@proton.me>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
```

### Comparing `bsphud-1.0.3/README.md` & `bsphud-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bsphud-1.0.3/src/bsphud/bsphud.py` & `bsphud-1.0.4/src/bsphud/bsphud.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     def mainloop(self):
         self.root.mainloop()
 
     def show(self):
         self.shown = True
         self.root.deiconify()
+        self.root.lift()
         self.root.update()
 
     def hide(self):
         self.shown = False
         self.root.withdraw()
         self.root.update()
         # Sometimes, when the window appears,
```

### Comparing `bsphud-1.0.3/src/bsphud.egg-info/PKG-INFO` & `bsphud-1.0.4/src/bsphud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: bsphud
-Version: 1.0.3
+Version: 1.0.4
 Summary: Desktop switcher popup for BSPWM
-Author-email: maybetree <maybetree48@gmail.com>
+Author-email: maybetree <maybetree48@proton.me>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
```

