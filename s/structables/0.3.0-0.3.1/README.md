# Comparing `tmp/structables-0.3.0.tar.gz` & `tmp/structables-0.3.1.tar.gz`

## Comparing `structables-0.3.0.tar` & `structables-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structables-0.3.0/cronjob.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/__init__.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/config.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/main.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/category.py
--rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/contest.py
--rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/main.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/member.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/routes/proxy.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/css/style.css
--rw-r--r--   0        0        0   232948 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css
--rw-r--r--   0        0        0   589161 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css.map
--rw-r--r--   0        0        0    80663 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   331886 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/img/logo.png
--rw-r--r--   0        0        0   912206 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/img/logo_lg.png
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/static/img/magnifying-glass-solid.svg
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/400.html
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/404.html
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/429.html
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/500.html
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/archives.html
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/article-review.html
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/article.html
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/base.html
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/category.html
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/collection.html
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/contest.html
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/contests.html
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/footer.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/header.html
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/iframe.html
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/index.html
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/member-instructables.html
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/member.html
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/privacypolicy.html
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/projects.html
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/sitemap.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/templates/style.html
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/utils/data.py
--rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 structables-0.3.0/src/structables/utils/helpers.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 structables-0.3.0/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 structables-0.3.0/LICENSE
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 structables-0.3.0/README.md
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 structables-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    43742 2020-02-02 00:00:00.000000 structables-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 structables-0.3.1/cronjob.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/__init__.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/config.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/main.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/routes/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/routes/category.py
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/routes/contest.py
+-rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/routes/main.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/routes/member.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/routes/proxy.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/css/style.css
+-rw-r--r--   0        0        0   232948 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/dist/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589161 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/dist/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0    80663 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331886 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0    24209 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/img/logo.png
+-rw-r--r--   0        0        0   912206 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/img/logo_lg.png
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/static/img/magnifying-glass-solid.svg
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/400.html
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/404.html
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/429.html
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/500.html
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/archives.html
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/article-review.html
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/article.html
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/base.html
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/category.html
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/collection.html
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/contest.html
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/contests.html
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/footer.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/header.html
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/iframe.html
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/index.html
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/member-instructables.html
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/member.html
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/privacypolicy.html
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/projects.html
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/sitemap.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/templates/style.html
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/utils/data.py
+-rw-r--r--   0        0        0    12799 2020-02-02 00:00:00.000000 structables-0.3.1/src/structables/utils/helpers.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 structables-0.3.1/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 structables-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 structables-0.3.1/README.md
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 structables-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    43709 2020-02-02 00:00:00.000000 structables-0.3.1/PKG-INFO
```

### Comparing `structables-0.3.0/src/structables/main.py` & `structables-0.3.1/src/structables/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 
 app = Flask(__name__, template_folder="templates", static_folder="static")
 app.config.from_object(Config)
 app.typesense_api_key = get_typesense_api_key()
 
 init_routes(app)
 
-if __name__ == "__main__":
+def main():
     app.run(port=app.config['PORT'], host=app.config['LISTEN_HOST'], debug=app.config['DEBUG'])
 
+if __name__ == "__main__":
+    main()
+
 # Initialize data when the server starts
 update_data(app)
```

### Comparing `structables-0.3.0/src/structables/routes/category.py` & `structables-0.3.1/src/structables/routes/category.py`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/routes/contest.py` & `structables-0.3.1/src/structables/routes/contest.py`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/routes/main.py` & `structables-0.3.1/src/structables/routes/main.py`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/routes/member.py` & `structables-0.3.1/src/structables/routes/member.py`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/routes/proxy.py` & `structables-0.3.1/src/structables/routes/proxy.py`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/static/css/style.css` & `structables-0.3.1/src/structables/static/css/style.css`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css` & `structables-0.3.1/src/structables/static/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/static/dist/css/bootstrap.min.css.map` & `structables-0.3.1/src/structables/static/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js` & `structables-0.3.1/src/structables/static/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/static/dist/js/bootstrap.bundle.min.js.map` & `structables-0.3.1/src/structables/static/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/static/img/logo.png` & `structables-0.3.1/src/structables/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/static/img/logo_lg.png` & `structables-0.3.1/src/structables/static/img/logo_lg.png`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/archives.html` & `structables-0.3.1/src/structables/templates/archives.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/article.html` & `structables-0.3.1/src/structables/templates/article.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/base.html` & `structables-0.3.1/src/structables/templates/base.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/category.html` & `structables-0.3.1/src/structables/templates/category.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/collection.html` & `structables-0.3.1/src/structables/templates/collection.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/contest.html` & `structables-0.3.1/src/structables/templates/contest.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/contests.html` & `structables-0.3.1/src/structables/templates/contests.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/header.html` & `structables-0.3.1/src/structables/templates/header.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/index.html` & `structables-0.3.1/src/structables/templates/index.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/member-instructables.html` & `structables-0.3.1/src/structables/templates/member-instructables.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/member.html` & `structables-0.3.1/src/structables/templates/member.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/projects.html` & `structables-0.3.1/src/structables/templates/projects.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/templates/sitemap.html` & `structables-0.3.1/src/structables/templates/sitemap.html`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/utils/data.py` & `structables-0.3.1/src/structables/utils/data.py`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/src/structables/utils/helpers.py` & `structables-0.3.1/src/structables/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/LICENSE` & `structables-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `structables-0.3.0/README.md` & `structables-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img align="right" src="src/structables/static/img/logo.png">
 
 # Structables
 
