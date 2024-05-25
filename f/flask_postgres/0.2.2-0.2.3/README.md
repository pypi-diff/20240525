# Comparing `tmp/flask_postgres-0.2.2.tar.gz` & `tmp/flask_postgres-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_postgres-0.2.2.tar", last modified: Mon Mar 14 00:38:49 2022, max compression
+gzip compressed data, was "flask_postgres-0.2.3.tar", last modified: Sat May 25 21:33:29 2024, max compression
```

## Comparing `flask_postgres-0.2.2.tar` & `flask_postgres-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      467 2021-11-28 00:46:40.336107 flask_postgres-0.2.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1512 2021-11-28 01:14:38.848005 flask_postgres-0.2.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3028 2021-11-28 22:41:15.031770 flask_postgres-0.2.2/.gitignore
--rw-r--r--   0        0        0     1080 2021-11-26 16:37:30.106975 flask_postgres-0.2.2/LICENSE
--rw-r--r--   0        0        0      184 2021-11-28 04:25:09.546225 flask_postgres-0.2.2/Makefile
--rw-r--r--   0        0        0     7455 2022-03-14 00:16:28.053104 flask_postgres-0.2.2/README.md
--rw-r--r--   0        0        0      905 2021-11-28 23:30:40.833015 flask_postgres-0.2.2/docs/mkdocs.yml
--rw-r--r--   0        0        0       89 2021-11-28 22:56:53.504954 flask_postgres-0.2.2/docs/requirements.txt
--rw-r--r--   0        0        0   269616 2021-11-27 16:25:00.298000 flask_postgres-0.2.2/docs/src/img/flask-postgres-banner.png
--rw-r--r--   0        0        0     4139 2021-11-29 02:38:27.697000 flask_postgres-0.2.2/docs/src/img/flask-postgres-logo-small.png
--rw-r--r--   0        0        0    12765 2021-11-29 02:37:43.250000 flask_postgres-0.2.2/docs/src/img/flask-postgres-logo.png
--rw-r--r--   0        0        0       17 2021-11-28 23:30:40.829320 flask_postgres-0.2.2/docs/src/index.md
--rw-r--r--   0        0        0      202 2022-03-14 00:18:03.780790 flask_postgres-0.2.2/flask_postgres/__init__.py
--rw-r--r--   0        0        0      927 2021-11-28 03:02:19.203233 flask_postgres-0.2.2/flask_postgres/_compat.py
--rw-r--r--   0        0        0       22 2021-11-28 19:45:15.992245 flask_postgres-0.2.2/flask_postgres/cli/__init__.py
--rw-r--r--   0        0        0     7286 2022-03-14 00:03:35.960987 flask_postgres-0.2.2/flask_postgres/cli/main.py
--rw-r--r--   0        0        0     2536 2022-03-14 00:21:26.245967 flask_postgres-0.2.2/flask_postgres/cli/types.py
--rw-r--r--   0        0        0     1626 2022-03-14 00:14:35.059679 flask_postgres-0.2.2/flask_postgres/config.py
--rw-r--r--   0        0        0     1977 2021-11-28 20:09:06.582787 flask_postgres-0.2.2/flask_postgres/exceptions.py
--rw-r--r--   0        0        0     4207 2021-11-28 22:09:33.030497 flask_postgres-0.2.2/flask_postgres/ops.py
--rw-r--r--   0        0        0     6202 2021-12-27 00:33:07.120864 flask_postgres-0.2.2/flask_postgres/types.py
--rw-r--r--   0        0        0     2601 2021-11-28 22:38:08.922963 flask_postgres-0.2.2/flask_postgres/utils.py
--rw-r--r--   0        0        0     1318 2022-03-14 00:33:05.784911 flask_postgres-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2021-11-27 19:11:21.187335 flask_postgres-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     2539 2021-11-28 21:37:37.533439 flask_postgres-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     9573 2021-11-28 20:49:53.514181 flask_postgres-0.2.2/tests/test_cli_normal_app_config.py
--rw-r--r--   0        0        0     4135 2021-12-27 01:08:56.958767 flask_postgres-0.2.2/tests/test_types.py
--rw-r--r--   0        0        0     2868 2021-11-28 22:29:34.095880 flask_postgres-0.2.2/tests/test_utils.py
--rw-r--r--   0        0        0     8924 1970-01-01 00:00:00.000000 flask_postgres-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      467 2021-11-28 00:46:40.336107 flask_postgres-0.2.3/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1836 2024-05-25 21:13:07.985539 flask_postgres-0.2.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3028 2021-11-28 22:41:15.031770 flask_postgres-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1080 2021-11-26 16:37:30.106975 flask_postgres-0.2.3/LICENSE
+-rw-r--r--   0        0        0      184 2021-11-28 04:25:09.546225 flask_postgres-0.2.3/Makefile
+-rw-r--r--   0        0        0     7455 2024-05-25 21:13:07.986691 flask_postgres-0.2.3/README.md
+-rw-r--r--   0        0        0      905 2021-11-28 23:30:40.833015 flask_postgres-0.2.3/docs/mkdocs.yml
+-rw-r--r--   0        0        0       89 2021-11-28 22:56:53.504954 flask_postgres-0.2.3/docs/requirements.txt
+-rw-r--r--   0        0        0   269616 2021-11-27 16:25:00.298000 flask_postgres-0.2.3/docs/src/img/flask-postgres-banner.png
+-rw-r--r--   0        0        0     4139 2021-11-29 02:38:27.697000 flask_postgres-0.2.3/docs/src/img/flask-postgres-logo-small.png
+-rw-r--r--   0        0        0    12765 2021-11-29 02:37:43.250000 flask_postgres-0.2.3/docs/src/img/flask-postgres-logo.png
+-rw-r--r--   0        0        0       17 2021-11-28 23:30:40.829320 flask_postgres-0.2.3/docs/src/index.md
+-rw-r--r--   0        0        0      202 2024-05-25 21:13:07.987408 flask_postgres-0.2.3/flask_postgres/__init__.py
+-rw-r--r--   0        0        0      927 2021-11-28 03:02:19.203233 flask_postgres-0.2.3/flask_postgres/_compat.py
+-rw-r--r--   0        0        0       22 2021-11-28 19:45:15.992245 flask_postgres-0.2.3/flask_postgres/cli/__init__.py
+-rw-r--r--   0        0        0     7286 2024-05-25 21:13:07.988558 flask_postgres-0.2.3/flask_postgres/cli/main.py
+-rw-r--r--   0        0        0     2536 2024-05-25 21:13:07.989625 flask_postgres-0.2.3/flask_postgres/cli/types.py
+-rw-r--r--   0        0        0     1626 2024-05-25 21:13:07.991076 flask_postgres-0.2.3/flask_postgres/config.py
+-rw-r--r--   0        0        0     1977 2021-11-28 20:09:06.582787 flask_postgres-0.2.3/flask_postgres/exceptions.py
+-rw-r--r--   0        0        0     4207 2021-11-28 22:09:33.030497 flask_postgres-0.2.3/flask_postgres/ops.py
+-rw-r--r--   0        0        0     6202 2024-05-25 21:13:07.992147 flask_postgres-0.2.3/flask_postgres/types.py
+-rw-r--r--   0        0        0     2897 2024-05-25 21:13:07.993620 flask_postgres-0.2.3/flask_postgres/utils.py
+-rw-r--r--   0        0        0     1318 2024-05-25 21:13:07.994730 flask_postgres-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-11-27 19:11:21.187335 flask_postgres-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     2539 2021-11-28 21:37:37.533439 flask_postgres-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     9573 2021-11-28 20:49:53.514181 flask_postgres-0.2.3/tests/test_cli_normal_app_config.py
+-rw-r--r--   0        0        0     4135 2024-05-25 21:13:07.996197 flask_postgres-0.2.3/tests/test_types.py
+-rw-r--r--   0        0        0     3008 2024-05-25 21:13:07.997666 flask_postgres-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0     8924 1970-01-01 00:00:00.000000 flask_postgres-0.2.3/PKG-INFO
```

### Comparing `flask_postgres-0.2.2/.github/workflows/tests.yml` & `flask_postgres-0.2.3/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -7,21 +7,28 @@
     branches:
     - main
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python: [3.6.x, 3.7.x, 3.8.x, 3.9.x, 3.10.x]
-        flask: [2.*]
+        python: [3.6.x, 3.7.x, 3.8.x, 3.9.x, 3.10.x, 3.11.x]
+        flask: [2.0.*, 2.*]
         click: [7.*, 8.*]
         psycopg: [psycopg2]
