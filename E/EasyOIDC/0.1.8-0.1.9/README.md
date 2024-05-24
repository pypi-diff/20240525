# Comparing `tmp/easyoidc-0.1.8.tar.gz` & `tmp/easyoidc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyoidc-0.1.8.tar", last modified: Tue Apr 30 23:29:11 2024, max compression
+gzip compressed data, was "easyoidc-0.1.9.tar", last modified: Fri May 24 22:17:57 2024, max compression
```

## Comparing `easyoidc-0.1.8.tar` & `easyoidc-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/EasyOIDC/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/EasyOIDC/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/nicegui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/frameworks/taipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-30 23:29:07.000000 easyoidc-0.1.8/EasyOIDC/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:29:11.141757 easyoidc-0.1.8/EasyOIDC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-30 23:29:11.000000 easyoidc-0.1.8/EasyOIDC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 23:29:07.000000 easyoidc-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-04-30 23:29:11.141757 easyoidc-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-04-30 23:29:07.000000 easyoidc-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:29:11.141757 easyoidc-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-30 23:29:07.000000 easyoidc-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:17:57.121511 easyoidc-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:17:57.117511 easyoidc-0.1.9/EasyOIDC/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8582 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:17:57.121511 easyoidc-0.1.9/EasyOIDC/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/frameworks/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/frameworks/nicegui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/frameworks/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/frameworks/taipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-24 22:17:53.000000 easyoidc-0.1.9/EasyOIDC/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:17:57.121511 easyoidc-0.1.9/EasyOIDC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-24 22:17:57.000000 easyoidc-0.1.9/EasyOIDC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-24 22:17:57.000000 easyoidc-0.1.9/EasyOIDC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:17:57.000000 easyoidc-0.1.9/EasyOIDC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-24 22:17:57.000000 easyoidc-0.1.9/EasyOIDC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 22:17:57.000000 easyoidc-0.1.9/EasyOIDC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-24 22:17:53.000000 easyoidc-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6765 2024-05-24 22:17:57.121511 easyoidc-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6111 2024-05-24 22:17:53.000000 easyoidc-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:17:57.121511 easyoidc-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-24 22:17:53.000000 easyoidc-0.1.9/setup.py
```

### Comparing `easyoidc-0.1.8/EasyOIDC/auth.py` & `easyoidc-0.1.9/EasyOIDC/auth.py`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/EasyOIDC/config.py` & `easyoidc-0.1.9/EasyOIDC/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,24 @@
     token_revoke_endpoint = None
     logout_endpoint = None
     post_logout_uri = None
     app_login_route = None
     app_logout_route = None
     app_authorize_route = None
     auth_service = None
+    base_unrestricted_routes = ['/favicon.ico']
 
     def __init__(self, config_path=None, **kwargs):
         # Defaults
         self.scope = ['openid', 'email', 'profile']
         self.app_login_route = '/login'
         self.app_logout_route = '/logout'
         self.app_authorize_route = '/authorize'
-        self.unrestricted_routes = ['/favicon.ico']
+        self.base_unrestricted_routes = kwargs.get('base_unrestricted_routes', self.base_unrestricted_routes)
+        self.unrestricted_routes = self.base_unrestricted_routes
 
         if config_path and (os.path.exists(config_path)):
             try:
                 self.load_from_json(config_path)
             except:
                 self.load_from_env_file(config_path)
         for key, value in kwargs.items():
@@ -63,14 +65,15 @@
             self.client_id = data['client_id']
             self.client_secret = data['client_secret']
             self.cookie_secret_key = data['cookie_secret_key']
             self.scope = data.get('scope', '').split(',')
             self.token_revoke_endpoint = data.get('token_revoke_endpoint', None)
             self.logout_endpoint = data.get('logout_endpoint', None)
             self.post_logout_uri = data.get('post_logout_uri', None)
+            self.unrestricted_routes = self.base_unrestricted_routes + data.get('unrestricted_routes', '').split(',')
 
     def load_from_env_file(self, config_path):
         from decouple import Config, RepositoryEnv
         config = Config(RepositoryEnv(config_path))
         self.well_known_openid_url = config('well_known_openid_url', None)
         self.authorization_endpoint = config('authorization_endpoint', None)
         self.token_endpoint = config('token_endpoint', None)
@@ -79,14 +82,15 @@
         self.client_id = config('client_id')
         self.client_secret = config('client_secret')
         self.scope = config('scope', '').split(',')
         self.cookie_secret_key = config('cookie_secret_key')
         self.token_revoke_endpoint = config('token_revoke_endpoint', None)
         self.logout_endpoint = config('logout_endpoint', None)
         self.post_logout_uri = config('post_logout_uri', None)
+        self.unrestricted_routes = self.base_unrestricted_routes + config('unrestricted_routes', '').split(',')
 
     def get_unrestricted_routes(self):
         return [self.app_login_route, self.app_authorize_route, self.app_logout_route] + self.unrestricted_routes
 
     def dump_configuration(self, hide_password=True):
         config = dict(well_known_openid_url=self.well_known_openid_url,
                       authorization_endpoint=self.authorization_endpoint,
@@ -149,12 +153,7 @@
             assert self.client_id is not None
             assert self.client_secret is not None
             assert self.cookie_secret_key is not None
             assert isinstance(self.scope, list)
         except Exception as e:
             raise Exception(f"Missing configuration parameters. {e}")
         return True
-
-
-
-
-
```

