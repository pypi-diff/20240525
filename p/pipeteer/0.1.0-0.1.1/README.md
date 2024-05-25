# Comparing `tmp/pipeteer-0.1.0.tar.gz` & `tmp/pipeteer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeteer-0.1.0.tar", last modified: Wed May 22 16:50:22 2024, max compression
+gzip compressed data, was "pipeteer-0.1.1.tar", last modified: Sat May 25 14:48:36 2024, max compression
```

## Comparing `pipeteer-0.1.0.tar` & `pipeteer-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-22 16:50:22.025351 pipeteer-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      366 2024-05-22 16:50:22.025351 pipeteer-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-21 18:18:23.000000 pipeteer-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-22 16:50:08.000000 pipeteer-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-22 16:50:22.025351 pipeteer-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-22 16:50:22.015351 pipeteer-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-22 16:50:22.015351 pipeteer-0.1.0/src/pipeteer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-22 15:58:37.000000 pipeteer-0.1.0/src/pipeteer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      219 2024-05-22 16:00:31.000000 pipeteer-0.1.0/src/pipeteer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2117 2024-05-22 16:42:35.000000 pipeteer-0.1.0/src/pipeteer/_codegen.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2186 2024-05-22 16:40:30.000000 pipeteer-0.1.0/src/pipeteer/queues.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1675 2024-05-22 16:28:20.000000 pipeteer-0.1.0/src/pipeteer/specs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-22 16:50:22.025351 pipeteer-0.1.0/src/pipeteer.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      366 2024-05-22 16:50:22.000000 pipeteer-0.1.0/src/pipeteer.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      324 2024-05-22 16:50:22.000000 pipeteer-0.1.0/src/pipeteer.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-22 16:50:22.000000 pipeteer-0.1.0/src/pipeteer.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       19 2024-05-22 16:50:22.000000 pipeteer-0.1.0/src/pipeteer.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-22 16:50:22.000000 pipeteer-0.1.0/src/pipeteer.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:48:36.954126 pipeteer-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      366 2024-05-25 14:48:36.954126 pipeteer-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       47 2024-05-21 18:18:23.000000 pipeteer-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      545 2024-05-25 14:48:13.000000 pipeteer-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-25 14:48:36.954126 pipeteer-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:48:36.914131 pipeteer-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:48:36.934129 pipeteer-0.1.1/src/pipeteer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      152 2024-05-22 15:58:37.000000 pipeteer-0.1.1/src/pipeteer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      241 2024-05-24 04:42:47.000000 pipeteer-0.1.1/src/pipeteer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3462 2024-05-24 08:24:07.000000 pipeteer-0.1.1/src/pipeteer/_codegen.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3552 2024-05-24 18:31:55.000000 pipeteer-0.1.1/src/pipeteer/queues.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2162 2024-05-24 05:44:15.000000 pipeteer-0.1.1/src/pipeteer/specs.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-25 14:48:36.954126 pipeteer-0.1.1/src/pipeteer.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      366 2024-05-25 14:48:36.000000 pipeteer-0.1.1/src/pipeteer.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      324 2024-05-25 14:48:36.000000 pipeteer-0.1.1/src/pipeteer.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-25 14:48:36.000000 pipeteer-0.1.1/src/pipeteer.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       19 2024-05-25 14:48:36.000000 pipeteer-0.1.1/src/pipeteer.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-25 14:48:36.000000 pipeteer-0.1.1/src/pipeteer.egg-info/top_level.txt
```

### Comparing `pipeteer-0.1.0/pyproject.toml` & `pipeteer-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pipeteer"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pipeline orchestrations made easy"
 dependencies = [
   "queue-api", "templang", 
 ]
```

### Comparing `pipeteer-0.1.0/src/pipeteer/_codegen.py` & `pipeteer-0.1.1/src/pipeteer/_codegen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,111 @@
 # BEGIN
 from typing import Unpack, TypedDict
-from dataclasses import dataclass
-from q.api import WriteQueue
+from q.api import WriteQueue, ReadQueue, Queue
 from pipeteer import MakeQueue, make_queues as _make_queues, PipelineQueues
 # UNCOMMENT from MODULE import MOD_IMPORTS
-
+INPUTS = str; OUTPUTS = str; INPUT_TYPE = str; OUTPUT_TYPE = str; STATEFUL_INPUT = str # DELETE
 class SUBFLOW_CLASS: # DELETE
   Queues = int # DELETE
