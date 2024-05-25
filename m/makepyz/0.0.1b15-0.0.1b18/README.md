# Comparing `tmp/makepyz-0.0.1b15.tar.gz` & `tmp/makepyz-0.0.1b18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makepyz-0.0.1b15.tar", last modified: Thu May 23 13:59:26 2024, max compression
+gzip compressed data, was "makepyz-0.0.1b18.tar", last modified: Fri May 24 15:51:44 2024, max compression
```

## Comparing `makepyz-0.0.1b15.tar` & `makepyz-0.0.1b18.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:26.774052 makepyz-0.0.1b15/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-23 13:59:26.774052 makepyz-0.0.1b15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-23 13:59:24.000000 makepyz-0.0.1b15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:59:26.774052 makepyz-0.0.1b15/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:26.766052 makepyz-0.0.1b15/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:26.770052 makepyz-0.0.1b15/src/makepyz/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 13:59:24.000000 makepyz-0.0.1b15/src/makepyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/scm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:26.770052 makepyz-0.0.1b15/src/makepyz/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/scripts/makepyzui.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/src/makepyz/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:26.774052 makepyz-0.0.1b15/src/makepyz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-23 13:59:26.000000 makepyz-0.0.1b15/src/makepyz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-23 13:59:26.000000 makepyz-0.0.1b15/src/makepyz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:59:26.000000 makepyz-0.0.1b15/src/makepyz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 13:59:26.000000 makepyz-0.0.1b15/src/makepyz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-23 13:59:26.000000 makepyz-0.0.1b15/src/makepyz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 13:59:26.000000 makepyz-0.0.1b15/src/makepyz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:59:26.770052 makepyz-0.0.1b15/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/tests/test_fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/tests/test_makepyx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-23 13:59:08.000000 makepyz-0.0.1b15/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:51:44.728917 makepyz-0.0.1b18/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-24 15:51:44.728917 makepyz-0.0.1b18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-24 15:51:42.000000 makepyz-0.0.1b18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 15:51:44.728917 makepyz-0.0.1b18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:51:44.720917 makepyz-0.0.1b18/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:51:44.724917 makepyz-0.0.1b18/src/makepyz/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 15:51:42.000000 makepyz-0.0.1b18/src/makepyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/scm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:51:44.724917 makepyz-0.0.1b18/src/makepyz/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/scripts/makepyzui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/src/makepyz/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:51:44.728917 makepyz-0.0.1b18/src/makepyz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-24 15:51:44.000000 makepyz-0.0.1b18/src/makepyz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-24 15:51:44.000000 makepyz-0.0.1b18/src/makepyz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 15:51:44.000000 makepyz-0.0.1b18/src/makepyz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-24 15:51:44.000000 makepyz-0.0.1b18/src/makepyz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 15:51:44.000000 makepyz-0.0.1b18/src/makepyz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 15:51:44.000000 makepyz-0.0.1b18/src/makepyz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 15:51:44.728917 makepyz-0.0.1b18/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/tests/test_fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/tests/test_makepyx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-24 15:51:25.000000 makepyz-0.0.1b18/tests/test_tree.py
```

### Comparing `makepyz-0.0.1b15/pyproject.toml` & `makepyz-0.0.1b18/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "makepyz"
-version = "0.0.1b15"
+version = "0.0.1b18"
 description = "a new kind of make tool"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
 keywords = [
   "git",
   "scm",
```

### Comparing `makepyz-0.0.1b15/src/makepyz/cli.py` & `makepyz-0.0.1b18/src/makepyz/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             help="path to a config file",
         )
 
     def error(self, message):
         raise AbortWrongArgumentError(message)
 
     def parse_args(self, args=None, namespace=None):
-        #options = super().parse_args(args, namespace)
+        # options = super().parse_args(args, namespace)
         options, arguments = super().parse_known_args(args, namespace)
 
         # setup the logging
         config = {}
         if value := self.module_variables.get("LOGGING_CONFIG"):
             config = value.copy()
```

### Comparing `makepyz-0.0.1b15/src/makepyz/exceptions.py` & `makepyz-0.0.1b18/src/makepyz/exceptions.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/src/makepyz/fileos.py` & `makepyz-0.0.1b18/src/makepyz/fileos.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """various file/dir related functions"""
 
 from __future__ import annotations
 
 import contextlib
 import os
+import subprocess
+import sys
 import shutil
 import tempfile
 import types
 from pathlib import Path
-from typing import Any, overload, Iterator
+from typing import overload, Iterator
 
 
 class FileOSError(Exception):
     pass
 
 
 class FileOSModuleNotFoundError(FileOSError):
@@ -100,37 +102,45 @@
             machinery.SOURCE_SUFFIXES.pop()
     return module
 
 
 ### FILE UTILITIES
 
 
-def zextract(path: Path | str, items: list[str] | None = None) -> dict[str, Any]:
+def zextract(
+    path: Path | str, items: list[str] | None = None, encoding: str | None = "utf-8"
+) -> dict[str, str | bytes]:
     """extracts from path (a zipfile/tarball) all data in a dictionary"""
     from tarfile import TarFile, is_tarfile
     from zipfile import ZipFile, is_zipfile
 
     path = Path(path)
