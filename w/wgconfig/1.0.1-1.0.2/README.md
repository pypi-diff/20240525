# Comparing `tmp/wgconfig-1.0.1.tar.gz` & `tmp/wgconfig-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgconfig-1.0.1.tar", last modified: Tue Jan 30 20:19:52 2024, max compression
+gzip compressed data, was "wgconfig-1.0.2.tar", last modified: Sat May 25 19:37:23 2024, max compression
```

## Comparing `wgconfig-1.0.1.tar` & `wgconfig-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 20:19:52.265150 wgconfig-1.0.1/
--rwxrw-r--   0 root         (0) root         (0)    34523 2020-07-09 19:46:10.000000 wgconfig-1.0.1/LICENSE.txt
--rwxrw-r--   0 root         (0) root         (0)       21 2020-07-12 10:54:35.000000 wgconfig-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12055 2024-01-30 20:19:52.265150 wgconfig-1.0.1/PKG-INFO
--rwxrw-r--   0 root         (0) root         (0)    11129 2024-01-28 11:45:53.000000 wgconfig-1.0.1/README.md
--rwxrw-r--   0 root         (0) root         (0)       78 2024-01-30 20:19:52.265150 wgconfig-1.0.1/setup.cfg
--rwxrw-r--   0 root         (0) root         (0)     1308 2024-01-28 13:03:24.000000 wgconfig-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 20:19:52.245150 wgconfig-1.0.1/wgconfig/
--rwxrw-r--   0 root         (0) root         (0)    15707 2023-07-27 11:46:04.000000 wgconfig-1.0.1/wgconfig/__init__.py
--rwxr--r--   0 root         (0) root         (0)     2611 2024-01-28 09:27:55.000000 wgconfig-1.0.1/wgconfig/wgexec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 20:19:52.261150 wgconfig-1.0.1/wgconfig.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12055 2024-01-30 20:19:52.000000 wgconfig-1.0.1/wgconfig.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      251 2024-01-30 20:19:52.000000 wgconfig-1.0.1/wgconfig.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 20:19:52.000000 wgconfig-1.0.1/wgconfig.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-01-30 20:19:52.000000 wgconfig-1.0.1/wgconfig.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-30 20:19:52.000000 wgconfig-1.0.1/wgconfig.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 19:37:23.155843 wgconfig-1.0.2/
+-rwxrw-r--   0 root         (0) root         (0)    34523 2020-07-09 19:46:10.000000 wgconfig-1.0.2/LICENSE
+-rwxrw-r--   0 root         (0) root         (0)       17 2024-05-23 19:36:11.000000 wgconfig-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12188 2024-05-25 19:37:23.151843 wgconfig-1.0.2/PKG-INFO
+-rwxrw-r--   0 root         (0) root         (0)    11266 2024-05-25 19:36:29.000000 wgconfig-1.0.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)       74 2024-05-25 19:37:23.159843 wgconfig-1.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1355 2024-05-24 14:12:58.000000 wgconfig-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 19:37:23.091844 wgconfig-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 19:37:23.119844 wgconfig-1.0.2/src/wgconfig/
+-rwxrw-r--   0 root         (0) root         (0)    15707 2023-07-27 11:46:04.000000 wgconfig-1.0.2/src/wgconfig/__init__.py
+-rwxr--r--   0 root         (0) root         (0)     2611 2024-01-28 09:27:55.000000 wgconfig-1.0.2/src/wgconfig/wgexec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 19:37:23.139844 wgconfig-1.0.2/src/wgconfig.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12188 2024-05-25 19:37:22.000000 wgconfig-1.0.2/src/wgconfig.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      290 2024-05-25 19:37:23.000000 wgconfig-1.0.2/src/wgconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-25 19:37:22.000000 wgconfig-1.0.2/src/wgconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-25 19:37:22.000000 wgconfig-1.0.2/src/wgconfig.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-25 19:37:22.000000 wgconfig-1.0.2/src/wgconfig.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-25 19:37:23.143844 wgconfig-1.0.2/test/
+-rwxrw-r--   0 root         (0) root         (0)    79296 2022-11-19 14:18:04.000000 wgconfig-1.0.2/test/test_1.py
```

### Comparing `wgconfig-1.0.1/LICENSE.txt` & `wgconfig-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wgconfig-1.0.1/PKG-INFO` & `wgconfig-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: parsing and writing WireGuard configuration files
 Home-page: https://www.github.com/towalink/wgconfig
 Author: Dirk Henrici
 Author-email: towalink.wgconfig@henrici.name
 Project-URL: Repository, https://www.github.com/towalink/wgconfig
 Project-URL: PyPi, https://pypi.org/project/wgconfig/
 Keywords: WireGuard configuration config wg
