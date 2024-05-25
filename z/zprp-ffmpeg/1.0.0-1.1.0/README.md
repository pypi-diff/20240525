# Comparing `tmp/zprp_ffmpeg-1.0.0.tar.gz` & `tmp/zprp_ffmpeg-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zprp_ffmpeg-1.0.0.tar", max compression
+gzip compressed data, was "zprp_ffmpeg-1.1.0.tar", max compression
```

## Comparing `zprp_ffmpeg-1.0.0.tar` & `zprp_ffmpeg-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,14 @@
--rw-r--r--   0        0        0       83 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/AUTHORS.rst
--rw-r--r--   0        0        0     1088 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/LICENSE
--rw-r--r--   0        0        0     4266 2024-05-10 14:32:43.968463 zprp_ffmpeg-1.0.0/README.rst
--rw-r--r--   0        0        0     1831 2024-05-10 14:32:43.968463 zprp_ffmpeg-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      638 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/BaseConnector.py
--rw-r--r--   0        0        0     3528 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/FilterGraph.py
--rw-r--r--   0        0        0     1389 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/ProcessConnector.py
--rw-r--r--   0        0        0      402 2024-05-10 14:32:43.968463 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/__init__.py
--rw-r--r--   0        0        0      392 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/__main__.py
--rw-r--r--   0        0        0     1023 2024-05-10 14:14:20.248797 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/_api_compat.py
--rw-r--r--   0        0        0     1812 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/_zprp_ffmpeg.c
--rw-r--r--   0        0        0      826 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/cli.py
--rw-r--r--   0        0        0      153 2024-04-10 16:02:25.189086 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/filters.py
--rw-r--r--   0        0        0     3680 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/generated_filters.py
--rw-r--r--   0        0        0        0 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/py.typed
--rw-r--r--   0        0        0     4966 1970-01-01 00:00:00.000000 zprp_ffmpeg-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.1.0/AUTHORS.rst
+-rw-r--r--   0        0        0     1088 2024-03-19 10:18:25.914851 zprp_ffmpeg-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4266 2024-05-25 15:58:32.615756 zprp_ffmpeg-1.1.0/README.rst
+-rw-r--r--   0        0        0     1873 2024-05-25 15:58:32.615756 zprp_ffmpeg-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      720 2024-05-20 20:33:29.596366 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/BaseConnector.py
+-rw-r--r--   0        0        0     3595 2024-05-25 15:27:33.619583 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/FilterGraph.py
+-rw-r--r--   0        0        0     1389 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/ProcessConnector.py
+-rw-r--r--   0        0        0      782 2024-05-25 15:58:32.615756 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/__init__.py
+-rw-r--r--   0        0        0     1028 2024-05-20 20:33:29.596366 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/_api_compat.py
+-rw-r--r--   0        0        0      153 2024-05-25 10:16:46.165449 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/filters.py
+-rw-r--r--   0        0        0   473018 2024-05-25 15:57:22.575778 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/generated_filters.py
+-rw-r--r--   0        0        0      907 2024-05-25 15:57:22.575778 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/probe.py
+-rw-r--r--   0        0        0        0 2024-05-10 14:12:06.788837 zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/py.typed
+-rw-r--r--   0        0        0     4966 1970-01-01 00:00:00.000000 zprp_ffmpeg-1.1.0/PKG-INFO
```

### Comparing `zprp_ffmpeg-1.0.0/LICENSE` & `zprp_ffmpeg-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-1.0.0/README.rst` & `zprp_ffmpeg-1.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/zprp-ffmpeg
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/zprp-ffmpeg.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/zprp-ffmpeg
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v1.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v1.1.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v1.0.0...main
+    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v1.1.0...main
 
 
 
 .. end-badges
 
 Implementation of the successor to the ffmpeg-python library
