# Comparing `tmp/dyff_client-0.7.0.tar.gz` & `tmp/dyff_client-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_client-0.7.0.tar", last modified: Wed May 22 20:49:48 2024, max compression
+gzip compressed data, was "dyff_client-0.8.0.tar", last modified: Sat May 25 00:52:37 2024, max compression
```

## Comparing `dyff_client-0.7.0.tar` & `dyff_client-0.8.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.377713 dyff_client-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-22 20:49:41.000000 dyff_client-0.7.0/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-22 20:49:41.000000 dyff_client-0.7.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-22 20:49:41.000000 dyff_client-0.7.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-22 20:49:41.000000 dyff_client-0.7.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-05-22 20:49:48.376713 dyff_client-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-22 20:49:41.000000 dyff_client-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.361713 dyff_client-0.7.0/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.366713 dyff_client-0.7.0/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.368713 dyff_client-0.7.0/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6489 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.369713 dyff_client-0.7.0/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6649 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.371713 dyff_client-0.7.0/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   842746 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.373713 dyff_client-0.7.0/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   900914 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    83364 2024-05-22 20:49:41.000000 dyff_client-0.7.0/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.376713 dyff_client-0.7.0/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-22 20:49:48.000000 dyff_client-0.7.0/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-22 20:49:41.000000 dyff_client-0.7.0/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-22 20:49:41.000000 dyff_client-0.7.0/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-22 20:49:41.000000 dyff_client-0.7.0/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-22 20:49:41.000000 dyff_client-0.7.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.362713 dyff_client-0.7.0/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.374713 dyff_client-0.7.0/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.375713 dyff_client-0.7.0/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-22 20:49:41.000000 dyff_client-0.7.0/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 20:49:48.377713 dyff_client-0.7.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:49:48.375713 dyff_client-0.7.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-22 20:49:41.000000 dyff_client-0.7.0/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.057973 dyff_client-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-25 00:52:30.000000 dyff_client-0.8.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1778 2024-05-25 00:52:30.000000 dyff_client-0.8.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-25 00:52:30.000000 dyff_client-0.8.0/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-25 00:52:30.000000 dyff_client-0.8.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-25 00:52:30.000000 dyff_client-0.8.0/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-25 00:52:30.000000 dyff_client-0.8.0/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-25 00:52:30.000000 dyff_client-0.8.0/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-25 00:52:30.000000 dyff_client-0.8.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-25 00:52:30.000000 dyff_client-0.8.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-25 00:52:37.056973 dyff_client-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-25 00:52:30.000000 dyff_client-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.041973 dyff_client-0.8.0/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.046973 dyff_client-0.8.0/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.048973 dyff_client-0.8.0/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.049973 dyff_client-0.8.0/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6649 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.051973 dyff_client-0.8.0/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   844066 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.053973 dyff_client-0.8.0/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   903394 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    85410 2024-05-25 00:52:30.000000 dyff_client-0.8.0/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.056973 dyff_client-0.8.0/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-25 00:52:37.000000 dyff_client-0.8.0/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-25 00:52:37.000000 dyff_client-0.8.0/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 00:52:37.000000 dyff_client-0.8.0/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-25 00:52:37.000000 dyff_client-0.8.0/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-25 00:52:37.000000 dyff_client-0.8.0/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-25 00:52:30.000000 dyff_client-0.8.0/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-25 00:52:30.000000 dyff_client-0.8.0/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-25 00:52:30.000000 dyff_client-0.8.0/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-25 00:52:30.000000 dyff_client-0.8.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.042973 dyff_client-0.8.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.054973 dyff_client-0.8.0/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-25 00:52:30.000000 dyff_client-0.8.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-25 00:52:30.000000 dyff_client-0.8.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.055973 dyff_client-0.8.0/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-25 00:52:30.000000 dyff_client-0.8.0/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-25 00:52:30.000000 dyff_client-0.8.0/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-25 00:52:30.000000 dyff_client-0.8.0/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-25 00:52:30.000000 dyff_client-0.8.0/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-25 00:52:37.057973 dyff_client-0.8.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 00:52:37.056973 dyff_client-0.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-25 00:52:30.000000 dyff_client-0.8.0/tests/test_import.py
```

### Comparing `dyff_client-0.7.0/.gitlab-ci.yml` & `dyff_client-0.8.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/.licenserc.yaml` & `dyff_client-0.8.0/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/.pre-commit-config.yaml` & `dyff_client-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/.secrets.baseline` & `dyff_client-0.8.0/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/CODE_OF_CONDUCT.md` & `dyff_client-0.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/LICENSE` & `dyff_client-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/PKG-INFO` & `dyff_client-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.7.0/README.md` & `dyff_client-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/__init__.py` & `dyff_client-0.8.0/dyff/client/_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/_client.py` & `dyff_client-0.8.0/dyff/client/_generated/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/_configuration.py` & `dyff_client-0.8.0/dyff/client/_generated/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/_patch.py` & `dyff_client-0.8.0/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/_serialization.py` & `dyff_client-0.8.0/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/_vendor.py` & `dyff_client-0.8.0/dyff/client/_generated/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/__init__.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/_client.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/_client.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/_configuration.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/_patch.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/_vendor.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/operations/__init__.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/operations/_operations.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,14 +358,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs: Any,
@@ -374,14 +375,16 @@
         """Get all Datasets matching a query.
 
         Get all Datasets matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -520,14 +523,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_datasets_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             headers=_headers,
@@ -2271,14 +2275,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         dataset: Optional[str] = None,
         inference_service: Optional[str] = None,
@@ -2291,14 +2296,16 @@
         """Get all Evaluations matching a query.
 
         Get all Evaluations matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -2561,14 +2568,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_evaluations_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             dataset=dataset,
             inference_service=inference_service,
