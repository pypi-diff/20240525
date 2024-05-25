# Comparing `tmp/kal_middleware-0.0.6.tar.gz` & `tmp/kal_middleware-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kal_middleware-0.0.6.tar", last modified: Thu May 23 17:09:39 2024, max compression
+gzip compressed data, was "kal_middleware-0.0.7.tar", last modified: Sat May 25 06:58:34 2024, max compression
```

## Comparing `kal_middleware-0.0.6.tar` & `kal_middleware-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.538576 kal_middleware-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.542576 kal_middleware-0.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.542576 kal_middleware-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/jwt.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/kal_middleware.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/sts.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/kal_middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/kal_middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/kal_middleware/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/kal_middleware/kal_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/kal_middleware/sts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/kal_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-23 17:09:39.000000 kal_middleware-0.0.6/kal_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-23 17:09:39.000000 kal_middleware-0.0.6/kal_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:09:39.000000 kal_middleware-0.0.6/kal_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 17:09:39.000000 kal_middleware-0.0.6/kal_middleware.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-23 17:09:39.000000 kal_middleware-0.0.6/kal_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 17:09:39.000000 kal_middleware-0.0.6/kal_middleware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:09:39.546576 kal_middleware-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 17:09:29.000000 kal_middleware-0.0.6/tests/test_kal_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.291207 kal_middleware-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.279207 kal_middleware-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.283207 kal_middleware-0.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.283207 kal_middleware-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-25 06:58:34.287207 kal_middleware-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.287207 kal_middleware-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.287207 kal_middleware-0.0.7/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/jwt.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/kal_middleware.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.287207 kal_middleware-0.0.7/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/sts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.287207 kal_middleware-0.0.7/kal_middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/kal_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/kal_middleware/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/kal_middleware/kal_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/kal_middleware/sts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.287207 kal_middleware-0.0.7/kal_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-05-25 06:58:34.000000 kal_middleware-0.0.7/kal_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-25 06:58:34.000000 kal_middleware-0.0.7/kal_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 06:58:34.000000 kal_middleware-0.0.7/kal_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-25 06:58:34.000000 kal_middleware-0.0.7/kal_middleware.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-25 06:58:34.000000 kal_middleware-0.0.7/kal_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-25 06:58:34.000000 kal_middleware-0.0.7/kal_middleware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 06:58:34.291207 kal_middleware-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:58:34.287207 kal_middleware-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-25 06:58:23.000000 kal_middleware-0.0.7/tests/test_kal_middleware.py
```

### Comparing `kal_middleware-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `kal_middleware-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/ISSUE_TEMPLATE/config.yml` & `kal_middleware-0.0.7/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/workflows/docs-build.yml` & `kal_middleware-0.0.7/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/workflows/docs.yml` & `kal_middleware-0.0.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/workflows/installation.yml` & `kal_middleware-0.0.7/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/workflows/macos.yml` & `kal_middleware-0.0.7/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/workflows/pypi.yml` & `kal_middleware-0.0.7/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/workflows/ubuntu.yml` & `kal_middleware-0.0.7/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.github/workflows/windows.yml` & `kal_middleware-0.0.7/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/.gitignore` & `kal_middleware-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/LICENSE` & `kal_middleware-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/PKG-INFO` & `kal_middleware-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-middleware
-Version: 0.0.6
+Version: 0.0.7
 Summary: Kaleidoo middleware package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-middleware
 Keywords: kal-middleware
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -82,15 +82,15 @@
     user = {
         "id": "333444",
         "firebase_uid": "12345",
         "org_id": "12345"
     }
     if body["org_id"] == user["org_id"]:
         return True, user
-    return False, None
+    return False, f"User {user.get('id')} from another organization then the one that was requested."
 
 @app.get("/your-route/<service>/<action>")
 @firebase_jwt_authenticated(get_user_capabilities, check_access)
 async def your_route_function(
         request: Request = None,
         service: Union[str, None] = None,
         action: Union[str, None] = None
```

### Comparing `kal_middleware-0.0.6/README.md` & `kal_middleware-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     user = {
         "id": "333444",
         "firebase_uid": "12345",
         "org_id": "12345"
     }
     if body["org_id"] == user["org_id"]:
         return True, user
-    return False, None
+    return False, f"User {user.get('id')} from another organization then the one that was requested."
 
 @app.get("/your-route/<service>/<action>")
 @firebase_jwt_authenticated(get_user_capabilities, check_access)
 async def your_route_function(
         request: Request = None,
         service: Union[str, None] = None,
         action: Union[str, None] = None
```

### Comparing `kal_middleware-0.0.6/docs/contributing.md` & `kal_middleware-0.0.7/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/docs/installation.md` & `kal_middleware-0.0.7/docs/installation.md`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/kal_middleware/jwt.py` & `kal_middleware-0.0.7/kal_middleware/jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             if request.method in ["POST", "PUT"]:
                 if check_access:
                     body = await request.json()
                     access, user  = await check_access(user_uid, body, user_capabilities)
                     if not access:
                         return Response(
                             status_code=status.HTTP_403_FORBIDDEN,
-                            content="User not permitted to perform this action.",
+                            content=f"User not permitted to perform this action. reason: {user}",
                         )
 
             request.state.uid = user_uid  # Attach the Firebase id to the request state for later use.
             if user:
                 request.state.user = user
             request.state.user_capabilities = user_capabilities
```

### Comparing `kal_middleware-0.0.6/kal_middleware/sts.py` & `kal_middleware-0.0.7/kal_middleware/sts.py`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/kal_middleware.egg-info/PKG-INFO` & `kal_middleware-0.0.7/kal_middleware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kal-middleware
-Version: 0.0.6
+Version: 0.0.7
 Summary: Kaleidoo middleware package
 Author-email: Bar Lander <barh@kaleidoo.ai>
 License: MIT License
 Project-URL: Homepage, https://github.com/BarLanderK/kal-middleware
 Keywords: kal-middleware
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -82,15 +82,15 @@
     user = {
         "id": "333444",
         "firebase_uid": "12345",
         "org_id": "12345"
     }
     if body["org_id"] == user["org_id"]:
         return True, user
-    return False, None
+    return False, f"User {user.get('id')} from another organization then the one that was requested."
 
 @app.get("/your-route/<service>/<action>")
 @firebase_jwt_authenticated(get_user_capabilities, check_access)
 async def your_route_function(
         request: Request = None,
         service: Union[str, None] = None,
         action: Union[str, None] = None
```

### Comparing `kal_middleware-0.0.6/kal_middleware.egg-info/SOURCES.txt` & `kal_middleware-0.0.7/kal_middleware.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/mkdocs.yml` & `kal_middleware-0.0.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kal_middleware-0.0.6/pyproject.toml` & `kal_middleware-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kal-middleware"
-version = "0.0.6"
+version = "0.0.7"
 dynamic = [
     "dependencies",
 ]
 description = "Kaleidoo middleware package"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.6"
+current_version = "0.0.7"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

