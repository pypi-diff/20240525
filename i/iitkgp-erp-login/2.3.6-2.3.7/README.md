# Comparing `tmp/iitkgp_erp_login-2.3.6.tar.gz` & `tmp/iitkgp_erp_login-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iitkgp_erp_login-2.3.6.tar", last modified: Fri Mar  1 05:26:07 2024, max compression
+gzip compressed data, was "iitkgp_erp_login-2.3.7.tar", last modified: Sat May 25 07:15:00 2024, max compression
```

## Comparing `iitkgp_erp_login-2.3.6.tar` & `iitkgp_erp_login-2.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:26:07.130057 iitkgp_erp_login-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-01 05:25:31.000000 iitkgp_erp_login-2.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-03-01 05:26:07.130057 iitkgp_erp_login-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-03-01 05:25:31.000000 iitkgp_erp_login-2.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-01 05:25:56.000000 iitkgp_erp_login-2.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 05:26:07.130057 iitkgp_erp_login-2.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:26:07.130057 iitkgp_erp_login-2.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:26:07.130057 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 05:25:31.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-01 05:25:31.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-03-01 05:25:31.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/erp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-01 05:25:31.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/read_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-03-01 05:25:31.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 05:26:07.130057 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-03-01 05:26:07.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-01 05:26:07.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 05:26:07.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-01 05:26:07.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-01 05:26:07.000000 iitkgp_erp_login-2.3.6/src/iitkgp_erp_login.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:15:00.105560 iitkgp_erp_login-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-25 07:14:32.000000 iitkgp_erp_login-2.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-05-25 07:15:00.105560 iitkgp_erp_login-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-05-25 07:14:32.000000 iitkgp_erp_login-2.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-25 07:14:50.000000 iitkgp_erp_login-2.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:15:00.105560 iitkgp_erp_login-2.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:15:00.105560 iitkgp_erp_login-2.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:15:00.105560 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 07:14:32.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-25 07:14:32.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-25 07:14:32.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/erp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-25 07:14:32.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/read_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-25 07:14:32.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:15:00.105560 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19187 2024-05-25 07:15:00.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-25 07:15:00.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:15:00.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-25 07:15:00.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 07:15:00.000000 iitkgp_erp_login-2.3.7/src/iitkgp_erp_login.egg-info/top_level.txt
```

### Comparing `iitkgp_erp_login-2.3.6/PKG-INFO` & `iitkgp_erp_login-2.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp_erp_login
-Version: 2.3.6
+Version: 2.3.7
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.3.6 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.3.7 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: bs4 Requires-Dist: ping3 Requires-Dist: requests
```

### Comparing `iitkgp_erp_login-2.3.6/README.md` & `iitkgp_erp_login-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.3.6/pyproject.toml` & `iitkgp_erp_login-2.3.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "iitkgp_erp_login"
-version = "2.3.6"
+version = "2.3.7"
 authors = [
   { name="Arpit Bhardwaj", email="proffapt@pm.me" },
 ]
 description = "A package to automate login process in ERP for IIT-KGP"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/erp.py` & `iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/erp.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,14 +195,15 @@
             from iitkgp_erp_login.read_mail import getOTP
             otp = getOTP(OTP_CHECK_INTERVAL, headers=headers, session=session, login_details=login_details, log=LOGGING)
             if LOGGING: logging.info(" Received OTP")
 
         except Exception as e:
             raise ErpLoginError(f"Failed to receive OTP: {str(e)}")
     else:
+        request_otp(headers=headers, session=session, login_details=login_details, log=LOGGING)
         otp = input("Enter the OTP sent to your registered email address: ").strip()
 
     login_details["email_otp"] = otp
 
     ssoToken = signin(headers=headers, session=session, login_details=login_details, log=LOGGING)
 
     if SESSION_STORAGE_FILE: write_tokens_to_file(token_file=token_file, ssoToken=ssoToken, sessionToken=sessionToken, log=LOGGING)
```

### Comparing `iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/read_mail.py` & `iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/read_mail.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.3.6/src/iitkgp_erp_login/utils.py` & `iitkgp_erp_login-2.3.7/src/iitkgp_erp_login/utils.py`

 * *Files identical despite different names*

### Comparing `iitkgp_erp_login-2.3.6/src/iitkgp_erp_login.egg-info/PKG-INFO` & `iitkgp_erp_login-2.3.7/src/iitkgp_erp_login.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iitkgp_erp_login
-Version: 2.3.6
+Version: 2.3.7
 Summary: A package to automate login process in ERP for IIT-KGP
 Author-email: Arpit Bhardwaj <proffapt@pm.me>
 Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.3.6 Summary: A package
+Metadata-Version: 2.1 Name: iitkgp_erp_login Version: 2.3.7 Summary: A package
 to automate login process in ERP for IIT-KGP Author-email: Arpit Bhardwaj
 pm.me> Project-URL: Homepage, https://github.com/proffapt/iitkgp-erp-login-pypi
 Project-URL: Bug Tracker, https://github.com/proffapt/iitkgp-erp-login-pypi/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: bs4 Requires-Dist: ping3 Requires-Dist: requests
```