@@ -4174,14 +4182,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         model: Optional[str] = None,
@@ -4192,14 +4201,16 @@
         """Get all InferenceServices matching a query.
 
         Get all InferenceServices matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -4404,14 +4415,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_inferenceservices_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             model=model,
@@ -6216,14 +6228,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         inference_service: Optional[str] = None,
@@ -6236,14 +6249,16 @@
         """Get all InferenceSessions matching a query.
 
         Get all InferenceSessions matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -6486,14 +6501,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_inferencesessions_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             inference_service=inference_service,
@@ -8398,36 +8414,39 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
         dataset: Optional[str] = None,
         evaluation: Optional[str] = None,
         inference_service: Optional[str] = None,
         model: Optional[str] = None,
-        inputs_any_of: Optional[str] = None,
+        inputs: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all Measurements matching a query.
 
         Get all Measurements matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -8442,16 +8461,16 @@
         :paramtype dataset: str
         :keyword evaluation: Default value is None.
         :paramtype evaluation: str
         :keyword inference_service: Default value is None.
         :paramtype inference_service: str
         :keyword model: Default value is None.
         :paramtype model: str
-        :keyword inputs_any_of: Default value is None.
-        :paramtype inputs_any_of: str
+        :keyword inputs: Default value is None.
+        :paramtype inputs: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -8657,26 +8676,27 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_measurements_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             method=method,
             method_name=method_name,
             dataset=dataset,
             evaluation=evaluation,
             inference_service=inference_service,
             model=model,
-            inputs_any_of=inputs_any_of,
+            inputs=inputs,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -10116,14 +10136,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         output_kind: Optional[str] = None,
@@ -10133,14 +10154,16 @@
         """Get all Methods matching a query.
 
         Get all Methods matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -10302,14 +10325,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_methods_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             output_kind=output_kind,
@@ -11903,14 +11927,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs: Any,
@@ -11919,14 +11944,16 @@
         """Get all Models matching a query.
 
         Get all Models matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -12066,14 +12093,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_models_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             headers=_headers,
