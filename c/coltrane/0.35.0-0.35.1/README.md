# Comparing `tmp/coltrane-0.35.0.tar.gz` & `tmp/coltrane-0.35.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coltrane-0.35.0.tar", max compression
+gzip compressed data, was "coltrane-0.35.1.tar", max compression
```

## Comparing `coltrane-0.35.0.tar` & `coltrane-0.35.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.35.0/LICENSE
--rw-r--r--   0        0        0     4722 2024-05-24 12:04:19.636824 coltrane-0.35.0/README.md
--rw-r--r--   0        0        0    14466 2024-05-23 23:43:03.471452 coltrane-0.35.0/coltrane/__init__.py
--rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.35.0/coltrane/config/__init__.py
--rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.35.0/coltrane/config/cache.py
--rw-r--r--   0        0        0     2918 2024-05-13 22:55:14.206087 coltrane-0.35.0/coltrane/config/paths.py
--rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.35.0/coltrane/config/redirects.py
--rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.35.0/coltrane/config/settings.py
--rw-r--r--   0        0        0     5177 2024-05-24 00:21:57.806314 coltrane-0.35.0/coltrane/console.py
--rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.35.0/coltrane/context_processors.py
--rw-r--r--   0        0        0     1346 2024-05-24 00:21:18.987673 coltrane-0.35.0/coltrane/default-files/Dockerfile
--rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.35.0/coltrane/default-files/README.md
--rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.35.0/coltrane/default-files/app.py
--rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.35.0/coltrane/default-files/env
--rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.35.0/coltrane/default-files/gitignore
--rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.35.0/coltrane/default-files/gunicorn.conf.py
--rw-r--r--   0        0        0      153 2024-05-24 12:13:06.821936 coltrane-0.35.0/coltrane/default-files/pyproject.toml
--rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.35.0/coltrane/default-files/watchmanconfig
--rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.35.0/coltrane/feeds.py
--rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.35.0/coltrane/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.35.0/coltrane/management/commands/__init__.py
--rw-r--r--   0        0        0    12032 2024-05-14 10:49:50.074140 coltrane-0.35.0/coltrane/management/commands/build.py
--rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.35.0/coltrane/manifest.py
--rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.35.0/coltrane/middleware.py
--rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.35.0/coltrane/module_finder.py
--rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.35.0/coltrane/renderer.py
--rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.35.0/coltrane/retriever.py
--rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.35.0/coltrane/sitemaps.py
--rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.35.0/coltrane/templates/coltrane/base.html
--rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.35.0/coltrane/templates/coltrane/content.html
--rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.35.0/coltrane/templatetags/__init__.py
--rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.35.0/coltrane/templatetags/coltrane_tags.py
--rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.35.0/coltrane/urls.py
--rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.35.0/coltrane/utils.py
--rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.35.0/coltrane/views.py
--rw-r--r--   0        0        0     5559 2024-05-24 00:16:57.340009 coltrane-0.35.0/pyproject.toml
--rw-r--r--   0        0        0     6753 1970-01-01 00:00:00.000000 coltrane-0.35.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-01-05 04:16:46.952062 coltrane-0.35.1/LICENSE
+-rw-r--r--   0        0        0     4722 2024-05-24 12:04:19.636824 coltrane-0.35.1/README.md
+-rw-r--r--   0        0        0    14466 2024-05-24 12:44:20.769647 coltrane-0.35.1/coltrane/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-08 22:33:55.376070 coltrane-0.35.1/coltrane/config/__init__.py
+-rw-r--r--   0        0        0     1404 2023-11-21 02:29:05.205562 coltrane-0.35.1/coltrane/config/cache.py
+-rw-r--r--   0        0        0     2918 2024-05-24 12:44:28.808968 coltrane-0.35.1/coltrane/config/paths.py
+-rw-r--r--   0        0        0     1022 2024-05-13 22:55:14.206208 coltrane-0.35.1/coltrane/config/redirects.py
+-rw-r--r--   0        0        0     2955 2024-05-13 22:55:14.206370 coltrane-0.35.1/coltrane/config/settings.py
+-rw-r--r--   0        0        0     5204 2024-05-24 12:48:22.833819 coltrane-0.35.1/coltrane/console.py
+-rw-r--r--   0        0        0       87 2024-05-13 22:55:14.206504 coltrane-0.35.1/coltrane/context_processors.py
+-rw-r--r--   0        0        0     1612 2024-05-25 14:38:06.294883 coltrane-0.35.1/coltrane/default-files/Dockerfile
+-rw-r--r--   0        0        0       79 2024-01-08 00:16:44.092955 coltrane-0.35.1/coltrane/default-files/README.md
+-rw-r--r--   0        0        0      245 2024-01-08 00:16:57.676856 coltrane-0.35.1/coltrane/default-files/app.py
+-rw-r--r--   0        0        0       68 2024-01-07 15:38:37.525852 coltrane-0.35.1/coltrane/default-files/env
+-rw-r--r--   0        0        0       10 2024-01-07 15:34:34.518859 coltrane-0.35.1/coltrane/default-files/gitignore
+-rw-r--r--   0        0        0      165 2024-01-07 15:33:37.336569 coltrane-0.35.1/coltrane/default-files/gunicorn.conf.py
+-rw-r--r--   0        0        0      153 2024-05-24 12:13:06.821936 coltrane-0.35.1/coltrane/default-files/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-01-07 15:35:30.796182 coltrane-0.35.1/coltrane/default-files/watchmanconfig
+-rw-r--r--   0        0        0     1281 2024-03-01 12:30:51.465959 coltrane-0.35.1/coltrane/feeds.py
+-rw-r--r--   0        0        0        0 2022-01-01 20:39:42.219557 coltrane-0.35.1/coltrane/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 02:02:14.248102 coltrane-0.35.1/coltrane/management/commands/__init__.py
+-rw-r--r--   0        0        0    12032 2024-05-14 10:49:50.074140 coltrane-0.35.1/coltrane/management/commands/build.py
+-rw-r--r--   0        0        0     7688 2023-11-21 02:29:05.207699 coltrane-0.35.1/coltrane/manifest.py
+-rw-r--r--   0        0        0      693 2023-12-03 02:20:31.935691 coltrane-0.35.1/coltrane/middleware.py
+-rw-r--r--   0        0        0      958 2024-05-13 22:55:14.206919 coltrane-0.35.1/coltrane/module_finder.py
+-rw-r--r--   0        0        0    14059 2024-05-13 22:55:14.207147 coltrane-0.35.1/coltrane/renderer.py
+-rw-r--r--   0        0        0     4292 2024-03-01 12:30:51.466354 coltrane-0.35.1/coltrane/retriever.py
+-rw-r--r--   0        0        0      342 2022-03-12 21:23:42.389804 coltrane-0.35.1/coltrane/sitemaps.py
+-rw-r--r--   0        0        0      408 2022-02-26 20:13:57.756348 coltrane-0.35.1/coltrane/templates/coltrane/base.html
+-rw-r--r--   0        0        0       92 2022-01-02 18:58:48.459102 coltrane-0.35.1/coltrane/templates/coltrane/content.html
+-rw-r--r--   0        0        0        0 2022-02-18 02:46:45.605179 coltrane-0.35.1/coltrane/templatetags/__init__.py
+-rw-r--r--   0        0        0     6625 2023-11-25 04:16:44.358354 coltrane-0.35.1/coltrane/templatetags/coltrane_tags.py
+-rw-r--r--   0        0        0     1539 2024-05-13 22:55:14.207307 coltrane-0.35.1/coltrane/urls.py
+-rw-r--r--   0        0        0     1740 2024-04-30 11:50:51.820465 coltrane-0.35.1/coltrane/utils.py
+-rw-r--r--   0        0        0     7526 2023-11-26 03:27:35.595687 coltrane-0.35.1/coltrane/views.py
+-rw-r--r--   0        0        0     5559 2024-05-25 14:39:09.446568 coltrane-0.35.1/pyproject.toml
+-rw-r--r--   0        0        0     6753 1970-01-01 00:00:00.000000 coltrane-0.35.1/PKG-INFO
```

### Comparing `coltrane-0.35.0/LICENSE` & `coltrane-0.35.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/README.md` & `coltrane-0.35.1/README.md`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/__init__.py` & `coltrane-0.35.1/coltrane/__init__.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/config/cache.py` & `coltrane-0.35.1/coltrane/config/cache.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/config/paths.py` & `coltrane-0.35.1/coltrane/config/paths.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/config/redirects.py` & `coltrane-0.35.1/coltrane/config/redirects.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/config/settings.py` & `coltrane-0.35.1/coltrane/config/settings.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/console.py` & `coltrane-0.35.1/coltrane/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     if not file_path.exists():
         raise Exception("app.py could not be found.")
 
     run_process([file_path, command_name, *list(args)])  # noqa: S603, PLW1510
 
 
-def _copy_file(file_name, in_app_dir=False) -> None:
+def _copy_file(file_name, in_app_dir=False) -> Path:
     default_file_name = file_name
 
     if file_name.startswith("."):
         default_file_name = file_name[1:]
 
     with (FILES_PATH / default_file_name).open() as f:
         file_text = f.read()
@@ -52,14 +52,16 @@
         path = Path(file_name)
 
         if in_app_dir:
             path = APP_DIR / path
 
         path.write_text(file_text)
 
+        return path
+
 
 class AliasedCommands(ClickAliasedGroup, RichCommand):
     pass
 
 
 @click.group(cls=AliasedCommands, help="Runs commands for coltrane.")
 @click.version_option()
@@ -91,25 +93,25 @@
         click.secho("- Create pyproject.toml")
         _copy_file("pyproject.toml")
 
         click.secho("- Create README.md")
         _copy_file("README.md")
 
         click.secho(f"- Create {APP_DIR}/.env")
-        _copy_file(".env", in_app_dir=True)
+        env_file = _copy_file(".env", in_app_dir=True)
 
         # Add randomly generated secret key
-        with (APP_DIR / Path(".env")).open("a") as f:
+        with env_file.open("a") as f:
             f.write(f"SECRET_KEY={get_random_secret_key()}")
 
         click.secho(f"- Create {APP_DIR}/.watchmanconfig")
         _copy_file(".watchmanconfig", in_app_dir=True)
 
         click.secho(f"- Create {APP_DIR}/app.py")
-        _copy_file("app.py", in_app_dir=True)
+        app_file = _copy_file("app.py", in_app_dir=True)
 
         click.secho(f"- Set {APP_DIR}/app.py as executable")
         app_file.chmod(app_file.stat().st_mode | S_IEXEC)
 
         click.secho(f"- Create {APP_DIR}/gunicorn.conf.py")
         _copy_file("gunicorn.conf.py", in_app_dir=True)
```

