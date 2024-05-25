# Comparing `tmp/fastblocks-0.4.4.tar.gz` & `tmp/fastblocks-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.4.4.tar", last modified: Mon May 20 11:11:27 2024, max compression
+gzip compressed data, was "fastblocks-0.4.5.tar", last modified: Sat May 25 10:52:22 2024, max compression
```

## Comparing `fastblocks-0.4.4.tar` & `fastblocks-0.4.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.4/LICENSE
--rw-r--r--   0        0        0     1181 2024-05-20 05:59:48.364048 fastblocks-0.4.4/README.md
--rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.4/fastblocks/Dockerfile
--rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.4/fastblocks/__init__.py
--rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.4/fastblocks/__main__.py
--rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.4/fastblocks/actions/__init__.py
--rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.4/fastblocks/actions/minify.py
--rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.4/fastblocks/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.4/fastblocks/adapters/admin/__init__.py
--rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.4/fastblocks/adapters/admin/_base.py
--rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.4/fastblocks/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.4/fastblocks/adapters/app/__init__.py
--rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.4/fastblocks/adapters/app/_base.py
--rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.4/fastblocks/adapters/app/main.py
--rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.4/fastblocks/adapters/auth/__init__.py
--rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.4/fastblocks/adapters/auth/_base.py
--rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.4/fastblocks/adapters/auth/basic.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.4/fastblocks/adapters/fonts/__init__.py
--rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.4/fastblocks/adapters/fonts/_base.py
--rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.4/fastblocks/adapters/fonts/google.py
--rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.4/fastblocks/adapters/routes/__init__.py
--rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.4/fastblocks/adapters/routes/_base.py
--rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.4/fastblocks/adapters/routes/default.py
--rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.4/fastblocks/adapters/sitemap/__init__.py
--rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.4/fastblocks/adapters/sitemap/_base.py
--rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.4/fastblocks/adapters/sitemap/sitemap.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.4/fastblocks/adapters/style/__init__.py
--rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.4/fastblocks/adapters/style/_base.py
--rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.4/fastblocks/adapters/style/bulma.py
--rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.4/fastblocks/adapters/templates/__init__.py
--rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.4/fastblocks/adapters/templates/_base.py
--rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.4/fastblocks/adapters/templates/_filters.py
--rw-r--r--   0        0        0    14844 2024-05-20 08:55:18.809237 fastblocks-0.4.4/fastblocks/adapters/templates/jinja2.py
--rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.4/fastblocks/applications.py
--rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.4/fastblocks/middleware.py
--rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.4/fastblocks/templates/admin/bootstrap/blocks/display_menu.html
--rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.4/fastblocks/templates/admin/bootstrap/blocks/menu_category.html
--rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.4/fastblocks/templates/admin/bootstrap/blocks/menu_item.html
--rw-r--r--   0        0        0     1965 2024-04-15 14:32:35.783285 fastblocks-0.4.4/fastblocks/templates/admin/bootstrap/layout.html
--rw-r--r--   0        0        0     3052 2024-05-20 11:11:27.548097 fastblocks-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 fastblocks-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1181 2024-05-20 05:59:48.364048 fastblocks-0.4.5/README.md
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.5/fastblocks/Dockerfile
+-rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.5/fastblocks/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.5/fastblocks/__main__.py
+-rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.5/fastblocks/actions/__init__.py
+-rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.5/fastblocks/actions/minify.py
+-rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.5/fastblocks/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.5/fastblocks/adapters/admin/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.5/fastblocks/adapters/admin/_base.py
+-rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.5/fastblocks/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.5/fastblocks/adapters/app/__init__.py
+-rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.5/fastblocks/adapters/app/_base.py
+-rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.5/fastblocks/adapters/app/main.py
+-rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.5/fastblocks/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.5/fastblocks/adapters/auth/_base.py
+-rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.5/fastblocks/adapters/auth/basic.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.5/fastblocks/adapters/fonts/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.5/fastblocks/adapters/fonts/_base.py
+-rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.5/fastblocks/adapters/fonts/google.py
+-rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.5/fastblocks/adapters/routes/__init__.py
+-rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.5/fastblocks/adapters/routes/_base.py
+-rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.5/fastblocks/adapters/routes/default.py
+-rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.5/fastblocks/adapters/sitemap/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.5/fastblocks/adapters/sitemap/_base.py
+-rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.5/fastblocks/adapters/sitemap/sitemap.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.5/fastblocks/adapters/style/__init__.py
+-rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.5/fastblocks/adapters/style/_base.py
+-rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.5/fastblocks/adapters/style/bulma.py
+-rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.5/fastblocks/adapters/templates/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.5/fastblocks/adapters/templates/_base.py
+-rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.5/fastblocks/adapters/templates/_filters.py
+-rw-r--r--   0        0        0    14835 2024-05-25 09:45:13.843280 fastblocks-0.4.5/fastblocks/adapters/templates/jinja2.py
+-rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.5/fastblocks/applications.py
+-rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.5/fastblocks/middleware.py
+-rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/display_menu.html
+-rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_category.html
+-rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_item.html
+-rw-r--r--   0        0        0     1974 2024-05-25 10:44:19.709513 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/layout.html
+-rw-r--r--   0        0        0     3052 2024-05-25 10:52:22.244897 fastblocks-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 fastblocks-0.4.5/PKG-INFO
```

### Comparing `fastblocks-0.4.4/LICENSE` & `fastblocks-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/README.md` & `fastblocks-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/admin/sqladmin.py` & `fastblocks-0.4.5/fastblocks/adapters/admin/sqladmin.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/app/main.py` & `fastblocks-0.4.5/fastblocks/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/auth/_base.py` & `fastblocks-0.4.5/fastblocks/adapters/auth/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/fonts/google.py` & `fastblocks-0.4.5/fastblocks/adapters/fonts/google.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/routes/default.py` & `fastblocks-0.4.5/fastblocks/adapters/routes/default.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/sitemap/sitemap.py` & `fastblocks-0.4.5/fastblocks/adapters/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/style/_base.py` & `fastblocks-0.4.5/fastblocks/adapters/style/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/templates/_filters.py` & `fastblocks-0.4.5/fastblocks/adapters/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/adapters/templates/jinja2.py` & `fastblocks-0.4.5/fastblocks/adapters/templates/jinja2.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             searchpaths.extend([path, path / "blocks"])
         loaders: list[AsyncBaseLoader] = [
             RedisLoader(searchpaths),
             CloudLoader(searchpaths),
         ]
         file_loaders: list[AsyncBaseLoader] = [FileSystemLoader(searchpaths)]
         if admin:
-            file_loaders.append(PackageLoader("sqladmin", "templates/sqladmin"))
+            file_loaders.append(PackageLoader("sqladmin", "templates"))
         jinja_loaders = loaders + file_loaders  # type: ignore[override]
         if not self.config.deployed and not self.config.debug.production:
             jinja_loaders = file_loaders + loaders  # type: ignore[override]
         return ChoiceLoader(jinja_loaders, template_paths.style)
 
     async def init_envs(
         self, template_paths: EnvTemplatePaths, admin: bool = False
```

### Comparing `fastblocks-0.4.4/fastblocks/applications.py` & `fastblocks-0.4.5/fastblocks/applications.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/middleware.py` & `fastblocks-0.4.5/fastblocks/middleware.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/templates/admin/bootstrap/blocks/menu_category.html` & `fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_category.html`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.4/fastblocks/templates/admin/bootstrap/layout.html` & `fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/layout.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[% extends "base.html" %]
+[% extends "sqladmin/base.html" %]
 [% block body %]
 <div class="wrapper">
   <aside class="navbar navbar-expand-lg navbar-vertical navbar-expand-md navbar-dark">
     <div class="container-fluid">
       <h1 class="navbar-brand navbar-brand-autodark">
         <a href="[[ url_for('admin:index') ]]">
           [% if admin.logo_url %]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-[% extends "base.html" %] [% block body %]
+[% extends "sqladmin/base.html" %] [% block body %]
 _[[_%%_ _ii_ff_ _aa_dd_mm_ii_nn_.._ll_oo_gg_oo____uu_rr_ll_ _%%_]]_ _[[_AA_dd_mm_ii_nn_]]_[[_%%_ _ee_ll_ss_ee_ _%%_]]
 _**_**_**_**_ _[[_[[_ _aa_dd_mm_ii_nn_.._tt_ii_tt_ll_ee_ _]]_]]_ _**_**_**_**
 _[[_%%_ _ee_nn_dd_ii_ff_ _%%_]]
 [[ render_block('display_menu.html', menu=admin._menu, request=request) ]]
 [% if admin.authentication_backend %]
 _L_o_g_o_u_t
 [% endif %]
```

### Comparing `fastblocks-0.4.4/pyproject.toml` & `fastblocks-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastblocks"
-version = "0.4.4"
+version = "0.4.5"
 description = "Starlette based app for the rapid delivery HTMX/Jinja template blocks"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -107,37 +107,37 @@
 
 [tool.creosote]
 paths = [
     "fastblocks",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
+    "pytest",
     "autotyping",
+    "libsass",
     "pdm",
-    "aiohttp",
-    "pyfiglet",
     "pdm-bump",
     "phonenumbers",
     "pre-commit",
-    "libsass",
-    "pytest",
+    "pyfiglet",
+    "aiohttp",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "fastblocks",
 ]
 skips = [
+    "B113",
+    "B404",
     "B603",
     "B403",
-    "B404",
-    "B113",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "fastblocks",
 ]
```

### Comparing `fastblocks-0.4.4/PKG-INFO` & `fastblocks-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastblocks
-Version: 0.4.4
+Version: 0.4.5
 Summary: Starlette based app for the rapid delivery HTMX/Jinja template blocks
 Keywords: starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic,sqlalchemy,redis
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastblocks Version: 0.4.4 Summary: Starlette based
+Metadata-Version: 2.1 Name: fastblocks Version: 0.4.5 Summary: Starlette based
 app for the rapid delivery HTMX/Jinja template blocks Keywords:
 starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic,sqlalchemy,redis
 Author-Email: lesleslie
 wedgwoodwebworks.com> Maintainer-Email: lesleslie
 wedgwoodwebworks.com> License: BSD-3-Clause Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
```

