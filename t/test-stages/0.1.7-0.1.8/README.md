# Comparing `tmp/test_stages-0.1.7.tar.gz` & `tmp/test_stages-0.1.8.tar.gz`

## Comparing `test_stages-0.1.7.tar` & `test_stages-0.1.8.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 test_stages-0.1.7/.editorconfig
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 test_stages-0.1.7/.readthedocs.yaml
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 test_stages-0.1.7/mkdocs.yml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 test_stages-0.1.7/ruff-base.toml
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 test_stages-0.1.7/tox.ini
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 test_stages-0.1.7/.reuse/dep5
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 test_stages-0.1.7/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 test_stages-0.1.7/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0        0        0    10793 2020-02-02 00:00:00.000000 test_stages-0.1.7/docs/changes.md
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 test_stages-0.1.7/docs/download.md
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 test_stages-0.1.7/docs/index.md
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 test_stages-0.1.7/docs/cmd/index.md
--rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 test_stages-0.1.7/docs/cmd/tox-stages.md
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 test_stages-0.1.7/docs/man/tox-stages.1
--rwxr-xr-x   0        0        0      495 2020-02-02 00:00:00.000000 test_stages-0.1.7/nix/cleanpy.sh
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 test_stages-0.1.7/nix/mkdocs.nix
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 test_stages-0.1.7/nix/python-vetox.nix
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 test_stages-0.1.7/nix/reformat.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 test_stages-0.1.7/nix/run-vetox.sh
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 test_stages-0.1.7/requirements/docs.txt
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 test_stages-0.1.7/requirements/install.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 test_stages-0.1.7/requirements/ruff.txt
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 test_stages-0.1.7/requirements/selftest.txt
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 test_stages-0.1.7/requirements/test.txt
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/selftest/__init__.py
--rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/selftest/__main__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/test_stages/__init__.py
--rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/test_stages/cmd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/test_stages/py.typed
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/test_stages/tox_stages/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/test_stages/tox_stages/__main__.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/tox_trivtags/__init__.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/tox_trivtags/parse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_stages-0.1.7/src/tox_trivtags/py.typed
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 test_stages-0.1.7/stubs/contextlib_chdir.pyi
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 test_stages-0.1.7/stubs/pyproject_hooks.pyi
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 test_stages-0.1.7/stubs/tox/__init__.pyi
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 test_stages-0.1.7/stubs/tox/config.pyi
--rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 test_stages-0.1.7/tests/vetox.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 test_stages-0.1.7/tests/unit/__init__.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 test_stages-0.1.7/tests/unit/test_functional.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 test_stages-0.1.7/.gitignore
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 test_stages-0.1.7/README.md
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 test_stages-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 test_stages-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 test_stages-0.1.8/.editorconfig
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 test_stages-0.1.8/.readthedocs.yaml
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 test_stages-0.1.8/mkdocs.yml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 test_stages-0.1.8/ruff-base.toml
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 test_stages-0.1.8/tox.ini
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 test_stages-0.1.8/.reuse/dep5
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 test_stages-0.1.8/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 test_stages-0.1.8/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0    11293 2020-02-02 00:00:00.000000 test_stages-0.1.8/docs/changes.md
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 test_stages-0.1.8/docs/download.md
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 test_stages-0.1.8/docs/index.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 test_stages-0.1.8/docs/cmd/index.md
+-rw-r--r--   0        0        0     5506 2020-02-02 00:00:00.000000 test_stages-0.1.8/docs/cmd/tox-stages.md
+-rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 test_stages-0.1.8/docs/man/tox-stages.1
+-rwxr-xr-x   0        0        0      495 2020-02-02 00:00:00.000000 test_stages-0.1.8/nix/cleanpy.sh
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 test_stages-0.1.8/nix/mkdocs.nix
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 test_stages-0.1.8/nix/python-vetox.nix
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 test_stages-0.1.8/nix/reformat.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 test_stages-0.1.8/nix/run-vetox.sh
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 test_stages-0.1.8/requirements/docs.txt
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 test_stages-0.1.8/requirements/install.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 test_stages-0.1.8/requirements/ruff.txt
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 test_stages-0.1.8/requirements/selftest-uv.txt
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 test_stages-0.1.8/requirements/selftest.txt
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 test_stages-0.1.8/requirements/test.txt
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/selftest/__init__.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/selftest/__main__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/test_stages/__init__.py
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/test_stages/cmd.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/test_stages/py.typed
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/test_stages/tox_stages/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/test_stages/tox_stages/__main__.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/tox_trivtags/__init__.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/tox_trivtags/parse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 test_stages-0.1.8/src/tox_trivtags/py.typed
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 test_stages-0.1.8/stubs/contextlib_chdir.pyi
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 test_stages-0.1.8/stubs/pyproject_hooks.pyi
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 test_stages-0.1.8/stubs/tox/__init__.pyi
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 test_stages-0.1.8/stubs/tox/config.pyi
+-rw-r--r--   0        0        0    11119 2020-02-02 00:00:00.000000 test_stages-0.1.8/tests/vetox.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 test_stages-0.1.8/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 test_stages-0.1.8/tests/unit/test_functional.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 test_stages-0.1.8/.gitignore
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 test_stages-0.1.8/README.md
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 test_stages-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 test_stages-0.1.8/PKG-INFO
```

### Comparing `test_stages-0.1.7/.editorconfig` & `test_stages-0.1.8/.editorconfig`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/mkdocs.yml` & `test_stages-0.1.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/ruff-base.toml` & `test_stages-0.1.8/ruff-base.toml`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/tox.ini` & `test_stages-0.1.8/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   format
   mypy
   reuse
   unit-tests-no-tox
   unit-tests-tox-3
   unit-tests-tox-4
   selftest
