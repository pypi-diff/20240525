# Comparing `tmp/traceme-0.5.0.tar.gz` & `tmp/traceme-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceme-0.5.0.tar", max compression
+gzip compressed data, was "traceme-0.6.0.tar", max compression
```

## Comparing `traceme-0.5.0.tar` & `traceme-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2024-02-10 16:20:36.182282 traceme-0.5.0/LICENSE
--rw-r--r--   0        0        0     2643 2024-02-10 16:20:36.182282 traceme-0.5.0/README.md
--rw-r--r--   0        0        0     1099 2024-02-10 16:20:47.134143 traceme-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      310 2024-02-10 16:20:36.182282 traceme-0.5.0/traceme/__init__.py
--rw-r--r--   0        0        0       22 2024-02-10 16:20:47.166142 traceme-0.5.0/traceme/_version.py
--rw-r--r--   0        0        0        0 2024-02-10 16:20:36.182282 traceme-0.5.0/traceme/py.typed
--rw-r--r--   0        0        0     8921 2024-02-10 16:20:36.182282 traceme-0.5.0/traceme/traceme.py
--rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 traceme-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-25 16:20:47.091556 traceme-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2395 2024-05-25 16:20:47.091556 traceme-0.6.0/README.md
+-rw-r--r--   0        0        0     1099 2024-05-25 16:20:55.019610 traceme-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      343 2024-05-25 16:20:47.095556 traceme-0.6.0/traceme/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-25 16:20:55.055611 traceme-0.6.0/traceme/_version.py
+-rw-r--r--   0        0        0        0 2024-05-25 16:20:47.095556 traceme-0.6.0/traceme/py.typed
+-rw-r--r--   0        0        0    10007 2024-05-25 16:20:47.095556 traceme-0.6.0/traceme/traceme.py
+-rw-r--r--   0        0        0     2933 1970-01-01 00:00:00.000000 traceme-0.6.0/PKG-INFO
```

### Comparing `traceme-0.5.0/LICENSE` & `traceme-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `traceme-0.5.0/pyproject.toml` & `traceme-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "traceme"
-version = "0.5.0"
+version = "0.6.0"
 description = "Python debug and tracer library"
 authors = ["Dag Brattli <dag@brattli.net>", "Cristina Ferrer Teixidor <cris.ferrer22@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "^13.7.0"
 structlog = "^24.1.0"
 colorama = "^0.4.6"
 
 [tool.poetry.group.dev.dependencies]
 dunamai = "^1.19.0"
-pre-commit = "^3.6.0"
-pytest = "^7.4.4"
+pre-commit = "^3.7.1"
+pytest = "^8.2.1"
 
 [tool.pyright]
 reportMissingImports = false
 typeCheckingMode = "strict"
 include = ["traceme", "tests"]
 
 [tool.ruff]
```

### Comparing `traceme-0.5.0/traceme/traceme.py` & `traceme-0.6.0/traceme/traceme.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import threading
-from collections.abc import Callable
+from collections.abc import Callable, Iterable
 from datetime import datetime, timedelta
-from enum import IntEnum
+from enum import Enum, IntEnum
 from types import TracebackType
 from typing import Any, ParamSpec, TypeVar, overload
 
 import colorama
 import structlog
 from structlog.processors import CallsiteParameter
 from structlog.typing import EventDict, WrappedLogger
@@ -33,15 +33,14 @@
 class TraceContext:
     def __init__(
         self,
         name: str,
         *args: Any,
         log_level: int = logging.INFO,
         log_exit: bool = False,
-        timeit: bool = False,
         **kwargs: Any,
     ):
         self.name = name
         self.args = args
         self.kwargs = kwargs
         self.log_exit = log_exit
         self.start: datetime | None = None
@@ -63,23 +62,23 @@
     def __exit__(
         self, exctype: type[BaseException] | None, excinst: BaseException | None, exctb: TracebackType | None
     ) -> None:
         """Exit and reset indentation."""
         _indentation.indentation -= 4
         elapsed = datetime.now() - self.start if self.start else None
 
-        match self.log_exit, excinst:
-            case True, None:
-                logger.log(event=self.name, level=self.log_level, direction=Direction.EXIT, elapsed=elapsed)
-            case True, exn:
-                logger.log(
-                    event=self.name, level=self.log_level, exc_info=exn, direction=Direction.EXIT, elapsed=elapsed
-                )
+        # If an exception was raised and it has not been logged before, log it
+        exc_seen = excinst and hasattr(excinst, "_traceme")
+        match self.log_exit, excinst, exc_seen:
+            case True, exn, False:
+                # Mark the exception as logged so we don't log it again in outer scopes
+                setattr(excinst, "_traceme", True)
+                logger.exception(event=self.name, exc_info=exn, direction=Direction.EXIT, elapsed=elapsed)
             case _:
