# Comparing `tmp/etypes-1.0.2.tar.gz` & `tmp/etypes-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etypes-1.0.2.tar", max compression
+gzip compressed data, was "etypes-1.0.3.tar", max compression
```

## Comparing `etypes-1.0.2.tar` & `etypes-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      153 2024-05-25 03:33:59.081981 etypes-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1818 2024-05-25 05:49:02.305655 etypes-1.0.2/README.md
--rw-r--r--   0        0        0      716 2024-05-25 06:02:18.210817 etypes-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      125 2024-05-25 01:56:25.963492 etypes-1.0.2/src/etypes/__init__.py
--rw-r--r--   0        0        0     2178 2024-05-25 05:48:58.274614 etypes-1.0.2/src/etypes/ansible/loader.py
--rw-r--r--   0        0        0     2156 2024-05-25 05:48:42.666022 etypes-1.0.2/src/etypes/auto_loader.py
--rw-r--r--   0        0        0     2884 2024-05-24 09:57:18.056365 etypes-1.0.2/src/etypes/cli/etypes.py
--rw-r--r--   0        0        0      205 2024-05-25 01:57:49.421162 etypes-1.0.2/src/etypes/etypes.py
--rw-r--r--   0        0        0      704 2024-05-25 04:11:29.533857 etypes-1.0.2/src/etypes/exceptions.py
--rw-r--r--   0        0        0      969 2024-05-24 09:57:18.020400 etypes-1.0.2/src/etypes/helpers.py
--rw-r--r--   0        0        0     4068 2024-05-25 03:18:00.326560 etypes-1.0.2/src/etypes/processor.py
--rw-r--r--   0        0        0      534 2024-05-24 09:57:18.010912 etypes-1.0.2/src/etypes/utils.py
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 etypes-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      153 2024-05-25 03:33:59.081981 etypes-1.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1983 2024-05-25 06:09:36.433451 etypes-1.0.3/README.md
+-rw-r--r--   0        0        0      843 2024-05-25 06:20:52.136924 etypes-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      125 2024-05-25 01:56:25.963492 etypes-1.0.3/src/etypes/__init__.py
+-rw-r--r--   0        0        0     2178 2024-05-25 05:48:58.274614 etypes-1.0.3/src/etypes/ansible/loader.py
+-rw-r--r--   0        0        0     2156 2024-05-25 05:48:42.666022 etypes-1.0.3/src/etypes/auto_loader.py
+-rw-r--r--   0        0        0     2884 2024-05-24 09:57:18.056365 etypes-1.0.3/src/etypes/cli/etypes.py
+-rw-r--r--   0        0        0      205 2024-05-25 01:57:49.421162 etypes-1.0.3/src/etypes/etypes.py
+-rw-r--r--   0        0        0      704 2024-05-25 04:11:29.533857 etypes-1.0.3/src/etypes/exceptions.py
+-rw-r--r--   0        0        0      969 2024-05-24 09:57:18.020400 etypes-1.0.3/src/etypes/helpers.py
+-rw-r--r--   0        0        0     4068 2024-05-25 03:18:00.326560 etypes-1.0.3/src/etypes/processor.py
+-rw-r--r--   0        0        0      534 2024-05-24 09:57:18.010912 etypes-1.0.3/src/etypes/utils.py
+-rw-r--r--   0        0        0     2889 1970-01-01 00:00:00.000000 etypes-1.0.3/PKG-INFO
```

### Comparing `etypes-1.0.2/README.md` & `etypes-1.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,39 +23,47 @@
 
 `$ etypes encrypt -p PASSWORD ./path/to/python_file.py`
 
 or 
 
 `$ etypes encrypt -pf ./path/to/password_file ./path/to/python_file.py`
 
+results in 
+
 ```
 from etypes import EncryptedSecret
 SECRET_VAR: EncryptedSecret = "gAAAAABmT9yA6HQOXF4BM6gvUG_ryKqrXK9BEgRY2W4lNQvDNBVbiCEOz50-viDLEMXA71upgcGgRbqvC-IAltbjE8w5MbSooJN5EV-8sVe1q3LndfBNzEg="
 ```
 
 ### decrypt
 
+To decrypt the file run 
+
 `$ etypes decrypt -p PASSWORD ./path/to/python_file.py`
 
 or 
 
 `$ etypes v -pf ./path/to/password_file ./path/to/python_file.py`
 
-To import this python file in your project and have it decrypt itself seamlessly when accessed
+## Autoloader
+
+To import this python file in your project and have it decrypt itself seamlessly when accessed.
 
 You must import the AutoLoader
+and configure it to accept a password via a environment variable or to look for a file at a path.
+
 ```
 # app/settings/secrets.py
 
 from etypes import EncryptedSecret, AutoLoader
 SECRET_VAR: EncryptedSecret = "gAAAAABmT9yA6HQOXF4BM6gvUG_ryKqrXK9BEgRY2W4lNQvDNBVbiCEOz50-viDLEMXA71upgcGgRbqvC-IAltbjE8w5MbSooJN5EV-8sVe1q3LndfBNzEg="
 
-AutoLoader(password="SOME_ENV_VAR_WHICH_CONTAINS_PASSWORD", locals())
+AutoLoader(locals(), password_var_name="SOME_ENV_VAR_WHICH_CONTAINS_PASSWORD")
 # or
-AutoLoader(password_file="/path/to/your/secret_file", locals())
+AutoLoader(locals(), password_file="/path/to/your/secret_file")
 
 ```
 import your settings/secrets file normally.
 
 ```
 # app/main.py
 
@@ -63,8 +71,10 @@
 print(secrets.SECRET_VAR)
 ```
 
 Run your application providing the password declaring in your AutoLoader
 `$ SOME_ENV_VAR_WHICH_CONTAINS_PASSWORD="PASSWORD" ./main.py`
 
 
