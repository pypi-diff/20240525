# Comparing `tmp/dyff_storage-0.8.0.tar.gz` & `tmp/dyff_storage-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_storage-0.8.0.tar", last modified: Thu May 23 22:41:49 2024, max compression
+gzip compressed data, was "dyff_storage-0.9.0.tar", last modified: Fri May 24 22:48:42 2024, max compression
```

## Comparing `dyff_storage-0.8.0.tar` & `dyff_storage-0.9.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.775149 dyff_storage-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-23 22:41:49.775149 dyff_storage-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.762149 dyff_storage-0.8.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.768149 dyff_storage-0.8.0/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.769149 dyff_storage-0.8.0/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.770149 dyff_storage-0.8.0/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2584 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.770149 dyff_storage-0.8.0/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.771149 dyff_storage-0.8.0/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.771149 dyff_storage-0.8.0/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.772149 dyff_storage-0.8.0/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7252 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    23188 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.772149 dyff_storage-0.8.0/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15691 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.774149 dyff_storage-0.8.0/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-23 22:41:49.000000 dyff_storage-0.8.0/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 22:41:49.775149 dyff_storage-0.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 22:41:49.774149 dyff_storage-0.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-23 22:41:43.000000 dyff_storage-0.8.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.635452 dyff_storage-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-24 22:48:42.634452 dyff_storage-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.622452 dyff_storage-0.9.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.628452 dyff_storage-0.9.0/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.628452 dyff_storage-0.9.0/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.630452 dyff_storage-0.9.0/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2584 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.630452 dyff_storage-0.9.0/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.631452 dyff_storage-0.9.0/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.631452 dyff_storage-0.9.0/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.632452 dyff_storage-0.9.0/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7252 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    24465 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.632452 dyff_storage-0.9.0/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15691 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.634452 dyff_storage-0.9.0/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-24 22:48:42.000000 dyff_storage-0.9.0/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 22:48:42.635452 dyff_storage-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 22:48:42.634452 dyff_storage-0.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-24 22:48:36.000000 dyff_storage-0.9.0/tests/test_import.py
```

### Comparing `dyff_storage-0.8.0/.gitignore` & `dyff_storage-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/.gitlab-ci.yml` & `dyff_storage-0.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/.licenserc.yaml` & `dyff_storage-0.9.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/.pre-commit-config.yaml` & `dyff_storage-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/.secrets.baseline` & `dyff_storage-0.9.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/CODE_OF_CONDUCT.md` & `dyff_storage-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/LICENSE` & `dyff_storage-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/PKG-INFO` & `dyff_storage-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.8.0/README.md` & `dyff_storage-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/__init__.py` & `dyff_storage-0.9.0/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/base/auth.py` & `dyff_storage-0.9.0/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/base/command.py` & `dyff_storage-0.9.0/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/base/query.py` & `dyff_storage-0.9.0/dyff/storage/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/base/storage.py` & `dyff_storage-0.9.0/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.9.0/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.9.0/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/mock/command.py` & `dyff_storage-0.9.0/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.9.0/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.9.0/dyff/storage/backend/mongodb/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from __future__ import annotations
 
 import json
 from typing import Collection, Iterable, Optional
 
 import pymongo
 
+from dyff.schema.errors import ClientError
 from dyff.schema.platform import (
     Audit,
     Dataset,
     DataSource,
     Documentation,
     Entities,
     Evaluation,
@@ -88,48 +89,87 @@
                     "$or": [
                         {"account": {"$in": list(whitelist.accounts)}},
                         {"_id": {"$in": list(whitelist.entities)}},
                     ]
                 }
             )
 