-# DELETE
-INPUTS = str; OUTPUTS = str; INPUT_TYPE = str; OUTPUT_TYPE = str # DELETE
-class WORKFLOW:
+class STATEFUL_PIPELINE: # DELETE
+  Queues = int # DELETE
+
+# LOOP PIPELINE_CLASS INPUTS OUTPUTS
+class PIPELINE_CLASS:
+  In = INPUTS
+  Out = OUTPUTS
+  QueueIn = ReadQueue[INPUTS]
+  QueueOut = WriteQueue[OUTPUTS]
+  Queues = PipelineQueues[INPUTS, OUTPUTS]
+
+# END
+
+# LOOP STATEFUL_CLASS STATEFUL_INPUT STATEFUL_PIPELINE
+class STATEFUL_CLASS:
   class Queues(TypedDict):
-    Qin: WriteQueue[INPUT_TYPE]
+    Qin: Queue[STATEFUL_INPUT]
+    internal: 'STATEFUL_PIPELINE.Queues'
+
+# END
+
+class WORKFLOW:
+  class InternalQueues(TypedDict):
     # LOOP SUBFLOW_ID SUBFLOW_CLASS
     SUBFLOW_ID: SUBFLOW_CLASS.Queues
     # END
-    # LOOP PIPELINE_ID INPUTS OUTPUTS
-    PIPELINE_ID: PipelineQueues[INPUTS, OUTPUTS]
+    # LOOP PIPELINE_ID PIPELINE_CLASS
+    PIPELINE_ID: PIPELINE_CLASS.Queues  
+    # END
+    # LOOP STATEFUL_ID STATEFUL_CLASS
+    STATEFUL_ID: STATEFUL_CLASS.Queues
     # END
 
+  class Queues(TypedDict):
+    Qin: Queue[INPUT_TYPE]
+    internal: 'WORKFLOW.InternalQueues'
+
   @staticmethod
   def make_queues(make_queue: MakeQueue, output_queue: WriteQueue[OUTPUT_TYPE]) -> Queues:
     VARIABLE = ... # type: ignore # DELETE
     return _make_queues(VARIABLE, make_queue, output_queue) # type: ignore
   
   @staticmethod
-  def artifacts(**queues: Unpack['WORKFLOW.Queues']):
+  def artifacts(**queues: Unpack['WORKFLOW.InternalQueues']):
     ...
     
 # END
 from typing import Sequence
 from haskellian import Thunk
 from templang import parse
-from pipeteer import Workflow
+from pipeteer import Workflow, Stateful
 
 source = Thunk(lambda: open(__file__).read())
 
 def union_type(types: Sequence[type]):
   return  ' | '.join(t.__name__ for t in types)
 
 def codegen(workflow: Workflow, *, variable: str, module: str, classname: str) -> str:
 
   translations = {
     'MODULE': module,
     'WORKFLOW': classname,
     'VARIABLE': variable,
     'INPUT_TYPE': workflow.input_type.__name__,
     'OUTPUT_TYPE': union_type(workflow.output_types),
-    'MOD_IMPORTS': '*',
     'SUBFLOW_CLASS': [],
     'SUBFLOW_ID': [],
+    'STATEFUL_CLASS': [],
+    'STATEFUL_PIPELINE': [],
+    'STATEFUL_ID': [],
+    'STATEFUL_INPUT': [],
     'PIPELINE_CLASS': [],
     'PIPELINE_ID': [],
     'INPUTS': [],
     'OUTPUTS': [],
   }
 
+  imports = [variable, workflow.input_type.__name__] + [t.__name__ for t in workflow.output_types]
+
   for id, pipe in workflow.pipelines.items():
     match pipe:
       case Workflow():
         translations['SUBFLOW_CLASS'].append(id.title())
         translations['SUBFLOW_ID'].append(id)
+        imports.append(id.title())
+      case Stateful():
+        translations['STATEFUL_CLASS'].append(id.title() + 'Stateful')
+        translations['STATEFUL_ID'].append(id)
+        translations['STATEFUL_INPUT'].append(pipe.input_type.__name__)
+        translations['STATEFUL_PIPELINE'].append(id.title())
+        imports.extend([pipe.input_type.__name__, id.title()])
       case _:
         translations['INPUTS'].append(pipe.input_type.__name__)
         translations['OUTPUTS'].append(union_type(pipe.output_types))
