# Comparing `tmp/misc_python_utils-0.1.8.tar.gz` & `tmp/misc_python_utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misc_python_utils-0.1.8.tar", max compression
+gzip compressed data, was "misc_python_utils-0.1.9.tar", max compression
```

## Comparing `misc_python_utils-0.1.8.tar` & `misc_python_utils-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1073 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/LICENSE
--rw-r--r--   0        0        0      973 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/README.md
--rw-r--r--   0        0        0       73 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/__init__.py
--rw-r--r--   0        0        0     1599 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/base64_utils.py
--rw-r--r--   0        0        0     5617 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/beartypes.py
--rw-r--r--   0        0        0       73 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/__init__.py
--rw-r--r--   0        0        0     3606 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/buildable.py
--rw-r--r--   0        0        0     1301 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/buildable_container.py
--rw-r--r--   0        0        0     4937 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/buildable_data.py
--rw-r--r--   0        0        0       33 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/readme.md
--rw-r--r--   0        0        0     1469 2024-04-11 10:25:51.538156 misc_python_utils-0.1.8/misc_python_utils/colored_logs_formatter.py
--rw-r--r--   0        0        0     1008 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/command_line_styling.py
--rw-r--r--   0        0        0     1256 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/dataclass_utils.py
--rw-r--r--   0        0        0     1628 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/dict_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/error_handling/__init__.py
--rw-r--r--   0        0        0     3311 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/error_handling/as_result_logged.py
--rw-r--r--   0        0        0     3924 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/error_handling/exception_as_err.py
--rw-r--r--   0        0        0      217 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/error_handling/readme.md
--rw-r--r--   0        0        0        0 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/file_utils/__init__.py
--rw-r--r--   0        0        0     3339 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/file_utils/download_extract_files.py
--rw-r--r--   0        0        0     2882 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/file_utils/readwrite_csv_files.py
--rw-r--r--   0        0        0     4205 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/file_utils/readwrite_files.py
--rw-r--r--   0        0        0     1371 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/file_utils/tarfile_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/gitrepo_utils/__init__.py
--rw-r--r--   0        0        0     1845 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/gitrepo_utils/git_repo_content.py
--rw-r--r--   0        0        0     4060 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/gitrepo_utils/git_repo_state.py
--rw-r--r--   0        0        0        0 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/hashcached_data/__init__.py
--rw-r--r--   0        0        0     6309 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/hashcached_data/hashcached_data.py
--rw-r--r--   0        0        0     2493 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/hashcached_data/hashcached_data_specific.py
--rw-r--r--   0        0        0        0 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/__init__.py
--rw-r--r--   0        0        0     5048 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py
--rw-r--r--   0        0        0     7603 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/flowchart_from_code.py
--rw-r--r--   0        0        0     1753 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/markdown_table_utils.py
--rw-r--r--   0        0        0     1114 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/mermaid_dag.py
--rw-r--r--   0        0        0     3355 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/mermaid_data_models.py
--rw-r--r--   0        0        0     1545 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py
--rw-r--r--   0        0        0     2204 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/prefix_suffix.py
--rw-r--r--   0        0        0        0 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/processing_utils/__init__.py
--rw-r--r--   0        0        0     1969 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/processing_utils/processing_utils.py
--rw-r--r--   0        0        0     2232 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/processing_utils/threadpool_with_backpressure.py
--rw-r--r--   0        0        0        0 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/text_processing/__init__.py
--rw-r--r--   0        0        0     2336 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/text_processing/diffmatchpatch_html.py
--rw-r--r--   0        0        0     3638 2024-04-11 10:25:51.542156 misc_python_utils-0.1.8/misc_python_utils/utils.py
--rw-r--r--   0        0        0      839 2024-04-11 10:26:03.010218 misc_python_utils-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 misc_python_utils-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/LICENSE
+-rw-r--r--   0        0        0      973 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/README.md
+-rw-r--r--   0        0        0       73 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/__init__.py
+-rw-r--r--   0        0        0     1599 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/base64_utils.py
+-rw-r--r--   0        0        0     5614 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/beartypes.py
+-rw-r--r--   0        0        0       73 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/__init__.py
+-rw-r--r--   0        0        0     3636 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/buildable.py
+-rw-r--r--   0        0        0     1301 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/buildable_container.py
+-rw-r--r--   0        0        0     4956 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/buildable_data.py
+-rw-r--r--   0        0        0       33 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/readme.md
+-rw-r--r--   0        0        0     1931 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/colored_logs_formatter.py
+-rw-r--r--   0        0        0     1008 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/command_line_styling.py
+-rw-r--r--   0        0        0     3768 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/dataclass_utils.py
+-rw-r--r--   0        0        0     1628 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/dict_utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/error_handling/__init__.py
+-rw-r--r--   0        0        0     3310 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/error_handling/as_result_logged.py
+-rw-r--r--   0        0        0     4791 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/error_handling/exception_as_err.py
+-rw-r--r--   0        0        0      217 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/error_handling/readme.md
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:02.811123 misc_python_utils-0.1.9/misc_python_utils/file_utils/__init__.py
+-rw-r--r--   0        0        0     3498 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/file_utils/download_extract_files.py
+-rw-r--r--   0        0        0     2882 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/file_utils/readwrite_csv_files.py
+-rw-r--r--   0        0        0     4133 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/file_utils/readwrite_files.py
+-rw-r--r--   0        0        0     1371 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/file_utils/tarfile_utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/gitrepo_utils/__init__.py
+-rw-r--r--   0        0        0     1845 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/gitrepo_utils/git_repo_content.py
+-rw-r--r--   0        0        0     4060 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/gitrepo_utils/git_repo_state.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/hashcached_data/__init__.py
+-rw-r--r--   0        0        0     6309 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/hashcached_data/hashcached_data.py
+-rw-r--r--   0        0        0     2493 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/hashcached_data/hashcached_data_specific.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/__init__.py
+-rw-r--r--   0        0        0     5048 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py
+-rw-r--r--   0        0        0     7603 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/flowchart_from_code.py
+-rw-r--r--   0        0        0     1753 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/markdown_table_utils.py
+-rw-r--r--   0        0        0     1114 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/mermaid_dag.py
+-rw-r--r--   0        0        0     3355 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/mermaid_data_models.py
+-rw-r--r--   0        0        0     1545 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py
+-rw-r--r--   0        0        0     2242 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/prefix_suffix.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/processing_utils/__init__.py
+-rw-r--r--   0        0        0     1969 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/processing_utils/processing_utils.py
+-rw-r--r--   0        0        0     2232 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/processing_utils/threadpool_with_backpressure.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/text_processing/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/text_processing/diffmatchpatch_html.py
+-rw-r--r--   0        0        0     3802 2024-04-24 11:58:02.815123 misc_python_utils-0.1.9/misc_python_utils/utils.py
+-rw-r--r--   0        0        0      839 2024-04-24 11:58:14.955322 misc_python_utils-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1726 1970-01-01 00:00:00.000000 misc_python_utils-0.1.9/PKG-INFO
```

### Comparing `misc_python_utils-0.1.8/LICENSE` & `misc_python_utils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/README.md` & `misc_python_utils-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/base64_utils.py` & `misc_python_utils-0.1.9/misc_python_utils/base64_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/beartypes.py` & `misc_python_utils-0.1.9/misc_python_utils/beartypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,24 +58,25 @@
 ExistingFile = File  # TODO: rename
 Directory = Annotated[str, Is[lambda f: Path(f).is_dir()]]
 # -------------------------------------------------------------------------------------
 # ----              NUMPY TYPES
 # -------------------------------------------------------------------------------------
 
 NDIM = "ndim"