-        for k, v in query.items():
-            if v is None:
-                continue
-            if k == "id":
-                k = "_id"
-
-            if k == "labels":
-                labels = json.loads(v)
-                labeled = Labeled(labels=labels)  # validate
-                for label_key, label_value in labeled.labels.items():
-                    mongo_conjunction.append(
-                        {k: {"$elemMatch": {"key": label_key, "value": label_value}}}
+        def json_decode(k: str, v: str):
+            try:
+                return json.loads(v)
+            except json.decoder.JSONDecodeError:
+                raise ClientError(f"{k}: json decode failed")
+
+        def build_query(query: dict) -> list:
+            conjunction: list = []
+            for k, v in query.items():
+                if v is None:
+                    continue
+                if k == "id":
+                    k = "_id"
+
+                if k == "labels":
+                    if isinstance(v, dict):
+                        labels = v
+                    else:
+                        labels = json_decode(k, v)
+                    labeled = Labeled(labels=labels)  # validate
+                    for label_key, label_value in labeled.labels.items():
+                        conjunction.append(
+                            {
+                                k: {
+                                    "$elemMatch": {
+                                        "key": label_key,
+                                        "value": label_value,
+                                    }
+                                }
+                            }
+                        )
+                # TODO:
+                # elif k == "annotations":
+                #     pass
+                elif k == "inputs":
+                    # This is a special query for Analysis-related entities. It
+                    # selects entities that reference any of the listed IDs in
+                    # their .inputs field.
+                    if isinstance(v, list):
+                        entity_list = v
+                    elif isinstance(v, str):
+                        entity_list = v.split(",")
+                    else:
+                        raise ClientError(f"inputs: must be list or str; got {type(v)}")
+                    conjunction.append(
+                        {"inputs": {"$elemMatch": {"entity": {"$in": entity_list}}}}
                     )
-            # TODO:
-            # elif k == "annotations":
-            #     pass
-            elif k == "inputsAnyOf":
-                # This is a special query for Analysis-related entities. It
-                # selects entities that reference any of the listed IDs in
-                # their .inputs field.
-                entity_list = v.split(",")
-                mongo_conjunction.append(
-                    {"inputs": {"$elemMatch": {"entity": {"$in": entity_list}}}}
-                )
-            elif isinstance(v, list):
-                mongo_conjunction.append({k: {"$in": list(v)}})
+                elif isinstance(v, list):
+                    conjunction.append({k: {"$in": list(v)}})
+                else:
+                    conjunction.append({k: v})
+            return conjunction
+
+        json_query_string = query.pop("query", None)
+        if json_query_string is not None:
+            json_query_object = json_decode("query", json_query_string)
+            if isinstance(json_query_object, list):
+                for item in json_query_object:
+                    mongo_conjunction.extend(build_query(item))
+            elif isinstance(json_query_object, dict):
+                mongo_conjunction.extend(build_query(json_query_object))
             else:
-                mongo_conjunction.append({k: v})
+                raise ClientError(
+                    f"query: must parse as dict or list[dict]; got {type(json_query_object)}"
+                )
+
+        mongo_conjunction.extend(build_query(query))
 
-        query = {"$and": mongo_conjunction} if mongo_conjunction else {}
-        print(f"query: {query}")
+        mongo_query = {"$and": mongo_conjunction} if mongo_conjunction else {}
+        print(f"query: {mongo_query}")
         collection_name = Resources.for_kind(kind)
         collection = self._workflows_db[collection_name]
-        results = collection.find(query)
+        results = collection.find(mongo_query)
 
         for result in results:
             yield self._convert_entity_response(result)
 
     def _rename_query_key(self, query_dict: dict, old_key: str, new_key: str) -> None:
         """If query_dict contains a value for old_key, pop the value and add it back at
         new_key."""
@@ -137,105 +177,92 @@
         value = query_dict.pop(old_key, unset)
         if value is not unset:
             query_dict[new_key] = value
 
     def get_audit(self, id: str) -> Optional[Audit]:
         """Retrieve an Audit entity.
 
-        Parameters:
-          id: The unique key of the Audit.
-
-        Returns:
-          The Audit, or None if no Audit with the specified key exists.
+        :param id: The unique key of the Audit.
+        :returns: The Audit, or None if no Audit with the specified key exists.
         """
         result = self._get_entity(Entities.Audit, id)
         return Audit.parse_obj(result) if result else None
 
     def query_audits(
         self, whitelist: Whitelist, query: AuditQueryRequest
     ) -> Collection[Audit]:
         """Retrieve all Audit entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Audit entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Audit entity. The returned
+            entities satisfy 'entity.field==value' for all items 'field: value' in
+            kwargs.
         """
         qdict = query.dict()
         results = self._query_entities(Entities.Audit, whitelist, qdict)
         return [Audit.parse_obj(result) for result in results]
 
     def get_data_source(self, id: str) -> Optional[DataSource]:
         """Retrieve a DataSource entity.
 
-        Parameters:
-          id: The unique key of the DataSource.
-
-        Returns:
-          The DataSource, or None if no DataSource with the specified key exists.
+        :param id: The unique key of the DataSource.
+        :returns: The DataSource, or None if no DataSource with the specified key
+            exists.
         """
         result = self._get_entity(Entities.DataSource, id)
         return DataSource.parse_obj(result) if result else None
 
     def query_data_sources(
         self, whitelist: Whitelist, **query
     ) -> Collection[DataSource]:
         """Retrieve all DataSource entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the DataSource entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the DataSource entity. The
+            returned entities satisfy 'entity.field==value' for all items 'field: value'
+            in kwargs.
         """
         results = self._query_entities(Entities.DataSource, whitelist, query)
         return [DataSource.parse_obj(result) for result in results]
 
     def get_dataset(self, id: str) -> Optional[Dataset]:
         """Retrieve a Dataset entity.
 
-        Parameters:
-          id: The unique key of the Dataset.
-
-        Returns:
-          The Dataset, or None if no Dataset with the specified key exists.
+        :param id: The unique key of the Dataset.
+        :returns: The Dataset, or None if no Dataset with the specified key exists.
         """
         result = self._get_entity(Entities.Dataset, id)
         return Dataset.parse_obj(result) if result else None
 
     def query_datasets(
         self, whitelist: Whitelist, query: DatasetQueryRequest
     ) -> Collection[Dataset]:
         """Retrieve all Dataset entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Dataset entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Dataset entity. The returned
+            entities satisfy 'entity.field==value' for all items 'field: value' in
+            kwargs.
         """
         qdict = query.dict()
         results = self._query_entities(Entities.Dataset, whitelist, qdict)
         return [Dataset.parse_obj(result) for result in results]
 
     def edit_documentation(
         self, id: str, edit: DocumentationEditRequest
     ) -> Optional[Documentation]:
         """Edit the Documentation entity associated with a resource.
 
-        Parameters:
-          id: ID of the documented resource.
-          edit: Edit request containing changes to make to the documentation.
-
-        Returns:
-          The new Documentation, or None if no resource exists with the given ID.
+        :param id: ID of the documented resource.
+        :param edit: Edit request containing changes to make to the documentation.
+        :returns: The new Documentation, or None if no resource exists with the given
+            ID.
         """
         collection = self._workflows_db["documentation"]
         # Users can explicitly set a field to None, but we don't want to
         # overwrite with None implicitly
         edit_dict = edit.dict(exclude_unset=True)
         result = collection.find_one_and_update(
             {"_id": id},
@@ -247,50 +274,44 @@
             return None
         del result["_id"]
         return Documentation.parse_obj(result)
 
     def get_documentation(self, id: str) -> Optional[Documentation]:
         """Retrieve the Documentation entity associated with a resource.
 
-        Parameters:
-          id: ID of the documented resource.
-
-        Returns:
-          The Documentation, or None if no resource exists with the given ID.
+        :param id: ID of the documented resource.
+        :returns: The Documentation, or None if no resource exists with the given ID.
         """
         collection = self._workflows_db["documentation"]
         result = collection.find_one({"_id": id})
         if result is None:
             return None
         del result["_id"]
         return Documentation.parse_obj(result)
 
     def get_evaluation(self, id: str) -> Optional[Evaluation]:
         """Retrieve an Evaluation entity.
 
-        Parameters:
-          id: The unique key of the Evaluation.
-
-        Returns:
-          The Evaluation, or None if no Evaluation with the specified key exists.
+        :param id: The unique key of the Evaluation.
+        :returns: The Evaluation, or None if no Evaluation with the specified key
+            exists.
         """
         result = self._get_entity(Entities.Evaluation, id)
         return Evaluation.parse_obj(result) if result else None
 
     def query_evaluations(
         self, whitelist: Whitelist, query: EvaluationQueryRequest
     ) -> Collection[Evaluation]:
         """Retrieve all Evaluation entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Evaluation entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Evaluation entity. The
+            returned entities satisfy 'entity.field==value' for all items 'field: value'
+            in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(
             qdict, "inferenceService", "inferenceSession.inferenceService.id"
         )
         self._rename_query_key(
             qdict, "inferenceServiceName", "inferenceSession.inferenceService.name"
@@ -303,290 +324,253 @@
         )
         results = self._query_entities(Entities.Evaluation, whitelist, qdict)
         return [Evaluation.parse_obj(result) for result in results]
 
     def get_family(self, id: str) -> Optional[Family]:
         """Retrieve a Family entity.
 
-        Parameters:
-          id: The unique ID of the Family.
-
-        Returns:
-          The Family, or None if no Family with the specified ID exists.
+        :param id: The unique ID of the Family.
+        :returns: The Family, or None if no Family with the specified ID exists.
         """
         result = self._get_entity(Entities.Family, id)
         return Family.parse_obj(result) if result else None
 
     def get_inference_service(self, id: str) -> Optional[InferenceService]:
         """Retrieve an InferenceService entity.
 
-        Parameters:
-          id: The unique key of the InferenceService.
-
-        Returns:
-          The InferenceService, or None if no InferenceService with the specified key exists.
+        :param id: The unique key of the InferenceService.
+        :returns: The InferenceService, or None if no InferenceService with the
+            specified key exists.
         """
         result = self._get_entity(Entities.InferenceService, id)
         return InferenceService.parse_obj(result) if result else None
 
     def query_inference_services(
         self, whitelist: Whitelist, query: InferenceServiceQueryRequest
     ) -> Collection[InferenceService]:
         """Retrieve all InferenceService entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the InferenceService entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the InferenceService entity. The
+            returned entities satisfy 'entity.field==value' for all items 'field: value'
+            in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "model", "model.id")
         self._rename_query_key(qdict, "modelName", "model.name")
         results = self._query_entities(Entities.InferenceService, whitelist, qdict)
         return [InferenceService.parse_obj(result) for result in results]
 
     def get_inference_session(self, id: str) -> Optional[InferenceSession]:
         """Retrieve an InferenceSession entity.
 
-        Parameters:
-          id: The unique key of the InferenceSession.
-
-        Returns:
-          The InferenceSession, or None if no InferenceSession with the specified key exists.
+        :param id: The unique key of the InferenceSession.
+        :returns: The InferenceSession, or None if no InferenceSession with the
+            specified key exists.
         """
         result = self._get_entity(Entities.InferenceSession, id)
         return InferenceSession.parse_obj(result) if result else None
 
     def query_inference_sessions(
         self, whitelist: Whitelist, query: InferenceSessionQueryRequest
     ) -> Collection[InferenceSession]:
         """Retrieve all InferenceSession entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the InferenceSession entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the InferenceSession entity. The
+            returned entities satisfy 'entity.field==value' for all items 'field: value'
+            in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "inferenceService", "inferenceService.id")
         self._rename_query_key(qdict, "inferenceServiceName", "inferenceService.name")
         self._rename_query_key(qdict, "model", "inferenceService.model.id")
         self._rename_query_key(qdict, "modelName", "inferenceService.model.name")
         results = self._query_entities(Entities.InferenceSession, whitelist, qdict)
         return [InferenceSession.parse_obj(result) for result in results]
 
     def get_measurement(self, id: str) -> Optional[Measurement]:
         """Retrieve a Measurement entity.
 
-        Parameters:
-          id: The unique key of the Measurement.
-
-        Returns:
-          The Measurement, or None if no Measurement with the specified key exists.
+        :param id: The unique key of the Measurement.
+        :returns: The Measurement, or None if no Measurement with the specified key
+            exists.
         """
         result = self._get_entity(Entities.Measurement, id)
         return Measurement.parse_obj(result) if result else None
 
     def query_measurements(
         self, whitelist: Whitelist, query: MeasurementQueryRequest
     ) -> Collection[Measurement]:
         """Retrieve all Measurement entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Measurement entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Measurement entity. The
+            returned entities satisfy 'entity.field==value' for all items 'field: value'
+            in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "method", "method.id")
         self._rename_query_key(qdict, "methodName", "method.name")
         self._rename_query_key(qdict, "dataset", "scope.dataset")
         self._rename_query_key(qdict, "evaluation", "scope.evaluation")
         self._rename_query_key(qdict, "inferenceService", "scope.inferenceService")
         self._rename_query_key(qdict, "model", "scope.model")
         results = self._query_entities(Entities.Measurement, whitelist, qdict)
         return [Measurement.parse_obj(result) for result in results]
 
     def get_method(self, id: str) -> Optional[Method]:
         """Retrieve a Method entity.
 
-        Parameters:
-          id: The unique key of the Method.
-
-        Returns:
-          The Method, or None if no Method with the specified key exists.
+        :param id: The unique key of the Method.
+        :returns: The Method, or None if no Method with the specified key exists.
         """
         result = self._get_entity(Entities.Method, id)
         return Method.parse_obj(result) if result else None
 
     def query_methods(
         self, whitelist: Whitelist, query: MethodQueryRequest
     ) -> Collection[Method]:
         """Retrieve all Method entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Method entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Method entity. The returned
+            entities satisfy 'entity.field==value' for all items 'field: value' in
+            kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "outputKind", "output.kind")
         results = self._query_entities(Entities.Method, whitelist, qdict)
         return [Method.parse_obj(result) for result in results]
 
     def get_model(self, id: str) -> Optional[Model]:
         """Retrieve a Model entity.
 
