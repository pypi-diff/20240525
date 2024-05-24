# Comparing `tmp/luxos-0.0.8b28.tar.gz` & `tmp/luxos-0.0.8b29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.8b28.tar", last modified: Wed May 22 21:28:13 2024, max compression
+gzip compressed data, was "luxos-0.0.8b29.tar", last modified: Fri May 24 22:34:15 2024, max compression
```

## Comparing `luxos-0.0.8b28.tar` & `luxos-0.0.8b29.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:28:13.547334 luxos-0.0.8b28/
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-22 21:28:13.547334 luxos-0.0.8b28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-22 21:27:24.000000 luxos-0.0.8b28/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 21:28:11.000000 luxos-0.0.8b28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:28:13.547334 luxos-0.0.8b28/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:28:13.539334 luxos-0.0.8b28/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:28:13.543334 luxos-0.0.8b28/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 21:28:11.000000 luxos-0.0.8b28/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:28:13.543334 luxos-0.0.8b28/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:28:13.543334 luxos-0.0.8b28/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-22 21:27:24.000000 luxos-0.0.8b28/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:28:13.547334 luxos-0.0.8b28/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-22 21:28:13.000000 luxos-0.0.8b28/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 21:28:13.000000 luxos-0.0.8b28/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:28:13.000000 luxos-0.0.8b28/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 21:28:13.000000 luxos-0.0.8b28/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 21:28:13.000000 luxos-0.0.8b28/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 21:28:13.000000 luxos-0.0.8b28/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:28:13.547334 luxos-0.0.8b28/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-22 21:27:24.000000 luxos-0.0.8b28/tests/test_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-22 21:27:24.000000 luxos-0.0.8b28/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-22 21:27:24.000000 luxos-0.0.8b28/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 21:27:24.000000 luxos-0.0.8b28/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-22 21:27:24.000000 luxos-0.0.8b28/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-22 21:27:24.000000 luxos-0.0.8b28/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:34:15.204831 luxos-0.0.8b29/
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-24 22:34:15.204831 luxos-0.0.8b29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-24 22:33:30.000000 luxos-0.0.8b29/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-24 22:34:13.000000 luxos-0.0.8b29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 22:34:15.204831 luxos-0.0.8b29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:34:15.196831 luxos-0.0.8b29/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:34:15.200831 luxos-0.0.8b29/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-24 22:34:13.000000 luxos-0.0.8b29/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:34:15.200831 luxos-0.0.8b29/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:34:15.204831 luxos-0.0.8b29/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-24 22:33:30.000000 luxos-0.0.8b29/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:34:15.204831 luxos-0.0.8b29/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-05-24 22:34:15.000000 luxos-0.0.8b29/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-24 22:34:15.000000 luxos-0.0.8b29/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 22:34:15.000000 luxos-0.0.8b29/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-24 22:34:15.000000 luxos-0.0.8b29/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 22:34:15.000000 luxos-0.0.8b29/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-24 22:34:15.000000 luxos-0.0.8b29/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 22:34:15.204831 luxos-0.0.8b29/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-24 22:33:30.000000 luxos-0.0.8b29/tests/test_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-24 22:33:30.000000 luxos-0.0.8b29/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-24 22:33:30.000000 luxos-0.0.8b29/tests/test_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-24 22:33:30.000000 luxos-0.0.8b29/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-24 22:33:30.000000 luxos-0.0.8b29/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-24 22:33:30.000000 luxos-0.0.8b29/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-24 22:33:30.000000 luxos-0.0.8b29/tests/test_utils.py
```

### Comparing `luxos-0.0.8b28/PKG-INFO` & `luxos-0.0.8b29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.8b28
+Version: 0.0.8b29
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.8b28/README.md` & `luxos-0.0.8b29/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/pyproject.toml` & `luxos-0.0.8b29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.8b28"
+version = "0.0.8b29"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
```

### Comparing `luxos-0.0.8b28/src/luxos/api.json` & `luxos-0.0.8b29/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/src/luxos/api.py` & `luxos-0.0.8b29/src/luxos/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def logon_required(cmd: str, commands_list=COMMANDS) -> bool | None:
     # Check if the command requires logon to LuxOS API
 
     if cmd not in COMMANDS:
         log.info(
-            "%s command is not supported. " "Try again with a different command.", cmd
+            "%s command is not supported. Try again with a different command.", cmd
         )
         return None
 
     return COMMANDS[cmd]["logon_required"]
 
 
 # TODO timeouts should be float | None
```

### Comparing `luxos-0.0.8b28/src/luxos/asyncops.py` & `luxos-0.0.8b29/src/luxos/asyncops.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,15 +199,15 @@
     timeout = TIMEOUT if timeout_sec is None else timeout_sec
     parameters = parameters or []
 
     sid = None
     if api.logon_required(cmd):
         sid = await logon(host, port)
         parameters = [sid, *parameters]
