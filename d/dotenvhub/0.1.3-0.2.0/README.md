# Comparing `tmp/dotenvhub-0.1.3.tar.gz` & `tmp/dotenvhub-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotenvhub-0.1.3.tar", last modified: Tue Apr  2 20:24:02 2024, max compression
+gzip compressed data, was "dotenvhub-0.2.0.tar", last modified: Sat May 25 06:57:47 2024, max compression
```

## Comparing `dotenvhub-0.1.3.tar` & `dotenvhub-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.257320 dotenvhub-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.261320 dotenvhub-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/images/
--rw-r--r--   0 runner    (1001) docker     (127)   131826 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/images/image_header.PNG
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.261320 dotenvhub-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.265320 dotenvhub-0.1.3/src/dotenvhub/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/src/dotenvhub/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/assets/modal_save.css
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/assets/modal_shell.css
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/assets/tui.css
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/tui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/src/dotenvhub/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/filepanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/interactionpanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/modals.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/src/dotenvhub/widgets/previewpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/src/dotenvhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 20:24:02.000000 dotenvhub-0.1.3/src/dotenvhub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:24:02.269320 dotenvhub-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-02 20:23:33.000000 dotenvhub-0.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.379054 dotenvhub-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.367054 dotenvhub-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.371054 dotenvhub-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-25 06:57:47.379054 dotenvhub-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.375054 dotenvhub-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.375054 dotenvhub-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.375054 dotenvhub-0.2.0/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   131826 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/images/image_header.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-25 06:57:47.379054 dotenvhub-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.367054 dotenvhub-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.375054 dotenvhub-0.2.0/src/dotenvhub/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.375054 dotenvhub-0.2.0/src/dotenvhub/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/assets/modal_save.css
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/assets/modal_shell.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/assets/tui.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/tui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.375054 dotenvhub-0.2.0/src/dotenvhub/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/widgets/filepanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/widgets/interactionpanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/widgets/modals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/src/dotenvhub/widgets/previewpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.379054 dotenvhub-0.2.0/src/dotenvhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-25 06:57:47.000000 dotenvhub-0.2.0/src/dotenvhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-25 06:57:47.000000 dotenvhub-0.2.0/src/dotenvhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 06:57:47.000000 dotenvhub-0.2.0/src/dotenvhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-25 06:57:47.000000 dotenvhub-0.2.0/src/dotenvhub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 06:57:47.000000 dotenvhub-0.2.0/src/dotenvhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-25 06:57:47.000000 dotenvhub-0.2.0/src/dotenvhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-25 06:57:47.000000 dotenvhub-0.2.0/src/dotenvhub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 06:57:47.379054 dotenvhub-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-25 06:57:22.000000 dotenvhub-0.2.0/tox.ini
```

### Comparing `dotenvhub-0.1.3/.coveragerc` & `dotenvhub-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/.github/workflows/ci.yml` & `dotenvhub-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/.gitignore` & `dotenvhub-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/.pre-commit-config.yaml` & `dotenvhub-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/.readthedocs.yml` & `dotenvhub-0.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/CONTRIBUTING.md` & `dotenvhub-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/LICENSE.txt` & `dotenvhub-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/PKG-INFO` & `dotenvhub-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dotenvhub
-Version: 0.1.3
+Version: 0.2.0
 Summary: Terminal App to manage .env files written in Python powered by Textual
 Home-page: https://github.com/Zaloog/dotenvhub
 Author: Zaloog
 Author-email: gramslars@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Zaloog/dotenvhub
 Project-URL: Source, https://github.com/Zaloog/dotenvhub
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
-Requires-Dist: textual<=0.55.1
+Requires-Dist: textual
 Requires-Dist: platformdirs
 Requires-Dist: pyperclip
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `dotenvhub-0.1.3/README.md` & `dotenvhub-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/docs/Makefile` & `dotenvhub-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/docs/conf.py` & `dotenvhub-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/docs/index.md` & `dotenvhub-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/images/image_header.PNG` & `dotenvhub-0.2.0/images/image_header.PNG`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/setup.cfg` & `dotenvhub-0.2.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
-	textual<=0.55.1
+	textual
 	platformdirs
 	pyperclip
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `dotenvhub-0.1.3/setup.py` & `dotenvhub-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/__init__.py` & `dotenvhub-0.2.0/src/dotenvhub/__init__.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/app.py` & `dotenvhub-0.2.0/src/dotenvhub/app.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/assets/modal_shell.css` & `dotenvhub-0.2.0/src/dotenvhub/assets/modal_shell.css`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/assets/tui.css` & `dotenvhub-0.2.0/src/dotenvhub/assets/tui.css`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/cli_parser.py` & `dotenvhub-0.2.0/src/dotenvhub/cli_parser.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/config.py` & `dotenvhub-0.2.0/src/dotenvhub/config.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/constants.py` & `dotenvhub-0.2.0/src/dotenvhub/constants.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/tui.py` & `dotenvhub-0.2.0/src/dotenvhub/tui.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/utils.py` & `dotenvhub-0.2.0/src/dotenvhub/utils.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/widgets/filepanel.py` & `dotenvhub-0.2.0/src/dotenvhub/widgets/filepanel.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/src/dotenvhub/widgets/interactionpanel.py` & `dotenvhub-0.2.0/src/dotenvhub/widgets/interactionpanel.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,28 +51,34 @@
         yield Button(
             "Save Env File", id="btn-save-file", disabled=True, variant="success"
         )
 
     # Export Interactions
     @on(Button.Pressed, "#btn-copy-path")
     def copy_env_path(self):
-        copy_path_to_clipboard(path=self.app.file_to_show_path)
+        copy_str = copy_path_to_clipboard(path=self.app.file_to_show_path)
+        self.notify(title="Copied to Clipboard", message=f"Path: [green]{copy_str}[/]")
 
     @on(Button.Pressed, "#btn-file-export")
     def export_env_file(self):
         export_filename = self.query_one(Input).value
         create_copy_in_cwd(
             filename=export_filename, filepath=self.app.file_to_show_path
         )
+        self.notify(title="Env File Created", message=f"Created: {export_filename}")
 
     @on(Button.Pressed, "#btn-shell-export")
     def export_env_str_shell(self):
-        create_shell_export_str(
+        shell_str = create_shell_export_str(
             shell=self.app.current_shell, env_content=self.app.current_content
         )
+        self.notify(
+            title="Copied to Clipboard",
+            message=f"Command: [green]{shell_str}[/]",
+        )
 
     # Shell Select Interactions
     @on(Button.Pressed, "#btn-shell-select")
     def pop_modal_shell(self):
         self.app.push_screen(ModalShellSelector())
 
     # Env File Interactions
```

