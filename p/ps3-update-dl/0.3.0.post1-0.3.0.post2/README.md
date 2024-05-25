# Comparing `tmp/ps3-update-dl-0.3.0.post1.tar.gz` & `tmp/ps3_update_dl-0.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ps3-update-dl-0.3.0.post1.tar", last modified: Thu May 27 13:56:34 2021, max compression
+gzip compressed data, was "ps3_update_dl-0.3.0.post2.tar", last modified: Sat May 25 05:50:25 2024, max compression
```

## Comparing `ps3-update-dl-0.3.0.post1.tar` & `ps3_update_dl-0.3.0.post2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-x---   0 user      (1000) user      (1000)        0 2021-05-27 13:56:34.404326 ps3-update-dl-0.3.0.post1/
--rw-------   0 user      (1000) user      (1000)    34160 2020-09-16 09:21:49.000000 ps3-update-dl-0.3.0.post1/LICENSE.md
--rw-r-----   0 user      (1000) user      (1000)     2968 2021-05-27 13:56:34.404326 ps3-update-dl-0.3.0.post1/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     1806 2021-05-27 13:54:59.000000 ps3-update-dl-0.3.0.post1/README.md
-drwxr-x---   0 user      (1000) user      (1000)        0 2021-05-27 13:56:34.404326 ps3-update-dl-0.3.0.post1/ps3_update_dl/
--rw-r-----   0 user      (1000) user      (1000)     6867 2021-05-27 13:56:14.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl/__init__.py
--rw-r-----   0 user      (1000) user      (1000)     2908 2021-05-18 02:23:46.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl/playstation-ca.crt
-drwxr-x---   0 user      (1000) user      (1000)        0 2021-05-27 13:56:34.404326 ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     2968 2021-05-27 13:56:34.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      327 2021-05-27 13:56:34.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2021-05-27 13:56:34.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       47 2021-05-27 13:56:34.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)       65 2021-05-27 13:56:34.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       14 2021-05-27 13:56:34.000000 ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)      101 2020-09-16 10:17:38.000000 ps3-update-dl-0.3.0.post1/pyproject.toml
--rw-r-----   0 user      (1000) user      (1000)       38 2021-05-27 13:56:34.404326 ps3-update-dl-0.3.0.post1/setup.cfg
--rwxr-x---   0 user      (1000) user      (1000)     1764 2021-05-27 13:55:19.000000 ps3-update-dl-0.3.0.post1/setup.py
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 05:50:25.310649 ps3_update_dl-0.3.0.post2/
+-rw-r-----   0 user      (1000) user      (1000)    34160 2024-05-25 05:45:22.000000 ps3_update_dl-0.3.0.post2/LICENSE.md
+-rw-r--r--   0 user      (1000) user      (1000)     3058 2024-05-25 05:50:25.310649 ps3_update_dl-0.3.0.post2/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)     1806 2024-05-25 05:45:22.000000 ps3_update_dl-0.3.0.post2/README.md
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 05:50:25.310649 ps3_update_dl-0.3.0.post2/ps3_update_dl/
+-rw-r-----   0 user      (1000) user      (1000)     6867 2024-05-25 05:49:16.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl/__init__.py
+-rw-r-----   0 user      (1000) user      (1000)     2908 2024-05-25 05:45:22.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl/playstation-ca.crt
+drwxr-x---   0 user      (1000) user      (1000)        0 2024-05-25 05:50:25.310649 ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     3058 2024-05-25 05:50:25.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/PKG-INFO
+-rw-r-----   0 user      (1000) user      (1000)      327 2024-05-25 05:50:25.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/SOURCES.txt
+-rw-r-----   0 user      (1000) user      (1000)        1 2024-05-25 05:50:25.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/dependency_links.txt
+-rw-r-----   0 user      (1000) user      (1000)       46 2024-05-25 05:50:25.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/entry_points.txt
+-rw-r-----   0 user      (1000) user      (1000)       65 2024-05-25 05:50:25.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/requires.txt
+-rw-r-----   0 user      (1000) user      (1000)       14 2024-05-25 05:50:25.000000 ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/top_level.txt
+-rw-r-----   0 user      (1000) user      (1000)      101 2024-05-25 05:45:22.000000 ps3_update_dl-0.3.0.post2/pyproject.toml
+-rw-r-----   0 user      (1000) user      (1000)       38 2024-05-25 05:50:25.310649 ps3_update_dl-0.3.0.post2/setup.cfg
+-rwxr-x---   0 user      (1000) user      (1000)     1782 2024-05-25 05:46:29.000000 ps3_update_dl-0.3.0.post2/setup.py
```

### Comparing `ps3-update-dl-0.3.0.post1/LICENSE.md` & `ps3_update_dl-0.3.0.post2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ps3-update-dl-0.3.0.post1/PKG-INFO` & `ps3_update_dl-0.3.0.post2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ps3-update-dl
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: Download all updates for a given PS3 game
 Home-page: https://github.com/iomintz/ps3-update-dl
 Author: io mintz
 Author-email: io@mintz.cc
 License: AGPLv3+
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: Utilities
@@ -22,14 +21,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown; variant=GFM
 License-File: LICENSE.md