### Comparing `easyoidc-0.1.8/EasyOIDC/frameworks/flask.py` & `easyoidc-0.1.9/EasyOIDC/frameworks/flask.py`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/EasyOIDC/frameworks/nicegui.py` & `easyoidc-0.1.9/EasyOIDC/frameworks/nicegui.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
         self._session_storage = session_storage
         self._nicegui_app = nicegui_app
 
         if 'unrestricted_routes' in kwargs:
             self._auth_config.unrestricted_routes = kwargs['unrestricted_routes']
         else:
             # Get all routes from nicegui app
-            nicegui_routes = [r.path.replace('{key:path}', '*').replace('{key}/{path:path}', '*') for r in nicegui_app.routes if isinstance(r, Route)]
-            self._auth_config.unrestricted_routes = nicegui_routes + ['/_nicegui/*']
+            nicegui_routes = ([r.path.replace('{key:path}', '*').replace('{key}/{path:path}', '*') for r in
+                              nicegui_app.routes if (type(r) == Route) or (r.path.startswith('/_nicegui'))] +
+                              ['/_nicegui/*'])
+            self._auth_config.unrestricted_routes += nicegui_routes
 
         if 'logger' in kwargs:
             self.logger = kwargs['logger']
 
         auth_middleware = AuthMiddleware
         auth_middleware.logger = self.logger
         auth_middleware.session_storage = session_storage
@@ -42,15 +44,17 @@
         auth_middleware.log_enabled = log_enabled
         auth_middleware.nicegui_app = nicegui_app
         self._nicegui_app.add_middleware(auth_middleware)
 
         self.set_redirector(lambda url: RedirectResponse(url))
 
         self.set_roles_getter(
-            lambda: self._session_storage[nicegui_app.storage.user.get(SESSION_STATE_VAR_NAME, '')].get('userinfo', {}).get('realm_access', {}).get(
+            lambda: self._session_storage[nicegui_app.storage.user.get(SESSION_STATE_VAR_NAME, '')].get('userinfo',
+                                                                                                        {}).get(
+                'realm_access', {}).get(
                 'roles', []))
 
         # Add FastAPI route /login to method login_route_handler
         self._nicegui_app.add_route(auth_config.app_login_route, self._login_route_handler)
 
         # Add FastAPI route /authorize to method authorize_route_handler
         self._nicegui_app.add_route(auth_config.app_authorize_route, self._authorize_route_handler)
```

### Comparing `easyoidc-0.1.8/EasyOIDC/frameworks/streamlit.py` & `easyoidc-0.1.9/EasyOIDC/frameworks/streamlit.py`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/EasyOIDC/frameworks/taipy.py` & `easyoidc-0.1.9/EasyOIDC/frameworks/taipy.py`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/EasyOIDC/session.py` & `easyoidc-0.1.9/EasyOIDC/session.py`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/EasyOIDC/utils.py` & `easyoidc-0.1.9/EasyOIDC/utils.py`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/EasyOIDC.egg-info/PKG-INFO` & `easyoidc-0.1.9/EasyOIDC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyOIDC
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy integration with OIDC authentication servers
 Home-page: https://github.com/jpmanson/EasyOIDC
 Author: Juan Pablo Manson
 Author-email: jpmanson@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easyoidc-0.1.8/LICENSE` & `easyoidc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/PKG-INFO` & `easyoidc-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyOIDC
-Version: 0.1.8
+Version: 0.1.9
 Summary: Easy integration with OIDC authentication servers
 Home-page: https://github.com/jpmanson/EasyOIDC
 Author: Juan Pablo Manson
 Author-email: jpmanson@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `easyoidc-0.1.8/README.md` & `easyoidc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `easyoidc-0.1.8/setup.py` & `easyoidc-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 from pathlib import Path
 
 README = (Path(__file__).parent/"README.md").read_text()
 
 setuptools.setup(
     name="EasyOIDC",
-    version="0.1.8",
+    version="0.1.9",
     author="Juan Pablo Manson",
     author_email="jpmanson@gmail.com",
     description="Easy integration with OIDC authentication servers",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/jpmanson/EasyOIDC",
     packages=setuptools.find_packages(),
```