@@ -13558,14 +13586,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs: Any,
@@ -13574,14 +13603,16 @@
         """Get all Modules matching a query.
 
         Get all Modules matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -13672,14 +13703,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_modules_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             headers=_headers,
@@ -15151,14 +15183,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         report: Optional[str] = None,
         dataset: Optional[str] = None,
@@ -15171,14 +15204,16 @@
         """Get all Reports matching a query.
 
         Get all Reports matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -15336,14 +15371,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_reports_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             report=report,
             dataset=dataset,
@@ -16522,36 +16558,39 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
     async def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
         dataset: Optional[str] = None,
         evaluation: Optional[str] = None,
         inference_service: Optional[str] = None,
         model: Optional[str] = None,
-        inputs_any_of: Optional[str] = None,
+        inputs: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all SafetyCase entities matching a query.
 
         Get all SafetyCase entities matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -16566,16 +16605,16 @@
         :paramtype dataset: str
         :keyword evaluation: Default value is None.
         :paramtype evaluation: str
         :keyword inference_service: Default value is None.
         :paramtype inference_service: str
         :keyword model: Default value is None.
         :paramtype model: str
-        :keyword inputs_any_of: Default value is None.
-        :paramtype inputs_any_of: str
+        :keyword inputs: Default value is None.
+        :paramtype inputs: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -16763,26 +16802,27 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_safetycases_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             method=method,
             method_name=method_name,
             dataset=dataset,
             evaluation=evaluation,
             inference_service=inference_service,
             model=model,
-            inputs_any_of=inputs_any_of,
+            inputs=inputs,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
```

### Comparing `dyff_client-0.7.0/dyff/client/_generated/aio/operations/_patch.py` & `dyff_client-0.8.0/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/operations/__init__.py` & `dyff_client-0.8.0/dyff/client/_generated/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/_generated/operations/_operations.py` & `dyff_client-0.8.0/dyff/client/_generated/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_datasets_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     name: Optional[str] = None,
     **kwargs: Any,
@@ -92,14 +93,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/datasets"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -307,14 +310,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_evaluations_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     dataset: Optional[str] = None,
     inference_service: Optional[str] = None,
@@ -328,14 +332,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/evaluations"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -471,14 +477,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_inferenceservices_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     name: Optional[str] = None,
     model: Optional[str] = None,
@@ -490,14 +497,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/inferenceservices"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -655,14 +664,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_inferencesessions_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     name: Optional[str] = None,
     inference_service: Optional[str] = None,
@@ -676,14 +686,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/inferencesessions"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -892,37 +904,40 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_measurements_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     method: Optional[str] = None,
     method_name: Optional[str] = None,
     dataset: Optional[str] = None,
     evaluation: Optional[str] = None,
     inference_service: Optional[str] = None,
     model: Optional[str] = None,
-    inputs_any_of: Optional[str] = None,
+    inputs: Optional[str] = None,
     **kwargs: Any,
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/measurements"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -939,18 +954,16 @@
         _params["evaluation"] = _SERIALIZER.query("evaluation", evaluation, "str")
     if inference_service is not None:
         _params["inferenceService"] = _SERIALIZER.query(
             "inference_service", inference_service, "str"
         )
     if model is not None:
         _params["model"] = _SERIALIZER.query("model", model, "str")