-        log.info("session id requested & obtained for %s:%i (%s)", host, port, sid)
+        log.debug("session id requested & obtained for %s:%i (%s)", host, port, sid)
     else:
         log.debug("no logon required for command '%s' on %s:%i", cmd, host, port)
 
     try:
         packet = {"command": cmd}
         if parameters:
             packet["parameter"] = ",".join(parameters)
@@ -222,15 +222,15 @@
         log.debug("received from %s:%s: %s", host, port, str(ret))
         return ((host, port), ret) if add_address else ret
     finally:
         if sid:
             await logoff(host, port, sid)
 
 
-def _rexec_paramteres(
+def _rexec_parameters(
     parameters: str | list[Any] | dict[str, Any] | None = None,
 ) -> list[str]:
     if isinstance(parameters, dict):
         data = []
         for key, value in parameters.items():
             if value is None:
                 value = "null"
@@ -252,15 +252,15 @@
     parameters: str | list[Any] | dict[str, Any] | None = None,
     timeout: float | None = None,
     retry: int | None = None,
     retry_delay: float | None = None,
 ) -> dict[str, Any] | None:
     from . import api
 
-    parameters = _rexec_paramteres(parameters)
+    parameters = _rexec_parameters(parameters)
 
     timeout = TIMEOUT if timeout is None else timeout
     retry = RETRY if retry is None else retry
     retry_delay = RETRY_DELAY if retry_delay is None else retry_delay
 
     # if cmd is logon/logoff we dealt with it differently
     if cmd in {"logon", "logoff"}:
@@ -283,15 +283,15 @@
     for i in range(retry + 1):
         if not api.logon_required(cmd):
             log.debug("no logon required for command '%s' on %s:%i", cmd, host, port)
             break
         try:
             sid = await logon(host, port, timeout)
             parameters = [sid, *parameters]
-            log.info("session id requested & obtained for %s:%i (%s)", host, port, sid)
+            log.debug("session id requested & obtained for %s:%i (%s)", host, port, sid)
             break
         except Exception as exc:
             failure = exc
         if retry and (i < retry) and retry_delay:
             await asyncio.sleep(retry_delay)
 
     if isinstance(failure, Exception):
```

### Comparing `luxos-0.0.8b28/src/luxos/cli/v1.py` & `luxos-0.0.8b29/src/luxos/cli/v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,16 @@
 import inspect
 import logging
 import sys
 import time
 from pathlib import Path
 from typing import Any, Callable
 
+from . import flags  # noqa: F401
+
 # SPECIAL MODULE LEVEL VARIABLES
 MODULE_VARIABLES = {
     "LOGGING_CONFIG": None,  # logging config dict
     # (passed to logging.basicConfig(**LOGGING_CONFIG))
     "CONFIGPATH": Path("config.yaml"),  # config default path
 }
 
@@ -282,13 +284,13 @@
 
             @functools.wraps(function)
             def _cli2(*args, **kwargs):
                 with setup() as ba:
                     log_sys_info()
                     return function(*ba.args, **ba.kwargs)
 