-        translations['PIPELINE_CLASS'].append(id.title())
+        translations['PIPELINE_CLASS'].append(id.title() + 'Pipeline')
         translations['PIPELINE_ID'].append(id)
+        imports.append(pipe.input_type.__name__)
+        imports.extend([t.__name__ for t in pipe.output_types])
+
+  translations['MOD_IMPORTS'] = ', '.join(set(imports))
 
   return parse(source(), translations)
```

### Comparing `pipeteer-0.1.0/src/pipeteer/queues.py` & `pipeteer-0.1.1/src/pipeteer/queues.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,105 @@
-from typing import Mapping, Protocol, TypedDict, Generic, Sequence, TypeVar, TypeAlias
-from haskellian import Left, Either
-from q.api import Queue, ReadQueue, WriteQueue, QueueError
-from .specs import Pipeline, Workflow
+from typing import Mapping, Protocol, TypedDict, Generic, Sequence, TypeVar, TypeAlias, Callable, NamedTuple
+from functools import cache
+from haskellian import Left, Either, either as E
+from q.api import Queue, ReadQueue, WriteQueue, QueueError, ops
+from .specs import Pipeline, Workflow, Stateful
 
 A = TypeVar('A')
 B = TypeVar('B')
+S1 = TypeVar('S1')
+S2 = TypeVar('S2')
 
 class PipelineQueues(TypedDict, Generic[A, B]):
-  Qin: ReadQueue[A]
+  Qin: Queue[A]
   Qout: WriteQueue[B]
 
-WorkflowQueues: TypeAlias = PipelineQueues | Mapping[str, 'WorkflowQueues']
+class NestedQueues(TypedDict, Generic[A, B]):
+  Qin: WriteQueue[A]
+  internal: Mapping[str, 'WorkflowQueues']
+
+WorkflowQueues: TypeAlias = PipelineQueues[A, B] | NestedQueues[A, B]
 
 class prejoin(WriteQueue[A], Generic[A]):
   def __init__(self, queues: Sequence[tuple[WriteQueue[A], Sequence[type[A]]]]):
     self.queues = queues
-
+  
   async def push(self, key: str, value: A) -> Either[QueueError, None]:
     for q, types in self.queues:
       for t in types:
         if isinstance(value, t):
           return await q.push(key, value)
     return Left(QueueError(f'Invalid type {type(value).__name__} for {value}'))
 
+class state_merged(WriteQueue[B], Generic[B]):
+  def __init__(
+    self, post: Callable[[S1, B], S2],
+    Qin: ReadQueue[S1], Qout: WriteQueue[S2]
+  ):
+    self.post = post
+    self.Qin = Qin
+    self.Qout = Qout
+
+  @E.do[QueueError]()
+  async def push(self, key: str, value: B): # type: ignore (python, bruh)
+    state = (await self.Qin.read(key)).unsafe()
+    next = self.post(state, value)
+    (await self.Qout.push(key, next)).unsafe()
+    (await self.Qin.pop(key)).unsafe()
+
 class MakeQueue(Protocol):
-  def __call__(self, id: Sequence[str], type: type[A]) -> Queue[A]:
+  def __call__(self, id: Sequence[str], type: type[A], /) -> Queue[A]:
     ...
 
 def make_queues(
-  workflow: Workflow,
+  workflow: Workflow[A, B],
   make_queue: MakeQueue,
-  output_queue: WriteQueue
-) -> WorkflowQueues:
+  output_queue: WriteQueue[B]
+) -> WorkflowQueues[A, B]:
   
-  def _input_queue(task: Pipeline, prefix: tuple[str, ...]) -> tuple[Queue[A], Sequence[type[A]]]:
+  def _input_queue(task: Pipeline[A, B], prefix: tuple[str, ...]) -> tuple[Queue[A], Sequence[type[A]]]:
     match task:
       case Workflow():
         return _input_queue(task.pipelines[task.input_task], prefix + (task.input_task,))
       case Pipeline():
         return make_queue(prefix, task.input_type), [task.input_type]
