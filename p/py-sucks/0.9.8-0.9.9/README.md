# Comparing `tmp/py-sucks-0.9.8.tar.gz` & `tmp/py-sucks-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-sucks-0.9.8.tar", last modified: Sun Sep  4 10:44:19 2022, max compression
+gzip compressed data, was "py-sucks-0.9.9.tar", last modified: Mon Feb 12 18:56:35 2024, max compression
```

## Comparing `py-sucks-0.9.8.tar` & `py-sucks-0.9.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 10:44:19.335176 py-sucks-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-09-04 10:44:16.000000 py-sucks-0.9.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5769 2022-09-04 10:44:19.335176 py-sucks-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5027 2022-09-04 10:44:16.000000 py-sucks-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 10:44:19.335176 py-sucks-0.9.8/py_sucks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5769 2022-09-04 10:44:19.000000 py-sucks-0.9.8/py_sucks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-04 10:44:19.000000 py-sucks-0.9.8/py_sucks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 10:44:19.000000 py-sucks-0.9.8/py_sucks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-04 10:44:19.000000 py-sucks-0.9.8/py_sucks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-04 10:44:19.000000 py-sucks-0.9.8/py_sucks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-04 10:44:19.000000 py-sucks-0.9.8/py_sucks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-04 10:44:19.335176 py-sucks-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2869 2022-09-04 10:44:16.000000 py-sucks-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 10:44:19.335176 py-sucks-0.9.8/sucks/
--rw-r--r--   0 runner    (1001) docker     (121)    21673 2022-09-04 10:44:16.000000 py-sucks-0.9.8/sucks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6909 2022-09-04 10:44:16.000000 py-sucks-0.9.8/sucks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:56:35.498062 py-sucks-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-02-12 18:56:31.000000 py-sucks-0.9.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-02-12 18:56:35.498062 py-sucks-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-02-12 18:56:31.000000 py-sucks-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:56:35.498062 py-sucks-0.9.9/py_sucks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-02-12 18:56:35.000000 py-sucks-0.9.9/py_sucks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-12 18:56:35.000000 py-sucks-0.9.9/py_sucks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 18:56:35.000000 py-sucks-0.9.9/py_sucks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-12 18:56:35.000000 py-sucks-0.9.9/py_sucks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-12 18:56:35.000000 py-sucks-0.9.9/py_sucks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-12 18:56:35.000000 py-sucks-0.9.9/py_sucks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 18:56:35.498062 py-sucks-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-02-12 18:56:31.000000 py-sucks-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 18:56:35.498062 py-sucks-0.9.9/sucks/
+-rw-r--r--   0 runner    (1001) docker     (127)    22041 2024-02-12 18:56:31.000000 py-sucks-0.9.9/sucks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-02-12 18:56:31.000000 py-sucks-0.9.9/sucks/cli.py
```

### Comparing `py-sucks-0.9.8/LICENSE.txt` & `py-sucks-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-sucks-0.9.8/PKG-INFO` & `py-sucks-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: py-sucks
-Version: 0.9.8
+Version: 0.9.9
 Summary: a library for controlling certain robot vacuums
 Home-page: https://github.com/mib1185/py-sucks
 Author: William Pietri
 Author-email: sucks-users@googlegroups.com
 License: GPL-3.0
 Keywords: home automation vacuum robot
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 [![Tests](https://github.com/mib1185/py-sucks/actions/workflows/tests.yaml/badge.svg)](https://github.com/mib1185/py-sucks/actions/workflows/tests.yaml)
 [![PyPI version](https://badge.fury.io/py/py-sucks.svg)](https://pypi.org/project/py-sucks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-sucks)](https://pypi.org/project/py-sucks)
```

### Comparing `py-sucks-0.9.8/README.md` & `py-sucks-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `py-sucks-0.9.8/py_sucks.egg-info/PKG-INFO` & `py-sucks-0.9.9/py_sucks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: py-sucks
-Version: 0.9.8
+Version: 0.9.9
 Summary: a library for controlling certain robot vacuums
 Home-page: https://github.com/mib1185/py-sucks
 Author: William Pietri
 Author-email: sucks-users@googlegroups.com
 License: GPL-3.0
 Keywords: home automation vacuum robot
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 [![Tests](https://github.com/mib1185/py-sucks/actions/workflows/tests.yaml/badge.svg)](https://github.com/mib1185/py-sucks/actions/workflows/tests.yaml)
 [![PyPI version](https://badge.fury.io/py/py-sucks.svg)](https://pypi.org/project/py-sucks)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-sucks)](https://pypi.org/project/py-sucks)
```

### Comparing `py-sucks-0.9.8/setup.py` & `py-sucks-0.9.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
 except FileNotFoundError:
     print("can't find python README; skipping")
 
 setup(
     name='py-sucks',
-    version='0.9.8',
+    version='0.9.9',
 
     description='a library for controlling certain robot vacuums',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     url='https://github.com/mib1185/py-sucks',
 
@@ -35,14 +35,16 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'Topic :: Home Automation',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 
     # What does your project relate to?
     keywords='home automation vacuum robot',
 
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
```

### Comparing `py-sucks-0.9.8/sucks/__init__.py` & `py-sucks-0.9.9/sucks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,23 @@
 
 COMPONENT_FROM_ECOVACS = {
     'brush': COMPONENT_MAIN_BRUSH,
     'side_brush': COMPONENT_SIDE_BRUSH,
     'dust_case_heap': COMPONENT_FILTER
 }
 
+ERROR_CODES = {
+    "100": "Robot is operational",
+    "101": "Low battery",
+    "102": "Robot is stuck",
+    "103": "Wheels are not moving as expected",
+    "104": "Down sensor is getting abnormal values",
+    "110": "Dust Bin Not installed",
+}
+
 class EcoVacsAPI:
     CLIENT_KEY = "eJUWrzRv34qFSaYk"
     SECRET = "Cyu5jcR4zyK6QEPn1hdIGXB5QIDAQABMA0GC"
     PUBLIC_KEY = 'MIIB/TCCAWYCCQDJ7TMYJFzqYDANBgkqhkiG9w0BAQUFADBCMQswCQYDVQQGEwJjbjEVMBMGA1UEBwwMRGVmYXVsdCBDaXR5MRwwGgYDVQQKDBNEZWZhdWx0IENvbXBhbnkgTHRkMCAXDTE3MDUwOTA1MTkxMFoYDzIxMTcwNDE1MDUxOTEwWjBCMQswCQYDVQQGEwJjbjEVMBMGA1UEBwwMRGVmYXVsdCBDaXR5MRwwGgYDVQQKDBNEZWZhdWx0IENvbXBhbnkgTHRkMIGfMA0GCSqGSIb3DQEBAQUAA4GNADCBiQKBgQDb8V0OYUGP3Fs63E1gJzJh+7iqeymjFUKJUqSD60nhWReZ+Fg3tZvKKqgNcgl7EGXp1yNifJKUNC/SedFG1IJRh5hBeDMGq0m0RQYDpf9l0umqYURpJ5fmfvH/gjfHe3Eg/NTLm7QEa0a0Il2t3Cyu5jcR4zyK6QEPn1hdIGXB5QIDAQABMA0GCSqGSIb3DQEBBQUAA4GBANhIMT0+IyJa9SU8AEyaWZZmT2KEYrjakuadOvlkn3vFdhpvNpnnXiL+cyWy2oU1Q9MAdCTiOPfXmAQt8zIvP2JC8j6yRTcxJCvBwORDyv/uBtXFxBPEC6MDfzU2gKAaHeeJUWrzRv34qFSaYkYta8canK+PSInylQTjJK9VqmjQ'
     MAIN_URL_FORMAT = 'https://eco-{country}-api.ecovacs.com/v1/private/{country}/{lang}/{deviceId}/{appCode}/{appVersion}/{channel}/{deviceType}'
     USER_URL_FORMAT = 'https://users-{continent}.ecouser.net:8000/user.do'
     REALM = 'ecouser.net'
@@ -285,15 +294,17 @@
 
     def _handle_ctl(self, ctl):
         method = '_handle_' + ctl['event']
         if hasattr(self, method):
             getattr(self, method)(ctl)
 
     def _handle_error(self, event):
-        error = event['error']
+        errno = event.get('errno')
+        if not errno or (error := ERROR_CODES.get(errno)) is None:
+            error = event.get('error', 'unknown')
         self.errorEvents.notify(error)
         _LOGGER.debug("*** error = " + error)
 
     def _handle_life_span(self, event):
         type = event['type']
         try:
             type = COMPONENT_FROM_ECOVACS[type]
```

### Comparing `py-sucks-0.9.8/sucks/cli.py` & `py-sucks-0.9.9/sucks/cli.py`

 * *Files identical despite different names*