-        Parameters:
-          id: The unique key of the Model.
-
-        Returns:
-          The Model, or None if no Model with the specified key exists.
+        :param id: The unique key of the Model.
+        :returns: The Model, or None if no Model with the specified key exists.
         """
         result = self._get_entity(Entities.Model, id)
         return Model.parse_obj(result) if result else None
 
     def query_models(
         self, whitelist: Whitelist, query: ModelQueryRequest
     ) -> Collection[Model]:
         """Retrieve all Model entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Model entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Model entity. The returned
+            entities satisfy 'entity.field==value' for all items 'field: value' in
+            kwargs.
         """
         qdict = query.dict()
         results = self._query_entities(Entities.Model, whitelist, qdict)
         return [Model.parse_obj(result) for result in results]
 
     def get_module(self, id: str) -> Optional[Module]:
         """Retrieve a Module entity.
 
-        Parameters:
-          id: The unique key of the Module.
-
-        Returns:
-          The Module, or None if no Module with the specified key exists.
+        :param id: The unique key of the Module.
+        :returns: The Module, or None if no Module with the specified key exists.
         """
         result = self._get_entity(Entities.Module, id)
         return Module.parse_obj(result) if result else None
 
     def query_modules(
         self, whitelist: Whitelist, query: ModuleQueryRequest
     ) -> Collection[Module]:
         """Retrieve all Module entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Module entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Module entity. The returned
