# Comparing `tmp/silverback-0.5.1.tar.gz` & `tmp/silverback-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverback-0.5.1.tar", last modified: Tue May 14 17:50:32 2024, max compression
+gzip compressed data, was "silverback-0.5.2.tar", last modified: Sat May 25 05:53:30 2024, max compression
```

## Comparing `silverback-0.5.1.tar` & `silverback-0.5.2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.743176 silverback-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.743176 silverback-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-14 17:49:08.000000 silverback-0.5.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-14 17:49:08.000000 silverback-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-14 17:49:08.000000 silverback-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-14 17:49:08.000000 silverback-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-14 17:49:08.000000 silverback-0.5.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-14 17:49:08.000000 silverback-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-14 17:50:32.751175 silverback-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-14 17:49:08.000000 silverback-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-14 17:49:08.000000 silverback-0.5.1/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/application.md
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/middlewares.md
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/runner.md
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/subscriptions.md
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.747176 silverback-0.5.1/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/userguides/development.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 17:49:08.000000 silverback-0.5.1/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-14 17:49:08.000000 silverback-0.5.1/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-14 17:49:08.000000 silverback-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-14 17:50:32.751175 silverback-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-14 17:49:08.000000 silverback-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/silverback/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16078 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-14 17:49:08.000000 silverback-0.5.1/silverback/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/silverback.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 17:50:32.000000 silverback-0.5.1/silverback.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 17:50:32.751175 silverback-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-14 17:49:08.000000 silverback-0.5.1/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.800545 silverback-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.792545 silverback-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.792545 silverback-0.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.792545 silverback-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-25 05:52:35.000000 silverback-0.5.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-25 05:52:35.000000 silverback-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-25 05:52:35.000000 silverback-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-25 05:52:35.000000 silverback-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-25 05:52:35.000000 silverback-0.5.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-25 05:52:35.000000 silverback-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-25 05:53:30.800545 silverback-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-25 05:52:35.000000 silverback-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-25 05:52:35.000000 silverback-0.5.2/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.796545 silverback-0.5.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.796545 silverback-0.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.796545 silverback-0.5.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9919 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.796545 silverback-0.5.2/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.796545 silverback-0.5.2/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/methoddocs/application.md
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/methoddocs/middlewares.md
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/methoddocs/runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/methoddocs/subscriptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.796545 silverback-0.5.2/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)     7897 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/userguides/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-25 05:52:35.000000 silverback-0.5.2/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-25 05:52:35.000000 silverback-0.5.2/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-25 05:52:35.000000 silverback-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-25 05:53:30.800545 silverback-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-25 05:52:35.000000 silverback-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.800545 silverback-0.5.2/silverback/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11962 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16078 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-25 05:52:35.000000 silverback-0.5.2/silverback/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.800545 silverback-0.5.2/silverback.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-25 05:53:30.000000 silverback-0.5.2/silverback.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 05:53:30.800545 silverback-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 05:52:35.000000 silverback-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-25 05:52:35.000000 silverback-0.5.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-25 05:52:35.000000 silverback-0.5.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-25 05:52:35.000000 silverback-0.5.2/tests/test_types.py
```

### Comparing `silverback-0.5.1/.github/ISSUE_TEMPLATE/bug.md` & `silverback-0.5.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/ISSUE_TEMPLATE/feature.md` & `silverback-0.5.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/ISSUE_TEMPLATE/work-item.md` & `silverback-0.5.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/release-drafter.yml` & `silverback-0.5.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/workflows/codeql.yaml` & `silverback-0.5.2/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/workflows/commitlint.yaml` & `silverback-0.5.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/workflows/docs.yaml` & `silverback-0.5.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/workflows/prtitle.yaml` & `silverback-0.5.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/workflows/publish.yaml` & `silverback-0.5.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.github/workflows/test.yaml` & `silverback-0.5.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.gitignore` & `silverback-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/.pre-commit-config.yaml` & `silverback-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/CONTRIBUTING.md` & `silverback-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/Dockerfile` & `silverback-0.5.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/LICENSE` & `silverback-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/PKG-INFO` & `silverback-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.5.1
+Version: 0.5.2
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.5.1/README.md` & `silverback-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/build_docs.py` & `silverback-0.5.2/build_docs.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/docs/_static/custom.css` & `silverback-0.5.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/docs/_static/custom.js` & `silverback-0.5.2/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/docs/_templates/layout.html` & `silverback-0.5.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/docs/conf.py` & `silverback-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/docs/favicon.ico` & `silverback-0.5.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/docs/logo.gif` & `silverback-0.5.2/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/docs/userguides/development.md` & `silverback-0.5.2/docs/userguides/development.md`

 * *Files 2% similar despite different names*

```diff
@@ -152,26 +152,24 @@
 
 The primary components are the client and workers.  The client handles Silverback events (blocks and contract event logs) and creates jobs for the workers to process in an asynchronous manner.
 
 For this to work, you must configure a [TaskIQ broker](https://taskiq-python.github.io/guide/architecture-overview.html#broker) capable of distributed processing.  For instance, with [`taskiq_redis`](https://github.com/taskiq-python/taskiq-redis) you could do something like this for the client:
 
 ```bash
 export SILVERBACK_BROKER_CLASS="taskiq_redis:ListQueueBroker"
-export SILVERBACK_BROKER_URI="redis://127.0.0.1:6379"
+export SILVERBACK_BROKER_KWARGS='{"queue_name": "taskiq", "url": "redis://127.0.0.1:6379"}'
 
-silverback run "example:app" \
-    --network :mainnet:alchemy \
-    --runner "silverback.runner:WebsocketRunner"
+silverback run "example:app" --network :mainnet:alchemy
 ```
 
 And then the worker process with 2 worker subprocesses:
 
 ```bash
 export SILVERBACK_BROKER_CLASS="taskiq_redis:ListQueueBroker"
-export SILVERBACK_BROKER_URI="redis://127.0.0.1:6379"
+export SILVERBACK_BROKER_KWARGS='{"url": "redis://127.0.0.1:6379"}'
 
 silverback worker -w 2 "example:app"
 ```
 
 This will run one client and 2 workers and all queue data will be go through Redis.
 
 ## Testing your Application
```

### Comparing `silverback-0.5.1/example.py` & `silverback-0.5.2/example.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/pyproject.toml` & `silverback-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/setup.py` & `silverback-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/_cli.py` & `silverback-0.5.2/silverback/_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 )
 from ape.exceptions import Abort
 from taskiq import AsyncBroker
 from taskiq.cli.worker.run import shutdown_broker
 from taskiq.receiver import Receiver
 
 from silverback._importer import import_from_string
