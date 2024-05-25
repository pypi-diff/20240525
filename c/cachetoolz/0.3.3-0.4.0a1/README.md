# Comparing `tmp/cachetoolz-0.3.3.tar.gz` & `tmp/cachetoolz-0.4.0a1.tar.gz`

## Comparing `cachetoolz-0.3.3.tar` & `cachetoolz-0.4.0a1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/__init__.py
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/decorator.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/exceptions.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/log.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/types.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/utils.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/abc/__init__.py
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/abc/backend.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/abc/coder.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/abc/serializer.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/backend/__init__.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/backend/inmemory.py
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/backend/mongo.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/backend/redis.py
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/coder/__init__.py
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/coder/decoder.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/cachetoolz/coder/encoder.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/LICENSE
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/README.md
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 cachetoolz-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/__init__.py
+-rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/decorator.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/exceptions.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/log.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/types.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/utils.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/abc/__init__.py
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/abc/backend.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/abc/coder.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/abc/serializer.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/backend/__init__.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/backend/inmemory.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/backend/mongo.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/backend/redis.py
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/coder/__init__.py
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/coder/decoder.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/cachetoolz/coder/encoder.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/.gitignore
+-rw-r--r--   0        0        0    35074 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/README.md
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 cachetoolz-0.4.0a1/PKG-INFO
```

### Comparing `cachetoolz-0.3.3/cachetoolz/decorator.py` & `cachetoolz-0.4.0a1/cachetoolz/decorator.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/log.py` & `cachetoolz-0.4.0a1/cachetoolz/log.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/types.py` & `cachetoolz-0.4.0a1/cachetoolz/types.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/utils.py` & `cachetoolz-0.4.0a1/cachetoolz/utils.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/abc/backend.py` & `cachetoolz-0.4.0a1/cachetoolz/abc/backend.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/abc/coder.py` & `cachetoolz-0.4.0a1/cachetoolz/abc/coder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/abc/serializer.py` & `cachetoolz-0.4.0a1/cachetoolz/abc/serializer.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/backend/inmemory.py` & `cachetoolz-0.4.0a1/cachetoolz/backend/inmemory.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/backend/mongo.py` & `cachetoolz-0.4.0a1/cachetoolz/backend/mongo.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/backend/redis.py` & `cachetoolz-0.4.0a1/cachetoolz/backend/redis.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/coder/__init__.py` & `cachetoolz-0.4.0a1/cachetoolz/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/coder/decoder.py` & `cachetoolz-0.4.0a1/cachetoolz/coder/decoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/cachetoolz/coder/encoder.py` & `cachetoolz-0.4.0a1/cachetoolz/coder/encoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/.gitignore` & `cachetoolz-0.4.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.3/README.md` & `cachetoolz-0.4.0a1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # Cache Toolz
 