-An open source alternative front-end to Instructables. This is a fork of <a href="https://codeberg.org/indestructables/indestructables">snowcatridge10's Indestructables</a> to get rid of Selenium. Indestructables itself is a fork of <a href="https://git.vern.cc/cobra/Destructables">Cobra's Destructables</a>.
+An open source alternative front-end to Instructables. This is a fork of <a href="https://codeberg.org/indestructables/indestructables">snowcatridge10's Indestructables</a>, which itself is a fork of <a href="https://git.vern.cc/cobra/Destructables">Cobra's Destructables</a>.
 
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 [![Matrix](https://shields.private.coffee/badge/Matrix-join%20us!-blue?logo=matrix)](https://matrix.pcof.fi/#/#structables:private.coffee)
 [![PyPI](https://shields.private.coffee/pypi/v/structables)](https://pypi.org/project/structables/)
 [![PyPI - Python Version](https://shields.private.coffee/pypi/pyversions/structables)](https://pypi.org/project/structables/)
 [![PyPI - License](https://shields.private.coffee/pypi/l/structables)](https://pypi.org/project/structables/)
 [![Latest Git Commit](https://shields.private.coffee/gitea/last-commit/privatecoffee/structables?gitea_url=https://git.private.coffee)](https://git.private.coffee/privatecoffee/structables)
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
 [src/structables/static/img/logo.png]# Structables An open source alternative
-front-end to Instructables. This is a fork of _s_n_o_w_c_a_t_r_i_d_g_e_1_0_'_s_ _I_n_d_e_s_t_r_u_c_t_a_b_l_e_s
-to get rid of Selenium. Indestructables itself is a fork of _C_o_b_r_a_'_s
-_D_e_s_t_r_u_c_t_a_b_l_e_s. [![Support Private.coffee!](https://shields.private.coffee/
-badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://
-private.coffee) [![Matrix](https://shields.private.coffee/badge/Matrix-
-join%20us!-blue?logo=matrix)](https://matrix.pcof.fi/#/#structables:
-private.coffee) [![PyPI](https://shields.private.coffee/pypi/v/structables)]
-(https://pypi.org/project/structables/) [![PyPI - Python Version](https://
-shields.private.coffee/pypi/pyversions/structables)](https://pypi.org/project/
-structables/) [![PyPI - License](https://shields.private.coffee/pypi/l/
-structables)](https://pypi.org/project/structables/) [![Latest Git Commit]
-(https://shields.private.coffee/gitea/last-commit/privatecoffee/
-structables?gitea_url=https://git.private.coffee)](https://git.private.coffee/
-privatecoffee/structables) ## Instances | URL | Provided by | Country |
-Comments | | ------------------------------------------------------------------
--------- | ----------------------------------------- | ------- | -------- | |
-[https://structables.private.coffee/](https://structables.private.coffee/) |
-[Private.coffee](https://private.coffee/) | Austria | | To add your own
-instance to this list, please open a pull request or issue. ## Opening Issues
-If you're having problems using Structables, or if you have ideas or feedback
-for us, feel free to open an issue in the [Private.coffee Git](https://
-git.private.coffee/PrivateCoffee/structables/issues) or on [Github](https://
-github.com/PrivateCoffee/structables/issues). Of course, you can also join our
-[Matrix room](https://matrix.pcof.fi/#/#structables:private.coffee) to discuss
-your ideas with us. ## Run your own instance ### Production 1. Create a virtual
-environment: `python3 -m venv venv` 2. Activate the virtual environment:
-`source venv/bin/activate` 3. Install the packages: `pip install structables
-uwsgi` 4. Run `uwsgi --plugin python3 --http-socket 0.0.0.0:8002 --module
-structables.main:app --processes 4 --threads 4` 5. Point your reverse proxy to
-http://localhost:8002 and (optionally) serve static files from the `venv/lib/
-pythonX.XX/site-packages/structables/static` directory 6. Connect to your
-instance under your domain ### Development 1. Clone the repository: `git clone
-https://git.private.coffee/privatecoffee/structables.git && cd structables` 2.
-Create a virtual environment: `python3 -m venv venv` 3. Activate the virtual
-environment: `source venv/bin/activate` 4. Install in editable mode: `pip
-install -e .` 5. Run `structables` 6. Connect to http://localhost:8002 ##
-License This project, as well as the two projects it is based on, are licensed
-under the GNU Affero General Public License v3. See the [LICENSE](LICENSE) file
-for more information.
+front-end to Instructables. This is a fork of _s_n_o_w_c_a_t_r_i_d_g_e_1_0_'_s_ _I_n_d_e_s_t_r_u_c_t_a_b_l_e_s,
+which itself is a fork of _C_o_b_r_a_'_s_ _D_e_s_t_r_u_c_t_a_b_l_e_s. [![Support Private.coffee!]
+(https://shields.private.coffee/badge/private.coffee-support%20us!-
+pink?logo=coffeescript)](https://private.coffee) [![Matrix](https://
+shields.private.coffee/badge/Matrix-join%20us!-blue?logo=matrix)](https://
+matrix.pcof.fi/#/#structables:private.coffee) [![PyPI](https://
+shields.private.coffee/pypi/v/structables)](https://pypi.org/project/
+structables/) [![PyPI - Python Version](https://shields.private.coffee/pypi/
+pyversions/structables)](https://pypi.org/project/structables/) [![PyPI -
+License](https://shields.private.coffee/pypi/l/structables)](https://pypi.org/
+project/structables/) [![Latest Git Commit](https://shields.private.coffee/
+gitea/last-commit/privatecoffee/structables?gitea_url=https://
+git.private.coffee)](https://git.private.coffee/privatecoffee/structables) ##
+Instances | URL | Provided by | Country | Comments | | ------------------------
+-------------------------------------------------- | --------------------------
+--------------- | ------- | -------- | | [https://structables.private.coffee/]
+(https://structables.private.coffee/) | [Private.coffee](https://
+private.coffee/) | Austria | | To add your own instance to this list, please
+open a pull request or issue. ## Opening Issues If you're having problems using
+Structables, or if you have ideas or feedback for us, feel free to open an
+issue in the [Private.coffee Git](https://git.private.coffee/PrivateCoffee/
+structables/issues) or on [Github](https://github.com/PrivateCoffee/
+structables/issues). Of course, you can also join our [Matrix room](https://
+matrix.pcof.fi/#/#structables:private.coffee) to discuss your ideas with us. ##
+Run your own instance ### Production 1. Create a virtual environment: `python3
+-m venv venv` 2. Activate the virtual environment: `source venv/bin/activate`
+3. Install the packages: `pip install structables uwsgi` 4. Run `uwsgi --plugin
+python3 --http-socket 0.0.0.0:8002 --module structables.main:app --processes 4
+--threads 4` 5. Point your reverse proxy to http://localhost:8002 and
+(optionally) serve static files from the `venv/lib/pythonX.XX/site-packages/
+structables/static` directory 6. Connect to your instance under your domain ###
+Development 1. Clone the repository: `git clone https://git.private.coffee/
+privatecoffee/structables.git && cd structables` 2. Create a virtual
+environment: `python3 -m venv venv` 3. Activate the virtual environment:
+`source venv/bin/activate` 4. Install in editable mode: `pip install -e .` 5.
+Run `structables` 6. Connect to http://localhost:8002 ## License This project,
+as well as the two projects it is based on, are licensed under the GNU Affero
+General Public License v3. See the [LICENSE](LICENSE) file for more
+information.
```

### Comparing `structables-0.3.0/pyproject.toml` & `structables-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "structables"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Private.coffee Team", email="support@private.coffee" },
 ]
 description = "A simple frontend for Instructables"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `structables-0.3.0/PKG-INFO` & `structables-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: structables
-Version: 0.3.0
+Version: 0.3.1
 Summary: A simple frontend for Instructables
 Project-URL: Homepage, https://git.private.coffee/privatecoffee/structables
 Project-URL: Bug Tracker, https://git.private.coffee/privatecoffee/structables/issues
 Project-URL: Source Code, https://git.private.coffee/privatecoffee/structables
 Author-email: "Private.coffee Team" <support@private.coffee>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
@@ -676,15 +676,15 @@
 Requires-Dist: flask
 Description-Content-Type: text/markdown
 
 <img align="right" src="src/structables/static/img/logo.png">
 
 # Structables
 
-An open source alternative front-end to Instructables. This is a fork of <a href="https://codeberg.org/indestructables/indestructables">snowcatridge10's Indestructables</a> to get rid of Selenium. Indestructables itself is a fork of <a href="https://git.vern.cc/cobra/Destructables">Cobra's Destructables</a>.
+An open source alternative front-end to Instructables. This is a fork of <a href="https://codeberg.org/indestructables/indestructables">snowcatridge10's Indestructables</a>, which itself is a fork of <a href="https://git.vern.cc/cobra/Destructables">Cobra's Destructables</a>.
 
 [![Support Private.coffee!](https://shields.private.coffee/badge/private.coffee-support%20us!-pink?logo=coffeescript)](https://private.coffee)
 [![Matrix](https://shields.private.coffee/badge/Matrix-join%20us!-blue?logo=matrix)](https://matrix.pcof.fi/#/#structables:private.coffee)
 [![PyPI](https://shields.private.coffee/pypi/v/structables)](https://pypi.org/project/structables/)
 [![PyPI - Python Version](https://shields.private.coffee/pypi/pyversions/structables)](https://pypi.org/project/structables/)
 [![PyPI - License](https://shields.private.coffee/pypi/l/structables)](https://pypi.org/project/structables/)
 [![Latest Git Commit](https://shields.private.coffee/gitea/last-commit/privatecoffee/structables?gitea_url=https://git.private.coffee)](https://git.private.coffee/privatecoffee/structables)
```

