# Comparing `tmp/djangobible-0.2.0.tar.gz` & `tmp/djangobible-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangobible-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "djangobible-0.2.1.tar", last modified: Sat May 25 03:24:07 2024, max compression
```

## Comparing `djangobible-0.2.0.tar` & `djangobible-0.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0       75 2022-07-15 23:13:41.269564 djangobible-0.2.0/.coveragerc
--rw-r--r--   0        0        0      282 2023-07-01 01:36:16.431867 djangobible-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2196 2023-09-12 18:03:07.927890 djangobible-0.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1011 2023-10-04 22:09:25.812441 djangobible-0.2.0/.github/workflows/django.yml
--rw-r--r--   0        0        0      571 2023-10-04 22:09:25.812642 djangobible-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1837 2021-06-22 14:59:30.263767 djangobible-0.2.0/.gitignore
--rw-r--r--   0        0        0     1089 2023-10-04 20:16:34.673471 djangobible-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2023-07-03 22:46:58.648769 djangobible-0.2.0/.sourcery.yaml
--rw-r--r--   0        0        0     1056 2023-10-04 22:09:25.813017 djangobible-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     3357 2021-06-22 14:59:30.263836 djangobible-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1429 2022-07-15 23:13:41.270254 djangobible-0.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1070 2021-06-22 14:59:30.263955 djangobible-0.2.0/LICENSE
--rw-r--r--   0        0        0     9130 2023-10-04 22:09:25.813288 djangobible-0.2.0/README.md
--rw-r--r--   0        0        0      231 2023-10-04 22:09:25.813483 djangobible-0.2.0/djangobible/__init__.py
--rw-r--r--   0        0        0      244 2022-07-15 23:13:41.270891 djangobible-0.2.0/djangobible/apps.py
--rw-r--r--   0        0        0     3025 2023-10-04 20:16:34.674662 djangobible-0.2.0/djangobible/fields.py
--rw-r--r--   0        0        0     1200 2023-10-04 20:16:34.674896 djangobible-0.2.0/djangobible/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-15 23:13:41.271368 djangobible-0.2.0/djangobible/migrations/__init__.py
--rw-r--r--   0        0        0     3028 2023-10-04 20:16:34.675578 djangobible-0.2.0/djangobible/models.py
--rw-r--r--   0        0        0        0 2021-06-22 14:59:30.264482 djangobible-0.2.0/djangobible/templatetags/__init__.py
--rw-r--r--   0        0        0     1728 2023-10-04 20:16:34.675973 djangobible-0.2.0/djangobible/templatetags/verse_tags.py
--rw-r--r--   0        0        0      853 2023-10-04 20:16:34.676143 djangobible-0.2.0/djangobible/validators.py
--rw-r--r--   0        0        0      711 2023-10-04 20:16:34.676677 djangobible-0.2.0/manage.py
--rw-r--r--   0        0        0      991 2023-10-04 22:09:25.813700 djangobible-0.2.0/noxfile.py
--rw-r--r--   0        0        0      505 2023-10-04 22:09:25.813926 djangobible-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       11 2022-07-15 23:13:41.272553 djangobible-0.2.0/requirements-dev.txt
--rw-r--r--   0        0        0       36 2023-10-04 22:09:25.814055 djangobible-0.2.0/requirements-test.txt
--rw-r--r--   0        0        0       42 2023-10-04 22:09:25.814186 djangobible-0.2.0/requirements.txt
--rw-r--r--   0        0        0     1608 2023-10-04 22:09:25.814366 djangobible-0.2.0/setup.cfg
--rw-r--r--   0        0        0        0 2022-07-15 23:13:41.273090 djangobible-0.2.0/test_django_app/__init__.py
--rw-r--r--   0        0        0      285 2023-10-04 20:16:34.677495 djangobible-0.2.0/test_django_app/admin.py
--rw-r--r--   0        0        0      229 2022-07-15 23:13:41.273461 djangobible-0.2.0/test_django_app/apps.py
--rw-r--r--   0        0        0      770 2023-10-04 20:16:34.678070 djangobible-0.2.0/test_django_app/migrations/0001_initial.py
--rw-r--r--   0        0        0      826 2023-10-04 20:16:34.678315 djangobible-0.2.0/test_django_app/migrations/0002_testsingleverseobject.py
--rw-r--r--   0        0        0      486 2023-05-27 20:57:45.008956 djangobible-0.2.0/test_django_app/migrations/0003_alter_testsingleverseobject_verse.py
--rw-r--r--   0        0        0        0 2022-07-15 23:13:41.274052 djangobible-0.2.0/test_django_app/migrations/__init__.py
--rw-r--r--   0        0        0      962 2023-10-04 20:16:34.678511 djangobible-0.2.0/test_django_app/models.py
--rw-r--r--   0        0        0      443 2023-05-27 21:02:17.828564 djangobible-0.2.0/test_django_app/templates/verse_tags.html
--rw-r--r--   0        0        0        0 2022-07-15 23:13:41.274479 djangobible-0.2.0/test_django_app/tests/__init__.py
--rw-r--r--   0        0        0     1028 2023-10-04 20:16:34.678763 djangobible-0.2.0/test_django_app/tests/factories.py
--rw-r--r--   0        0        0        0 2023-10-04 22:09:25.814449 djangobible-0.2.0/test_django_app/tests/functional_tests/__init__.py
--rw-r--r--   0        0        0     2491 2023-10-04 22:09:25.814593 djangobible-0.2.0/test_django_app/tests/functional_tests/test_admin.py
--rw-r--r--   0        0        0     1535 2023-10-04 22:09:25.814689 djangobible-0.2.0/test_django_app/tests/functional_tests/test_tags_functional.py
--rw-r--r--   0        0        0        0 2023-10-04 22:09:25.814731 djangobible-0.2.0/test_django_app/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0    11108 2023-10-04 22:09:25.814842 djangobible-0.2.0/test_django_app/tests/unit_tests/test_models.py
--rw-r--r--   0        0        0     1861 2023-10-04 22:09:25.814933 djangobible-0.2.0/test_django_app/tests/unit_tests/test_search.py
--rw-r--r--   0        0        0     4398 2023-10-04 22:09:25.815025 djangobible-0.2.0/test_django_app/tests/unit_tests/test_tags.py
--rw-r--r--   0        0        0      964 2023-10-04 22:09:25.815098 djangobible-0.2.0/test_django_app/tests/unit_tests/test_validators.py
--rw-r--r--   0        0        0      357 2023-10-04 20:16:34.681215 djangobible-0.2.0/test_django_app/views.py
--rw-r--r--   0        0        0        0 2022-07-15 23:13:41.277131 djangobible-0.2.0/test_django_project/__init__.py
--rw-r--r--   0        0        0      451 2023-10-04 20:16:34.681406 djangobible-0.2.0/test_django_project/asgi.py
--rw-r--r--   0        0        0     3141 2023-10-04 20:16:34.681732 djangobible-0.2.0/test_django_project/settings.py
--rw-r--r--   0        0        0      247 2022-07-15 23:13:41.277617 djangobible-0.2.0/test_django_project/urls.py
--rw-r--r--   0        0        0      451 2023-10-04 20:16:34.681863 djangobible-0.2.0/test_django_project/wsgi.py
--rw-r--r--   0        0        0     9509 1970-01-01 00:00:00.000000 djangobible-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       90 2024-05-25 03:06:48.391094 djangobible-0.2.1/.coveragerc
+-rw-r--r--   0        0        0      282 2023-10-03 04:19:40.555239 djangobible-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2196 2024-05-25 03:06:48.393560 djangobible-0.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1011 2024-05-25 03:06:48.396155 djangobible-0.2.1/.github/workflows/django.yml
+-rw-r--r--   0        0        0      499 2024-05-25 03:21:10.053837 djangobible-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1837 2023-03-24 19:59:22.650268 djangobible-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1089 2024-05-25 03:06:48.402038 djangobible-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2023-10-03 04:19:40.562212 djangobible-0.2.1/.sourcery.yaml
+-rw-r--r--   0        0        0     1691 2024-05-25 03:21:10.054833 djangobible-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3357 2023-03-24 19:59:22.650693 djangobible-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1429 2023-03-24 19:59:22.650844 djangobible-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1070 2023-03-24 19:59:22.650981 djangobible-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9301 2024-05-25 03:21:10.055858 djangobible-0.2.1/README.md
+-rw-r--r--   0        0        0      231 2024-05-25 03:21:10.056219 djangobible-0.2.1/djangobible/__init__.py
+-rw-r--r--   0        0        0      244 2023-03-24 19:59:22.651481 djangobible-0.2.1/djangobible/apps.py
+-rw-r--r--   0        0        0     3025 2023-10-03 04:19:40.563290 djangobible-0.2.1/djangobible/fields.py
+-rw-r--r--   0        0        0     1200 2023-03-24 19:59:22.651836 djangobible-0.2.1/djangobible/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-03-24 19:59:22.651908 djangobible-0.2.1/djangobible/migrations/__init__.py
+-rw-r--r--   0        0        0     3028 2023-03-24 19:59:22.652076 djangobible-0.2.1/djangobible/models.py
+-rw-r--r--   0        0        0        0 2023-03-24 19:59:22.652207 djangobible-0.2.1/djangobible/templatetags/__init__.py
+-rw-r--r--   0        0        0     1728 2023-10-03 04:19:40.563567 djangobible-0.2.1/djangobible/templatetags/verse_tags.py
+-rw-r--r--   0        0        0      853 2023-03-24 19:59:22.652646 djangobible-0.2.1/djangobible/validators.py
+-rw-r--r--   0        0        0      711 2023-03-24 19:59:22.652832 djangobible-0.2.1/manage.py
+-rw-r--r--   0        0        0     1050 2024-05-25 03:21:10.056723 djangobible-0.2.1/noxfile.py
+-rw-r--r--   0        0        0      505 2024-05-25 03:21:10.057086 djangobible-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-03-24 19:59:22.653137 djangobible-0.2.1/requirements-dev.txt
+-rw-r--r--   0        0        0       36 2023-10-11 01:57:06.917344 djangobible-0.2.1/requirements-test.txt
+-rw-r--r--   0        0        0       37 2024-05-25 03:21:10.057395 djangobible-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     1608 2023-10-11 01:57:06.919563 djangobible-0.2.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-03-24 19:59:22.653646 djangobible-0.2.1/test_django_app/__init__.py
+-rw-r--r--   0        0        0      285 2023-03-24 19:59:22.653783 djangobible-0.2.1/test_django_app/admin.py
+-rw-r--r--   0        0        0      229 2023-03-24 19:59:22.653908 djangobible-0.2.1/test_django_app/apps.py
+-rw-r--r--   0        0        0      770 2023-03-24 19:59:22.654099 djangobible-0.2.1/test_django_app/migrations/0001_initial.py
+-rw-r--r--   0        0        0      826 2023-03-24 19:59:22.654270 djangobible-0.2.1/test_django_app/migrations/0002_testsingleverseobject.py
+-rw-r--r--   0        0        0      486 2023-03-24 19:59:22.654433 djangobible-0.2.1/test_django_app/migrations/0003_alter_testsingleverseobject_verse.py
+-rw-r--r--   0        0        0        0 2023-03-24 19:59:22.654503 djangobible-0.2.1/test_django_app/migrations/__init__.py
+-rw-r--r--   0        0        0      962 2023-03-24 19:59:22.654657 djangobible-0.2.1/test_django_app/models.py
+-rw-r--r--   0        0        0      443 2023-10-03 04:19:40.564864 djangobible-0.2.1/test_django_app/templates/verse_tags.html
+-rw-r--r--   0        0        0        0 2023-03-24 19:59:22.655104 djangobible-0.2.1/test_django_app/tests/__init__.py
+-rw-r--r--   0        0        0     1028 2023-03-24 19:59:22.655362 djangobible-0.2.1/test_django_app/tests/factories.py
+-rw-r--r--   0        0        0        0 2023-10-11 01:57:06.920029 djangobible-0.2.1/test_django_app/tests/functional_tests/__init__.py
+-rw-r--r--   0        0        0     2491 2023-10-11 01:57:06.920296 djangobible-0.2.1/test_django_app/tests/functional_tests/test_admin.py
+-rw-r--r--   0        0        0     1535 2023-10-11 01:57:06.920479 djangobible-0.2.1/test_django_app/tests/functional_tests/test_tags_functional.py
+-rw-r--r--   0        0        0        0 2023-10-11 01:57:06.920624 djangobible-0.2.1/test_django_app/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0    11108 2023-10-11 01:57:06.920955 djangobible-0.2.1/test_django_app/tests/unit_tests/test_models.py
+-rw-r--r--   0        0        0     1861 2023-10-11 01:57:06.921135 djangobible-0.2.1/test_django_app/tests/unit_tests/test_search.py
+-rw-r--r--   0        0        0     4398 2023-10-11 01:57:06.921334 djangobible-0.2.1/test_django_app/tests/unit_tests/test_tags.py
+-rw-r--r--   0        0        0      964 2023-10-11 01:57:06.921483 djangobible-0.2.1/test_django_app/tests/unit_tests/test_validators.py
+-rw-r--r--   0        0        0      357 2023-10-03 04:19:40.566160 djangobible-0.2.1/test_django_app/views.py
+-rw-r--r--   0        0        0        0 2023-03-24 19:59:22.657071 djangobible-0.2.1/test_django_project/__init__.py
+-rw-r--r--   0        0        0      451 2023-03-24 19:59:22.657242 djangobible-0.2.1/test_django_project/asgi.py
+-rw-r--r--   0        0        0     3142 2024-05-25 03:06:48.405855 djangobible-0.2.1/test_django_project/settings.py
+-rw-r--r--   0        0        0      247 2023-03-24 19:59:22.657742 djangobible-0.2.1/test_django_project/urls.py
+-rw-r--r--   0        0        0      451 2023-03-24 19:59:22.657917 djangobible-0.2.1/test_django_project/wsgi.py
+-rw-r--r--   0        0        0     9680 1970-01-01 00:00:00.000000 djangobible-0.2.1/PKG-INFO
```

### Comparing `djangobible-0.2.0/.github/workflows/codeql-analysis.yml` & `djangobible-0.2.1/.github/workflows/codeql-analysis.yml`

 * *Files 5% similar despite different names*

```diff
@@ -30,33 +30,33 @@
 
     steps:
     - name: Checkout repository
       uses: actions/checkout@v4
 
     # Initializes the CodeQL tools for scanning.
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v2
+      uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
         # If you wish to specify custom queries, you can do so here or in a config file.
         # By default, queries listed here will override any specified in a config file.
         # Prefix the list here with "+" to use these queries and those in the config file.
         # queries: ./path/to/local/query, your-org/your-repo/queries@main
 
     # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
     # If this step fails, then you should remove it and run the build manually (see below)
     - name: Autobuild