+  selftest-uv
   docs
 isolated_build = True
 
 [defs]
 pyfiles_mypy =
   src/selftest \
   src/test_stages \
@@ -125,14 +126,27 @@
   hatchling >= 1.14.1, < 2
   hatch-requirements-txt >= 0.4, < 0.5
 setenv =
   PYTHONPATH = {toxinidir}/src
 commands =
   python3 -m selftest
 
+[testenv:selftest-uv]
+tags =
+  tests
+deps =
+  -r requirements/install.txt
+  -r requirements/selftest-uv.txt
+  hatchling >= 1.14.1, < 2
+  hatch-requirements-txt >= 0.4, < 0.5
+setenv =
+  PYTHONPATH = {toxinidir}/src
+commands =
+  python3 -m selftest
+
 # The pyupgrade tool does not seem to have a "check only" mode
 [testenv:pyupgrade]
 skip_install = True
 tags =
   check
   manual
 deps =
```

### Comparing `test_stages-0.1.7/LICENSES/BSD-2-Clause.txt` & `test_stages-0.1.8/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/LICENSES/BSD-3-Clause.txt` & `test_stages-0.1.8/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/docs/changes.md` & `test_stages-0.1.8/docs/changes.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,33 @@
 All notable changes to the test-stages project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.8] - 2024-05-25
+
+### Fixes
+
+- run `tox config` with the `-q` option to avoid diagnostic output from Tox plugins to
+  mix in with the actual configuration settings
+- documentation:
+    - correct the 0.1.7 tag link on the downloads page
+
+### Additions
+
+- add `publync` configuration to the `pyproject.toml` file
+
+### Other changes
+
+- test suite:
+    - Ruff:
+        - use Ruff 0.4.5 with no changes
+
 ## [0.1.7] - 2024-03-17
 
 ### Fixes
 
 - documentation:
     - correct the 0.1.6 release date on the download page
 
@@ -262,15 +281,16 @@
 
 - First public release.
 
 [readthedocs]: https://test-stages.readthedocs.io/en/latest/
 [ringlet-test-stages]: https://devel.ringlet.net/devel/test-stages/ "The Ringlet test-stages homepage"
 [tool-mkdocs]: https://www.mkdocs.org/ "Project documentation with Markdown"
 
-[Unreleased]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.7...main
+[Unreleased]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.8...main
+[0.1.8]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.7...release%2F0.1.8
 [0.1.7]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.6...release%2F0.1.7
 [0.1.6]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.5...release%2F0.1.6
 [0.1.5]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.4...release%2F0.1.5
 [0.1.4]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.3...release%2F0.1.4
 [0.1.3]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.2...release%2F0.1.3
 [0.1.2]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.1...release%2F0.1.2
 [0.1.1]: https://gitlab.com/ppentchev/test-stages/-/compare/release%2F0.1.0...release%2F0.1.1
```

### Comparing `test_stages-0.1.7/docs/download.md` & `test_stages-0.1.8/docs/download.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,38 @@
 SPDX-License-Identifier: BSD-2-Clause
 -->
 
 # Download
 
 These are the released versions of [test-stages](index.md) available for download.
 
+## [0.1.8] - 2024-05-25
+
+### Source tarball
+
+- [test_stages-0.1.8.tar.gz](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.8.tar.gz)
+  (with [a PGP signature](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.8.tar.gz.asc))
+
+### Python wheel
+
+- [test_stages-0.1.8-py3-none-any.whl](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.8-py3-none-any.whl)
+  (with [a PGP signature](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.8-py3-none-any.whl.asc))
+
 ## [0.1.7] - 2024-03-17
 
 ### Source tarball
 
 - [test_stages-0.1.7.tar.gz](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.7.tar.gz)
   (with [a PGP signature](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.7.tar.gz.asc))
 
 ### Python wheel
 
 - [test_stages-0.1.7-py3-none-any.whl](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.7-py3-none-any.whl)
   (with [a PGP signature](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.7-py3-none-any.whl.asc))
 