-    if inputs_any_of is not None:
-        _params["inputsAnyOf"] = _SERIALIZER.query(
-            "inputs_any_of", inputs_any_of, "str"
-        )
+    if inputs is not None:
+        _params["inputs"] = _SERIALIZER.query("inputs", inputs, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(
         method="GET", url=_url, params=_params, headers=_headers, **kwargs
     )
@@ -1062,14 +1075,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_methods_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     name: Optional[str] = None,
     output_kind: Optional[str] = None,
@@ -1080,14 +1094,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/methods"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -1237,14 +1253,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_models_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     name: Optional[str] = None,
     **kwargs: Any,
@@ -1254,14 +1271,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/models"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -1409,14 +1428,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_modules_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     name: Optional[str] = None,
     **kwargs: Any,
@@ -1426,14 +1446,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/modules"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -1641,14 +1663,15 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_reports_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     report: Optional[str] = None,
     dataset: Optional[str] = None,
@@ -1662,14 +1685,16 @@
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/reports"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -1799,37 +1824,40 @@
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
 
 
 def build_safetycases_query_request(
     *,
+    query: Optional[str] = None,
     id: Optional[str] = None,
     account: Optional[str] = None,
     status: Optional[str] = None,
     reason: Optional[str] = None,
     labels: Optional[str] = None,
     method: Optional[str] = None,
     method_name: Optional[str] = None,
     dataset: Optional[str] = None,
     evaluation: Optional[str] = None,
     inference_service: Optional[str] = None,
     model: Optional[str] = None,
-    inputs_any_of: Optional[str] = None,
+    inputs: Optional[str] = None,
     **kwargs: Any,
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/safetycases"
 
     # Construct parameters
+    if query is not None:
+        _params["query"] = _SERIALIZER.query("query", query, "str")
     if id is not None:
         _params["id"] = _SERIALIZER.query("id", id, "str")
     if account is not None:
         _params["account"] = _SERIALIZER.query("account", account, "str")
     if status is not None:
         _params["status"] = _SERIALIZER.query("status", status, "str")
     if reason is not None:
@@ -1846,18 +1874,16 @@
         _params["evaluation"] = _SERIALIZER.query("evaluation", evaluation, "str")
     if inference_service is not None:
         _params["inferenceService"] = _SERIALIZER.query(
             "inference_service", inference_service, "str"
         )
     if model is not None:
         _params["model"] = _SERIALIZER.query("model", model, "str")
-    if inputs_any_of is not None:
-        _params["inputsAnyOf"] = _SERIALIZER.query(
-            "inputs_any_of", inputs_any_of, "str"
-        )
+    if inputs is not None:
+        _params["inputs"] = _SERIALIZER.query("inputs", inputs, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(
         method="GET", url=_url, params=_params, headers=_headers, **kwargs
     )
@@ -2178,14 +2204,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs: Any,
@@ -2194,14 +2221,16 @@
         """Get all Datasets matching a query.
 
         Get all Datasets matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -2340,14 +2369,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_datasets_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             headers=_headers,
@@ -4089,14 +4119,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         dataset: Optional[str] = None,
         inference_service: Optional[str] = None,
@@ -4109,14 +4140,16 @@
         """Get all Evaluations matching a query.
 
         Get all Evaluations matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -4379,14 +4412,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_evaluations_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             dataset=dataset,
             inference_service=inference_service,
@@ -5990,14 +6024,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         model: Optional[str] = None,
@@ -6008,14 +6043,16 @@
         """Get all InferenceServices matching a query.
 
         Get all InferenceServices matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -6220,14 +6257,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_inferenceservices_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             model=model,
@@ -8032,14 +8070,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         inference_service: Optional[str] = None,
@@ -8052,14 +8091,16 @@
         """Get all InferenceSessions matching a query.
 
         Get all InferenceSessions matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -8302,14 +8343,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_inferencesessions_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             inference_service=inference_service,
@@ -10214,36 +10256,39 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
         dataset: Optional[str] = None,
         evaluation: Optional[str] = None,
         inference_service: Optional[str] = None,
         model: Optional[str] = None,
-        inputs_any_of: Optional[str] = None,
+        inputs: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all Measurements matching a query.
 
         Get all Measurements matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -10258,16 +10303,16 @@
         :paramtype dataset: str
         :keyword evaluation: Default value is None.
         :paramtype evaluation: str
         :keyword inference_service: Default value is None.
         :paramtype inference_service: str
         :keyword model: Default value is None.
         :paramtype model: str
-        :keyword inputs_any_of: Default value is None.
-        :paramtype inputs_any_of: str
+        :keyword inputs: Default value is None.
+        :paramtype inputs: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -10473,26 +10518,27 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_measurements_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             method=method,
             method_name=method_name,
             dataset=dataset,
             evaluation=evaluation,
             inference_service=inference_service,
             model=model,
-            inputs_any_of=inputs_any_of,
+            inputs=inputs,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
@@ -11930,14 +11976,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         output_kind: Optional[str] = None,
@@ -11947,14 +11994,16 @@
         """Get all Methods matching a query.
 
         Get all Methods matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -12116,14 +12165,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_methods_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             output_kind=output_kind,
@@ -13717,14 +13767,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs: Any,
@@ -13733,14 +13784,16 @@
         """Get all Models matching a query.
 
         Get all Models matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -13880,14 +13933,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_models_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             headers=_headers,
@@ -15372,14 +15426,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         name: Optional[str] = None,
         **kwargs: Any,
@@ -15388,14 +15443,16 @@
         """Get all Modules matching a query.
 
         Get all Modules matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -15486,14 +15543,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_modules_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             name=name,
             headers=_headers,
@@ -16965,14 +17023,15 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         report: Optional[str] = None,
         dataset: Optional[str] = None,
@@ -16985,14 +17044,16 @@
         """Get all Reports matching a query.
 
         Get all Reports matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -17150,14 +17211,15 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_reports_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             report=report,
             dataset=dataset,
@@ -18336,36 +18398,39 @@
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
     @distributed_trace
     def query(
         self,
         *,
+        query: Optional[str] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[str] = None,
         method: Optional[str] = None,
         method_name: Optional[str] = None,
         dataset: Optional[str] = None,
         evaluation: Optional[str] = None,
         inference_service: Optional[str] = None,
         model: Optional[str] = None,
-        inputs_any_of: Optional[str] = None,
+        inputs: Optional[str] = None,
         **kwargs: Any,
     ) -> Union[List[JSON], JSON]:
         # pylint: disable=line-too-long
         """Get all SafetyCase entities matching a query.
 
         Get all SafetyCase entities matching a query.
 
         The query is a set of equality constraints specified as key-value
         pairs.
 
+        :keyword query: Default value is None.
+        :paramtype query: str
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -18380,16 +18445,16 @@
         :paramtype dataset: str
         :keyword evaluation: Default value is None.
         :paramtype evaluation: str
         :keyword inference_service: Default value is None.
         :paramtype inference_service: str
         :keyword model: Default value is None.
         :paramtype model: str
-        :keyword inputs_any_of: Default value is None.
-        :paramtype inputs_any_of: str
+        :keyword inputs: Default value is None.
+        :paramtype inputs: str
         :return: list of JSON object or JSON object
         :rtype: list[JSON] or JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -18577,26 +18642,27 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
 
         _request = build_safetycases_query_request(
+            query=query,
             id=id,
             account=account,
             status=status,
             reason=reason,
             labels=labels,
             method=method,
             method_name=method_name,
             dataset=dataset,
             evaluation=evaluation,
             inference_service=inference_service,
             model=model,
-            inputs_any_of=inputs_any_of,
+            inputs=inputs,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = (
```

### Comparing `dyff_client-0.7.0/dyff/client/_generated/operations/_patch.py` & `dyff_client-0.8.0/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/dyff/client/client.py` & `dyff_client-0.8.0/dyff/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import json
 import sys
 import time
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Callable, Optional, TypeVar
+from typing import Any, Callable, Optional, TypeVar, Union
 from warnings import warn
 
 import httpx
 from azure.core.credentials import AccessToken, TokenCredential
 
 # We bring this into our namespace so that people can catch it without being
 # confused by having to import 'azure.core'
@@ -109,23 +109,34 @@
 ]
 
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
+QueryT = Union[str, dict[str, Any], list[dict[str, Any]]]
+
+
 def _require_id(x: DyffEntity | str) -> str:
     if isinstance(x, str):
         return x
     elif x.id is not None:
         return x.id
     else:
         raise ValueError(".id attribute not set")
 
 
+def _encode_query(query: QueryT | None) -> Optional[str]:
+    if query is None:
+        return None
+    elif isinstance(query, (list, dict)):
+        query = json.dumps(query)
+    return query
+
+
 def _encode_labels(labels: Optional[dict[str, str]]) -> Optional[str]:
     """The Python client accepts 'annotations' and 'labels' as dicts, but they need to
     be json-encoded so that they can be forwarded as part of the HTTP query
     parameters."""
     if labels is None:
         return None
     # validate
@@ -328,24 +339,27 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(dataset_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
     ) -> list[Dataset]:
         """Get all Datasets matching a query. The query is a set of equality constraints
         specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
         :keyword reason:
@@ -357,14 +371,15 @@
         :return: list of ``Dataset`` resources satisfying the query.
         :rtype: list[Dataset]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Dataset.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
             )
@@ -587,28 +602,31 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(evaluation_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         dataset: Optional[str] = None,
         inferenceService: Optional[str] = None,
         inferenceServiceName: Optional[str] = None,
         model: Optional[str] = None,
         modelName: Optional[str] = None,
     ) -> list[Evaluation]:
         """Get all Evaluations matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
         :keyword reason:
@@ -628,14 +646,15 @@
         :return: list of ``Evaluation`` resources satisfying the query.
         :rtype: list[Evaluation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Evaluation.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 dataset=dataset,
                 inference_service=inferenceService,
@@ -734,26 +753,29 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(service_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
         model: Optional[str] = None,
         modelName: Optional[str] = None,
     ) -> list[InferenceService]:
         """Get all InferenceServices matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
         :keyword reason:
@@ -769,14 +791,15 @@
         :return: list of ``InferenceService`` resources satisfying the query.
         :rtype: list[InferenceService]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             InferenceService.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
                 model=model,
@@ -904,28 +927,31 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(session_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
         inferenceService: Optional[str] = None,
         inferenceServiceName: Optional[str] = None,
         model: Optional[str] = None,
         modelName: Optional[str] = None,
     ) -> list[InferenceSession]:
         """Get all InferenceSessions matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
         :keyword reason:
@@ -941,14 +967,15 @@
         :return: list of ``InferenceSession`` resources satisfying the query.
         :rtype: list[InferenceSession]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             InferenceSession.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
                 inference_service=inferenceService,
@@ -1132,14 +1159,15 @@
         :return: The Measurement with the given ID.
         """
         return Measurement.parse_obj(self._raw_ops.get(measurement_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         method: Optional[str] = None,
         methodName: Optional[str] = None,
@@ -1148,14 +1176,16 @@
         inferenceService: Optional[str] = None,
         model: Optional[str] = None,
         inputsAnyOf: Optional[list[str]] = None,
     ) -> list[Measurement]:
         """Get all Measurement entities matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -1179,14 +1209,15 @@
         :return: Entities matching the query
         :rtype: list[Measurement]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Measurement.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 method=method,
                 method_name=methodName,
@@ -1286,39 +1317,43 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(analysis_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
         output_kind: Optional[str] = None,
     ) -> list[Method]:
         """Get all Method entities matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
-        :keyword id: Default value is None.
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]] :keyword id:
+            Default value is None.
         :paramtype id: str :keyword account: Default value is None.
         :paramtype account: str :keyword status: Default value is None.
         :paramtype status: str :keyword reason: Default value is None.
         :paramtype reason: str :keyword labels: Default value is None.
         :paramtype labels: dict[str, str] :keyword name: Default value is None.
         :paramtype name: str :keyword output_kind: Default value is None.
         :paramtype output_kind: str
         :return: list of Method entities matching query
         :rtype: list[Method] :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Method.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
                 output_kind=output_kind,
@@ -1421,24 +1456,27 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(model_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
     ) -> list[Model]:
         """Get all Models matching a query. The query is a set of equality constraints
         specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
         :keyword reason:
@@ -1450,14 +1488,15 @@
         :return: list of ``Model`` resources satisfying the query.
         :rtype: list[Model]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Model.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
             )
@@ -1579,24 +1618,27 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(module_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         name: Optional[str] = None,
     ) -> list[Module]:
         """Get all Modules matching a query. The query is a set of equality constraints
         specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
         :keyword reason:
@@ -1608,14 +1650,15 @@
         :return: list of ``Module`` resources satisfying the query.
         :rtype: list[Module]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Module.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 name=name,
             )