+is_1_dimensional = IsAttr[NDIM, IsEqual[1]]
+
 try:  # noqa: WPS229
     # TODO: looks somewhat ugly!
     from numpy import float32, floating, int16, int32, number
     from numpy.typing import NDArray
 
     firstdim_nonempty = lambda x: x.shape[0] > 0
     seconddim_nonempty = lambda x: x.shape[1] > 0
 
     # 1 Dimensional
-    is_1_dimensional = IsAttr[NDIM, IsEqual[1]]
     NpNumberDim1 = Annotated[NDArray[number], is_1_dimensional]
     NeNpNumberDim1 = Annotated[NpNumberDim1, Is[firstdim_nonempty]]
 
     NpFloatDim1 = Annotated[NDArray[floating], is_1_dimensional]
     NpFloat32Dim1 = Annotated[NDArray[float32], is_1_dimensional]
     NpInt16Dim1 = Annotated[NDArray[int16], is_1_dimensional]
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/buildable.py` & `misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/buildable.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import logging
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from dataclasses import dataclass, fields
 from time import time
 from typing import ClassVar, Generic, TypeVar, final
 
-from misc_python_utils.dataclass_utils import all_undefined_must_be_filled
+from misc_python_utils.dataclass_utils import (
+    MaybeEnforcedSlots,
+    all_undefined_must_be_filled,
+)
 
 logger = logging.getLogger(
     __name__,
 )  # "The name is potentially a period-separated hierarchical", see: https://docs.python.org/3.10/library/logging.html
 
 
 class GotWasBuilt(ABC):