-      
-  def _make_queues(task: Pipeline, prefix: tuple[str, ...], output_queue: WriteQueue) -> WorkflowQueues:
+  
+  @cache
+  def _make_queues(task: Pipeline[A, B], prefix: tuple[str, ...], output_queue: WriteQueue[B]) -> WorkflowQueues[A, B]:
     match task:
       case Workflow():
+        def input_of(id: str) -> tuple[WriteQueue, Sequence[type]]:
+          if id == 'output':
+            return output_queue, task.output_types
+          else:
+            return _make_queues(task.pipelines[id], prefix + (id,), output_queue)['Qin'], [task.pipelines[id].input_type]
+
         queues = {
           id: _make_queues(
             pipe, prefix + (id,),
             prejoin([
-              ((output_queue, task.output_types) if id == 'output' else _input_queue(task.pipelines[id], prefix + (id,)))
+              input_of(id)
               for id in task.next_tasks(pipe.output_types)
             ])
           )
           for id, pipe in task.pipelines.items()
         }
-        return queues | { 'Qin': queues[task.input_task]['Qin'] } # type: ignore
+        return NestedQueues(
+          Qin=queues[task.input_task]['Qin'],
+          internal=queues
+        )
+      case Stateful():
+        Qstate = make_queue(prefix, task.input_type)
+        Qout = state_merged(task.post, Qstate, output_queue)
+        queues = dict(_make_queues(task.pipeline, prefix + ('internal',), Qout))
+        Qin: Queue = queues['Qin'] # type: ignore
+        return NestedQueues(
+          Qin=ops.tee(Qstate, Qin.premap(task.pre)),
+          internal=queues # type: ignore
+        )
       case Pipeline():
         return PipelineQueues(
           Qin=_input_queue(task, prefix)[0],
           Qout=output_queue
         )
 
   return _make_queues(workflow, (), output_queue)
```

### Comparing `pipeteer-0.1.0/src/pipeteer/specs.py` & `pipeteer-0.1.1/src/pipeteer/specs.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,41 @@
-from typing import Mapping, Generic, TypeVar, Sequence, Union
+from typing import Mapping, Protocol, Generic, TypeVar, Sequence, Union, Callable, Self
 import os
 
 A = TypeVar('A', covariant=True)
 B = TypeVar('B', covariant=True)
+S1 = TypeVar('S1')
+S2 = TypeVar('S2')
 
 class Pipeline(Generic[A, B]):
   def __init__(self, input_type: type[A], *output_types: type[B]):
     self.input_type = input_type
     self.output_types: Sequence[type] = output_types
 
   @property
   def output_type(self) -> type[B]:
     return Union[*self.output_types] # type: ignore
 
+class Stateful(Pipeline[S1, S2], Generic[S1, S2, A, B]):
+  def __init__(
+    self, input_type: type[S1], output_types: Sequence[type[S2]],
+    pipeline: Pipeline[A, B],
+    pre: Callable[[S1], A], post: Callable[[S1, B], S2]
+  ):
+    self.pipeline = pipeline
+    self.input_type = input_type
+    self.output_types = output_types
+    self.pre = pre
+    self.post = post
+
 class Workflow(Pipeline[A, B], Generic[A, B]):
   input_task: str
   pipelines: Mapping[str, Pipeline]
 
-  def __init__(self, input_task: str, *output_types: type[B], pipelines: Mapping[str, Pipeline]):
+  def __init__(self, input_task: str, /, *output_types: type[B], pipelines: Mapping[str, Pipeline]):
     self.input_task = input_task
     self.output_types = output_types
     self.pipelines = pipelines
 
   @property
   def input_type(self):
     return self.pipelines[self.input_task].input_type
@@ -35,20 +49,21 @@
       tasks.append('output')
     return tasks
   
   def codegen(
     self, __file__: str, *,
     variable: str = 'workflow',
     classname: str = 'Workflow',
+    overwrite: bool = False
   ):
     folder, file = os.path.split(__file__)
     module, py = os.path.splitext(file)
     outfile = os.path.join(folder, f'{module}_codegen{py}')
 
     from ._codegen import codegen
     source = codegen(self, variable=variable, module=f'.{module}', classname=classname)
 
     try:
-      with open(outfile, 'x') as f:
+      with open(outfile, 'w' if overwrite else 'x') as f:
         f.write(source)
     except FileExistsError:
       print('Codegen file already exists. Delete it to regenerate. File:', outfile)
```