-        # flask: [1.*, 2.*]
-        # click: [6.*, 7.*, 8.*]
-        # psycopg: [psycopg, psycopg2]
+        flask-sqlalchemy: [2.*, 3.*]
+        exclude:
+          - flask: 2.*
+            flask-sqlalchemy: 3.*
+          - python: 3.6.x
+            flask-sqlalchemy: 3.*
+          - flask: 2.*
+            click: 7.*
+          - python: 3.6.x
+            flask: 2.*
     services:
       postgres:
         image: postgres:12-alpine
         env:
           POSTGRES_USER: postgres
           POSTGRES_PASSWORD: postgres
         options: >-
@@ -41,16 +48,18 @@
       run: |
         sudo apt-get update
         sudo apt-get install python-dev libpq-dev
         pip install --upgrade pip
         make install
         pip install --upgrade flask=="${FLASK_VERSION}"
         pip install --upgrade click=="${CLICK_VERSION}"
+        pip install --upgrade flask-sqlalchemy=="${FLASK_SQLALCHEMY_VERSION}"
         pip install "${PSYCOPG_PACKAGE}"
       env:
         FLASK_VERSION: ${{ matrix.flask }}
+        FLASK_SQLALCHEMY_VERSION: ${{ matrix.flask-sqlalchemy }}
         CLICK_VERSION: ${{ matrix.click }}
         PSYCOPG_PACKAGE: ${{ matrix.psycopg }}
     - name: Run tests
       run: make test
       env:
         TEST_DATABASE_URI: postgresql://postgres:postgres@localhost:5432/flask_postgres_test_database