@@ -21,15 +24,14 @@
     def _was_built(self) -> bool:
         ...
 
 
 TBuildable = TypeVar("TBuildable", bound="Buildable")
 
 
-@dataclass(slots=True)
 class BuildableBehavior(ABC, Generic[TBuildable]):
     @classmethod
     @abstractmethod
     def it_is_ready(cls, obj: TBuildable) -> bool:
         ...
 
     @classmethod
@@ -46,15 +48,15 @@
         pass
 
 
 NamedChild = namedtuple("NamedChild", "name child")  # noqa: PYI024
 
 
 @dataclass(kw_only=True)
-class Buildable:
+class Buildable(MaybeEnforcedSlots):
     """
     base-class for "buildable Dataclasses"
 
     key-idea: a Dataclass has fields (attributes) those can be interpreted as "dependencies"
         in order to "build" a Dataclass it is necessary to first build all ites dependencies (=children)
 
     the build-method essentially does 2 things:
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/buildable_container.py` & `misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/buildable_container.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/buildable_dataclasses/buildable_data.py` & `misc_python_utils-0.1.9/misc_python_utils/buildable_dataclasses/buildable_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Iterator
 from dataclasses import asdict, dataclass, field
 from pathlib import Path
-from typing import Annotated, Any, ClassVar, TypeVar
+from typing import Annotated, ClassVar, TypeVar
 
 from beartype.vale import Is
 from slugify import slugify
 
 from misc_python_utils.beartypes import NeStr
 from misc_python_utils.buildable_dataclasses.buildable import (
     Buildable,
@@ -36,14 +36,15 @@
 
 
 CasedSlugStr = Annotated[NeStr, Is[lambda s: is_cased_sluggy(s)]]
 
 TBuildableData = TypeVar("TBuildableData", bound="BuildableData")
 
 
+@dataclass(slots=True)
 class DataBuilder(BuildableBehavior[TBuildableData]):
     @classmethod
     def it_is_ready(cls, obj: TBuildableData) -> bool:
         return obj._is_data_valid  # noqa: SLF001
 
     @classmethod
     def build_it(cls, obj: TBuildableData) -> None:
@@ -141,15 +142,15 @@
     def _is_data_valid(self) -> bool:
         return Path(self.jsonl_file).is_file()
 
     @abstractmethod
     def _generate_dataclasses(self) -> Iterator[SomeDataclass]:
         raise NotImplementedError
 
-    def _build_data(self) -> Any:
+    def _build_data(self) -> None:
         Path(self.data_dir).mkdir(parents=True, exist_ok=True)
         write_jsonl(
             self.jsonl_file,
             (
                 dc.to_dict() if hasattr(dc, "to_dict") else asdict(dc)
                 for dc in self._generate_dataclasses()
             ),
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/colored_logs_formatter.py` & `misc_python_utils-0.1.9/misc_python_utils/colored_logs_formatter.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,19 +27,29 @@
 
     def format(self, record: logging.LogRecord) -> str:  # noqa: A003
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
 
-def prepare_logger(namespaces: str | list[str], log_level: int = logging.DEBUG) -> None:
-    if isinstance(namespaces, str):
-        namespaces = [namespaces]
+def prepare_logger(
+    namespaces: str | list[str] | None = None,
+    log_level: int = logging.DEBUG,
+    namespaces2loglevel: dict[tuple[str, ...] | str, int] = None,  # noqa: RUF013
+) -> None:
+    if namespaces2loglevel is None:
+        if isinstance(namespaces, str):
+            namespaces2loglevel = {(namespaces,): log_level}
+        elif isinstance(namespaces, list):
+            namespaces2loglevel = {tuple(namespaces): log_level}
 
     ch = logging.StreamHandler()
     ch.setFormatter(CustomFormatter())
     root_logger = logging.getLogger()
     root_logger.handlers.clear()
     root_logger.addHandler(ch)
-    for ns in namespaces:
-        logger = logging.getLogger(ns)
-        logger.setLevel(log_level)
+    for logger_names, log_level in namespaces2loglevel.items():
+        if isinstance(logger_names, str):
+            logger_names = (logger_names,)  # noqa: PLW2901
+        for ns in logger_names:
+            logger = logging.getLogger(ns)
+            logger.setLevel(log_level)
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/command_line_styling.py` & `misc_python_utils-0.1.9/misc_python_utils/command_line_styling.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/dict_utils.py` & `misc_python_utils-0.1.9/misc_python_utils/dict_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/error_handling/as_result_logged.py` & `misc_python_utils-0.1.9/misc_python_utils/error_handling/as_result_logged.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def as_result_logged(
     *exceptions: type[TBE],
     panic_exceptions: set[type[BaseException]] | None = None,
 ) -> Callable[[Callable[P, R]], Callable[P, Result[R, TBE]]]:
     """
     key-idea: results as_result is not working with beartype and not logging errors!