+            entities satisfy 'entity.field==value' for all items 'field: value' in
+            kwargs.
         """
         qdict = query.dict()
         results = self._query_entities(Entities.Module, whitelist, qdict)
         return [Module.parse_obj(result) for result in results]
 
     def get_report(self, id: str) -> Optional[Report]:
         """Retrieve a Report entity.
 
-        Parameters:
-          id: The unique key of the Report.
-
-        Returns:
-          The Report, or None if no Report with the specified key exists.
+        :param id: The unique key of the Report.
+        :returns: The Report, or None if no Report with the specified key exists.
         """
         result = self._get_entity(Entities.Report, id)
         return Report.parse_obj(result) if result else None
 
     def query_reports(
         self, whitelist: Whitelist, query: ReportQueryRequest
     ) -> Collection[Report]:
         """Retrieve all Report entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the Report entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the Report entity. The returned
+            entities satisfy 'entity.field==value' for all items 'field: value' in
+            kwargs.
         """
         qdict = query.dict()
         results = self._query_entities(Entities.Report, whitelist, qdict)
         return [Report.parse_obj(result) for result in results]
 
     def get_safetycase(self, id: str) -> Optional[SafetyCase]:
         """Retrieve a SafetyCase entity.
 
-        Parameters:
-          id: The unique key of the SafetyCase.
-
-        Returns:
-          The SafetyCase, or None if no SafetyCase with the specified key exists.
+        :param id: The unique key of the SafetyCase.
+        :returns: The SafetyCase, or None if no SafetyCase with the specified key
+            exists.
         """
         result = self._get_entity(Entities.SafetyCase, id)
         return SafetyCase.parse_obj(result) if result else None
 
     def query_safetycases(
         self, whitelist: Whitelist, query: SafetyCaseQueryRequest
     ) -> Collection[SafetyCase]:
         """Retrieve all SafetyCase entities matching the query parameters.
 