### Comparing `coltrane-0.35.0/coltrane/default-files/Dockerfile` & `coltrane-0.35.1/coltrane/default-files/Dockerfile`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 # Layer with Python and some shared environment variables
-FROM python:3.10-slim as python
+FROM python:3.10-slim-bullseye as python
 
-ENV PIP_DISABLE_PIP_VERSION_CHECK=1
 ENV PYTHONDONTWRITEBYTECODE=1
 ENV PYTHONUNBUFFERED=1
-ENV PATH=".venv/bin:$PATH"
-
 
 # Layer for installing Python dependencies
 FROM python as dependencies
 
+ENV PIP_DISABLE_PIP_VERSION_CHECK=1
+ENV VIRTUAL_ENV=/opt/venv
+
 # Add some libraries sometimes needed for building Python dependencies, e.g. gcc
 RUN --mount=type=cache,target=/var/cache/apt,sharing=locked --mount=type=cache,target=/var/lib/apt,sharing=locked \
     apt-get update --fix-missing && \
     apt-get install --no-install-recommends -y \
     build-essential
 
-# Copy our Python requirements here to cache them
+# Copy our Python requirements here
 COPY ./pyproject.toml .
 
 # Install uv and Python dependencies
+# Note: Turn off pip progress bar because it seemed to cause some issues on deployment
 # Note: Using a virtualenv seems unnecessary, but it reduces the size of the resulting Docker image
 RUN --mount=type=cache,target=/root/.cache/pip --mount=type=cache,target=/root/.cache/uv \
