# Comparing `tmp/UnityPredict-0.1.3.tar.gz` & `tmp/UnityPredict-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnityPredict-0.1.3.tar", last modified: Sat May 25 07:34:30 2024, max compression
+gzip compressed data, was "UnityPredict-0.1.4.tar", last modified: Sat May 25 10:45:50 2024, max compression
```

## Comparing `UnityPredict-0.1.3.tar` & `UnityPredict-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 07:34:30.524171 UnityPredict-0.1.3/
--rw-rw-rw-   0        0        0     6878 2024-05-25 07:34:30.522164 UnityPredict-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6774 2024-05-22 07:02:45.000000 UnityPredict-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 07:34:30.516264 UnityPredict-0.1.3/UnityPredict/
--rw-rw-rw-   0        0        0     3306 2024-05-19 13:56:42.000000 UnityPredict-0.1.3/UnityPredict/Models.py
--rw-rw-rw-   0        0        0     2383 2024-05-11 17:05:18.000000 UnityPredict-0.1.3/UnityPredict/Platform.py
--rw-rw-rw-   0        0        0    18322 2024-05-21 16:10:04.000000 UnityPredict-0.1.3/UnityPredict/UnityPredictLocalHost.py
--rw-rw-rw-   0        0        0       53 2024-05-12 18:12:20.000000 UnityPredict-0.1.3/UnityPredict/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-25 07:34:30.520163 UnityPredict-0.1.3/UnityPredict.egg-info/
--rw-rw-rw-   0        0        0     6878 2024-05-25 07:34:30.000000 UnityPredict-0.1.3/UnityPredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-25 07:34:30.000000 UnityPredict-0.1.3/UnityPredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 07:34:30.000000 UnityPredict-0.1.3/UnityPredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-25 07:34:30.000000 UnityPredict-0.1.3/UnityPredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 07:34:30.524171 UnityPredict-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      439 2024-05-25 07:34:23.000000 UnityPredict-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:45:50.291705 UnityPredict-0.1.4/
+-rw-rw-rw-   0        0        0     6878 2024-05-25 10:45:50.289702 UnityPredict-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6774 2024-05-22 07:02:45.000000 UnityPredict-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 10:45:50.285713 UnityPredict-0.1.4/UnityPredict/
+-rw-rw-rw-   0        0        0     3306 2024-05-19 13:56:42.000000 UnityPredict-0.1.4/UnityPredict/Models.py
+-rw-rw-rw-   0        0        0     2383 2024-05-11 17:05:18.000000 UnityPredict-0.1.4/UnityPredict/Platform.py
+-rw-rw-rw-   0        0        0    18322 2024-05-21 16:10:04.000000 UnityPredict-0.1.4/UnityPredict/UnityPredictLocalHost.py
+-rw-rw-rw-   0        0        0       53 2024-05-12 18:12:20.000000 UnityPredict-0.1.4/UnityPredict/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-25 10:45:50.288703 UnityPredict-0.1.4/UnityPredict.egg-info/
+-rw-rw-rw-   0        0        0     6878 2024-05-25 10:45:50.000000 UnityPredict-0.1.4/UnityPredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-25 10:45:50.000000 UnityPredict-0.1.4/UnityPredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 10:45:50.000000 UnityPredict-0.1.4/UnityPredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-25 10:45:50.000000 UnityPredict-0.1.4/UnityPredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 10:45:50.291705 UnityPredict-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      439 2024-05-25 10:45:46.000000 UnityPredict-0.1.4/setup.py
```

### Comparing `UnityPredict-0.1.3/PKG-INFO` & `UnityPredict-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnityPredict
-Version: 0.1.3
+Version: 0.1.4
 Description-Content-Type: text/markdown
 
 # UnityPredict Local App Engine Creator
 
 ## Introduction
 
 This library allows you to create App Engines in your local system and finetune the engines before updating it to the [ModelCentral](https://modelcentral.ai) repositories.
```

### Comparing `UnityPredict-0.1.3/README.md` & `UnityPredict-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.3/UnityPredict/Models.py` & `UnityPredict-0.1.4/UnityPredict/Models.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.3/UnityPredict/Platform.py` & `UnityPredict-0.1.4/UnityPredict/Platform.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.3/UnityPredict/UnityPredictLocalHost.py` & `UnityPredict-0.1.4/UnityPredict/UnityPredictLocalHost.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1.3/UnityPredict.egg-info/PKG-INFO` & `UnityPredict-0.1.4/UnityPredict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnityPredict
-Version: 0.1.3
+Version: 0.1.4
 Description-Content-Type: text/markdown
 
 # UnityPredict Local App Engine Creator
 
 ## Introduction
 
 This library allows you to create App Engines in your local system and finetune the engines before updating it to the [ModelCentral](https://modelcentral.ai) repositories.
```

