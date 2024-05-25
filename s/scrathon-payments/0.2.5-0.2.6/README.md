# Comparing `tmp/scrathon_payments-0.2.5.tar.gz` & `tmp/scrathon_payments-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrathon_payments-0.2.5.tar", last modified: Fri May 24 16:23:50 2024, max compression
+gzip compressed data, was "scrathon_payments-0.2.6.tar", last modified: Sat May 25 07:53:57 2024, max compression
```

## Comparing `scrathon_payments-0.2.5.tar` & `scrathon_payments-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:23:50.736808 scrathon_payments-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-24 16:23:47.000000 scrathon_payments-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 16:23:50.736808 scrathon_payments-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-24 16:23:47.000000 scrathon_payments-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:23:50.732807 scrathon_payments-0.2.5/ScrathonPayments/
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-24 16:23:47.000000 scrathon_payments-0.2.5/ScrathonPayments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 16:23:50.736808 scrathon_payments-0.2.5/scrathon_payments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-24 16:23:50.000000 scrathon_payments-0.2.5/scrathon_payments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 16:23:50.000000 scrathon_payments-0.2.5/scrathon_payments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 16:23:50.000000 scrathon_payments-0.2.5/scrathon_payments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 16:23:50.000000 scrathon_payments-0.2.5/scrathon_payments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 16:23:50.000000 scrathon_payments-0.2.5/scrathon_payments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 16:23:50.736808 scrathon_payments-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-24 16:23:47.000000 scrathon_payments-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:53:57.027634 scrathon_payments-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-25 07:53:53.000000 scrathon_payments-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-25 07:53:57.027634 scrathon_payments-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-25 07:53:53.000000 scrathon_payments-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:53:57.027634 scrathon_payments-0.2.6/ScrathonPayments/
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-05-25 07:53:53.000000 scrathon_payments-0.2.6/ScrathonPayments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 07:53:57.027634 scrathon_payments-0.2.6/scrathon_payments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-25 07:53:57.000000 scrathon_payments-0.2.6/scrathon_payments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-25 07:53:57.000000 scrathon_payments-0.2.6/scrathon_payments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 07:53:57.000000 scrathon_payments-0.2.6/scrathon_payments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-25 07:53:57.000000 scrathon_payments-0.2.6/scrathon_payments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-25 07:53:57.000000 scrathon_payments-0.2.6/scrathon_payments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 07:53:57.027634 scrathon_payments-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-25 07:53:53.000000 scrathon_payments-0.2.6/setup.py
```

### Comparing `scrathon_payments-0.2.5/LICENSE` & `scrathon_payments-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.5/PKG-INFO` & `scrathon_payments-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.2.5
+Version: 0.2.6
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.2.5/README.md` & `scrathon_payments-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.2.5/ScrathonPayments/__init__.py` & `scrathon_payments-0.2.6/ScrathonPayments/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,15 +33,23 @@
             })
             try:
                 success = str(request.json().get("success")) == "True"
             except Exception as e:
                 print(f"Didn't recognise json: {request.text}")
                 raise e from None
             return convert[success]
-            
+        @client.request
+        def userexist():
+            request = requests.post("http://45.140.188.129:6623/userexist/", json={"username": username})
+            try:
+                success = str(request.json().get("userexist")) == "True"
+            except Exception as e:
+                print(f"Didn't recognise json: {request.text}")
+                raise e from None
+            return convert[success]
         @client.request
         def purchasecheck(price):
             request = requests.post("http://45.140.188.129:6623/checkpurchase", json={
                 "price": price,
                 "buyer": client.get_requester(),
                 "seller": self.username
             })
```

### Comparing `scrathon_payments-0.2.5/scrathon_payments.egg-info/PKG-INFO` & `scrathon_payments-0.2.6/scrathon_payments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.2.5
+Version: 0.2.6
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.2.5/setup.py` & `scrathon_payments-0.2.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scrathon-payments',
-    version='0.2.5',
+    version='0.2.6',
     author='Ryan_shamu',
     author_email='Ryanshamu418@gmail.com',
     description='API Wrapper for ScrathonPayments',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Ryan-shamu-YT/ScrathonPayments',
     packages=find_packages(exclude=[]),
```