-        Parameters:
-          whitelist: The set of accounts and entities that the caller has
-            been granted access to.
-          **query: Equality constraints on fields of the SafetyCase entity.
-            The returned entities satisfy 'entity.field==value' for all items
-            'field: value' in kwargs.
+        :param whitelist: The set of accounts and entities that the caller has been
+            granted access to.
+        :param query: Equality constraints on fields of the SafetyCase entity. The
+            returned entities satisfy 'entity.field==value' for all items 'field: value'
+            in kwargs.
         """
         qdict = query.dict()
         self._rename_query_key(qdict, "method", "method.id")
         self._rename_query_key(qdict, "methodName", "method.name")
         self._rename_query_key(qdict, "dataset", "scope.dataset")
         self._rename_query_key(qdict, "evaluation", "scope.evaluation")
         self._rename_query_key(qdict, "inferenceService", "scope.inferenceService")
         self._rename_query_key(qdict, "model", "scope.model")
         results = self._query_entities(Entities.SafetyCase, whitelist, qdict)
         return [SafetyCase.parse_obj(result) for result in results]
 
     def get_tag(self, id: str) -> Optional[Tag]:
         """Retrieve a Tag entity.
 
-        Parameters:
-          id: The unique ID of the Tag.
-
-        Returns:
-          The Tag, or None if no Tag with the specified ID exists.
+        :param id: The unique ID of the Tag.
+        :returns: The Tag, or None if no Tag with the specified ID exists.
         """
         result = self._get_entity(Entities.Tag, id)
         return Tag.parse_obj(result) if result else None
 
     def create_tag(self, family: str, tag_request: TagCreateRequest) -> Optional[Tag]:
         """Create a new Tag in an existing Family. Has no effect and returns None if a
         tag with the same name already exists.
 