@@ -1835,28 +1878,31 @@
         :rtype: dyff.schema.platform.Status
         """
         return Status.parse_obj(self._raw_ops.delete(report_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         report: Optional[str] = None,
         dataset: Optional[str] = None,
         evaluation: Optional[str] = None,
         inferenceService: Optional[str] = None,
         model: Optional[str] = None,
     ) -> list[Report]:
         """Get all Reports matching a query. The query is a set of equality constraints
         specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id:
         :paramtype id: str
         :keyword account:
         :paramtype account: str
         :keyword status:
         :paramtype status: str
         :keyword reason:
@@ -1876,14 +1922,15 @@
         :return: list of ``Report`` resources satisfying the query.
         :rtype: list[Report]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             Report.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 report=report,
                 dataset=dataset,
@@ -1974,14 +2021,15 @@
         :return: The SafetyCase with the given ID.
         """
         return SafetyCase.parse_obj(self._raw_ops.get(safetycase_id))
 
     def query(
         self,
         *,
+        query: Optional[QueryT] = None,
         id: Optional[str] = None,
         account: Optional[str] = None,
         status: Optional[str] = None,
         reason: Optional[str] = None,
         labels: Optional[dict[str, str]] = None,
         method: Optional[str] = None,
         methodName: Optional[str] = None,
@@ -1990,14 +2038,16 @@
         inferenceService: Optional[str] = None,
         model: Optional[str] = None,
         inputsAnyOf: Optional[str] = None,
     ) -> list[SafetyCase]:
         """Get all SafetyCase entities matching a query. The query is a set of equality
         constraints specified as key-value pairs.
 