### Comparing `dotenvhub-0.1.3/src/dotenvhub/widgets/modals.py` & `dotenvhub-0.2.0/src/dotenvhub/widgets/modals.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,18 @@
     def pop_up_shell_select(self, event: Button.Pressed) -> None:
         self.dismiss()
         selected_shell = event.button.id
         self.app.current_shell = selected_shell
         cfg.shell = self.app.current_shell
 
         self.app.query_one("#btn-shell-select").label = self.app.current_shell
+        self.notify(
+            title="Shell Selected",
+            message=f"Current active Shell: [green]{self.app.current_shell}[/]",
+        )
 
 
 class ModalSaveScreen(ModalScreen):
     CSS_PATH = Path("../assets/modal_save.css")
     preview = reactive(":page_facing_up: Enter File Name")
 
     def compose(self) -> ComposeResult:
```

### Comparing `dotenvhub-0.1.3/src/dotenvhub.egg-info/PKG-INFO` & `dotenvhub-0.2.0/src/dotenvhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dotenvhub
-Version: 0.1.3
+Version: 0.2.0
 Summary: Terminal App to manage .env files written in Python powered by Textual
 Home-page: https://github.com/Zaloog/dotenvhub
 Author: Zaloog
 Author-email: gramslars@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Zaloog/dotenvhub
 Project-URL: Source, https://github.com/Zaloog/dotenvhub
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
-Requires-Dist: textual<=0.55.1
+Requires-Dist: textual
 Requires-Dist: platformdirs
 Requires-Dist: pyperclip
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `dotenvhub-0.1.3/src/dotenvhub.egg-info/SOURCES.txt` & `dotenvhub-0.2.0/src/dotenvhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/tests/test_utils.py` & `dotenvhub-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dotenvhub-0.1.3/tox.ini` & `dotenvhub-0.2.0/tox.ini`

 * *Files identical despite different names*