-     -> instead of silenctly catching exceptions, we log them!
+     -> instead of silently catching exceptions, we log them!
     based on: https://github.com/rustedpy/result/blob/021d9945f9cad12eb49386691d933c6688ac89a9/src/result/result.py#L439
     :exceptions: exceptions to catch and turn into ``Err(exc)``.
     :panic_exceptions: exceptions to catch and re-raise.
     Make a decorator to turn a function into one that returns a ``Result``.
 
     Regular return values are turned into ``Ok(return_value)``. Raised
     exceptions of the specified exception type(s) are turned into ``Err(exc)``.
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/file_utils/download_extract_files.py` & `misc_python_utils-0.1.9/misc_python_utils/file_utils/download_extract_files.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,110 +1,114 @@
 import os
-import re
+import re  # noqa: F401
 from collections.abc import Callable
+from pathlib import Path
 
 from misc_python_utils.beartypes import Directory
 from misc_python_utils.processing_utils.processing_utils import exec_command
 
 
-def download_data(
+def download_and_extract(
     base_url: str,
     file_name: str,
     data_dir: Directory,
     verbose: bool = False,
-    unzip_it: bool = False,
-    do_raise: bool = True,
     remove_zipped: bool = False,
 ) -> str | None:
-    url = base_url + "/" + file_name
-    file = data_dir + "/" + file_name
+    """
+    formerly called "download_data"
+    """
+    file = data_dir + "/" + file_name  # noqa: F841
+
+    suffixes = [".zip", ".ZIP", ".tar.gz", ".tgz", ".gz", ".GZ", ".tar", ".TAR"]
+    regex = r"|".join([f"(?:{s})" for s in suffixes])
+    extract_folder = re.sub(regex, "", file)
+    assert extract_folder != file
+
+    if not Path(extract_folder).is_dir():
+        wget_file(base_url + "/" + file_name, data_dir, verbose)
+        Path(extract_folder).mkdir(exist_ok=True)
+        extract_file(file, extract_folder, get_build_extract_command_fun(file))
+        if remove_zipped:
+            Path(file).unlink()
+    return extract_folder
 
-    try:
-        if unzip_it:
-            suffixes = [".zip", ".ZIP", ".tar.gz", ".tgz", ".gz", ".GZ", ".tar", ".TAR"]
-            regex = r"|".join([f"(?:{s})" for s in suffixes])
-            extract_folder = re.sub(regex, "", file)
-            assert extract_folder != file
-
-            if not os.path.isdir(extract_folder):
-                wget_file(url, data_dir, verbose)
-                os.makedirs(extract_folder, exist_ok=True)
-                extract_file(file, extract_folder, get_build_extract_command_fun(file))
-                if remove_zipped:
-                    os.remove(file)
-            return extract_folder
-        elif not os.path.isfile(file):
-            wget_file(url, data_dir, verbose)
-    except FileNotFoundError as e:
-        if do_raise:
-            raise e
 
-
-def get_build_extract_command_fun(file: str):
+def get_build_extract_command_fun(file: str) -> Callable:  # noqa: C901,WPS231
     if any(file.endswith(suf) for suf in [".zip", ".ZIP"]):
 
-        def fun(dirr, file):
+        def fun(dirr, file):  # noqa: ANN001, ANN202
             return f"unzip -d {dirr} {file}"
 
     elif any(file.endswith(suf) for suf in [".tar.gz", ".tgz"]):
 
-        def fun(dirr, file):
+        def fun(dirr, file):  # noqa: ANN001, ANN202
             return f"tar xzf {file} -C {dirr}"
 
     elif any(file.endswith(suf) for suf in [".tar", ".TAR"]):
 
-        def fun(dirr, file):
+        def fun(dirr, file):  # noqa: ANN001, ANN202
             return f"tar xf {file} -C {dirr}"
 
     elif any(file.endswith(suf) for suf in [".gz", ".GZ"]):
 
-        def fun(dirr, file):
+        def fun(dirr, file):  # noqa: ANN001, ANN202
             return f"gzip -dc {file} {dirr}"
 
     else:
         raise NotImplementedError
     return fun
 
 
-def extract_file(file, extract_folder, build_extract_command_fun: Callable):
+def extract_file(
+    file: str,
+    extract_folder: str,
+    build_extract_command_fun: Callable,
+) -> None:
     cmd = build_extract_command_fun(extract_folder, file)
     _, stderr = exec_command(cmd)
     assert len(stderr) == 0, f"{cmd=}: {stderr=}"
 
 
-def wget_file(
+def wget_file(  # noqa: PLR0913
     url: str,
     data_folder: str,
-    verbose=False,
+    verbose: bool = False,
     file_name: str | None = None,
     user: str | None = None,
     password: str | None = None,
-):
+) -> None:
     # TODO(tilo): wget.download cannot continue ??
     passw = f" --password {password} " if password is not None else ""
     user = f' --user "{user}" ' if user is not None else ""
     quiet = " -q " if not verbose else ""
     if file_name is None:
         file_name = url.split("/")[-1]
     file = f"{data_folder}/{file_name}"
-    os.makedirs(data_folder, exist_ok=True)
-    if os.path.isfile(file):
+    os.makedirs(data_folder, exist_ok=True)  # noqa: PTH103
+    if Path(file).is_file():  # noqa: PTH113
         cmd = f'wget -O {file} -c -N{quiet}{passw}{user} -P {data_folder} "{url}"'
     else:
         cmd = f'wget -O {file} -c {quiet}{passw}{user} -P {data_folder} "{url}"'
 
-    print(f"{cmd=}")
-    os.system(cmd)
+    print(f"{cmd=}")  # noqa: T201
+    os.system(cmd)  # noqa: S605
     # TODO: why is subprocess not working?
     # download_output = exec_command(cmd)
     # if err_code != 0:
     #     raise FileNotFoundError(f"could not download {url}")
 
 
-def main():
-    file_name = "/test-other.tar.gz"
-    base_url = "http://www.openslr.org/resources/12"
-    download_data(base_url, file_name, "/tmp/test_data", unzip_it=True, verbose=True)
+# def main():  # noqa: ANN201
+#     file_name = "/test-other.tar.gz"
+#     base_url = "http://www.openslr.org/resources/12"
+#     download_data(
+#         base_url,
+#         file_name,
+#         "/tmp/test_data",  # noqa: S108
+#         unzip_it=True,
+#         verbose=True,  # noqa: S108, COM812
+#     )  # noqa: S108
 
 
-if __name__ == "__main__":
-    main()
+# if __name__ == "__main__":
+#     main()
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/file_utils/readwrite_csv_files.py` & `misc_python_utils-0.1.9/misc_python_utils/file_utils/readwrite_csv_files.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/file_utils/readwrite_files.py` & `misc_python_utils-0.1.9/misc_python_utils/file_utils/readwrite_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import bz2
 import gzip
 import json
 import locale
 from collections.abc import Iterable, Iterator
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Literal
+from typing import Any
 
 assert locale.getpreferredencoding(False) == "UTF-8"
 
 FilePath = str | Path
 
 
 def write_jsonl(
     file: FilePath,
     data: Iterable[dict | (list | tuple)],
-    mode: Literal["w", "a"] = "w",
+    mode: str = "w",  # str
     do_flush: bool = False,
 ) -> None:
     file = str(file)
 
     def process_line(d: dict) -> str | bytes:
         line = json.dumps(d, skipkeys=True, ensure_ascii=False)
         line = line + "\n"
@@ -30,15 +30,15 @@
         if do_flush:
             f.flush()
 
 
 def write_json(
     file: FilePath,
     datum: dict,
-    mode: Literal["w", "a"] = "w",
+    mode: str = "w",
     do_flush: bool = False,
     indent: int | None = None,  # use indent =4 for "pretty json"
 ) -> None:
     file = str(file)
     with writable(file, mode) as f:
         line = json.dumps(datum, skipkeys=True, ensure_ascii=False, indent=indent)
         line = line.encode("utf-8")
@@ -46,15 +46,15 @@
         if do_flush:
             f.flush()
 
 
 def write_file(
     file: FilePath,
     s: str,
-    mode: Literal["w", "a"] = "w",
+    mode: str = "w",
     do_flush: bool = False,
 ) -> None:
     file = str(file)
     with writable(file, mode) as f:
         f.write(s.encode("utf-8"))
         if do_flush:
             f.flush()
@@ -70,30 +70,30 @@
     with file_io_supplier() as f:
         return f.read()
 
 
 def write_lines(
     file: FilePath,
     lines: Iterable[str],
-    mode: Literal["w", "a"] = "w",
+    mode: str = "w",
 ) -> None:
     file = str(file)
 
     def process_line(line: str) -> str | bytes:
         line = line + "\n"
         return line.encode("utf-8")
 
     with writable(file, mode) as f:
         f.writelines(process_line(l) for l in lines)
 
 
 @contextmanager
 def writable(  # noqa: ANN201
     file: str,
-    mode: Literal["w", "a"] = "w",
+    mode: str = "w",
 ):  # python 3.10 does not like this type-hint (it works for 3.12): Iterator[TextIO | gzip.GzipFile]
     mode += "b"
     if file.endswith(".gz"):
         with open(file, mode=mode) as f:  # noqa: SIM117, PTH123
             # exlcuding timestamp from gzip, see: https://stackoverflow.com/questions/25728472/python-gzip-omit-the-original-filename-and-timestamp
 
             with gzip.GzipFile(fileobj=f, mode=mode, filename="", mtime=0) as fgz:
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/file_utils/tarfile_utils.py` & `misc_python_utils-0.1.9/misc_python_utils/file_utils/tarfile_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/gitrepo_utils/git_repo_content.py` & `misc_python_utils-0.1.9/misc_python_utils/gitrepo_utils/git_repo_content.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/gitrepo_utils/git_repo_state.py` & `misc_python_utils-0.1.9/misc_python_utils/gitrepo_utils/git_repo_state.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/hashcached_data/hashcached_data.py` & `misc_python_utils-0.1.9/misc_python_utils/hashcached_data/hashcached_data.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/hashcached_data/hashcached_data_specific.py` & `misc_python_utils-0.1.9/misc_python_utils/hashcached_data/hashcached_data_specific.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py` & `misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/_mermaid_markdown_from_nested_dataclasses.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/flowchart_from_code.py` & `misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/flowchart_from_code.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/markdown_table_utils.py` & `misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/markdown_table_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/mermaid_dag.py` & `misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/mermaid_dag.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/mermaid_data_models.py` & `misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/mermaid_data_models.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py` & `misc_python_utils-0.1.9/misc_python_utils/mermaid_utils/mermaid_markdown_diagrams.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/prefix_suffix.py` & `misc_python_utils-0.1.9/misc_python_utils/prefix_suffix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import dataclasses
 from dataclasses import dataclass
 from typing import Any, ClassVar, TypeVar
 
+from typing_extensions import Self
+
 from misc_python_utils.buildable_dataclasses.buildable import Buildable
 from misc_python_utils.dataclass_utils import UNDEFINED, Undefined
 
 TPrefixSuffix = TypeVar("TPrefixSuffix", bound="PrefixSuffix")
 BASE_PATHES: dict[str, str | TPrefixSuffix] = {}
 BASE_PATHES[
     "pwd"
 ] = "."  # noqa: S105 -> this is a false-positive! pwd does not stand for "password" but the "current path"
 
 
-@dataclass
+@dataclass(slots=True)
 class PrefixSuffix(Buildable):
     prefix_key: str | Undefined = UNDEFINED
     suffix: str | Undefined = UNDEFINED
 
     prefix: str = dataclasses.field(init=False)
     __exclude_from_hash__: ClassVar[list[str]] = ["prefix"]
 
@@ -49,14 +51,14 @@
             repr_ = this_is_only_used_for_hashing
         return repr_
 
     def _set_prefix(self) -> None:
         self.prefix = BASE_PATHES[self.prefix_key]
         # assert len(self.prefix) > 0, f"base_path is empty!"
 
-    def from_str_same_prefix(self, path: str) -> "PrefixSuffix":
+    def from_str_same_prefix(self, path: str) -> Self:
         assert str(path).startswith(self.prefix)
         file_suffix = str(path).replace(f"{self.prefix}/", "")
         return PrefixSuffix(self.prefix_key, file_suffix)
 
     def __hash__(self):
         return hash(repr(self))
```

### Comparing `misc_python_utils-0.1.8/misc_python_utils/processing_utils/processing_utils.py` & `misc_python_utils-0.1.9/misc_python_utils/processing_utils/processing_utils.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/processing_utils/threadpool_with_backpressure.py` & `misc_python_utils-0.1.9/misc_python_utils/processing_utils/threadpool_with_backpressure.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/text_processing/diffmatchpatch_html.py` & `misc_python_utils-0.1.9/misc_python_utils/text_processing/diffmatchpatch_html.py`

 * *Files identical despite different names*

### Comparing `misc_python_utils-0.1.8/misc_python_utils/utils.py` & `misc_python_utils-0.1.9/misc_python_utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -114,14 +114,22 @@
         if fail_return_message_builder is not None:
             out = fail_return_message_builder(error=e, sys_stderr=sys.stderr)
         else:
             out = default
     return out
 
 
+TIn = TypeVar("TIn")
+TOut = TypeVar("TOut")
+
+
+def maybe(val: TIn | None, fun: Callable[[TIn], TOut]) -> TOut | None:
+    return None if val is None else fun(val)
+
+
 def slugify_with_underscores(s: str) -> str:
     regex_pattern_to_allow_underscores = r"[^-a-z0-9_]+"
     return slugify(s, regex_pattern=regex_pattern_to_allow_underscores)
 
 
 def slugify_en_olny(s: str) -> str:
     return slugify(s, regex_pattern=r"[^-a-z0-9]+")
```

### Comparing `misc_python_utils-0.1.8/pyproject.toml` & `misc_python_utils-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "misc-python-utils"
-version = "0.1.8" # see: https://pypi.org/project/poetry-dynamic-versioning/
+version = "0.1.9" # see: https://pypi.org/project/poetry-dynamic-versioning/
 description = ""
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 repository = "https://github.com/dertilo/misc-python-utils"
 
 readme = "README.md"
 packages = [{ include = "misc_python_utils" }]
```

### Comparing `misc_python_utils-0.1.8/PKG-INFO` & `misc_python_utils-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misc-python-utils
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/dertilo/misc-python-utils
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

