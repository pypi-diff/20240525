# Comparing `tmp/labtech-0.5.1.tar.gz` & `tmp/labtech-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labtech-0.5.1.tar", max compression
+gzip compressed data, was "labtech-0.6.0.tar", max compression
```

## Comparing `labtech-0.5.1.tar` & `labtech-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    35149 2023-09-13 02:58:38.522441 labtech-0.5.1/LICENSE
--rw-r--r--   0        0        0     6074 2024-04-05 07:15:21.269246 labtech-0.5.1/README.md
--rw-r--r--   0        0        0      706 2024-04-05 07:21:09.988779 labtech-0.5.1/labtech/__init__.py
--rw-r--r--   0        0        0     6688 2024-04-03 08:01:09.692172 labtech-0.5.1/labtech/cache.py
--rw-r--r--   0        0        0     6914 2024-04-05 07:20:35.553228 labtech-0.5.1/labtech/diagram.py
--rw-r--r--   0        0        0      741 2023-09-13 02:58:38.538441 labtech-0.5.1/labtech/exceptions.py
--rw-r--r--   0        0        0     1396 2024-04-03 08:25:57.589634 labtech-0.5.1/labtech/executors.py
--rw-r--r--   0        0        0    22346 2024-04-03 08:01:09.692172 labtech-0.5.1/labtech/lab.py
--rw-r--r--   0        0        0     4059 2024-04-03 08:27:41.813199 labtech-0.5.1/labtech/mypy_plugin.py
--rw-r--r--   0        0        0        0 2024-02-13 05:01:34.041748 labtech-0.5.1/labtech/py.typed
--rw-r--r--   0        0        0     4630 2024-02-06 01:46:44.484931 labtech-0.5.1/labtech/serialization.py
--rw-r--r--   0        0        0     2455 2024-03-31 09:09:14.445769 labtech-0.5.1/labtech/storage.py
--rw-r--r--   0        0        0     9763 2024-04-03 08:01:09.696173 labtech-0.5.1/labtech/tasks.py
--rw-r--r--   0        0        0     5230 2024-04-03 08:41:02.359333 labtech-0.5.1/labtech/types.py
--rw-r--r--   0        0        0     3090 2024-02-06 01:43:13.057829 labtech-0.5.1/labtech/utils.py
--rw-r--r--   0        0        0     1025 2024-04-05 07:21:16.020700 labtech-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     7025 1970-01-01 00:00:00.000000 labtech-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-13 02:58:38.522441 labtech-0.6.0/LICENSE
+-rw-r--r--   0        0        0     6474 2024-05-25 00:11:51.894250 labtech-0.6.0/README.md
+-rw-r--r--   0        0        0      706 2024-05-25 00:14:23.811136 labtech-0.6.0/labtech/__init__.py
+-rw-r--r--   0        0        0     6688 2024-05-25 00:11:51.938250 labtech-0.6.0/labtech/cache.py
+-rw-r--r--   0        0        0     6932 2024-05-25 00:11:51.938250 labtech-0.6.0/labtech/diagram.py
+-rw-r--r--   0        0        0      741 2023-09-13 02:58:38.538441 labtech-0.6.0/labtech/exceptions.py
+-rw-r--r--   0        0        0     1396 2024-05-25 00:11:51.938250 labtech-0.6.0/labtech/executors.py
+-rw-r--r--   0        0        0    26887 2024-05-25 00:13:19.894525 labtech-0.6.0/labtech/lab.py
+-rw-r--r--   0        0        0     7293 2024-05-25 00:13:19.894525 labtech-0.6.0/labtech/monitor.py
+-rw-r--r--   0        0        0     4038 2024-05-25 00:11:51.938250 labtech-0.6.0/labtech/mypy_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-13 05:01:34.041748 labtech-0.6.0/labtech/py.typed
+-rw-r--r--   0        0        0     4630 2024-05-25 00:11:51.938250 labtech-0.6.0/labtech/serialization.py
+-rw-r--r--   0        0        0     3358 2024-05-25 00:13:33.198627 labtech-0.6.0/labtech/storage.py
+-rw-r--r--   0        0        0    10014 2024-05-25 00:11:51.938250 labtech-0.6.0/labtech/tasks.py
+-rw-r--r--   0        0        0     5322 2024-05-25 00:11:51.942250 labtech-0.6.0/labtech/types.py
+-rw-r--r--   0        0        0     3196 2024-05-25 00:11:51.942250 labtech-0.6.0/labtech/utils.py
+-rw-r--r--   0        0        0     1442 2024-05-25 00:13:59.442869 labtech-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7464 1970-01-01 00:00:00.000000 labtech-0.6.0/PKG-INFO
```

### Comparing `labtech-0.5.1/LICENSE` & `labtech-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `labtech-0.5.1/README.md` & `labtech-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 <div align="center">
 
+<img alt="Labtech logo - FIFO the Labrador in a lab coat and goggles working on a laptop with the labtech 'lt' icon." src="https://ben-denham.github.io/labtech/images/fifo.svg">
+
 <h1>labtech</h1>
 
 <a href="">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/labtech">
 </a>
 
 <p>
@@ -35,14 +37,15 @@
 ```
 pip install labtech
 ```
 
 
 ## Usage
 
+<!-- N.B. keep this code in-sync with tests/integration/readme/usage.py -->
 ```python
 from time import sleep
 
 import labtech
 
 # Decorate your task class with @labtech.task:
 @labtech.task