-[![License MIT](https://img.shields.io/pypi/l/cachetoolz?label=License&color=%234B78E6)](https://codeberg.org/taconi/cachetoolz/src/branch/main/LICENSE)
-[![status-badge](https://ci.codeberg.org/api/badges/13098/status.svg)](https://ci.codeberg.org/repos/13098)
-[![codecov](https://img.shields.io/codecov/c/github/taconi/cachetoolz?logo=codecov&style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/taconi/cachetoolz)
+[![License GPLv3+](https://img.shields.io/pypi/l/cachetoolz?label=License&color=%234B78E6)](https://codeberg.org/taconi/cachetoolz/src/branch/main/LICENSE)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cachetoolz.svg?logo=python&label=Python&color=%234B78E6)](https://pypi.python.org/pypi/cachetoolz/)
 [![PyPI version](https://img.shields.io/pypi/v/cachetoolz.svg?logo=pypi&label=PyPI&color=%23FA9BFA)](https://pypi.org/project/cachetoolz/)
 [![Downloads](https://img.shields.io/pypi/dm/cachetoolz?logo=pypi&label=Downloads&color=%2373DC8C)](https://pypi.org/project/cachetoolz/)
 [![Documentation](https://img.shields.io/badge/Documentation-1769AA?color=%234B78E6)](https://cachetoolz.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/Changelog-1769AA?color=%2373DC8C)](https://cachetoolz.readthedocs.io/changelog)
 [![Issue Tracker](https://img.shields.io/badge/Issue%20Tracker-1769AA?color=%23FA9BFA)]("https://codeberg.org/taconi/cachetoolz/issues")
 [![Contributing](https://img.shields.io/badge/Contributing-1769AA?color=%234B78E6)](https://cachetoolz.readthedocs.io/contributing)
```

### Comparing `cachetoolz-0.3.3/pyproject.toml` & `cachetoolz-0.4.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cachetoolz"
-version = "0.3.3"
+version = "0.4.0a1"
 description = "This library provides a decorator for caching functions"
-license = "MIT"
-authors = [{ name = "Igor Taconi", email = "igor.taconi@protonmail.com" }]
-maintainers = [{ name = "Igor Taconi", email = "igor.taconi@protonmail.com" }]
+license = "GPL-3.0-or-later"
+authors = [{ name = "taconi", email = "igor.taconi@protonmail.com" }]
+maintainers = [{ name = "taconi", email = "igor.taconi@protonmail.com" }]
 readme = "README.md"
 keywords = ["python", "cache", "async", "redis", "mongo"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
-  "License :: OSI Approved :: MIT License",
+  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
 ]
 
 requires-python = ">=3.8"
 
 dependencies = [
@@ -95,20 +95,23 @@
 # autoflake --in-place -r cachetoolz
 isort cachetoolz
 black cachetoolz
 docformatter --in-place -r cachetoolz
 """
 
 check = """
+gitlint --ignore-stdin
 flake8 cachetoolz
 isort --check-only --diff cachetoolz
 black --check --diff cachetoolz
 docformatter -r cachetoolz
 """
 
+precommit = "pre-commit run --all-files"
+
 [tool.hatch.envs.docs]
 dependencies = ["mkdocs-material>=9.5.11", "mkdocstrings-python>=1.8.0"]
 
 [tool.hatch.envs.docs.scripts]
 serve = "mkdocs serve"
 build = "mkdocs build"
 deploy = "mkdocs gh-deploy --force -b pages"
@@ -130,14 +133,15 @@
 skip-string-normalization = true
 
 [tool.flake8]
 ignore = [
   "E121",
   "E123",
   "E126",
+  "E231",
   "E226",
   "E24",
   "E704",
   "W503",
   "W504",
   "D401",
   "D412",
```

### Comparing `cachetoolz-0.3.3/PKG-INFO` & `cachetoolz-0.4.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cachetoolz
-Version: 0.3.3
+Version: 0.4.0a1
 Summary: This library provides a decorator for caching functions
 Project-URL: Homepage, https://codeberg.org/taconi/cachetoolz/#cache-toolz
 Project-URL: Changelog, https://cachetoolz.readthedocs.io/changelog
 Project-URL: Contributing, https://cachetoolz.readthedocs.io/contributing
 Project-URL: Documentation, https://cachetoolz.readthedocs.io
 Project-URL: Issue Tracker, https://codeberg.org/taconi/cachetoolz/issues
 Project-URL: Repository, https://codeberg.org/taconi/cachetoolz/
-Author-email: Igor Taconi <igor.taconi@protonmail.com>
-Maintainer-email: Igor Taconi <igor.taconi@protonmail.com>
-License-Expression: MIT
+Author-email: taconi <igor.taconi@protonmail.com>
+Maintainer-email: taconi <igor.taconi@protonmail.com>
+License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Keywords: async,cache,mongo,python,redis
 Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -34,17 +34,15 @@
 Requires-Dist: pymongo>=4.6.2; extra == 'mongo'
 Provides-Extra: redis
 Requires-Dist: redis>=5.0.1; extra == 'redis'
 Description-Content-Type: text/markdown
 
 # Cache Toolz
 
-[![License MIT](https://img.shields.io/pypi/l/cachetoolz?label=License&color=%234B78E6)](https://codeberg.org/taconi/cachetoolz/src/branch/main/LICENSE)
-[![status-badge](https://ci.codeberg.org/api/badges/13098/status.svg)](https://ci.codeberg.org/repos/13098)
-[![codecov](https://img.shields.io/codecov/c/github/taconi/cachetoolz?logo=codecov&style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/taconi/cachetoolz)
+[![License GPLv3+](https://img.shields.io/pypi/l/cachetoolz?label=License&color=%234B78E6)](https://codeberg.org/taconi/cachetoolz/src/branch/main/LICENSE)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/cachetoolz.svg?logo=python&label=Python&color=%234B78E6)](https://pypi.python.org/pypi/cachetoolz/)
 [![PyPI version](https://img.shields.io/pypi/v/cachetoolz.svg?logo=pypi&label=PyPI&color=%23FA9BFA)](https://pypi.org/project/cachetoolz/)
 [![Downloads](https://img.shields.io/pypi/dm/cachetoolz?logo=pypi&label=Downloads&color=%2373DC8C)](https://pypi.org/project/cachetoolz/)
 [![Documentation](https://img.shields.io/badge/Documentation-1769AA?color=%234B78E6)](https://cachetoolz.readthedocs.io)
 [![Changelog](https://img.shields.io/badge/Changelog-1769AA?color=%2373DC8C)](https://cachetoolz.readthedocs.io/changelog)
 [![Issue Tracker](https://img.shields.io/badge/Issue%20Tracker-1769AA?color=%23FA9BFA)]("https://codeberg.org/taconi/cachetoolz/issues")
 [![Contributing](https://img.shields.io/badge/Contributing-1769AA?color=%234B78E6)](https://cachetoolz.readthedocs.io/contributing)
```

