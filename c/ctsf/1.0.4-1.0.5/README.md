# Comparing `tmp/ctsf-1.0.4.tar.gz` & `tmp/ctsf-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctsf-1.0.4.tar", last modified: Tue May 14 03:28:03 2024, max compression
+gzip compressed data, was "ctsf-1.0.5.tar", last modified: Sat May 25 09:08:20 2024, max compression
```

## Comparing `ctsf-1.0.4.tar` & `ctsf-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-14 03:27:59.000000 ctsf-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 03:28:03.844659 ctsf-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-14 03:27:59.000000 ctsf-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.840659 ctsf-1.0.4/ctsf/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/ctsf/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/core/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/core/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/ctsf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/ctsf/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/modules/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-14 03:27:59.000000 ctsf-1.0.4/ctsf/modules/who.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 03:28:03.844659 ctsf-1.0.4/ctsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-14 03:28:03.000000 ctsf-1.0.4/ctsf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 03:28:03.844659 ctsf-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-14 03:27:59.000000 ctsf-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:08:20.146357 ctsf-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-25 09:08:09.000000 ctsf-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-25 09:08:20.142357 ctsf-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-25 09:08:09.000000 ctsf-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:08:20.142357 ctsf-1.0.5/ctsf/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:08:20.142357 ctsf-1.0.5/ctsf/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/core/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/core/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/ctsf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:08:20.142357 ctsf-1.0.5/ctsf/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/modules/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-25 09:08:09.000000 ctsf-1.0.5/ctsf/modules/who.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 09:08:20.142357 ctsf-1.0.5/ctsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-25 09:08:20.000000 ctsf-1.0.5/ctsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-25 09:08:20.000000 ctsf-1.0.5/ctsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 09:08:20.000000 ctsf-1.0.5/ctsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-25 09:08:20.000000 ctsf-1.0.5/ctsf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-25 09:08:20.000000 ctsf-1.0.5/ctsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-25 09:08:20.000000 ctsf-1.0.5/ctsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 09:08:20.146357 ctsf-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-25 09:08:09.000000 ctsf-1.0.5/setup.py
```

### Comparing `ctsf-1.0.4/LICENSE` & `ctsf-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctsf-1.0.4/PKG-INFO` & `ctsf-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ctsf
-Version: 1.0.4
+Version: 1.0.5
 Summary: Certificate Transparency Subdomain Finder + WHOIS Data
 Home-page: https://erfansamandarian.com/ctsf
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-whois
+Requires-Dist: tabulate
+Requires-Dist: termcolor
 
 # CTSF
 
 Certificate Transparency Subdomain Finder + WHOIS Data
 
 ```
 .------..------..------..------.
```

### Comparing `ctsf-1.0.4/README.md` & `ctsf-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ctsf-1.0.4/ctsf.egg-info/PKG-INFO` & `ctsf-1.0.5/ctsf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: ctsf
-Version: 1.0.4
+Version: 1.0.5
 Summary: Certificate Transparency Subdomain Finder + WHOIS Data
 Home-page: https://erfansamandarian.com/ctsf
 Author: Erfan Samandarian
 Author-email: mail@erfansamandarian.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: python-whois
+Requires-Dist: tabulate
+Requires-Dist: termcolor
 
 # CTSF
 
 Certificate Transparency Subdomain Finder + WHOIS Data
 
 ```
 .------..------..------..------.
```

### Comparing `ctsf-1.0.4/setup.py` & `ctsf-1.0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     description="Certificate Transparency Subdomain Finder + WHOIS Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Erfan Samandarian",
     author_email="mail@erfansamandarian.com",
     url="https://erfansamandarian.com/ctsf",
     license="MIT",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
-    install_requires=["requests", "python-whois"],
+    install_requires=["requests", "python-whois", "tabulate", "termcolor"],
     py_modules=["ctsf"],
     entry_points={"console_scripts": ["ctsf=ctsf:main"]},
 )
```