+    python -m pip config --user set global.progress_bar off && \
     python -m pip install --upgrade pip uv && \
-    uv venv && \
+    uv venv /opt/venv && \
     uv pip install --requirement pyproject.toml
 
 
 # Layer with only the Python dependencies needed for serving the app in production
 FROM python as production
 
+# Copy over just the code
 COPY /site /site
-COPY --from=dependencies .venv /site/.venv
+
+# Copy over the virtualenv and add it to the path
+COPY --from=dependencies /opt/venv /opt/venv
+ENV PATH="/opt/venv/bin:$PATH"
 
 WORKDIR /site
 
 EXPOSE 80
 
 # Collect static assets
 RUN python app.py collectstatic -v 2 --noinput
```

### Comparing `coltrane-0.35.0/coltrane/feeds.py` & `coltrane-0.35.1/coltrane/feeds.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/management/commands/build.py` & `coltrane-0.35.1/coltrane/management/commands/build.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/manifest.py` & `coltrane-0.35.1/coltrane/manifest.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/middleware.py` & `coltrane-0.35.1/coltrane/middleware.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/module_finder.py` & `coltrane-0.35.1/coltrane/module_finder.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/renderer.py` & `coltrane-0.35.1/coltrane/renderer.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/retriever.py` & `coltrane-0.35.1/coltrane/retriever.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/templatetags/coltrane_tags.py` & `coltrane-0.35.1/coltrane/templatetags/coltrane_tags.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/urls.py` & `coltrane-0.35.1/coltrane/urls.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/utils.py` & `coltrane-0.35.1/coltrane/utils.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/coltrane/views.py` & `coltrane-0.35.1/coltrane/views.py`

 * *Files identical despite different names*

### Comparing `coltrane-0.35.0/pyproject.toml` & `coltrane-0.35.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "coltrane"
 authors = [{name = "Adam Hill", email = "adam@adamghill.com"}]
 dynamic = ["version", "description"]
 
 [tool.poetry]
 name = "coltrane"
-version = "0.35.0"
+version = "0.35.1"
 description = "A minimal app framework for content sites 🎵"
 authors = ["adamghill <adam@adamghill.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["django", "python", "static", "markdown"]
 packages = [{ include = "coltrane" }]
 repository = "https://github.com/adamghill/coltrane/"
```

### Comparing `coltrane-0.35.0/PKG-INFO` & `coltrane-0.35.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coltrane
-Version: 0.35.0
+Version: 0.35.1
 Summary: A minimal app framework for content sites 🎵
 Home-page: https://github.com/adamghill/coltrane/
 License: MIT
 Keywords: django,python,static,markdown
 Author: adamghill
 Author-email: adam@adamghill.com
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: coltrane Version: 0.35.0 Summary: A minimal app
+Metadata-Version: 2.1 Name: coltrane Version: 0.35.1 Summary: A minimal app
 framework for content sites ðµ Home-page: https://github.com/adamghill/
 coltrane/ License: MIT Keywords: django,python,static,markdown Author:
 adamghill Author-email: adam@adamghill.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