-        Parameters:
-          family: The ID of the Family to add the tag to.
-          request: TagCreateRequest
-
-        Returns:
-          The created Tag, or None if no Tag was created. This could be because
-          the Family doesn't exist, or because a tag with the same name already
-          exists in the family.
+        :param family: The ID of the Family to add the tag to.
+        :param request: TagCreateRequest
+        :returns: The created Tag, or None if no Tag was created. This could be because
+            the Family doesn't exist, or because a tag with the same name already exists
+            in the family.
         """
         tag_dict = tag_request.dict()
         tag_dict["created"] = timestamp.now()
         new_tag = Tag.parse_obj(tag_dict)
         families_collection = self._workflows_db[Resources.Family]
         # Atomically check if the tag exists and add it only if it does not exist
         result = families_collection.update_one(
```

### Comparing `dyff_storage-0.8.0/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.9.0/dyff/storage/backend/s3/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/config.py` & `dyff_storage-0.9.0/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/paths.py` & `dyff_storage-0.9.0/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff/storage/timestamp.py` & `dyff_storage-0.9.0/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.9.0/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.8.0/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.9.0/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/makefile` & `dyff_storage-0.9.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/pyproject.toml` & `dyff_storage-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.8.0/tests/test_import.py` & `dyff_storage-0.9.0/tests/test_import.py`

 * *Files identical despite different names*