```

### Comparing `flask_postgres-0.2.2/.gitignore` & `flask_postgres-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/LICENSE` & `flask_postgres-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/README.md` & `flask_postgres-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/docs/mkdocs.yml` & `flask_postgres-0.2.3/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/docs/src/img/flask-postgres-banner.png` & `flask_postgres-0.2.3/docs/src/img/flask-postgres-banner.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/docs/src/img/flask-postgres-logo-small.png` & `flask_postgres-0.2.3/docs/src/img/flask-postgres-logo-small.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/docs/src/img/flask-postgres-logo.png` & `flask_postgres-0.2.3/docs/src/img/flask-postgres-logo.png`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/_compat.py` & `flask_postgres-0.2.3/flask_postgres/_compat.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/cli/main.py` & `flask_postgres-0.2.3/flask_postgres/cli/main.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/cli/types.py` & `flask_postgres-0.2.3/flask_postgres/cli/types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/config.py` & `flask_postgres-0.2.3/flask_postgres/config.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/exceptions.py` & `flask_postgres-0.2.3/flask_postgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/ops.py` & `flask_postgres-0.2.3/flask_postgres/ops.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/types.py` & `flask_postgres-0.2.3/flask_postgres/types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/flask_postgres/utils.py` & `flask_postgres-0.2.3/flask_postgres/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,29 +26,39 @@
 
 def get_db() -> SQLAlchemy:
     if not has_app_context():
         # RuntimeError is the same err type raised by flask.globals
         raise RuntimeError("The app context is currently not active.")
     if "sqlalchemy" not in current_app.extensions:
         raise SqlaExtensionNotFound
-    return current_app.extensions["sqlalchemy"].db
+    if hasattr(current_app.extensions["sqlalchemy"], "db"):
+        db = current_app.extensions["sqlalchemy"].db
+    else:
+        db = current_app.extensions["sqlalchemy"]
+    return db
 
 
 def raise_err_if_disallowed():
     """
     You can protect your app against accidental or (some, but not much)
     malicious use in sensitive environments with the
     `FLASK_POSTGRES_CLI_DISALLOWED_ENVS` config variable.
 
     This is only enabled for the CLI.
     """
     li = config.get("FLASK_POSTGRES_CLI_DISALLOWED_ENVS")
     if isinstance(li, str):
         li = li.split(";")
-    if current_app.env in li:
+    if li is None:
+        return
+    if hasattr(current_app, "env"):
+        app_env = current_app.env
+    else:
+        app_env = current_app.config.get("FLASK_ENV")
+    if app_env in li:
         raise EnvironmentNotAllowed
 
 
 def resolve_init_db_callback(
         callback: callable
 ) -> t.Callable[[Flask, SQLAlchemy], t.Any]:
```

### Comparing `flask_postgres-0.2.2/pyproject.toml` & `flask_postgres-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/tests/conftest.py` & `flask_postgres-0.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/tests/test_cli_normal_app_config.py` & `flask_postgres-0.2.3/tests/test_cli_normal_app_config.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/tests/test_types.py` & `flask_postgres-0.2.3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `flask_postgres-0.2.2/tests/test_utils.py` & `flask_postgres-0.2.3/tests/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     assert db_is_arg == bool("db" in inspect.signature(func).parameters)
 
     new_func = resolve_init_db_callback(func)
 
     assert "app" in inspect.signature(new_func).parameters
     assert "db" in inspect.signature(new_func).parameters
 
+    base_app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///test.db/"
     db = SQLAlchemy(base_app)
 
     assert capsys.readouterr().out == ""
 
     with base_app.app_context():
         new_func(app=base_app, db=db)  # noqa
 
@@ -68,14 +69,15 @@
 def test_get_db_function(base_app):
     # No db extension
     with pytest.raises(SqlaExtensionNotFound):
         with base_app.app_context():
             get_db()
 
     # This works perfectly fine.
+    base_app.config["SQLALCHEMY_DATABASE_URI"] = "sqlite:///test.db/"
     db1 = SQLAlchemy(base_app)
     with base_app.app_context():
         db2 = get_db()
     assert db1 is db2
 
     # No app context
     with pytest.raises(RuntimeError):
```

### Comparing `flask_postgres-0.2.2/PKG-INFO` & `flask_postgres-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_postgres
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple CLI for managing Postgres databases in Flask.
 Home-page: https://github.com/dwreeves/flask-postgres
 License: MIT
 Author: Daniel Reeves
 Author-email: xdanielreeves@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