-        _cli2.attributes = {
+        _cli2.attributes = {  # type: ignore[attr-defined]
             "doc": function.__doc__ or module.__doc__ or "",
         }
         return _cli2
 
     return _cli1
```

### Comparing `luxos-0.0.8b28/src/luxos/exceptions.py` & `luxos-0.0.8b29/src/luxos/exceptions.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/src/luxos/misc.py` & `luxos-0.0.8b29/src/luxos/misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/src/luxos/scripts/async_luxos.py` & `luxos-0.0.8b29/src/luxos/scripts/async_luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/src/luxos/scripts/health_checker.py` & `luxos-0.0.8b29/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/src/luxos/scripts/luxos.py` & `luxos-0.0.8b29/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/src/luxos/text.py` & `luxos-0.0.8b29/src/luxos/text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/src/luxos/utils.py` & `luxos-0.0.8b29/src/luxos/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """user facing functions for normal use"""
 
 from __future__ import annotations
 
 import asyncio
-from pathlib import Path
 from typing import Any, Callable
 
 import luxos.misc
+
+# we bring here functions from other modules
 from luxos.asyncops import rexec  # noqa: F401
+from luxos.ips import load_ips_from_csv  # noqa: F401
+from luxos.scripts.luxos import execute_command  # noqa: F401
 
 
-def ip_ranges(txt: str, gsep: str = ":", rsep: str = "-") -> list[str]:
+def ip_ranges(
+    txt: str, rsep: str = "-", gsep: str = ":"
+) -> list[tuple[str, int | None]]:
     """return a list of ips given a text expression.
 
     Eg.
         >>> for ip in ip_ranges("127.0.0.1"):
         ...     print(ip)
         127.0.0.1
 
@@ -22,24 +27,17 @@
         ...     print(ip)
         127.0.0.1
         127.0.0.2
         127.0.0.3
 
     NOTE: use the `:` (gsep) to separate ips groups, and `-` (rsep) to define a range.
     """
-    return list(luxos.misc.iter_ip_ranges(txt, gsep, rsep))
-
-
-def load_ips_from_csv(path: Path | str, port: int = 4028) -> list[tuple[str, int]]:
-    from luxos.scripts.luxos import load_ip_list_from_csv
+    from .ips import iter_ip_ranges
 
-    result = []
-    for ip in load_ip_list_from_csv(str(path)):
-        result.append((ip, port))
-    return result
+    return list(iter_ip_ranges(txt, rsep=rsep, gsep=gsep))
 
 
 async def launch(
     addresses: list[tuple[str, int]], call: Callable[[str, int], Any], *args, **kwargs
 ) -> Any:
     """launch an async function on a list of (host, port) miners
```

### Comparing `luxos-0.0.8b28/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.8b29/src/luxos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.8b28
+Version: 0.0.8b29
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.8b28/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.8b29/src/luxos.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 pyproject.toml
 src/luxos/__init__.py
 src/luxos/__main__.py
 src/luxos/api.json
 src/luxos/api.py
 src/luxos/asyncops.py
 src/luxos/exceptions.py
+src/luxos/ips.py
 src/luxos/misc.py
 src/luxos/py.typed
 src/luxos/text.py
 src/luxos/utils.py
 src/luxos.egg-info/PKG-INFO
 src/luxos.egg-info/SOURCES.txt
 src/luxos.egg-info/dependency_links.txt
 src/luxos.egg-info/entry_points.txt
 src/luxos.egg-info/requires.txt
 src/luxos.egg-info/top_level.txt
 src/luxos/cli/__init__.py
+src/luxos/cli/flags.py
 src/luxos/cli/v1.py
 src/luxos/scripts/__init__.py
 src/luxos/scripts/async_luxos.py
 src/luxos/scripts/health_checker.py
 src/luxos/scripts/luxos.py
 tests/test_asyncops.py
 tests/test_cli.py
+tests/test_ips.py
 tests/test_luxos.py
 tests/test_misc.py
 tests/test_text.py
 tests/test_utils.py
```

### Comparing `luxos-0.0.8b28/tests/test_asyncops.py` & `luxos-0.0.8b29/tests/test_asyncops.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 def getminer() -> None | tuple[str, int]:
     if not (minerd := os.getenv("LUXOS_TEST_MINER")):
         return None
     host, port = minerd.split(":")
     return host.strip(), int(port)
 
 
-def test_rexec_paramteres():
-    assert aapi._rexec_paramteres(None) == []
-    assert aapi._rexec_paramteres("hello") == ["hello"]
-    assert aapi._rexec_paramteres(["hello", "world"]) == ["hello", "world"]
-    assert aapi._rexec_paramteres(["hello", 1]) == ["hello", "1"]
-    assert aapi._rexec_paramteres({"hello": 1}) == ["hello=1"]
-    assert aapi._rexec_paramteres({"hello": True}) == ["hello=true"]
+def test_rexec_parameters():
+    assert aapi._rexec_parameters(None) == []
+    assert aapi._rexec_parameters("hello") == ["hello"]
+    assert aapi._rexec_parameters(["hello", "world"]) == ["hello", "world"]
+    assert aapi._rexec_parameters(["hello", 1]) == ["hello", "1"]
+    assert aapi._rexec_parameters({"hello": 1}) == ["hello=1"]
+    assert aapi._rexec_parameters({"hello": True}) == ["hello=true"]
 
 
 def test_validate_message():
     pytest.raises(
         exceptions.MinerCommandMalformedMessageError, aapi.validate_message, "a", 0, {}
     )
     host, port = "a", 0
```

### Comparing `luxos-0.0.8b28/tests/test_cli.py` & `luxos-0.0.8b29/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/tests/test_misc.py` & `luxos-0.0.8b29/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/tests/test_text.py` & `luxos-0.0.8b29/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b28/tests/test_utils.py` & `luxos-0.0.8b29/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     }
 
     ret = await utils.launch(addresses, call, batch=100)
     assert set(ret) == expected
 
 
 def test_util_ip_ranges():
-    assert set(utils.ip_ranges("127.0.0.1")) == {"127.0.0.1"}
+    assert set(utils.ip_ranges("127.0.0.1")) == {("127.0.0.1", None)}
     assert set(utils.ip_ranges("127.0.0.1->127.0.0.3", gsep="\n", rsep="->")) == {
-        "127.0.0.1",
-        "127.0.0.2",
-        "127.0.0.3",
+        ("127.0.0.1", None),
+        ("127.0.0.2", None),
+        ("127.0.0.3", None),
     }
     assert set(utils.ip_ranges("127.0.0.1-127.0.0.3\n127.0.0.15", gsep="\n")) == {
-        "127.0.0.1",
-        "127.0.0.2",
-        "127.0.0.3",
-        "127.0.0.15",
+        ("127.0.0.1", None),
+        ("127.0.0.2", None),
+        ("127.0.0.3", None),
+        ("127.0.0.15", None),
     }
```

