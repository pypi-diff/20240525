# Comparing `tmp/thread-2.0.1.tar.gz` & `tmp/thread-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thread-2.0.1.tar", max compression
+gzip compressed data, was "thread-2.0.2.tar", max compression
```

## Comparing `thread-2.0.1.tar` & `thread-2.0.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0     1496 2024-04-28 08:08:00.664454 thread-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     4657 2024-04-28 08:08:00.664454 thread-2.0.1/README.md
--rw-r--r--   0        0        0     1625 2024-04-28 08:08:00.664454 thread-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      657 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/__init__.py
--rw-r--r--   0        0        0      139 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/__main__.py
--rw-r--r--   0        0        0     1522 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/_types.py
--rw-r--r--   0        0        0      272 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/cli.py
--rw-r--r--   0        0        0       93 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/decorators/__init__.py
--rw-r--r--   0        0        0     4846 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/decorators/_processor.py
--rw-r--r--   0        0        0     3889 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/decorators/_threaded.py
--rw-r--r--   0        0        0     2196 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/py.typed
--rw-r--r--   0        0        0    22008 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/thread.py
--rw-r--r--   0        0        0      123 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/utils/__init__.py
--rw-r--r--   0        0        0     1385 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/utils/algorithm.py
--rw-r--r--   0        0        0     4527 2024-04-28 08:08:00.664454 thread-2.0.1/src/thread/utils/config.py
--rw-r--r--   0        0        0       61 2024-04-28 08:08:00.668455 thread-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0     1232 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_algorithm.py
--rw-r--r--   0        0        0     1816 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_concurrentprocessing.py
--rw-r--r--   0        0        0     9467 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_dataframe_compatibility.py
--rw-r--r--   0        0        0     2114 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_decorator.py
--rw-r--r--   0        0        0     3405 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_thread.py
--rw-r--r--   0        0        0     1480 2024-04-28 08:08:00.668455 thread-2.0.1/tests/test_verbosity.py
--rw-r--r--   0        0        0     6043 1970-01-01 00:00:00.000000 thread-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-05-25 13:15:28.335379 thread-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     4657 2024-05-25 13:15:28.335379 thread-2.0.2/README.md
+-rw-r--r--   0        0        0     1685 2024-05-25 13:15:28.335379 thread-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      675 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/__main__.py
+-rw-r--r--   0        0        0       33 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/__version__.py
+-rw-r--r--   0        0        0     1470 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/_types.py
+-rw-r--r--   0        0        0      272 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/cli.py
+-rw-r--r--   0        0        0       93 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/decorators/__init__.py
+-rw-r--r--   0        0        0     4794 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/decorators/_processor.py
+-rw-r--r--   0        0        0     3837 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/decorators/_threaded.py
+-rw-r--r--   0        0        0     2144 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/py.typed
+-rw-r--r--   0        0        0    21956 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/thread.py
+-rw-r--r--   0        0        0      123 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/algorithm.py
+-rw-r--r--   0        0        0     4586 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/config.py
+-rw-r--r--   0        0        0      183 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/utils/meta.py
+-rw-r--r--   0        0        0      101 2024-05-25 13:15:28.335379 thread-2.0.2/src/thread/version.py
+-rw-r--r--   0        0        0       61 2024-05-25 13:15:28.335379 thread-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0      280 2024-05-25 13:15:28.335379 thread-2.0.2/tests/library/test_version.py
+-rw-r--r--   0        0        0     1232 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_algorithm.py
+-rw-r--r--   0        0        0     1816 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_concurrentprocessing.py
+-rw-r--r--   0        0        0     9467 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_dataframe_compatibility.py
+-rw-r--r--   0        0        0     2114 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_decorator.py
+-rw-r--r--   0        0        0     3405 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_thread.py
+-rw-r--r--   0        0        0     1480 2024-05-25 13:15:28.335379 thread-2.0.2/tests/test_verbosity.py
+-rw-r--r--   0        0        0     6111 1970-01-01 00:00:00.000000 thread-2.0.2/PKG-INFO
```

### Comparing `thread-2.0.1/LICENSE.txt` & `thread-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/README.md` & `thread-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/pyproject.toml` & `thread-2.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thread"
-version = "2.0.1"
+version = "2.0.2"
 description = "Threading module extension"
 authors = ["Alex <contact@ngjx.org>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 packages = [
   { include = "thread", from = "src" },
   { include = "thread/py.typed", from = "src" },
@@ -26,27 +26,27 @@
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: Implementation :: CPython",
   "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 Homepage = "https://thread.ngjx.org"
-Documentation = "https://thread.ngjx.org/docs/v2.0.1"
+Documentation = "https://thread.ngjx.org/docs/v2.0.2"
 Source = "https://github.com/python-thread/thread"
 Download = "https://pypi.org/project/thread/#files"
 "Release Notes" = "https://github.com/python-thread/thread/releases"
 "Bug Tracker" = "https://github.com/python-thread/thread/issues"
 
 [tool.poetry.scripts]
 thread = "thread.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typing-extensions = "^4.9.0"
-
+importlib-metadata = { version = ">=4.4", python = "<3.10" }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 ruff = "^0.1.5"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `thread-2.0.1/src/thread/__init__.py` & `thread-2.0.2/src/thread/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 ## Thread Library
-Documentation at https://thread.ngjx.org/docs/2.0.1
+Documentation at https://thread.ngjx.org/docs/2.0.2
 
 
 ---
 
 Released under the BSD-3 License
 
 Copyright (c) thread.ngjx.org, All rights reserved
@@ -13,33 +13,28 @@
 """
 This file contains the exports to
 ```py
 import thread
 ```
 """
 
+from .version import __version__
 
-__version__ = '2.0.1'
-
-
-# Export Core
-from .thread import Thread, ConcurrentProcessing
-
-
-from . import _types as types, exceptions
-
+from . import _types as types
+from . import exceptions
 
 # Export decorators
-from .decorators import threaded, processor
+from .decorators import processor, threaded
 
+# Export Core
+from .thread import ConcurrentProcessing, Thread
 
 # Configuration
 from .utils import Settings
 
-
 # Wildcard Export
 __all__ = [
     'Thread',
     'ConcurrentProcessing',
     'threaded',
     'processor',
     'types',
```

### Comparing `thread-2.0.1/src/thread/_types.py` & `thread-2.0.2/src/thread/_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 ## Types
-
-Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 from typing import Any, Literal, Callable, Union, Sized
 from typing_extensions import (
     ParamSpec,
     TypeVar,
     Concatenate,
```

### Comparing `thread-2.0.1/src/thread/decorators/_processor.py` & `thread-2.0.2/src/thread/decorators/_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 ## Processor
-
-Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 from functools import wraps
 from ..thread import ConcurrentProcessing
 
 from .._types import (
     Overflow_In,
```

### Comparing `thread-2.0.1/src/thread/decorators/_threaded.py` & `thread-2.0.2/src/thread/decorators/_threaded.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 ## Threaded
-
-Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 from functools import wraps
 from ..thread import Thread
 
 from .._types import Overflow_In, Data_In
 from typing import Callable, Mapping, Sequence, Optional, Union, overload
```

### Comparing `thread-2.0.1/src/thread/exceptions.py` & `thread-2.0.2/src/thread/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """
 ## Thread Exceptions
-
-Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 import traceback
 from typing import Any, Optional, Sequence, Tuple
 
 
 class ErrorBase(Exception):
```

### Comparing `thread-2.0.1/src/thread/thread.py` & `thread-2.0.2/src/thread/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 ```py
 class Thread: ...
 
 
 class ConcurrentProcessing: ...
 ```
-
-Documentation: https://thread.ngjx.org/docs/v2.0.1
 """
 
 import sys
 import time
 import ctypes
 import signal
 import threading
```

### Comparing `thread-2.0.1/src/thread/utils/algorithm.py` & `thread-2.0.2/src/thread/utils/algorithm.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/src/thread/utils/config.py` & `thread-2.0.2/src/thread/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Literal, Union
+from typing import Any, Callable, Literal, Union, cast
 
 _Verbosity_Num = Literal[0, 1, 2]
 _Verbosity_Enum = Literal['quiet', 'normal', 'verbose']
 VerbosityLevel = Union[_Verbosity_Num, _Verbosity_Enum]
 VerbosityMapping: dict[_Verbosity_Enum, _Verbosity_Num] = {
     'quiet': 0,
     'normal': 1,
@@ -75,14 +75,15 @@
     ) -> bool:
         if isinstance(other, Verbosity):
             return operator(self.level_number, other.level_number)
         if isinstance(other, int):
             return operator(self.level_number, other)
         if isinstance(other, str):
             if Verbosity.is_valid_level(other):
+                other = cast(_Verbosity_Enum, other)
                 return operator(self.level_number, VerbosityMapping[other])
             return operator(self.level_string, other)
         raise ValueError('Cannot compare Verbosity with other types')
 
     @staticmethod
     def is_valid_level(level: Any) -> bool:
         """
```

### Comparing `thread-2.0.1/tests/test_algorithm.py` & `thread-2.0.2/tests/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/tests/test_concurrentprocessing.py` & `thread-2.0.2/tests/test_concurrentprocessing.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/tests/test_dataframe_compatibility.py` & `thread-2.0.2/tests/test_dataframe_compatibility.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/tests/test_decorator.py` & `thread-2.0.2/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/tests/test_thread.py` & `thread-2.0.2/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/tests/test_verbosity.py` & `thread-2.0.2/tests/test_verbosity.py`

 * *Files identical despite different names*

### Comparing `thread-2.0.1/PKG-INFO` & `thread-2.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thread
-Version: 2.0.1
+Version: 2.0.2
 Summary: Threading module extension
 License: BSD-3-Clause
 Keywords: thread,threading,extension,multiprocessing
 Author: Alex
 Author-email: contact@ngjx.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,17 +17,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
+Requires-Dist: importlib-metadata (>=4.4) ; python_version < "3.10"
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.1
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.2
 Project-URL: Download, https://pypi.org/project/thread/#files
 Project-URL: Homepage, https://thread.ngjx.org
 Project-URL: Release Notes, https://github.com/python-thread/thread/releases
 Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
 
 <a name="readme-top"></a>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: thread Version: 2.0.1 Summary: Threading module
+Metadata-Version: 2.1 Name: thread Version: 2.0.2 Summary: Threading module
 extension License: BSD-3-Clause Keywords:
 thread,threading,extension,multiprocessing Author: Alex Author-email:
 contact@ngjx.org Requires-Python: >=3.9,<4.0 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: BSD License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: Implementation :: CPython Classifier: Topic :: Software Development
-Classifier: Typing :: Typed Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
+Classifier: Typing :: Typed Requires-Dist: importlib-metadata (>=4.4) ;
+python_version < "3.10" Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/python-thread/thread/issues
-Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.1 Project-URL:
+Project-URL: Documentation, https://thread.ngjx.org/docs/v2.0.2 Project-URL:
 Download, https://pypi.org/project/thread/#files Project-URL: Homepage, https:/
 /thread.ngjx.org Project-URL: Release Notes, https://github.com/python-thread/
 thread/releases Project-URL: Source, https://github.com/python-thread/thread
 Description-Content-Type: text/markdown
  _[_!_[_P_Y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_v_e_r_s_i_o_n_-_s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_P_Y_P_I_ _-_ _D_o_w_n_l_o_a_d_s_]_[_d_o_w_n_l_o_a_d_s_-
  _s_h_i_e_l_d_]_]_[_p_y_p_i_-_u_r_l_] _[_!_[_F_o_r_k_s_]_[_f_o_r_k_s_-_s_h_i_e_l_d_]_]_[_f_o_r_k_s_-_u_r_l_] _[_!_[_S_t_a_r_g_a_z_e_r_s_]_[_s_t_a_r_s_-
   _s_h_i_e_l_d_]_]_[_s_t_a_r_s_-_u_r_l_] _[_!_[_B_S_D_-_3_-_C_l_a_u_s_e_ _L_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_-_s_h_i_e_l_d_]_]_[_l_i_c_e_n_s_e_-_u_r_l_]
```