+
+
 > TODO: Add support for the environs package
```

### Comparing `etypes-1.0.2/pyproject.toml` & `etypes-1.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "etypes"
-version = "1.0.2"
+version = "1.0.3"
 description = "A python module to store, encrypt and decrypt type hinted strings in a python file"
 authors = ["Dan Brosnan <dpjbrosnan@gmail.com>"]
 packages = [{ include = "etypes", from = "src" }]
 readme = ["README.md", "CHANGELOG.md"]
+keywords = ["encrypt", "secret string", "secret", "decrypt", "env var"]
+repository = "https://github.com/falsaform/etypes.git"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.0"
 ansible = {version = "^9", optional = true}
```

### Comparing `etypes-1.0.2/src/etypes/ansible/loader.py` & `etypes-1.0.3/src/etypes/ansible/loader.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.2/src/etypes/auto_loader.py` & `etypes-1.0.3/src/etypes/auto_loader.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.2/src/etypes/cli/etypes.py` & `etypes-1.0.3/src/etypes/cli/etypes.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.2/src/etypes/exceptions.py` & `etypes-1.0.3/src/etypes/exceptions.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.2/src/etypes/helpers.py` & `etypes-1.0.3/src/etypes/helpers.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.2/src/etypes/processor.py` & `etypes-1.0.3/src/etypes/processor.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.2/src/etypes/utils.py` & `etypes-1.0.3/src/etypes/utils.py`

 * *Files identical despite different names*

### Comparing `etypes-1.0.2/PKG-INFO` & `etypes-1.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: etypes
-Version: 1.0.2
+Version: 1.0.3
 Summary: A python module to store, encrypt and decrypt type hinted strings in a python file
+Home-page: https://github.com/falsaform/etypes.git
+Keywords: encrypt,secret string,secret,decrypt,env var
 Author: Dan Brosnan
 Author-email: dpjbrosnan@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: ansible
 Requires-Dist: ansible (>=9,<10) ; extra == "ansible"
 Requires-Dist: click (>=8.0,<9.0)
+Project-URL: Repository, https://github.com/falsaform/etypes.git
 Description-Content-Type: text/markdown
 
 ## ETYPES
 
 This package allows for encrypting secret strings in python files in a human readable way using type hints. 
 it also supports dynamic loading of python files which contain encrypted strings, providing the password via an environment variable
  
@@ -39,39 +42,47 @@
 
 `$ etypes encrypt -p PASSWORD ./path/to/python_file.py`
 
 or 
 
 `$ etypes encrypt -pf ./path/to/password_file ./path/to/python_file.py`
 
+results in 
+
 ```
 from etypes import EncryptedSecret
 SECRET_VAR: EncryptedSecret = "gAAAAABmT9yA6HQOXF4BM6gvUG_ryKqrXK9BEgRY2W4lNQvDNBVbiCEOz50-viDLEMXA71upgcGgRbqvC-IAltbjE8w5MbSooJN5EV-8sVe1q3LndfBNzEg="
 ```
 
 ### decrypt
 
+To decrypt the file run 
+
 `$ etypes decrypt -p PASSWORD ./path/to/python_file.py`
 
 or 
 
 `$ etypes v -pf ./path/to/password_file ./path/to/python_file.py`
 
-To import this python file in your project and have it decrypt itself seamlessly when accessed
+## Autoloader
+
+To import this python file in your project and have it decrypt itself seamlessly when accessed.
 
 You must import the AutoLoader
+and configure it to accept a password via a environment variable or to look for a file at a path.
+
 ```
 # app/settings/secrets.py
 
 from etypes import EncryptedSecret, AutoLoader
 SECRET_VAR: EncryptedSecret = "gAAAAABmT9yA6HQOXF4BM6gvUG_ryKqrXK9BEgRY2W4lNQvDNBVbiCEOz50-viDLEMXA71upgcGgRbqvC-IAltbjE8w5MbSooJN5EV-8sVe1q3LndfBNzEg="
 
-AutoLoader(password="SOME_ENV_VAR_WHICH_CONTAINS_PASSWORD", locals())
+AutoLoader(locals(), password_var_name="SOME_ENV_VAR_WHICH_CONTAINS_PASSWORD")
 # or
-AutoLoader(password_file="/path/to/your/secret_file", locals())
+AutoLoader(locals(), password_file="/path/to/your/secret_file")
 
 ```
 import your settings/secrets file normally.
 
 ```
 # app/main.py
 
@@ -79,14 +90,16 @@
 print(secrets.SECRET_VAR)
 ```
 
 Run your application providing the password declaring in your AutoLoader
 `$ SOME_ENV_VAR_WHICH_CONTAINS_PASSWORD="PASSWORD" ./main.py`
 
 
+
+
 > TODO: Add support for the environs package 
 
 ## Changelog
 
 1.0.1 breaking changes but still initial 1.0 release
 - rename hits EncryptedSecret and DecryptedSecret
```