-from silverback.runner import PollingRunner
+from silverback.runner import PollingRunner, WebsocketRunner
 
 
 @click.group()
 def cli():
     """Work with Silverback applications in local context (using Ape)."""
 
 
 def _runner_callback(ctx, param, val):
     if not val:
-        return PollingRunner
+        return None
 
     elif runner := import_from_string(val):
         return runner
 
     raise ValueError(f"Failed to import runner '{val}'.")
 
 
@@ -95,27 +95,39 @@
 @network_option(
     default=os.environ.get("SILVERBACK_NETWORK_CHOICE", "auto"),
     callback=_network_callback,
 )
 @click.option("--account", type=AccountAliasPromptChoice(), callback=_account_callback)
 @click.option(
     "--runner",
+    "runner_class",
     help="An import str in format '<module>:<CustomRunner>'",
     callback=_runner_callback,
 )
 @click.option(
     "--recorder",
     help="An import string in format '<module>:<CustomRecorder>'",
     callback=_recorder_callback,
 )
 @click.option("-x", "--max-exceptions", type=int, default=3)
 @click.argument("path")
-def run(cli_ctx, account, runner, recorder, max_exceptions, path):
+def run(cli_ctx, account, runner_class, recorder, max_exceptions, path):
+    if not runner_class:
+        # NOTE: Automatically select runner class
+        if cli_ctx.provider.ws_uri:
+            runner_class = WebsocketRunner
+        elif cli_ctx.provider.http_uri:
+            runner_class = PollingRunner
+        else:
+            raise click.BadOptionUsage(
+                option_name="network", message="Network choice cannot support running app"
+            )
+
     app = import_from_string(path)