@@ -13,15 +13,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 Requires-Dist: future; python_version == "2.7"
 
 # wgconfig
 
 Parsing and writing WireGuard configuration files (comment preserving)
 
 WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most libraries handling configuration files. Most existing libraries are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
@@ -45,14 +45,20 @@
 
 Install using PyPi:
 
 ```shell
 pip3 install wgconfig
 ```
 
+Or download the provided Debian package (in the desired version) and install it:
+
+```shell
+dpkg -i python3-wgconfig_1.0.2-1_all.deb
+```
+
 ---
 
 ## Quickstart
 
 ### Reading and parsing an existing WireGuard configuration file
 
 Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
@@ -330,9 +336,9 @@
 ---
 
 ## License
 
 [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
 
 - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-- Copyright 2020-2023 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
+- Copyright 2020-2024 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
 - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

### Comparing `wgconfig-1.0.1/README.md` & `wgconfig-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
 Install using PyPi:
 
 ```shell
 pip3 install wgconfig
 ```
 
+Or download the provided Debian package (in the desired version) and install it:
+
+```shell
+dpkg -i python3-wgconfig_1.0.2-1_all.deb
+```
+
 ---
 
 ## Quickstart
 
 ### Reading and parsing an existing WireGuard configuration file
 
 Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
@@ -308,9 +314,9 @@
 ---
 
 ## License
 
 [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
 
 - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-- Copyright 2020-2023 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
+- Copyright 2020-2024 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
 - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

### Comparing `wgconfig-1.0.1/setup.py` & `wgconfig-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'wgconfig',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'author': 'Dirk Henrici',
     'author_email': 'towalink.wgconfig@henrici.name',
     'description': 'parsing and writing WireGuard configuration files',
     'long_description': long_description,
     'long_description_content_type': 'text/markdown',
     'url': 'https://www.github.com/towalink/wgconfig',
-    'packages': setuptools.find_packages(),
+    'packages': setuptools.find_namespace_packages('src'),
+    'package_dir': {'': 'src'},
     'classifiers': [
         'Programming Language :: Python',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: POSIX :: Linux',
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: System Administrators',
         'Intended Audience :: Developers',
```

### Comparing `wgconfig-1.0.1/wgconfig/__init__.py` & `wgconfig-1.0.2/src/wgconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `wgconfig-1.0.1/wgconfig/wgexec.py` & `wgconfig-1.0.2/src/wgconfig/wgexec.py`

 * *Files identical despite different names*

### Comparing `wgconfig-1.0.1/wgconfig.egg-info/PKG-INFO` & `wgconfig-1.0.2/src/wgconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wgconfig
-Version: 1.0.1
+Version: 1.0.2
 Summary: parsing and writing WireGuard configuration files
 Home-page: https://www.github.com/towalink/wgconfig
 Author: Dirk Henrici
 Author-email: towalink.wgconfig@henrici.name
 Project-URL: Repository, https://www.github.com/towalink/wgconfig
 Project-URL: PyPi, https://pypi.org/project/wgconfig/
 Keywords: WireGuard configuration config wg
@@ -13,15 +13,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+License-File: LICENSE
 Requires-Dist: future; python_version == "2.7"
 
 # wgconfig
 
 Parsing and writing WireGuard configuration files (comment preserving)
 
 WireGuard config files are ini-style. Since all "Peer" sections have the same name, these files cannot be parsed and modified by most libraries handling configuration files. Most existing libraries are not able to preserve or even add comments when modifying a config file. "wgconfig" was created to work with WireGuard configuration files and to preserve comments.
@@ -45,14 +45,20 @@
 
 Install using PyPi:
 
 ```shell
 pip3 install wgconfig
 ```
 
+Or download the provided Debian package (in the desired version) and install it:
+
+```shell
+dpkg -i python3-wgconfig_1.0.2-1_all.deb
+```
+
 ---
 
 ## Quickstart
 
 ### Reading and parsing an existing WireGuard configuration file
 
 Read and parse the existing WireGuard configuration file 'wg0.conf' located in '/etc/wireguard':
@@ -330,9 +336,9 @@
 ---
 
 ## License
 
 [![License](http://img.shields.io/:license-agpl3-blue.svg?style=flat-square)](https://opensource.org/licenses/AGPL-3.0)
 
 - **[AGPL3 license](https://opensource.org/licenses/AGPL-3.0)**
-- Copyright 2020-2023 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
+- Copyright 2020-2024 © <a href="https://github.com/towalink/wgconfig" target="_blank">Dirk Henrici</a>.
 - [WireGuard](https://www.wireguard.com/) is a registered trademark of Jason A. Donenfeld.
```