-                pass
+                logger.log(event=self.name, level=self.log_level, direction=Direction.EXIT, elapsed=elapsed)
 
 
 def _trace(log_level: int = logging.INFO) -> Callable[..., Any]:
     def _trace(
         *args: Any,
         **kwargs: Any,
     ) -> Any:
@@ -105,55 +104,49 @@
             case _:
                 return decorator(func_or_string)
 
     return _trace
 
 
 @overload
-def info(func: Callable[_P, _T]) -> Callable[_P, _T]:
-    ...
+def info(func: Callable[_P, _T]) -> Callable[_P, _T]: ...
 
 
 @overload
-def info(log_exit: bool = False) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]:
-    ...
+def info(log_exit: bool = False) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]: ...
 
 
 def info(
     *args: Any,
     **kwargs: Any,
 ) -> Any:
     return _trace(log_level=logging.INFO)(*args, **kwargs)
 
 
 @overload
-def debug(func: Callable[_P, _T]) -> Callable[_P, _T]:
-    ...
+def debug(func: Callable[_P, _T]) -> Callable[_P, _T]: ...
 
 
 @overload
-def debug(log_exit: bool = False) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]:
-    ...
+def debug(log_exit: bool = False) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]: ...
 
 
 def debug(
     *args: Any,
     **kwargs: Any,
 ) -> Any:
     return _trace(log_level=logging.DEBUG)(*args, **kwargs)
 
 
 @overload
-def error(func: Callable[_P, _T]) -> Callable[_P, _T]:
-    ...
+def error(func: Callable[_P, _T]) -> Callable[_P, _T]: ...
 
 
 @overload
-def error(log_exit: bool = False) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]:
-    ...
+def error(log_exit: bool = False) -> Callable[[Callable[_P, _T]], Callable[_P, _T]]: ...
 
 
 def error(
     *args: Any,
     **kwargs: Any,
 ) -> Any:
     return _trace(log_level=logging.ERROR)(*args, **kwargs)
@@ -181,14 +174,25 @@
 # https://www.structlog.org/en/stable/processors.html
 def indentation_processor(logger: WrappedLogger, method_name: str, event_dict: EventDict) -> EventDict:
     """A structlog processor that uses the TraceContext."""
     event_dict["indentation"] = _indentation.indentation
     return event_dict
 
 
+def production_processor(logger: WrappedLogger, method_name: str, event_dict: EventDict) -> EventDict:
+    """A structlog processor that uses the TraceContext.
+
+    Removes tracme specific keys from the event_dict.
+    """
+    keys = ["indentation", "direction", "elapsed", "args", "kwargs"]
+    for key in keys:
+        event_dict.pop(key, None)
+    return event_dict
+
+
 class IndentationFormatter:
     def __init__(self, style: str = "") -> None:
         self.color = style or colorama.Fore.LIGHTBLACK_EX
 
     def __call__(self, key: str, value: Any) -> str:
         return f"{self.color}{'│   ' * (value // 4)}│"
 
@@ -289,31 +293,53 @@
             reset_style=colorama.Style.RESET_ALL,
             value_repr=str,
         ),
     ),
 ]
 
 
-def configure() -> None:
+class Environment(Enum):
+    PRODUCTION = 1
+    DEVELOPMENT = 2
+
+
+develoment_processors = [
+    structlog.processors.TimeStamper(fmt="iso"),
+    structlog.processors.add_log_level,
+    indentation_processor,
+    structlog.processors.CallsiteParameterAdder(
+        parameters=[CallsiteParameter.MODULE],
+        additional_ignores=[__name__],
+    ),
+    structlog.dev.ConsoleRenderer(
+        columns=columns, exception_formatter=structlog.dev.RichTracebackFormatter(suppress=["traceme"])
+    ),
+]
+
+production_processors = [
+    structlog.processors.TimeStamper(fmt="iso"),
+    structlog.processors.add_log_level,
+    production_processor,
+    structlog.processors.JSONRenderer(),
+]
+
+
+def configure(environment: Environment = Environment.DEVELOPMENT, processors: Iterable[Any] | None = None) -> None:
     structlog.configure(
-        processors=[
-            structlog.processors.TimeStamper(fmt="iso"),
-            structlog.processors.add_log_level,
-            indentation_processor,
-            structlog.processors.CallsiteParameterAdder(
-                parameters=[CallsiteParameter.MODULE],
-                additional_ignores=[__name__],
-            ),
-            structlog.dev.ConsoleRenderer(columns=columns),
-        ]
+        processors=processors
+        if processors
+        else develoment_processors
+        if environment == Environment.DEVELOPMENT
+        else production_processors
     )
 
 
 __all__ = [
     "info",
     "debug",
     "error",
     "configure",
     "columns",
     "indentation_column",
     "direction_column",
+    "Environment",
 ]
```