-      uses: github/codeql-action/autobuild@v2
+      uses: github/codeql-action/autobuild@v3
 
     # ℹ️ Command-line programs to run using the OS shell.
     # 📚 https://git.io/JvXDl
 
     # ✏️ If the Autobuild fails above, remove it and uncomment the following three lines
     #    and modify them (or add more) to build your code if your project
     #    uses a compiled language
 
     #- run: |
     #   make bootstrap
     #   make release
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v2
+      uses: github/codeql-action/analyze@v3
```

### Comparing `djangobible-0.2.0/.github/workflows/django.yml` & `djangobible-0.2.1/.github/workflows/django.yml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       max-parallel: 4
       matrix:
         python-version: ["3.11"]
 
     steps:
     - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -U -r requirements.txt
         pip install -U -r requirements-test.txt
```

### Comparing `djangobible-0.2.0/.gitignore` & `djangobible-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/.pre-commit-config.yaml` & `djangobible-0.2.1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: debug-statements
       - id: requirements-txt-fixer
       - id: check-added-large-files
   - repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 24.4.2
     hooks:
       - id: black
   - repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
       - id: isort
   - repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
       - id: flake8
         additional_dependencies:
           - flake8-alfred
           - flake8-annotations
           - flake8-bandit
           - flake8-blind-except