+Requires-Dist: requests<3.0.0,>=2.23.0
+Requires-Dist: tqdm<5.0.0,>=4.49.0
+Requires-Dist: PyYAML<6.0.0,>=5.4.1
 
 # ps3-update-dl
 
 [![Build Status](https://img.shields.io/travis/com/ioistired/ps3-update-dl/trunk.svg?label=tests)](https://travis-ci.com/ioistired/ps3-update-dl)
 
 Downloads all updates for a given title directly from the PlayStation servers.
 
@@ -79,9 +81,7 @@
 ps3-update-dl is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with ps3-update-dl. If not, see <https://www.gnu.org/licenses/>.
-
-
```

### Comparing `ps3-update-dl-0.3.0.post1/README.md` & `ps3_update_dl-0.3.0.post2/README.md`

 * *Files identical despite different names*

### Comparing `ps3-update-dl-0.3.0.post1/ps3_update_dl/__init__.py` & `ps3_update_dl-0.3.0.post2/ps3_update_dl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-__version__ = '0.3.0.post1'
+__version__ = '0.3.0.post2'
 
 import io
 import sys
 import yaml
 import typing
 import hashlib
 import pkg_resources
```

### Comparing `ps3-update-dl-0.3.0.post1/ps3_update_dl/playstation-ca.crt` & `ps3_update_dl-0.3.0.post2/ps3_update_dl/playstation-ca.crt`

 * *Files identical despite different names*

### Comparing `ps3-update-dl-0.3.0.post1/ps3_update_dl.egg-info/PKG-INFO` & `ps3_update_dl-0.3.0.post2/ps3_update_dl.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ps3-update-dl
-Version: 0.3.0.post1
+Version: 0.3.0.post2
 Summary: Download all updates for a given PS3 game
 Home-page: https://github.com/iomintz/ps3-update-dl
 Author: io mintz
 Author-email: io@mintz.cc
 License: AGPLv3+
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: System :: Emulators
 Classifier: Topic :: Utilities
@@ -22,14 +21,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown; variant=GFM
 License-File: LICENSE.md
+Requires-Dist: requests<3.0.0,>=2.23.0
+Requires-Dist: tqdm<5.0.0,>=4.49.0
+Requires-Dist: PyYAML<6.0.0,>=5.4.1
 
 # ps3-update-dl
 
 [![Build Status](https://img.shields.io/travis/com/ioistired/ps3-update-dl/trunk.svg?label=tests)](https://travis-ci.com/ioistired/ps3-update-dl)
 
 Downloads all updates for a given title directly from the PlayStation servers.
 
@@ -79,9 +81,7 @@
 ps3-update-dl is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU Affero General Public License for more details.
 
 You should have received a copy of the GNU Affero General Public License
 along with ps3-update-dl. If not, see <https://www.gnu.org/licenses/>.
-
-
```

### Comparing `ps3-update-dl-0.3.0.post1/setup.py` & `ps3_update_dl-0.3.0.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open(HERE / 'ps3_update_dl' / '__init__.py') as f:
 	VERSION = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', f.read(), re.MULTILINE).group(1)
 
 if not VERSION:
 	raise RuntimeError('version is not set')
 
-with open(HERE / 'README.md') as f:
+with open(HERE / 'README.md', encoding='utf-8') as f:
 	README = f.read()
 
 setuptools.setup(
 	name='ps3-update-dl',
 	author='io mintz',
 	author_email='io@mintz.cc',
 	url='https://github.com/iomintz/ps3-update-dl',
```