```

### Comparing `zprp_ffmpeg-1.0.0/pyproject.toml` & `zprp_ffmpeg-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zprp-ffmpeg"
-version = "1.0.0"
+version = "1.1.0"
 description = "ffmpeg filter graph bindings for python"
 authors = ["Your Name <you@example.com>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -68,11 +68,11 @@
 [tool.ruff.lint.isort]
 forced-separate = ["conftest"]
 force-single-line = true
 
 [tool.black]
 line-length = 140
 target-version = ["py38"]
-
+force-exclude = "tests.*"
 [tool.mypy]
 implicit_reexport = true
-exclude = ["src/filters_autogen/FFmpeg/*","src/filters_autogen/pycparser/*"]
+exclude = ["src/filters_autogen/FFmpeg/*","src/filters_autogen/pycparser/*", "tests/assets/"]
```

### Comparing `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/FilterGraph.py` & `zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/FilterGraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """There is no general 'Node' class, because it doesn't work well with object relations, source and sink filters are kind of orthogonal.
 It slightly violates DRY, but the parameter types are different. It is what it is"""
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any
+from typing import List
 from typing import Optional
 from typing import Union
 
 
 class FilterType(Enum):
     VIDEO = "AVMEDIA_TYPE_VIDEO"
     AUDIO = "AVMEDIA_TYPE_AUDIO"
@@ -18,45 +19,47 @@
     name: str
     value: Any
 
 
 class Filter:
     """Filters can have many inputs and many outputs, holds the filter name and potential params"""
 
-    def __init__(self, command: str, params: Optional[list[FilterOption]] = None, filter_type: FilterType = FilterType.VIDEO):
-        self._out: list[AnyNode] = []
-        self._in: list[AnyNode] = []
+    def __init__(self, command: str, params: Optional[List[FilterOption]] = None, filter_type: str = FilterType.VIDEO.value):
+        self._out: List[AnyNode] = []
+        self._in: List[AnyNode] = []
         self.command = command
         self.params = params if params else []
         self.filter_type = filter_type
 
     def add_output(self, parent: "Filter | SinkFilter"):
         self._out.append(parent)
 
     def add_input(self, child: "Filter | SourceFilter"):
         self._in.append(child)
 
     def get_command(self):
-        joined_params = ":".join(p.name + "=" + p.value for p in self.params if p.value)
+        joined_params = ":".join(p.name + "=" + str(p.value) for p in self.params if p.value)
         if joined_params:  # if there was no option, leave empty string
             joined_params = "=" + joined_params
         if self.filter_type == "AVMEDIA_TYPE_VIDEO":
             return "-vf " + self.command + joined_params
 
         elif self.filter_type == "AVMEDIA_TYPE_AUDIO":
             return "-af " + self.command + joined_params
 
+        return ""  # in case no match
+
 
 # names as per ffmpeg documentation
 class SourceFilter:
     """There can't be any input node to input filter, it provides the input itself."""
 
     def __init__(self, in_path: str):
         self.in_path: str = in_path
-        self._out: list[AnyNode] = []
+        self._out: List[AnyNode] = []
 
     def add_output(self, parent: "Filter | SinkFilter"):
         self._out.append(parent)
 
     def add_input(self, child: "Filter"):
         raise NotImplementedError("This node can't have inputs")
 
@@ -65,15 +68,15 @@
 
 
 class SinkFilter:
     """Similarly to SourceFilter, it doesn't make sense to output anything further, this is the end of graph."""
 
     def __init__(self, out_path: str):
         self.out_path: str = out_path
-        self._in: list[AnyNode] = []
+        self._in: List[AnyNode] = []
 
     def add_input(self, parent: "Filter | SourceFilter"):
         self._in.append(parent)
 
     def add_output(self, parent: "Filter"):
         raise NotImplementedError("This node can't have outputs")
 
@@ -88,15 +91,15 @@
 
 
 class Stream:
     """One directional sequence of nodes, in future will be able to visualize them.
     Streams can be concatenated and split with certain filters."""
 
     def __init__(self) -> None:
-        self._nodes: list[AnyNode] = []
+        self._nodes: List[AnyNode] = []
 
     def append(self, node: AnyNode) -> "Stream":
         if len(self._nodes) > 0:
             # connect head with new node
             if not isinstance(self._nodes[-1], SinkFilter) and not isinstance(node, SourceFilter):
                 self._nodes[-1].add_output(node)
                 node.add_input(self._nodes[-1])
```

### Comparing `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/ProcessConnector.py` & `zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/ProcessConnector.py`

 * *Files identical despite different names*

### Comparing `zprp_ffmpeg-1.0.0/src/zprp_ffmpeg/_api_compat.py` & `zprp_ffmpeg-1.1.0/src/zprp_ffmpeg/_api_compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def output(stream: Stream, filename: str):
     sink = SinkFilter(filename)
     stream.append(sink)
     return stream
 
 
 # this api always uses process
-def run(stream: Stream, extra_options: str) -> Tuple[str, str]:
+def run(stream: Stream, extra_options: str = "") -> Tuple[str, str]:
     """Returns (stdout,stderr) tuple"""
     return ProcessConnector.run(stream, extra_options).communicate()
 
 
 # this api always uses process
 def run_async(stream: Stream) -> BaseConnector:
     """Returns handle to a process. Can raise an exception if script tries to terminate before ffmpeg is done."""
```

### Comparing `zprp_ffmpeg-1.0.0/PKG-INFO` & `zprp_ffmpeg-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zprp-ffmpeg
-Version: 1.0.0
+Version: 1.1.0
 Summary: ffmpeg filter graph bindings for python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -102,17 +102,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/zprp-ffmpeg
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/zprp-ffmpeg.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/zprp-ffmpeg
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v1.0.0.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/ffmpeg-zprp/zprp-ffmpeg/v1.1.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v1.0.0...main
+    :target: https://github.com/ffmpeg-zprp/zprp-ffmpeg/compare/v1.1.0...main
 
 
 
 .. end-badges
 
 Implementation of the successor to the ffmpeg-python library
```