```

### Comparing `djangobible-0.2.0/CHANGELOG.md` & `djangobible-0.2.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,31 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+### [0.2.1] - 2024-05-24
+
+- Added support for Django 5.0
+- Added full support for Python 3.12
+  - Added automated functional testing now that there is a version of greenlet that supports Python 3.12
+- ~~Added automated testing for Python 3.13-beta~~ (not yet supported by greenlet)
+- Added automated testing for Django 5.1-alpha
+
+### Changed
+
+- Require the latest version of pythonbible (0.13.1)
+
+### Removed
+
+- Removed official support for Django 3.2 (due to end of life on 2024-04-01)
+- Removed official support for Django 4.1 (due to end of life on 2023-12-01)
+
 ## [0.2.0] - 2023-10-04
 
 ### Added
 
 - Added support for Python 3.12
 - Added automated testing for Python 3.8 - 3.12; Django 3.2, 4.1, 4.2; and Ubuntu, macOS, and Windows
 
@@ -34,10 +51,11 @@
 
 - Added this changelog
 
 ### Removed
 
 - Removed Python 3.7 support (due to end of life on 2023-06-27)
 
-[unreleased]: https://github.com/avendesora/djangobible/compare/v0.2.0...HEAD
-[0.2.0]: https://github.com/avendesora/djangobible/releases/tag/v0.1.1...v0.2.0
+[unreleased]: https://github.com/avendesora/djangobible/compare/v0.2.1...HEAD
+[0.2.1]: https://github.com/avendesora/djangobible/compare/v0.2.0...v0.2.1
+[0.2.0]: https://github.com/avendesora/djangobible/compare/v0.1.1...v0.2.0
 [0.1.1]: https://github.com/avendesora/djangobible/releases/tag/v0.1.1