-    result = {}
+    result: dict[str, str | bytes] = {}
     if is_tarfile(path):
         with TarFile.open(path) as tfp:
             for member in tfp.getmembers():
                 fp = tfp.extractfile(member)
                 if not fp:
                     continue
                 result[member.name] = str(fp.read(), encoding="utf-8")
     elif is_zipfile(path):
         with ZipFile(path) as tfp:
             for zinfo in tfp.infolist():
                 if items and zinfo.filename not in items:
                     continue
                 with tfp.open(zinfo.filename) as fp:
-                    result[zinfo.filename] = str(fp.read(), encoding="utf-8").replace(
-                        "\r", ""
-                    )
+                    data = fp.read()
+                    try:
+                        if encoding:
+                            out = str(data, encoding=encoding).replace("\r", "")
+                            result[zinfo.filename] = out
+                        else:
+                            result[zinfo.filename] = data
+                    except UnicodeDecodeError:
+                        pass
 
     return result
 
 
 def backup(path: Path, ext: str, overwrite: bool = False, abort: bool = True) -> Path:
     """creates a backup of path"""
     from shutil import copyfile, copymode
@@ -186,7 +196,31 @@
     try:
         yield save
     finally:
         for backup in pathlist:
             original = Path(backup).with_suffix("")
             original.unlink()
             shutil.move(Path(backup), original)
+
+
+def check_call(*args, **kwargs):
+    """multiplatform check_call"""
+
+    # this takes care of win/*nix fdifferences
+    shell = False
+    env = kwargs.get("env", os.environ).copy()
+    if sys.platform == "win32":
+        epath = os.environ.get("PATH", "").split(os.pathsep)
+        exedir = Path(sys.executable).parent / "Scripts"
+        if str(exedir) not in epath:
+            epath.insert(0, str(exedir))
+        env["PATH"] = os.pathsep.join(str(e) for e in epath)
+
+        eext = os.environ.get("PATHEXT", "").split(os.pathsep)
+        exeext = ".EXE"
+        if exeext not in eext:
+            eext.insert(0, str(exeext))
+        env["PATHEXT"] = os.pathsep.join(str(e) for e in eext)
+        shell = True
+    kwargs["shell"] = shell
+    kwargs["env"] = env
+    return subprocess.check_call(*args, **kwargs)
```

### Comparing `makepyz-0.0.1b15/src/makepyz/github.py` & `makepyz-0.0.1b18/src/makepyz/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,11 +36,9 @@
 
     """
     gdata = (
         json.loads(Path(github_dump[1:]).read_text())
         if github_dump.startswith("@")
         else json.loads(github_dump)
     )
-    validate_gdata(
-        gdata, ["run_number", "sha", "ref_name", "ref_type", "workflow_ref"]
-    )
-    return gdata
+    validate_gdata(gdata, ["run_number", "sha", "ref_name", "ref_type", "workflow_ref"])
+    return gdata
```

### Comparing `makepyz-0.0.1b15/src/makepyz/scm.py` & `makepyz-0.0.1b18/src/makepyz/scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/src/makepyz/scripts/makepyzui.py` & `makepyz-0.0.1b18/src/makepyz/scripts/makepyzui.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/src/makepyz/tasks.py` & `makepyz-0.0.1b18/src/makepyz/tasks.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/src/makepyz/text.py` & `makepyz-0.0.1b18/src/makepyz/text.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/src/makepyz/tree.py` & `makepyz-0.0.1b18/src/makepyz/tree.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/src/makepyz.egg-info/SOURCES.txt` & `makepyz-0.0.1b18/src/makepyz.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 src/makepyz/__main__.py
 src/makepyz/api.py
 src/makepyz/cli.py
 src/makepyz/exceptions.py
 src/makepyz/fileos.py
 src/makepyz/github.py
 src/makepyz/misc.py
+src/makepyz/packaging.py
 src/makepyz/py.typed
 src/makepyz/scm.py
 src/makepyz/tasks.py
 src/makepyz/text.py
 src/makepyz/tree.py
 src/makepyz.egg-info/PKG-INFO
 src/makepyz.egg-info/SOURCES.txt
 src/makepyz.egg-info/dependency_links.txt
 src/makepyz.egg-info/entry_points.txt
 src/makepyz.egg-info/requires.txt
 src/makepyz.egg-info/top_level.txt
 src/makepyz/scripts/makepyzui.py
+tests/test_cli.py
 tests/test_fileos.py
 tests/test_makepyx.py
+tests/test_packaging.py
 tests/test_scm.py
 tests/test_text.py
 tests/test_tree.py
```

### Comparing `makepyz-0.0.1b15/tests/test_fileos.py` & `makepyz-0.0.1b18/tests/test_fileos.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/tests/test_scm.py` & `makepyz-0.0.1b18/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `makepyz-0.0.1b15/tests/test_text.py` & `makepyz-0.0.1b18/tests/test_text.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from __future__ import annotations
+import types
+
 from makepyz import text
 
-try:
-    import rich
-except ModuleNotFoundError:
-    rich = None
+import importlib.util
+
+rich: types.ModuleType | None = None
+if _spec := importlib.util.find_spec("rich"):
+    rich = importlib.util.module_from_spec(_spec)
 
 
 def test_indent():
     txt = """
 
             Lorem Ipsum is simply dummy text of the printing and
           typesetting industry. Lorem Ipsum has been the industry's standard
```

### Comparing `makepyz-0.0.1b15/tests/test_tree.py` & `makepyz-0.0.1b18/tests/test_tree.py`

 * *Files identical despite different names*