@@ -84,30 +87,30 @@
 if __name__ == '__main__':
     main()
 ```
 
 ![Animated GIF of labtech demo on the command-line](https://ben-denham.github.io/labtech/images/labtech-demo.gif)
 
 Labtech can also produce graphical progress bars in
-[Jupyter](https://jupyter.org/) when the `Lab` is initialized with
-`notebook=True`:
+[Jupyter](https://jupyter.org/) notebooks:
 
 ![Animated GIF of labtech demo in Jupyter](https://ben-denham.github.io/labtech/images/labtech-demo-jupyter.gif)
 
 Tasks parameters can be any of the following types:
 
 * Simple scalar types: `str`, `bool`, `float`, `int`, `None`
 * Collections of any of these types: `list`, `tuple`, `dict`, `Enum`
 * Task types: A task parameter is a "nested task" that will be
   executed before its parent so that it may make use of the nested
   result.
 
 Here's an example of defining a single long-running task to produce a
 result for a large number of dependent tasks:
 
+<!-- N.B. keep this code in-sync with tests/integration/readme/dependents_and_mermaid.py -->
 ```python
 from time import sleep
 
 import labtech
 
 @labtech.task
 class SlowTask:
@@ -142,14 +145,15 @@
 if __name__ == '__main__':
     main()
 ```
 
 Labtech can even generate a [Mermaid diagram](https://mermaid.js.org/syntax/classDiagram.html)
 to visualise your tasks:
 
+<!-- N.B. keep this code in-sync with tests/integration/readme/dependents_and_mermaid.py -->
 ```python
 from labtech.diagram import display_task_diagram
 
 some_slow_task = SlowTask(base=42)
 dependent_tasks = [
     DependentTask(
         slow_task=some_slow_task,
```

### Comparing `labtech-0.5.1/labtech/__init__.py` & `labtech-0.6.0/labtech/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 results = lab.run_tasks(experiments)
 print(results)
 
 ```
 
 """
 
-__version__ = '0.5.1'
+__version__ = '0.6.0'
 
-from .types import is_task, is_task_type
-from .tasks import task
 from .lab import Lab
+from .tasks import task
+from .types import is_task, is_task_type
 from .utils import logger
 
 __all__ = [
     'is_task_type',
     'is_task',
     'task',
     'Lab',
```

### Comparing `labtech-0.5.1/labtech/cache.py` & `labtech-0.6.0/labtech/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Cache classes that control formatting of task results in storage."""
 
 
-from abc import abstractmethod
-from datetime import datetime, timedelta
 import hashlib
 import json
 import pickle
+from abc import abstractmethod
+from datetime import datetime, timedelta
 from typing import Any, Optional, Type
 
 from . import __version__ as labtech_version
-from .types import Task, TaskT, ResultT, ResultMeta, TaskResult, Cache, Storage
 from .exceptions import CacheError, TaskNotFound
 from .serialization import Serializer
+from .types import Cache, ResultMeta, ResultT, Storage, Task, TaskResult, TaskT
 
 
 class NullCache(Cache):
     """Cache that never stores results in the storage provider."""
 
     def cache_key(self, task: Task) -> str:
         return 'null'
```

### Comparing `labtech-0.5.1/labtech/diagram.py` & `labtech-0.6.0/labtech/diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass, fields
 from textwrap import indent
-from typing import Dict, Sequence, Type, get_origin, get_args, get_type_hints
+from typing import Dict, Sequence, Type, get_args, get_origin, get_type_hints
 
-from .types import Task, is_task
 from .tasks import find_tasks_in_param
+from .types import Task, is_task
+from .utils import is_ipython
 
 
 @dataclass(frozen=True)
 class TaskRelKey:
     from_param_name: str
     to_task_type: Type[Task]
 
@@ -182,13 +183,12 @@
     diagram tasks that you trust.
 
     Accepts the same arguments as
     [build_task_diagram][labtech.diagram.build_task_diagram].
 
     """
     diagram = build_task_diagram(tasks, **kwargs)
-    try:
-        from IPython.display import display, Markdown
-    except ImportError:
-        print(diagram)
-    else:
+    if is_ipython():
+        from IPython.display import Markdown, display
         display(Markdown(f'```mermaid\n{diagram}\n```'))
+    else:
+        print(diagram)
```

### Comparing `labtech-0.5.1/labtech/exceptions.py` & `labtech-0.6.0/labtech/exceptions.py`

 * *Files identical despite different names*

### Comparing `labtech-0.5.1/labtech/executors.py` & `labtech-0.6.0/labtech/executors.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from concurrent.futures import Executor, Future, FIRST_COMPLETED, wait
+from concurrent.futures import FIRST_COMPLETED, Executor, Future, wait
 from typing import Callable, Sequence
 
 
 class SerialFuture(Future):
 
     def __init__(self, fn: Callable, /, *args, **kwargs):
         super().__init__()
```

### Comparing `labtech-0.5.1/labtech/lab.py` & `labtech-0.6.0/labtech/lab.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,61 @@
 """Lab and related utilities responsible for running tasks."""
 
-from collections import Counter, defaultdict
 import concurrent.futures
 import concurrent.futures.process
+import logging
+import math
+import multiprocessing
+import signal
+import sys
+from collections import Counter, defaultdict
 from contextlib import contextmanager
 from dataclasses import fields
 from datetime import datetime
 from enum import Enum
-import logging
 from logging.handlers import QueueHandler
-import math
-import multiprocessing
 from pathlib import Path
-import signal
-import sys
+from queue import Queue
 from threading import Thread
-from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Type, Union
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Set, Type, Union, cast
 
 from frozendict import frozendict
 from tqdm import tqdm
-from tqdm.notebook import tqdm as tqdm_notebook
 from tqdm.contrib.logging import logging_redirect_tqdm
+from tqdm.notebook import tqdm as tqdm_notebook
 
-from .types import Task, TaskT, ResultT, ResultMeta, ResultsMap, TaskResult, Storage, is_task
-from .tasks import find_tasks_in_param
 from .exceptions import LabError, TaskNotFound
-from .utils import OrderedSet, LoggerFileProxy, logger
-from .storage import NullStorage, LocalStorage
 from .executors import SerialExecutor, wait_for_first_future
+from .monitor import TaskEndEvent, TaskMonitor, TaskStartEvent
+from .storage import LocalStorage, NullStorage
+from .tasks import find_tasks_in_param
+from .types import ResultMeta, ResultsMap, ResultT, Storage, Task, TaskResult, TaskT, is_task, is_task_type
+from .utils import LoggerFileProxy, OrderedSet, is_ipython, logger
 
 _IN_TASK_SUBPROCESS = False
 
 
+def check_tasks(tasks: Sequence[Task]) -> None:
+    for task in tasks:
+        if not is_task(task):
+            raise LabError(
+                (f'`{repr(task)}` is not a task, please provide a task object '
+                 'made from a class decorated with @labtech.task.')
+            )
+
+
+def check_task_types(task_types: Sequence[Type[Task]]) -> None:
+    for task_type in task_types:
+        if not is_task_type(task_type):
+            raise LabError(
+                (f'`{repr(task_type)}` is not a task type, please provide a '
+                 'class decorated with @labtech.task.')
+            )
+
+
 @contextmanager
 def optional_mlflow(task: Task):
 
     def log_params(value: Any, *, path: str = ''):
         prefix = path if path == '' else f'{path}.'
         if is_task(value):
             for field in fields(value):
@@ -201,20 +221,26 @@
     sys.stdout = LoggerFileProxy(logger.info, 'Captured STDOUT:\n')
     sys.stderr = LoggerFileProxy(logger.error, 'Captured STDERR:\n')
 
 
 class TaskRunner:
 
     def __init__(self, lab: 'Lab', bust_cache: bool, keep_nested_results: bool,
-                 disable_progress: bool):
+                 disable_progress: bool, disable_top: bool, top_format: str,
+                 top_sort: str, top_n: int):
         self.lab = lab
         self.bust_cache = bust_cache
         self.keep_nested_results = keep_nested_results
         self.disable_progress = disable_progress
+        self.disable_top = disable_top
+        self.top_format = top_format
+        self.top_sort = top_sort
+        self.top_n = top_n
         self.log_queue = multiprocessing.Manager().Queue(-1)
+        self.task_monitor_queue: Optional[Queue] = None
 
     def get_executor(self, serial: bool = False):
         if (self.lab.max_workers is not None and self.lab.max_workers == 1):
             serial = True
 
         if serial:
             return SerialExecutor()
@@ -229,14 +255,15 @@
         pbar_func = tqdm_notebook if self.lab.notebook else tqdm
         return pbar_func(
             desc=task_type.__qualname__,
             unit='tasks',
             total=task_count,
             bar_format='{desc}: {n_fmt}/{total_fmt} [{elapsed}, {rate_fmt}{postfix}] |{bar}| {percentage:3.0f}% [{remaining} remaining]',
             disable=self.disable_progress,
+            dynamic_ncols=True,
         )
 
     def handle_failure(self, *, ex: Exception, message: str):
         # Simplify subprocess error tracebacks by reporting the cause directly.
         if isinstance(ex.__cause__, concurrent.futures.process._RemoteTraceback):
             ex = ex.__cause__
 
@@ -253,16 +280,24 @@
 
     def use_cache(self, task: Task) -> bool:
         return (not self.bust_cache) and self.lab.is_cached(task)
 
     def run_or_load_task(self, process_name: str, task: Task) -> TaskResult:
         orig_process_name = multiprocessing.current_process().name
         try:
-            multiprocessing.current_process().name = process_name
-            if self.use_cache(task):
+            current_process = multiprocessing.current_process()
+            current_process.name = process_name
+            use_cache = self.use_cache(task)
+            if self.task_monitor_queue is not None:
+                self.task_monitor_queue.put(TaskStartEvent(
+                    process_name=process_name,
+                    pid=cast(int, current_process.pid),
+                    use_cache=use_cache,
+                ))
+            if use_cache:
                 logger.debug(f"Loading from cache: '{task}'")
                 task_result = task._lt.cache.load_result_with_meta(self.lab._storage, task)
                 return task_result
             else:
                 logger.debug(f"Running: '{task}'")
                 task.set_context(self.lab.context)
                 with optional_mlflow(task):
@@ -276,15 +311,19 @@
                         duration=(end - start),
                     ),
                 )
                 task._lt.cache.save(self.lab._storage, task, task_result)
                 logger.debug(f"Completed: '{task}'")
                 return task_result
         finally:
-            multiprocessing.current_process().name = orig_process_name
+            current_process.name = orig_process_name
+            if self.task_monitor_queue is not None:
+                self.task_monitor_queue.put(TaskEndEvent(
+                    process_name=process_name,
+                ))
 
     def logger_thread(self):
         # See: https://docs.python.org/3/howto/logging-cookbook.html#logging-to-a-single-file-from-multiple-processes
         while True:
             record = self.log_queue.get()
             if record is None:
                 break
@@ -308,14 +347,28 @@
         pbars = {
             task_type: self.get_pbar(
                 task_type=task_type,
                 task_count=task_count,
             )
             for task_type, task_count in task_type_counts.items()
         }
+
+        task_monitor = None
+        if not self.disable_top:
+            self.task_monitor_queue = multiprocessing.Manager().Queue(-1)
+            task_monitor = TaskMonitor(
+                task_monitor_queue=self.task_monitor_queue,
+                top_format=self.top_format,
+                top_sort=self.top_sort,
+                top_n=self.top_n,
+                notebook=self.lab.notebook,
+            )
+            task_monitor.show()
+            task_monitor.start()
+
         executor = self.get_executor()
         serial_executor = self.get_executor(serial=True)
         future_to_task: Dict[concurrent.futures.Future, Task] = {}
         redirected_loggers = [] if self.lab.notebook else [logger]
         with logging_redirect_tqdm(loggers=redirected_loggers):
             try:
                 try:
@@ -366,14 +419,16 @@
                 for process in executor._processes.values():
                     process.terminate()
                 executor.shutdown(wait=False)
             finally:
                 for pbar in pbars.values():
                     pbar.close()
                 self.log_queue.put(None)
+                if task_monitor is not None:
+                    task_monitor.close()
                 log_thread.join()
 
             raise KeyboardInterrupt
 
 
 class Lab:
     """Primary interface for configuring, running, and getting results of tasks.
@@ -388,15 +443,15 @@
 
     """
 
     def __init__(self, *,
                  storage: Union[str, Path, None, Storage],
                  continue_on_failure: bool = True,
                  max_workers: Optional[int] = None,
-                 notebook: bool = False,
+                 notebook: Optional[bool] = None,
                  context: Optional[dict[str, Any]] = None):
         """
         Args:
             storage: Where task results should be cached to. A string or
                 [`Path`](https://docs.python.org/3/library/pathlib.html#pathlib.Path)
                 will be interpreted as the path to a local directory, `None`
                 will result in no caching. Any [Storage][labtech.types.Storage]
@@ -404,37 +459,42 @@
             continue_on_failure: If `True`, exceptions raised by tasks will be
                 logged, but execution of other tasks will continue.
             max_workers: The maximum number of parallel worker processes for
                 running tasks. Uses the same default as
                 `concurrent.futures.ProcessPoolExecutor`: the number of
                 processors on the machine. When `max_workers=1`, all tasks will
                 be run in the main process, without multi-processing.
-            notebook: Should be set to `True` if run from a Jupyter notebook
-                for graphical progress bars.
+            notebook: Determines whether to use notebook-friendly graphical
+                progress bars. When set to `None` (the default), labtech will
+                detect whether the code is being run from an IPython notebook.
             context: A dictionary of additional variables to make available to
                 tasks. The context will not be cached, so the values should not
                 affect results (e.g. parallelism factors) or should be kept
                 constant between runs (e.g. datasets).
         """
         if isinstance(storage, str) or isinstance(storage, Path):
             storage = LocalStorage(storage)
         elif storage is None:
             storage = NullStorage()
         self._storage = storage
         self.continue_on_failure = continue_on_failure
         self.max_workers = max_workers
-        self.notebook = notebook
+        self.notebook = is_ipython() if notebook is None else notebook
         if context is None:
             context = {}
         self.context = context
 
     def run_tasks(self, tasks: Sequence[TaskT], *,
                   bust_cache: bool = False,
                   keep_nested_results: bool = False,
-                  disable_progress: bool = False) -> Dict[TaskT, Any]:
+                  disable_progress: bool = False,
+                  disable_top: bool = False,
+                  top_format: str = '$name $status since $start_time CPU: $cpu MEM: $rss',
+                  top_sort: str = 'start_time',
+                  top_n: int = 10) -> Dict[TaskT, Any]:
         """Run the given tasks with as much process parallelism as possible.
         Loads task results from the cache storage where possible and
         caches results of executed tasks.
 
         Any attribute of a task that is itself a task object is
         considered a "nested task", and will be executed or loaded so
         that it's result is made available to its parent task. If the
@@ -451,24 +511,56 @@
             bust_cache: If `True`, no task results will be loaded from the
                 cache storage; all tasks will be re-executed.
             keep_nested_results: If `False`, results of nested tasks that were
                 executed or loaded in order to complete the provided tasks will
                 be cleared from memory once they are no longer needed.
             disable_progress: If `True`, do not display a tqdm progress bar
                 tracking task execution.
+            disable_top: If `True`, do not display the list of top active tasks.
+            top_format: Format for each top active task. Follows the format
+                rules for
+                [template strings](https://docs.python.org/3/library/string.html#template-strings)
+                and may include any of the following attributes for
+                substitution:
+
+                * `name`: The task's name displayed in logs.
+                * `pid`: The task's primary process id.
+                * `status`: Whether the task is being run or loaded from cache.
+                * `start_time`: The time the task's primary process started.
+                * `children`: The number of child tasks of the task's primary
+                  process.
+                * `threads`: The number of active CPU threads for the task
+                  (including across any child processes).
+                * `cpu`: The CPU percentage (1 core = 100%) being used by the
+                  task (including across any child processes).
+                * `rss`: The resident set size (RSS) memory percentage being
+                  used by the task (including across any child processes). RSS
+                  is the primary measure of memory usage.
+                * `vms`: The virtual memory size (VMS) percentage being used by
+                  the task (including across any child processes).
+            top_sort: Sort order for the top active tasks. Can be any of the
+                attributes available for use in `top_format`. If the string is
+                preceded by a `-`, the sort order will be reversed. Defaults to
+                showing oldest tasks first.
+            top_n: The maximum number of top active tasks to display.
 
         Returns:
             A dictionary mapping each of the provided tasks to its
                 corresponding result.
 
         """
+        check_tasks(tasks)
         runner = TaskRunner(self,
                             bust_cache=bust_cache,
                             keep_nested_results=keep_nested_results,
-                            disable_progress=disable_progress)
+                            disable_progress=disable_progress,
+                            disable_top=disable_top,
+                            top_format=top_format,
+                            top_sort=top_sort,
+                            top_n=top_n)
         results = runner.run(tasks)
         # Return results in the same order as tasks
         return {task: results[task] for task in tasks}
 
     def run_task(self, task: Task[ResultT], **kwargs) -> ResultT:
         """Run a single task and return its result. Supports the same keyword
         arguments as `run_tasks`.
@@ -490,14 +582,15 @@
 
         Does not load task results from the cache storage, but they
         can be loaded by calling
         [`run_tasks()`][labtech.Lab.run_tasks] with the returned task
         instances.
 
         """
+        check_task_types(task_types)
         keys = self._storage.find_keys()
         tasks = []
         for key in keys:
             for task_type in task_types:
                 try:
                     task = task_type._lt.cache.load_task(self._storage, task_type, key)
                 except TaskNotFound:
@@ -506,15 +599,17 @@
                     tasks.append(task)
                     break
         return tasks
 
     def is_cached(self, task: Task) -> bool:
         """Checks if a result is present for given task in the Lab's cache
         storage."""
+        check_tasks([task])
         return task._lt.cache.is_cached(self._storage, task)
 
     def uncache_tasks(self, tasks: Sequence[Task]):
         """Removes cached results for the given tasks from the Lab's cache
         storage."""
+        check_tasks(tasks)
         for task in tasks:
             if self.is_cached(task):
                 task._lt.cache.delete(self._storage, task)
```

### Comparing `labtech-0.5.1/labtech/mypy_plugin.py` & `labtech-0.6.0/labtech/mypy_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Mypy plugin for classes decorated with `labtech.task`."""
 
 from typing import Type
+
 import mypy.plugins.dataclasses
-from mypy.nodes import COVARIANT
-from mypy.plugin import Plugin, ClassDefContext
+from mypy.nodes import COVARIANT, ArgKind
+from mypy.plugin import ClassDefContext, Plugin
 from mypy.plugins.common import add_attribute_to_class
-from mypy.types import Instance, LiteralType, AnyType, TypeOfAny, TypeVarType, CallableType, NoneType, UnionType
-from mypy.nodes import ArgKind
+from mypy.types import AnyType, CallableType, Instance, LiteralType, NoneType, TypeOfAny, TypeVarType, UnionType
 
 task_makers = {'labtech.tasks.task'}
 """Set of decorator functions that return "task" classes."""
 
 
 def task_tag_callback(ctx: ClassDefContext):
     """Add attributes to a "task" class."""
```

### Comparing `labtech-0.5.1/labtech/serialization.py` & `labtech-0.6.0/labtech/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Serialization/deserialization of tasks to/from JSON."""
 
 from dataclasses import fields
 from enum import Enum
-from typing import cast, Dict, List, Optional, Type, Union
+from typing import Dict, List, Optional, Type, Union, cast
 
 from frozendict import frozendict
 
-from .types import Task, ResultMeta, is_task
 from .exceptions import SerializationError
+from .types import ResultMeta, Task, is_task
 from .utils import ensure_dict_key_str
 
 # Type to represent any value that can be handled by Python's default
 # json encoder and decoder.
 jsonable = Union[None, str, bool, float, int,
                  Dict[str, 'jsonable'], List['jsonable']]
```

### Comparing `labtech-0.5.1/labtech/tasks.py` & `labtech-0.6.0/labtech/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 """Utilities for defining tasks."""
 
 from dataclasses import dataclass, fields
 from enum import Enum
 from inspect import isclass
-from typing import cast, Any, Dict, Optional, Sequence, Set, Union
+from types import UnionType
+from typing import Any, Dict, Optional, Sequence, Set, TypeAlias, Union, cast
 
 from frozendict import frozendict
 
-from .types import Task, ResultT, TaskInfo, ResultMeta, ResultsMap, Cache, is_task_type, is_task
-from .cache import PickleCache, NullCache
+from .cache import NullCache, PickleCache
 from .exceptions import TaskError
+from .types import Cache, ResultMeta, ResultsMap, ResultT, Task, TaskInfo, is_task, is_task_type
 from .utils import ensure_dict_key_str
 
+ParamScalar: TypeAlias = None | str | bool | float | int | Enum
+
 
 class CacheDefault:
     pass
 
 
 CACHE_DEFAULT = CacheDefault()
 
 
+_RESERVED_ATTRS = [
+    '_lt', '_is_task', 'cache_key', 'result', '_results_map', '_set_results_map',
+    'result_meta', '_set_result_meta', 'context', 'set_context', '__post_init__',
+]
+"""Reserved attribute names for task types."""
+
+
 def immutable_param_value(key: str, value: Any) -> Any:
     """Converts a parameter value to an immutable equivalent that is hashable."""
     if isinstance(value, list) or isinstance(value, tuple):
-        return tuple(immutable_param_value(f'{key}.{i}', item) for i, item in enumerate(value))
+        return tuple(immutable_param_value(f'{key}[{i}]', item) for i, item in enumerate(value))
     if isinstance(value, dict) or isinstance(value, frozendict):
         return frozendict({
-            ensure_dict_key_str(dict_key, exception_type=TaskError): immutable_param_value(f'{key}.{dict_key}', dict_value)
+            ensure_dict_key_str(dict_key, exception_type=TaskError): immutable_param_value(f'{key}["{dict_key}"]', dict_value)
             for dict_key, dict_value in value.items()
         })
-    is_scalar = (
-        (value is None)
-        or isinstance(value, str)
-        or isinstance(value, bool)
-        or isinstance(value, float)
-        or isinstance(value, int)
-        or isinstance(value, Enum)
-    )
+    is_scalar = isinstance(value, cast(UnionType, ParamScalar))
     if is_scalar or is_task(value):
         return value
     raise TaskError(f"Unsupported type '{type(value).__qualname__}' in parameter value '{key}'.")
 
 
 def _task_post_init(self: Task):
     # Ensure parameter values are immutable.
@@ -183,20 +186,16 @@
             mlflow logging calls from the task's `run()` method.
 
     """
 
     def decorator(cls):
         nonlocal cache
 
-        reserved_attrs = [
-            '_lt', '_is_task', 'cache_key', 'result', '_results_map', '_set_results_map',
-            'result_meta', '_set_result_meta', 'context', 'set_context',
-        ]
         if not is_task_type(cls):
-            for reserved_attr in reserved_attrs:
+            for reserved_attr in _RESERVED_ATTRS:
                 if hasattr(cls, reserved_attr):
                     raise AttributeError(f"Task type already defines reserved attribute '{reserved_attr}'.")
 
         post_init = getattr(cls, 'post_init', None)
         cls.__post_init__ = _task_post_init
 
         cls = dataclass(frozen=True, eq=True, order=True)(cls)
@@ -242,17 +241,22 @@
     elif isinstance(param_value, list) or isinstance(param_value, tuple):
         searched_coll_ids = searched_coll_ids | {id(param_value)}
         return [
             task
             for item in param_value
             for task in find_tasks_in_param(item, searched_coll_ids)
         ]
-    elif isinstance(param_value, dict):
+    elif isinstance(param_value, dict) or isinstance(param_value, frozendict):
         searched_coll_ids = searched_coll_ids | {id(param_value)}
         return [
             task
             # We only need to search the values, as all parameter
             # dictionary keys must be strings.
             for item in param_value.values()
             for task in find_tasks_in_param(item, searched_coll_ids)
         ]
-    return []
+    elif isinstance(param_value, cast(UnionType, ParamScalar)):
+        return []
+
+    # This should be impossible.
+    msg = f"Unexpected type {type(param_value).__qualname__} encountered in task parameter value."
+    raise TaskError(msg)
```

### Comparing `labtech-0.5.1/labtech/types.py` & `labtech-0.6.0/labtech/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 """Core types of labtech."""
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from inspect import isclass
 from typing import (
-    Any, Callable, Dict, Generic, IO, Literal,
-    Optional, Protocol, Sequence, Type, TypeVar,
+    IO,
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    Literal,
+    Optional,
+    Protocol,
+    Sequence,
+    Type,
+    TypeVar,
 )
 
 
 @dataclass(frozen=True)
 class TaskInfo:
     orig_post_init: Optional[Callable]
     cache: 'Cache'
@@ -82,20 +91,20 @@
 
 TaskT = TypeVar("TaskT", bound=Task)
 
 
 def is_task_type(cls):
     """Returns `True` if the given `cls` is a class decorated with
     [`labtech.task`][labtech.task]."""
-    return isclass(cls) and hasattr(cls, '_lt')
+    return isclass(cls) and isinstance(getattr(cls, '_lt', None), TaskInfo)
 
 
 def is_task(obj):
     """Returns `True` if the given `obj` is an instance of a task class."""
-    return hasattr(obj, '_is_task')
+    return is_task_type(type(obj)) and hasattr(obj, '_is_task')
 
 
 class Storage(ABC):
     """Storage provider for persisting cached task results."""
 
     @abstractmethod
     def find_keys(self) -> Sequence[str]:
```

### Comparing `labtech-0.5.1/labtech/utils.py` & `labtech-0.6.0/labtech/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """General labtech utilities."""
 
+import builtins
 import logging
 import re
-from typing import cast, Dict, Generic, Optional, Sequence, TypeVar, Type
+from typing import Dict, Generic, Optional, Sequence, Type, TypeVar, cast
 
 
 def get_logger():
     logger = logging.getLogger('labtech')
     default_logger_handler = logging.StreamHandler()
     logger.addHandler(default_logger_handler)
     default_logger_handler.setFormatter(logging.Formatter(
@@ -105,13 +106,18 @@
 def ensure_dict_key_str(value, *, exception_type: Type[Exception]) -> str:
     if not isinstance(value, str):
         raise exception_type(("Parameter dictionary keys must be strings, "
                               f"found: '{value}'"))
     return cast(str, value)
 
 
+def is_ipython() -> bool:
+    return hasattr(builtins, '__IPYTHON__')
+
+
 __all__ = [
     'logger',
     'OrderedSet',
     'LoggerFileProxy',
     'ensure_dict_key_str',
+    'is_ipython',
 ]
```

### Comparing `labtech-0.5.1/pyproject.toml` & `labtech-0.6.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labtech"
-version = "0.5.1"
+version = "0.6.0"
 license = "GPL-3.0-only"
 description = "Easily run experiment permutations with multi-processing and caching."
 authors = ["Ben Denham <ben@denham.nz>"]
 readme = "README.md"
 repository = "https://github.com/ben-denham/labtech"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -15,25 +15,46 @@
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 tqdm = "^4.66.2"
 frozendict = "^2.4.0"
+psutil = "^5.9.8"
 
-[tool.poetry.dev-dependencies]
-flake8 = "^5.0.4"
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.10.0"
 mkdocs = "^1.5.2"
 mkdocstrings-python = "^1.5.2"
 mkdocs-material = "^9.2.4"
 mypy = "^1.9.0"
 jupyterlab = "^4.1.5"
 IPython = "8.23.0"
 ipywidgets = "^8.1.2"
 mlflow = "^2.10.0"
+types-tqdm = "^4.66.0.20240417"
+ruff = "^0.4.1"
+types-psutil = "^5.9.5.20240516"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.mypy]
+plugins = ["labtech/mypy_plugin.py"]
+
+[[tool.mypy.overrides]]
+module="mlflow.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module="ipywidgets.*"
+ignore_missing_imports = true
+
+[tool.ruff]
+line-length = 160
+extend-exclude = ["tests/integration/readme/*.py"]
+
+[tool.ruff.lint]
+select = ["E", "F", "W", "I"]
```

### Comparing `labtech-0.5.1/PKG-INFO` & `labtech-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labtech
-Version: 0.5.1
+Version: 0.6.0
 Summary: Easily run experiment permutations with multi-processing and caching.
 Home-page: https://github.com/ben-denham/labtech
 License: GPL-3.0-only
 Author: Ben Denham
 Author-email: ben@denham.nz
 Requires-Python: >=3.10
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,20 +13,23 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: frozendict (>=2.4.0,<3.0.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/ben-denham/labtech
 Description-Content-Type: text/markdown
 
 <div align="center">
 
+<img alt="Labtech logo - FIFO the Labrador in a lab coat and goggles working on a laptop with the labtech 'lt' icon." src="https://ben-denham.github.io/labtech/images/fifo.svg">
+
 <h1>labtech</h1>
 
 <a href="">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/labtech">
 </a>
 
 <p>
@@ -58,14 +61,15 @@
 ```
 pip install labtech
 ```
 
 
 ## Usage
 
+<!-- N.B. keep this code in-sync with tests/integration/readme/usage.py -->
 ```python
 from time import sleep
 
 import labtech
 
 # Decorate your task class with @labtech.task:
 @labtech.task
@@ -107,30 +111,30 @@
 if __name__ == '__main__':
     main()
 ```
 
 ![Animated GIF of labtech demo on the command-line](https://ben-denham.github.io/labtech/images/labtech-demo.gif)
 
 Labtech can also produce graphical progress bars in
-[Jupyter](https://jupyter.org/) when the `Lab` is initialized with
-`notebook=True`:
+[Jupyter](https://jupyter.org/) notebooks:
 
 ![Animated GIF of labtech demo in Jupyter](https://ben-denham.github.io/labtech/images/labtech-demo-jupyter.gif)
 
 Tasks parameters can be any of the following types:
 
 * Simple scalar types: `str`, `bool`, `float`, `int`, `None`
 * Collections of any of these types: `list`, `tuple`, `dict`, `Enum`
 * Task types: A task parameter is a "nested task" that will be
   executed before its parent so that it may make use of the nested
   result.
 
 Here's an example of defining a single long-running task to produce a
 result for a large number of dependent tasks:
 
+<!-- N.B. keep this code in-sync with tests/integration/readme/dependents_and_mermaid.py -->
 ```python
 from time import sleep
 
 import labtech
 
 @labtech.task
 class SlowTask:
@@ -165,14 +169,15 @@
 if __name__ == '__main__':
     main()
 ```
 
 Labtech can even generate a [Mermaid diagram](https://mermaid.js.org/syntax/classDiagram.html)
 to visualise your tasks:
 
+<!-- N.B. keep this code in-sync with tests/integration/readme/dependents_and_mermaid.py -->
 ```python
 from labtech.diagram import display_task_diagram
 
 some_slow_task = SlowTask(base=42)
 dependent_tasks = [
     DependentTask(
         slow_task=some_slow_task,
```