```

### Comparing `djangobible-0.2.0/CODE_OF_CONDUCT.md` & `djangobible-0.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/CONTRIBUTING.md` & `djangobible-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/LICENSE` & `djangobible-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/README.md` & `djangobible-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: djangobible
+Version: 0.2.1
+Summary: djangobible python library.
+Home-page: https://github.com/avendesora/djangobible
+Author: Nathan Patton
+Author-email: npatton@gmail.com
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: Django>=4.2.0
+Requires-Dist: pythonbible==0.13.1
+
 # djangobible
 
 The djangobible library is a Django app that wraps the [pythonbible](https://github.com/avendesora/pythonbible) library and provides models, managers, and other tools to easily index an object by a scripture reference.
 
 <table>
     <tr>
         <td>Latest Version</td>
@@ -13,16 +26,17 @@
     <tr>
         <td>License</td>
         <td><a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-orange.svg"></a></td>
     </tr>
     <tr>
         <td>Tests</td>
         <td>
-            <img src="https://github.com/avendesora/djangobible/workflows/Django%20CI/badge.svg">
-            <a href="https://www.codacy.com/gh/avendesora/djangobible/dashboard?utm_source=github.com&utm_medium=referral&utm_content=avendesora/djangobible&utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/83a28131bf6642ed9e439344122686fc"></a>
+            <img src="https://github.com/avendesora/djangobible/actions/workflows/tests.yml/badge.svg">
+            <img src="https://github.com/avendesora/djangobible/workflows/Django%20CI/badge.svg"><br/>
+            <a href="https://app.codacy.com/gh/avendesora/djangobible/coverage/dashboard"><img src="https://app.codacy.com/project/badge/Coverage/83a28131bf6642ed9e439344122686fc"></a>
         </td>
     </tr>
     <tr>
         <td>Code Quality</td>
         <td>
             <img src="https://github.com/avendesora/djangobible/workflows/CodeQL/badge.svg">
             <a href="https://app.codacy.com/gh/avendesora/djangobible?utm_source=github.com&utm_medium=referral&utm_content=avendesora/djangobible&utm_campaign=Badge_Grade_Settings"><img src="https://api.codacy.com/project/badge/Grade/ca34603bdaf8446ba288430b69092093"></a><br/>
@@ -30,15 +44,16 @@
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
         </td>
     </tr>
     <tr>
         <td>Supported Python/Django Versions</td>
         <td>
             <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue?logo=python&logoColor=lightgray"></a><br />
-            <a href="https://www.djangoproject.com/download/"><img src="https://img.shields.io/badge/Django-3.2%20%7C%204.1%20%7C%204.2-blue"></a>
+            <a href="https://www.djangoproject.com/download/"><img src="https://img.shields.io/badge/Django-4.2%20%7C%205.0%20%7C%205.1alpha-blue"></a><br />
+            Attempted to test with Python 3.13, but the testing framework has a dependency that has not yet been updated to work with Python 3.13.
         </td>
     </tr>
 </table>
 
 ## Installation
 
 Pip install the djangobible library.
@@ -235,7 +250,8 @@
 >>> my_object.verses.all()
 [<Verse: Genesis 1:1>, <Verse: Genesis 1:3>]
 >>> MyModel.objects.filter(verses__in=[1001001])
 [<MyModel: My Object>]
 ```
 
 Ideally, the form field would be a text field where the user could enter a list of Scripture references (e.g. "Genesis 1:1,3-10;Psalm 119;Luke 2:1-18;John 3:16")
+
```

### Comparing `djangobible-0.2.0/djangobible/fields.py` & `djangobible-0.2.1/djangobible/fields.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/djangobible/migrations/0001_initial.py` & `djangobible-0.2.1/djangobible/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/djangobible/models.py` & `djangobible-0.2.1/djangobible/models.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/djangobible/templatetags/verse_tags.py` & `djangobible-0.2.1/djangobible/templatetags/verse_tags.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/djangobible/validators.py` & `djangobible-0.2.1/djangobible/validators.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/manage.py` & `djangobible-0.2.1/manage.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/setup.cfg` & `djangobible-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/migrations/0001_initial.py` & `djangobible-0.2.1/test_django_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/migrations/0002_testsingleverseobject.py` & `djangobible-0.2.1/test_django_app/migrations/0002_testsingleverseobject.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/models.py` & `djangobible-0.2.1/test_django_app/models.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/tests/factories.py` & `djangobible-0.2.1/test_django_app/tests/factories.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/tests/functional_tests/test_admin.py` & `djangobible-0.2.1/test_django_app/tests/functional_tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/tests/functional_tests/test_tags_functional.py` & `djangobible-0.2.1/test_django_app/tests/functional_tests/test_tags_functional.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/tests/unit_tests/test_models.py` & `djangobible-0.2.1/test_django_app/tests/unit_tests/test_models.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/tests/unit_tests/test_search.py` & `djangobible-0.2.1/test_django_app/tests/unit_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/tests/unit_tests/test_tags.py` & `djangobible-0.2.1/test_django_app/tests/unit_tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_app/tests/unit_tests/test_validators.py` & `djangobible-0.2.1/test_django_app/tests/unit_tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `djangobible-0.2.0/test_django_project/settings.py` & `djangobible-0.2.1/test_django_project/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 For more information on this file, see
 https://docs.djangoproject.com/en/3.1/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/3.1/ref/settings/
 """
+
 from __future__ import annotations
 
 from pathlib import Path
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 from typing import Any
```

### Comparing `djangobible-0.2.0/PKG-INFO` & `djangobible-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: djangobible
-Version: 0.2.0
-Summary: djangobible python library.
-Home-page: https://github.com/avendesora/djangobible
-Author: Nathan Patton
-Author-email: npatton@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: Django>=3.2.0
-Requires-Dist: pythonbible==0.12.0
-
 # djangobible
 
 The djangobible library is a Django app that wraps the [pythonbible](https://github.com/avendesora/pythonbible) library and provides models, managers, and other tools to easily index an object by a scripture reference.
 
 <table>
     <tr>
         <td>Latest Version</td>
@@ -26,16 +13,17 @@
     <tr>
         <td>License</td>
         <td><a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-orange.svg"></a></td>
     </tr>
     <tr>
         <td>Tests</td>
         <td>
-            <img src="https://github.com/avendesora/djangobible/workflows/Django%20CI/badge.svg">
-            <a href="https://www.codacy.com/gh/avendesora/djangobible/dashboard?utm_source=github.com&utm_medium=referral&utm_content=avendesora/djangobible&utm_campaign=Badge_Coverage"><img src="https://app.codacy.com/project/badge/Coverage/83a28131bf6642ed9e439344122686fc"></a>
+            <img src="https://github.com/avendesora/djangobible/actions/workflows/tests.yml/badge.svg">
+            <img src="https://github.com/avendesora/djangobible/workflows/Django%20CI/badge.svg"><br/>
+            <a href="https://app.codacy.com/gh/avendesora/djangobible/coverage/dashboard"><img src="https://app.codacy.com/project/badge/Coverage/83a28131bf6642ed9e439344122686fc"></a>
         </td>
     </tr>
     <tr>
         <td>Code Quality</td>
         <td>
             <img src="https://github.com/avendesora/djangobible/workflows/CodeQL/badge.svg">
             <a href="https://app.codacy.com/gh/avendesora/djangobible?utm_source=github.com&utm_medium=referral&utm_content=avendesora/djangobible&utm_campaign=Badge_Grade_Settings"><img src="https://api.codacy.com/project/badge/Grade/ca34603bdaf8446ba288430b69092093"></a><br/>
@@ -43,15 +31,16 @@
             <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
         </td>
     </tr>
     <tr>
         <td>Supported Python/Django Versions</td>
         <td>
             <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue?logo=python&logoColor=lightgray"></a><br />
-            <a href="https://www.djangoproject.com/download/"><img src="https://img.shields.io/badge/Django-3.2%20%7C%204.1%20%7C%204.2-blue"></a>
+            <a href="https://www.djangoproject.com/download/"><img src="https://img.shields.io/badge/Django-4.2%20%7C%205.0%20%7C%205.1alpha-blue"></a><br />
+            Attempted to test with Python 3.13, but the testing framework has a dependency that has not yet been updated to work with Python 3.13.
         </td>
     </tr>
 </table>
 
 ## Installation
 
 Pip install the djangobible library.
@@ -248,8 +237,7 @@
 >>> my_object.verses.all()
 [<Verse: Genesis 1:1>, <Verse: Genesis 1:3>]
 >>> MyModel.objects.filter(verses__in=[1001001])
 [<MyModel: My Object>]
 ```
 
 Ideally, the form field would be a text field where the user could enter a list of Scripture references (e.g. "Genesis 1:1,3-10;Psalm 119;Luke 2:1-18;John 3:16")
-
```