+        :keyword query:
+        :paramtype query: str | dict[str, Any] | list[dict[str, Any]]
         :keyword id: Default value is None.
         :paramtype id: str
         :keyword account: Default value is None.
         :paramtype account: str
         :keyword status: Default value is None.
         :paramtype status: str
         :keyword reason: Default value is None.
@@ -2021,14 +2071,15 @@
         :return: Entities matching the query
         :rtype: list[SafetyCase]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         return [
             SafetyCase.parse_obj(obj)
             for obj in self._raw_ops.query(
+                query=_encode_query(query),
                 id=id,
                 account=account,
                 status=status,
                 reason=reason,
                 labels=_encode_labels(labels),
                 method=method,
                 method_name=methodName,
```

### Comparing `dyff_client-0.7.0/dyff_client.egg-info/PKG-INFO` & `dyff_client-0.8.0/dyff_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.7.0
+Version: 0.8.0
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.7.0/dyff_client.egg-info/SOURCES.txt` & `dyff_client-0.8.0/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/makefile` & `dyff_client-0.8.0/makefile`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/pyproject.toml` & `dyff_client-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff_client-0.8.0/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff_client-0.8.0/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/scripts/models/databricks--dolly-v2-3b.py` & `dyff_client-0.8.0/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/scripts/models/tiiuae--falcon-7b.py` & `dyff_client-0.8.0/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.7.0/tests/test_import.py` & `dyff_client-0.8.0/tests/test_import.py`

 * *Files identical despite different names*