-    runner = runner(app, recorder=recorder, max_exceptions=max_exceptions)
+    runner = runner_class(app, recorder=recorder, max_exceptions=max_exceptions)
     asyncio.run(runner.run())
 
 
 @cli.command(cls=ConnectedProviderCommand, help="Run Silverback application task workers")
 @ape_cli_context()
 @verbosity_option()
 @network_option(
```

### Comparing `silverback-0.5.1/silverback/_importer.py` & `silverback-0.5.2/silverback/_importer.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/application.py` & `silverback-0.5.2/silverback/application.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/exceptions.py` & `silverback-0.5.2/silverback/exceptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/middlewares.py` & `silverback-0.5.2/silverback/middlewares.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/recorder.py` & `silverback-0.5.2/silverback/recorder.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/runner.py` & `silverback-0.5.2/silverback/runner.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/settings.py` & `silverback-0.5.2/silverback/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from ape.api import AccountAPI, ProviderContextManager
 from ape.utils import ManagerAccessMixin
 from pydantic_settings import BaseSettings, SettingsConfigDict
 from taskiq import (
     AsyncBroker,
     AsyncResultBackend,
     InMemoryBroker,
@@ -22,15 +24,16 @@
     testing or deployment purposes. Defaults to a working in-memory broker.
     """
 
     # A unique identifier for this silverback instance
     APP_NAME: str = "bot"
 
     BROKER_CLASS: str = "taskiq:InMemoryBroker"
-    BROKER_URI: str = ""
+    BROKER_URI: str = ""  # to be deprecated in 0.6
+    BROKER_KWARGS: dict[str, Any] = dict()
 
     ENABLE_METRICS: bool = False
 
     RESULT_BACKEND_CLASS: str = ""
     RESULT_BACKEND_URI: str = ""
 
     NETWORK_CHOICE: str = ""
@@ -65,16 +68,21 @@
 
     def get_broker(self) -> AsyncBroker:
         broker_class = import_from_string(self.BROKER_CLASS)
         if broker_class == InMemoryBroker:
             broker = broker_class()
 
         else:
-            # TODO: Not all brokers share a common arg signature.
-            broker = broker_class(self.BROKER_URI or None)
+            broker_kwargs = self.BROKER_KWARGS
+
+            if self.BROKER_URI:
+                # TODO: Maybe add a deprecation warning here for v0.6
+                broker_kwargs["url"] = self.BROKER_URI
+
+            broker = broker_class(**broker_kwargs)
 
         if middlewares := self.get_middlewares():
             broker = broker.with_middlewares(*middlewares)
 
         if result_backend := self.get_result_backend():
             broker = broker.with_result_backend(result_backend)
```

### Comparing `silverback-0.5.1/silverback/state.py` & `silverback-0.5.2/silverback/state.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/subscriptions.py` & `silverback-0.5.2/silverback/subscriptions.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/types.py` & `silverback-0.5.2/silverback/types.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback/utils.py` & `silverback-0.5.2/silverback/utils.py`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback.egg-info/PKG-INFO` & `silverback-0.5.2/silverback.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverback
-Version: 0.5.1
+Version: 0.5.2
 Summary: Ape SDK for the Silverback platform
 Home-page: https://github.com/ApeWorX/silverback
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `silverback-0.5.1/silverback.egg-info/SOURCES.txt` & `silverback-0.5.2/silverback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/silverback.egg-info/requires.txt` & `silverback-0.5.2/silverback.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `silverback-0.5.1/tests/test_types.py` & `silverback-0.5.2/tests/test_types.py`

 * *Files identical despite different names*

