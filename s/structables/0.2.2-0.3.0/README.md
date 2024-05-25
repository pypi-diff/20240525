# Comparing `tmp/structables-0.2.2.tar.gz` & `tmp/structables-0.3.0.tar.gz`

## Comparing `structables-0.2.2.tar` & `structables-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,47 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structables-0.2.2/cronjob.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/__init__.py
--rw-r--r--   0        0        0    40613 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/main.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/css/style.css
--rw-r--r--   0        0        0   232948 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/dist/css/bootstrap.min.css
--rw-r--r--   0        0        0   589161 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/dist/css/bootstrap.min.css.map
--rw-r--r--   0        0        0    80663 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331886 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/img/logo.png
--rw-r--r--   0        0        0   912206 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/img/logo_lg.png
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/static/img/magnifying-glass-solid.svg
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/400.html
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/404.html
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/429.html
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/500.html
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/archives.html
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/article-review.html
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/article.html
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/base.html
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/category.html
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/collection.html
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/contest.html
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/contests.html
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/footer.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/header.html
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/iframe.html
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/index.html
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/member-instructables.html
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/member.html
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/privacypolicy.html
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/projects.html
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/sitemap.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 structables-0.2.2/src/structables/templates/style.html
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 structables-0.2.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 structables-0.2.2/LICENSE
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 structables-0.2.2/README.md
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 structables-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    43742 2020-02-02 00:00:00.000000 structables-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structables-0.3.0/cronjob.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/__init__.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/config.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/main.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/category.py
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/contest.py
+-rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/main.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/member.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/proxy.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/css/style.css
+-rw-r--r--   0        0        0   232948 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589161 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0    80663 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331886 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/img/logo.png
+-rw-r--r--   0        0        0   912206 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/img/logo_lg.png
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/img/magnifying-glass-solid.svg
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/400.html
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/404.html
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/429.html
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/500.html
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/archives.html
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/article-review.html
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/article.html
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/base.html
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/category.html
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/collection.html
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/contest.html
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/contests.html
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/footer.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/header.html
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/iframe.html
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/index.html
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/member-instructables.html
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/member.html
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/privacypolicy.html
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/projects.html
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/sitemap.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/style.html
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/utils/data.py
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/utils/helpers.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 structables-0.3.0/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 structables-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 structables-0.3.0/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 structables-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    43742 2020-02-02 00:00:00.000000 structables-0.3.0/PKG-INFO
```

### Comparing `structables-0.2.2/src/structables/static/css/style.css` & `structables-0.3.0/src/structables/static/css/style.css`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/static/dist/css/bootstrap.min.css` & `structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/static/dist/css/bootstrap.min.css.map` & `structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/static/dist/js/bootstrap.bundle.min.js` & `structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/static/dist/js/bootstrap.bundle.min.js.map` & `structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/static/img/logo.png` & `structables-0.3.0/src/structables/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/static/img/logo_lg.png` & `structables-0.3.0/src/structables/static/img/logo_lg.png`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/archives.html` & `structables-0.3.0/src/structables/templates/archives.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/article.html` & `structables-0.3.0/src/structables/templates/article.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/base.html` & `structables-0.3.0/src/structables/templates/base.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/category.html` & `structables-0.3.0/src/structables/templates/category.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/collection.html` & `structables-0.3.0/src/structables/templates/collection.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/contest.html` & `structables-0.3.0/src/structables/templates/contest.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/contests.html` & `structables-0.3.0/src/structables/templates/contests.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/header.html` & `structables-0.3.0/src/structables/templates/header.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/index.html` & `structables-0.3.0/src/structables/templates/index.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/member-instructables.html` & `structables-0.3.0/src/structables/templates/member-instructables.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/member.html` & `structables-0.3.0/src/structables/templates/member.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/projects.html` & `structables-0.3.0/src/structables/templates/projects.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/src/structables/templates/sitemap.html` & `structables-0.3.0/src/structables/templates/sitemap.html`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/LICENSE` & `structables-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/README.md` & `structables-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `structables-0.2.2/pyproject.toml` & `structables-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "structables"
-version = "0.2.2"
+version = "0.3.0"
 authors = [
   { name="Private.coffee Team", email="support@private.coffee" },
 ]
 description = "A simple frontend for Instructables"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `structables-0.2.2/PKG-INFO` & `structables-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: structables
-Version: 0.2.2
+Version: 0.3.0
 Summary: A simple frontend for Instructables
 Project-URL: Homepage, https://git.private.coffee/privatecoffee/structables
 Project-URL: Bug Tracker, https://git.private.coffee/privatecoffee/structables/issues
 Project-URL: Source Code, https://git.private.coffee/privatecoffee/structables
 Author-email: "Private.coffee Team" <support@private.coffee>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

