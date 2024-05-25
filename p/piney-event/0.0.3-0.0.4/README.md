# Comparing `tmp/piney_event-0.0.3.tar.gz` & `tmp/piney_event-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piney_event-0.0.3.tar", last modified: Sun Mar 10 22:44:31 2024, max compression
+gzip compressed data, was "piney_event-0.0.4.tar", last modified: Sat May 25 20:06:32 2024, max compression
```

## Comparing `piney_event-0.0.3.tar` & `piney_event-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-03-10 22:44:31.810177 piney_event-0.0.3/
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)     1471 2024-03-06 19:19:14.000000 piney_event-0.0.3/LICENSE
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      949 2024-03-10 22:44:31.810177 piney_event-0.0.3/PKG-INFO
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      437 2024-03-06 19:17:56.000000 piney_event-0.0.3/README.md
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      582 2024-03-10 22:43:36.000000 piney_event-0.0.3/pyproject.toml
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)       38 2024-03-10 22:44:31.810177 piney_event-0.0.3/setup.cfg
-drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-03-10 22:44:31.810177 piney_event-0.0.3/src/
-drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-03-10 22:44:31.810177 piney_event-0.0.3/src/piney_event/
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)     2531 2024-03-08 17:42:56.000000 piney_event-0.0.3/src/piney_event/event.py
-drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-03-10 22:44:31.810177 piney_event-0.0.3/src/piney_event.egg-info/
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      949 2024-03-10 22:44:31.000000 piney_event-0.0.3/src/piney_event.egg-info/PKG-INFO
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      213 2024-03-10 22:44:31.000000 piney_event-0.0.3/src/piney_event.egg-info/SOURCES.txt
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)        1 2024-03-10 22:44:31.000000 piney_event-0.0.3/src/piney_event.egg-info/dependency_links.txt
--rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)       12 2024-03-10 22:44:31.000000 piney_event-0.0.3/src/piney_event.egg-info/top_level.txt
+drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-05-25 20:06:32.903420 piney_event-0.0.4/
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)     1471 2024-03-06 19:19:14.000000 piney_event-0.0.4/LICENSE
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      949 2024-05-25 20:06:32.903420 piney_event-0.0.4/PKG-INFO
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      437 2024-03-06 19:17:56.000000 piney_event-0.0.4/README.md
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      582 2024-05-25 20:04:49.000000 piney_event-0.0.4/pyproject.toml
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)       38 2024-05-25 20:06:32.903420 piney_event-0.0.4/setup.cfg
+drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-05-25 20:06:32.903420 piney_event-0.0.4/src/
+drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-05-25 20:06:32.903420 piney_event-0.0.4/src/piney_event/
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)     4165 2024-05-25 19:53:27.000000 piney_event-0.0.4/src/piney_event/event.py
+drwxr-xr-x   0 hohfchns  (1000) hohfchns  (1000)        0 2024-05-25 20:06:32.903420 piney_event-0.0.4/src/piney_event.egg-info/
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      949 2024-05-25 20:06:32.000000 piney_event-0.0.4/src/piney_event.egg-info/PKG-INFO
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)      213 2024-05-25 20:06:32.000000 piney_event-0.0.4/src/piney_event.egg-info/SOURCES.txt
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)        1 2024-05-25 20:06:32.000000 piney_event-0.0.4/src/piney_event.egg-info/dependency_links.txt
+-rw-r--r--   0 hohfchns  (1000) hohfchns  (1000)       12 2024-05-25 20:06:32.000000 piney_event-0.0.4/src/piney_event.egg-info/top_level.txt
```

### Comparing `piney_event-0.0.3/LICENSE` & `piney_event-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `piney_event-0.0.3/PKG-INFO` & `piney_event-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piney_event
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tiny Event System for Python
 Author-email: Sahar Shulman <dillpickledev@gmail.com>
 Project-URL: Homepage, https://github.com/hohfchns/piney_event
 Project-URL: Issues, https://github.com/hohfchns/piney_event/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `piney_event-0.0.3/pyproject.toml` & `piney_event-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=59.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "piney_event"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Sahar Shulman", email="dillpickledev@gmail.com" },
 ]
 description = "A tiny Event System for Python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `piney_event-0.0.3/src/piney_event.egg-info/PKG-INFO` & `piney_event-0.0.4/src/piney_event.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piney_event
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tiny Event System for Python
 Author-email: Sahar Shulman <dillpickledev@gmail.com>
 Project-URL: Homepage, https://github.com/hohfchns/piney_event
 Project-URL: Issues, https://github.com/hohfchns/piney_event/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