-
 ## [0.1.6] - 2024-02-08
 
 ### Source tarball
 
 - [test_stages-0.1.6.tar.gz](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.6.tar.gz)
   (with [a PGP signature](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.6.tar.gz.asc))
 
@@ -52,10 +63,11 @@
   (with [a PGP signature](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.4.tar.gz.asc))
 
 ### Python wheel
 
 - [test_stages-0.1.4-py3-none-any.whl](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.4-py3-none-any.whl)
   (with [a PGP signature](https://devel.ringlet.net/files/devel/test-stages/test_stages-0.1.4-py3-none-any.whl.asc))
 
+[0.1.7]: https://gitlab.com/ppentchev/test-stages/-/tags/release%2F0.1.7
 [0.1.6]: https://gitlab.com/ppentchev/test-stages/-/tags/release%2F0.1.6
 [0.1.5]: https://gitlab.com/ppentchev/test-stages/-/tags/release%2F0.1.5
 [0.1.4]: https://gitlab.com/ppentchev/test-stages/-/tags/release%2F0.1.4
```

### Comparing `test_stages-0.1.7/docs/index.md` & `test_stages-0.1.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/docs/cmd/tox-stages.md` & `test_stages-0.1.8/docs/cmd/tox-stages.md`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/docs/man/tox-stages.1` & `test_stages-0.1.8/docs/man/tox-stages.1`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/nix/mkdocs.nix` & `test_stages-0.1.8/nix/mkdocs.nix`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/nix/python-vetox.nix` & `test_stages-0.1.8/nix/python-vetox.nix`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/src/selftest/__main__.py` & `test_stages-0.1.8/src/selftest/__main__.py`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/src/test_stages/cmd.py` & `test_stages-0.1.8/src/test_stages/cmd.py`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/src/test_stages/tox_stages/__main__.py` & `test_stages-0.1.8/src/test_stages/tox_stages/__main__.py`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/src/tox_trivtags/__init__.py` & `test_stages-0.1.8/src/tox_trivtags/__init__.py`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/src/tox_trivtags/parse.py` & `test_stages-0.1.8/src/tox_trivtags/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,17 +84,18 @@
     *,
     env: dict[str, str] | None = None,
     tox_invoke: list[str | pathlib.Path] | None = None,
 ) -> dict[str, TestenvTags]:
     """Run `tox --showconfig` and look for tags in its output."""
     if tox_invoke is None:
         tox_invoke = [sys.executable, "-u", "-m", "tox"]
+    tox_cfg_command: Final = ["--showconfig"] if HAVE_MOD_TOX_3 else ["-q", "config"]
     tox_cmd: Final = [
         *tox_invoke,
-        "--showconfig" if HAVE_MOD_TOX_3 else "config",
+        *tox_cfg_command,
         "-c",
         filename,
         "-e",
         "ALL",
     ]
 
     def parse_output() -> configparser.ConfigParser:
```

### Comparing `test_stages-0.1.7/stubs/tox/config.pyi` & `test_stages-0.1.8/stubs/tox/config.pyi`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/tests/vetox.py` & `test_stages-0.1.8/tests/vetox.py`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/tests/unit/test_functional.py` & `test_stages-0.1.8/tests/unit/test_functional.py`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/README.md` & `test_stages-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `test_stages-0.1.7/pyproject.toml` & `test_stages-0.1.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -69,14 +69,23 @@
 
 [tool.hatch.version]
 path = "src/test_stages/__init__.py"
 
 [tool.mypy]
 strict = true
 
+[tool.publync.format.version]
+major = 0
+minor = 1
+
+[tool.publync.build.tox]
+
+[tool.publync.sync.rsync]
+remote = "marla.ludost.net:vhosts/devel.ringlet.net/public_html/devel/test-stages"
+
 [tool.ruff]
 extend = "ruff-base.toml"
 output-format = "concise"
 preview = true
 
 [tool.ruff.lint]
 select = ["ALL"]
```

### Comparing `test_stages-0.1.7/PKG-INFO` & `test_stages-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: test_stages
-Version: 0.1.7
+Version: 0.1.8
 Summary: Group Tox, Nox, etc environments into stages, run them in parallel
 Project-URL: Homepage, https://devel.ringlet.net/devel/test-stages
 Project-URL: Changes, https://devel.ringlet.net/devel/test-stages/changes/
 Project-URL: Issue Tracker, https://gitlab.com/ppentchev/test-stages/-/issues
 Project-URL: Source Code, https://gitlab.com/ppentchev/test-stages
 Author-email: Peter Pentchev <roam@ringlet.net>
 License: BSD-2-Clause
```

