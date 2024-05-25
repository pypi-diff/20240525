# Comparing `tmp/autonomous_app-0.2.8.tar.gz` & `tmp/autonomous_app-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous_app-0.2.8.tar", last modified: Mon Apr 22 19:08:04 2024, max compression
+gzip compressed data, was "autonomous_app-0.2.9.tar", last modified: Mon Apr 29 02:34:44 2024, max compression
```

## Comparing `autonomous_app-0.2.8.tar` & `autonomous_app-0.2.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.074269 autonomous_app-0.2.8/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-22 19:08:04.074269 autonomous_app-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 19:08:04.074269 autonomous_app-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.066269 autonomous_app-0.2.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.066269 autonomous_app-0.2.8/src/autonomous/
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-22 19:07:48.000000 autonomous_app-0.2.8/src/autonomous/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.066269 autonomous_app-0.2.8/src/autonomous/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.8/src/autonomous/ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7128 2024-04-19 19:59:58.000000 autonomous_app-0.2.8/src/autonomous/ai/oaiagent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.070269 autonomous_app-0.2.8/src/autonomous/auth/
--rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.8/src/autonomous/auth/autoauth.py
--rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/auth/github.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/auth/google.py
--rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.8/src/autonomous/auth/user.py
--rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.070269 autonomous_app-0.2.8/src/autonomous/db/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.8/src/autonomous/db/autodb.py
--rw-r--r--   0 root         (0) root         (0)     4582 2024-04-22 17:36:31.000000 autonomous_app-0.2.8/src/autonomous/db/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.070269 autonomous_app-0.2.8/src/autonomous/errors/
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/errors/__init__.py
--rw-r--r--   0 root         (0) root         (0)      321 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/errors/danglingreferenceerror.py
--rw-r--r--   0 root         (0) root         (0)     1844 2024-04-18 14:33:06.000000 autonomous_app-0.2.8/src/autonomous/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.070269 autonomous_app-0.2.8/src/autonomous/model/
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.8/src/autonomous/model/autoattribute.py
--rw-r--r--   0 root         (0) root         (0)    11296 2024-04-20 17:24:46.000000 autonomous_app-0.2.8/src/autonomous/model/automodel.py
--rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.8/src/autonomous/model/orm.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.8/src/autonomous/model/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.070269 autonomous_app-0.2.8/src/autonomous/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.8/src/autonomous/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3966 2024-04-17 14:41:12.000000 autonomous_app-0.2.8/src/autonomous/storage/imagestorage.py
--rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/storage/localstorage.py
--rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.8/src/autonomous/storage/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.070269 autonomous_app-0.2.8/src/autonomous/storage/version_control/
--rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/storage/version_control/GHCallbacks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/storage/version_control/GHOrganization.py
--rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/storage/version_control/GHRepo.py
--rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/storage/version_control/GHVersionControl.py
--rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/storage/version_control/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.074269 autonomous_app-0.2.8/src/autonomous/tasks/
--rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.8/src/autonomous/tasks/autotask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 19:08:04.074269 autonomous_app-0.2.8/src/autonomous_app.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-22 19:08:04.000000 autonomous_app-0.2.8/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1372 2024-04-22 19:08:04.000000 autonomous_app-0.2.8/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 19:08:04.000000 autonomous_app-0.2.8/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2024-04-22 19:08:04.000000 autonomous_app-0.2.8/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-22 19:08:04.000000 autonomous_app-0.2.8/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.181782 autonomous_app-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-29 02:34:44.181782 autonomous_app-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-02-28 15:34:22.000000 autonomous_app-0.2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     1321 2024-04-16 15:28:50.000000 autonomous_app-0.2.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-17 20:37:08.000000 autonomous_app-0.2.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 02:34:44.181782 autonomous_app-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.177782 autonomous_app-0.2.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.177782 autonomous_app-0.2.9/src/autonomous/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-29 02:34:23.000000 autonomous_app-0.2.9/src/autonomous/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.177782 autonomous_app-0.2.9/src/autonomous/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:34.000000 autonomous_app-0.2.9/src/autonomous/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7128 2024-04-19 19:59:58.000000 autonomous_app-0.2.9/src/autonomous/ai/oaiagent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.177782 autonomous_app-0.2.9/src/autonomous/auth/
+-rw-r--r--   0 root         (0) root         (0)      161 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-02-20 18:09:54.000000 autonomous_app-0.2.9/src/autonomous/auth/autoauth.py
+-rw-r--r--   0 root         (0) root         (0)      886 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/auth/github.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/auth/google.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-03-30 04:51:47.000000 autonomous_app-0.2.9/src/autonomous/auth/user.py
+-rw-r--r--   0 root         (0) root         (0)       42 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.177782 autonomous_app-0.2.9/src/autonomous/db/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2024-03-20 18:44:15.000000 autonomous_app-0.2.9/src/autonomous/db/autodb.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2024-04-22 17:36:31.000000 autonomous_app-0.2.9/src/autonomous/db/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.177782 autonomous_app-0.2.9/src/autonomous/errors/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/errors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-23 10:54:04.000000 autonomous_app-0.2.9/src/autonomous/errors/danglingreferenceerror.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2024-04-18 14:33:06.000000 autonomous_app-0.2.9/src/autonomous/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.177782 autonomous_app-0.2.9/src/autonomous/model/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      588 2024-02-20 20:56:13.000000 autonomous_app-0.2.9/src/autonomous/model/autoattribute.py
+-rw-r--r--   0 root         (0) root         (0)    11853 2024-04-28 19:54:50.000000 autonomous_app-0.2.9/src/autonomous/model/automodel.py
+-rw-r--r--   0 root         (0) root         (0)     2521 2024-03-30 05:04:37.000000 autonomous_app-0.2.9/src/autonomous/model/orm.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-03-24 18:25:01.000000 autonomous_app-0.2.9/src/autonomous/model/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.181782 autonomous_app-0.2.9/src/autonomous/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 19:48:54.000000 autonomous_app-0.2.9/src/autonomous/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3970 2024-04-27 13:56:58.000000 autonomous_app-0.2.9/src/autonomous/storage/imagestorage.py
+-rw-r--r--   0 root         (0) root         (0)     2286 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2024-04-17 21:07:33.000000 autonomous_app-0.2.9/src/autonomous/storage/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.181782 autonomous_app-0.2.9/src/autonomous/storage/version_control/
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/storage/version_control/GHCallbacks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/storage/version_control/GHOrganization.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/storage/version_control/GHRepo.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/storage/version_control/GHVersionControl.py
+-rw-r--r--   0 root         (0) root         (0)      117 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/storage/version_control/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.181782 autonomous_app-0.2.9/src/autonomous/tasks/
+-rw-r--r--   0 root         (0) root         (0)       32 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-02-14 21:26:11.000000 autonomous_app-0.2.9/src/autonomous/tasks/autotask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 02:34:44.181782 autonomous_app-0.2.9/src/autonomous_app.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-29 02:34:44.000000 autonomous_app-0.2.9/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-04-29 02:34:44.000000 autonomous_app-0.2.9/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 02:34:44.000000 autonomous_app-0.2.9/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2024-04-29 02:34:44.000000 autonomous_app-0.2.9/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-29 02:34:44.000000 autonomous_app-0.2.9/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous_app-0.2.8/LICENSE` & `autonomous_app-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/PKG-INFO` & `autonomous_app-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.8
+Version: 0.2.9
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.8/README.md` & `autonomous_app-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/pyproject.toml` & `autonomous_app-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/requirements.txt` & `autonomous_app-0.2.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/ai/oaiagent.py` & `autonomous_app-0.2.9/src/autonomous/ai/oaiagent.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/auth/autoauth.py` & `autonomous_app-0.2.9/src/autonomous/auth/autoauth.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/auth/github.py` & `autonomous_app-0.2.9/src/autonomous/auth/github.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/auth/google.py` & `autonomous_app-0.2.9/src/autonomous/auth/google.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/auth/user.py` & `autonomous_app-0.2.9/src/autonomous/auth/user.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/db/autodb.py` & `autonomous_app-0.2.9/src/autonomous/db/autodb.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/db/table.py` & `autonomous_app-0.2.9/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/logger.py` & `autonomous_app-0.2.9/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/model/autoattribute.py` & `autonomous_app-0.2.9/src/autonomous/model/autoattribute.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/model/automodel.py` & `autonomous_app-0.2.9/src/autonomous/model/automodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,14 +337,28 @@
             AutoModel or None: The first matching AutoModel instance, or None if not found.
         """
         for k, v in kwargs.items():
             kwargs[k] = AutoEncoder.encode(v)
         attribs = cls.table().find(**kwargs)
         return cls(**attribs) if attribs else None
 
+    def update(self, values):
+        """
+        Delete this model from the database.
+        """
+        if not isinstance(values, dict):
+            raise ValueError("Values must be a dictionary")
+        for k, v in values.items():
+            if k in self.attributes or f"_{k}" in self.attributes:
+                if getattr(self.__class__, k, None) and getattr(self.__class__, k).fset:
+                    getattr(self.__class__, k).fset(self, v)
+                elif k in self.attributes:
+                    setattr(self, k, v)
+        self.save()
+
     def delete(self):
         """
         Delete this model from the database.
         """
         return self.table().delete(self.pk)
 
     def serialize(self):
```

### Comparing `autonomous_app-0.2.8/src/autonomous/model/orm.py` & `autonomous_app-0.2.9/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/model/serializer.py` & `autonomous_app-0.2.9/src/autonomous/model/serializer.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/storage/imagestorage.py` & `autonomous_app-0.2.9/src/autonomous/storage/imagestorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,20 +95,20 @@
             return os.path.join(self.base_path, f"{asset_path}")
         else:
             return self.base_path
 
     def search(self, folder="", **kwargs):
         imgs = []
         for f in os.listdir(f"{self.base_path}/{folder}"):
-            log(f"{self.base_path}/{folder}", f)
+            # log(f"{self.base_path}/{folder}", f)
             img_key = self._get_key(
                 f"{folder}",
                 pkey=f,
             )
-            log(img_key)
+            # log(img_key)
             imgs.append(img_key)
         return imgs
 
     def remove(self, asset_id):
         file_path = self.get_path(asset_id)
         if os.path.isdir(file_path):
             shutil.rmtree(file_path)
```

### Comparing `autonomous_app-0.2.8/src/autonomous/storage/localstorage.py` & `autonomous_app-0.2.9/src/autonomous/storage/localstorage.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/storage/markdown.py` & `autonomous_app-0.2.9/src/autonomous/storage/markdown.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/storage/version_control/GHCallbacks.py` & `autonomous_app-0.2.9/src/autonomous/storage/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/storage/version_control/GHOrganization.py` & `autonomous_app-0.2.9/src/autonomous/storage/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/storage/version_control/GHRepo.py` & `autonomous_app-0.2.9/src/autonomous/storage/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous/tasks/autotask.py` & `autonomous_app-0.2.9/src/autonomous/tasks/autotask.py`

 * *Files identical despite different names*

### Comparing `autonomous_app-0.2.8/src/autonomous_app.egg-info/PKG-INFO` & `autonomous_app-0.2.9/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.2.8
+Version: 0.2.9
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `autonomous_app-0.2.8/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous_app-0.2.9/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

