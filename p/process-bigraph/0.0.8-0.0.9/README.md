# Comparing `tmp/process-bigraph-0.0.8.tar.gz` & `tmp/process-bigraph-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process-bigraph-0.0.8.tar", last modified: Mon Dec 18 16:02:35 2023, max compression
+gzip compressed data, was "process-bigraph-0.0.9.tar", last modified: Fri Dec 22 22:31:53 2023, max compression
```

## Comparing `process-bigraph-0.0.8.tar` & `process-bigraph-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2023-12-18 16:02:35.879762 process-bigraph-0.0.8/
--rw-r--r--   0 eranagmon   (503) staff       (20)      143 2023-08-22 14:39:44.000000 process-bigraph-0.0.8/AUTHORS.md
--rw-r--r--   0 eranagmon   (503) staff       (20)    11358 2023-08-22 14:39:44.000000 process-bigraph-0.0.8/LICENSE
--rw-r--r--   0 eranagmon   (503) staff       (20)     6272 2023-12-18 16:02:35.879603 process-bigraph-0.0.8/PKG-INFO
--rw-r--r--   0 eranagmon   (503) staff       (20)     5309 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/README.md
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2023-12-18 16:02:35.878078 process-bigraph-0.0.8/process_bigraph/
--rw-r--r--   0 eranagmon   (503) staff       (20)      935 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    25946 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/composite.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    24609 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/emitter.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2023-12-18 16:02:35.879192 process-bigraph-0.0.8/process_bigraph/experiments/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-22 14:39:44.000000 process-bigraph-0.0.8/process_bigraph/experiments/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     7475 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/experiments/minimal_gillespie.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    28239 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/experiments/signal_modulation.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1057 2023-08-22 14:39:44.000000 process-bigraph-0.0.8/process_bigraph/protocols.py
--rw-r--r--   0 eranagmon   (503) staff       (20)      525 2023-11-09 14:24:37.000000 process-bigraph-0.0.8/process_bigraph/registry.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2023-12-18 16:02:35.879419 process-bigraph-0.0.8/process_bigraph/testing/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/testing/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)      706 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/testing/test_emitter.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    10229 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/tests.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    11946 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/process_bigraph/type_system.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2023-12-18 16:02:35.878784 process-bigraph-0.0.8/process_bigraph.egg-info/
--rw-r--r--   0 eranagmon   (503) staff       (20)     6272 2023-12-18 16:02:35.000000 process-bigraph-0.0.8/process_bigraph.egg-info/PKG-INFO
--rw-r--r--   0 eranagmon   (503) staff       (20)      642 2023-12-18 16:02:35.000000 process-bigraph-0.0.8/process_bigraph.egg-info/SOURCES.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)        1 2023-12-18 16:02:35.000000 process-bigraph-0.0.8/process_bigraph.egg-info/dependency_links.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)       76 2023-12-18 16:02:35.000000 process-bigraph-0.0.8/process_bigraph.egg-info/requires.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)       16 2023-12-18 16:02:35.000000 process-bigraph-0.0.8/process_bigraph.egg-info/top_level.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)       38 2023-12-18 16:02:35.879831 process-bigraph-0.0.8/setup.cfg
--rw-r--r--   0 eranagmon   (503) staff       (20)     1719 2023-12-18 16:00:38.000000 process-bigraph-0.0.8/setup.py
+drwxr-xr-x   0 rspangler   (502) staff       (20)        0 2023-12-22 22:31:53.947825 process-bigraph-0.0.9/
+-rw-r--r--   0 rspangler   (502) staff       (20)      143 2023-07-11 21:30:02.000000 process-bigraph-0.0.9/AUTHORS.md
+-rw-r--r--   0 rspangler   (502) staff       (20)    11358 2023-07-11 21:30:02.000000 process-bigraph-0.0.9/LICENSE
+-rw-r--r--   0 rspangler   (502) staff       (20)     6218 2023-12-22 22:31:53.947666 process-bigraph-0.0.9/PKG-INFO
+-rw-r--r--   0 rspangler   (502) staff       (20)     5309 2023-12-19 00:36:16.000000 process-bigraph-0.0.9/README.md
+drwxr-xr-x   0 rspangler   (502) staff       (20)        0 2023-12-22 22:31:53.945599 process-bigraph-0.0.9/process_bigraph/
+-rw-r--r--   0 rspangler   (502) staff       (20)      935 2023-12-19 00:36:16.000000 process-bigraph-0.0.9/process_bigraph/__init__.py
+-rw-r--r--   0 rspangler   (502) staff       (20)    24690 2023-12-22 22:25:12.000000 process-bigraph-0.0.9/process_bigraph/composite.py
+-rw-r--r--   0 rspangler   (502) staff       (20)    24609 2023-12-19 00:36:16.000000 process-bigraph-0.0.9/process_bigraph/emitter.py
+drwxr-xr-x   0 rspangler   (502) staff       (20)        0 2023-12-22 22:31:53.946885 process-bigraph-0.0.9/process_bigraph/experiments/
+-rw-r--r--   0 rspangler   (502) staff       (20)        0 2023-08-08 20:46:18.000000 process-bigraph-0.0.9/process_bigraph/experiments/__init__.py
+-rw-r--r--   0 rspangler   (502) staff       (20)     7339 2023-12-22 22:25:12.000000 process-bigraph-0.0.9/process_bigraph/experiments/minimal_gillespie.py
+-rw-r--r--   0 rspangler   (502) staff       (20)    28969 2023-12-22 22:30:30.000000 process-bigraph-0.0.9/process_bigraph/experiments/signal_modulation.py
+-rw-r--r--   0 rspangler   (502) staff       (20)     1057 2023-12-01 23:00:32.000000 process-bigraph-0.0.9/process_bigraph/protocols.py
+-rw-r--r--   0 rspangler   (502) staff       (20)      525 2023-11-07 22:42:38.000000 process-bigraph-0.0.9/process_bigraph/registry.py
+drwxr-xr-x   0 rspangler   (502) staff       (20)        0 2023-12-22 22:31:53.947439 process-bigraph-0.0.9/process_bigraph/testing/
+-rw-r--r--   0 rspangler   (502) staff       (20)        0 2023-12-19 00:36:16.000000 process-bigraph-0.0.9/process_bigraph/testing/__init__.py
+-rw-r--r--   0 rspangler   (502) staff       (20)      706 2023-12-19 00:36:16.000000 process-bigraph-0.0.9/process_bigraph/testing/test_emitter.py
+-rw-r--r--   0 rspangler   (502) staff       (20)    10608 2023-12-22 22:25:12.000000 process-bigraph-0.0.9/process_bigraph/tests.py
+-rw-r--r--   0 rspangler   (502) staff       (20)     9782 2023-12-22 22:25:12.000000 process-bigraph-0.0.9/process_bigraph/type_system.py
+drwxr-xr-x   0 rspangler   (502) staff       (20)        0 2023-12-22 22:31:53.946384 process-bigraph-0.0.9/process_bigraph.egg-info/
+-rw-r--r--   0 rspangler   (502) staff       (20)     6218 2023-12-22 22:31:53.000000 process-bigraph-0.0.9/process_bigraph.egg-info/PKG-INFO
+-rw-r--r--   0 rspangler   (502) staff       (20)      642 2023-12-22 22:31:53.000000 process-bigraph-0.0.9/process_bigraph.egg-info/SOURCES.txt
+-rw-r--r--   0 rspangler   (502) staff       (20)        1 2023-12-22 22:31:53.000000 process-bigraph-0.0.9/process_bigraph.egg-info/dependency_links.txt
+-rw-r--r--   0 rspangler   (502) staff       (20)       76 2023-12-22 22:31:53.000000 process-bigraph-0.0.9/process_bigraph.egg-info/requires.txt
+-rw-r--r--   0 rspangler   (502) staff       (20)       16 2023-12-22 22:31:53.000000 process-bigraph-0.0.9/process_bigraph.egg-info/top_level.txt
+-rw-r--r--   0 rspangler   (502) staff       (20)       38 2023-12-22 22:31:53.947866 process-bigraph-0.0.9/setup.cfg
+-rw-r--r--   0 rspangler   (502) staff       (20)     1719 2023-12-22 22:31:35.000000 process-bigraph-0.0.9/setup.py
```

### Comparing `process-bigraph-0.0.8/LICENSE` & `process-bigraph-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/PKG-INFO` & `process-bigraph-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: process-bigraph
-Version: 0.0.8
-Summary: UNKNOWN
+Version: 0.0.9
 Home-page: https://github.com/vivarium-collective/process-bigraph
 Author: Ryan Spangler, Eran Agmon
 Author-email: ryan.spangler@gmail.com, agmon.eran@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -140,9 +137,7 @@
 about how to adjust the final look of your bigraph figure.
 * [Ecoli](https://raw.githubusercontent.com/vivarium-collective/bigraph-viz/main/doc/_static/ecoli.png) for the wiring
 diagraph of a whole-cell E. coli model.
 
 ## License
 
 Bigraph-schema is open-source software released under the [Apache 2 License](https://github.com/vivarium-collective/process-bigraph/blob/main/LICENSE).
-
-
```

### Comparing `process-bigraph-0.0.8/README.md` & `process-bigraph-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/process_bigraph/__init__.py` & `process-bigraph-0.0.9/process_bigraph/__init__.py`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/process_bigraph/composite.py` & `process-bigraph-0.0.9/process_bigraph/composite.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import abc
 import copy
 import math
 import collections
 from typing import Dict
 from bigraph_schema.registry import deep_merge, validate_merge, get_path
+from bigraph_schema.type_system import Edge
 from process_bigraph.type_system import types
 from process_bigraph.protocols import local_lookup_module
 
 
 def hierarchy_depth(hierarchy, path=()):
     """
     Create a mapping of every path in the hierarchy to the node living at
@@ -38,76 +39,46 @@
     def __init__(self, update):
         self.update = update
 
     def get(self):
         return self.update
 
 
-# TODO: create base class for Step and Process
-#   maybe it comes from bigraph-schema?
-class Edge:
-    def __init__(self):
-        pass
-
-
 class Step(Edge):
     """Step base class."""
     # TODO: support trigger every time
     #   as well as dependency trigger
     config_schema = {}
 
+
     def __init__(self, config=None, local_types=None):
         self.types = local_types or types
 
         if config is None:
             config = {}
 
         self.config = self.types.fill(
             self.config_schema,
             config)
 
+
     def schema(self):
         return {}
 
+
     def initial_state(self):
         return {}
-        # initial = {}
-        # return types.fill(
-        #     self.schema(),
-        #     initial)
-
-
-    def project_state(self, ports, wires, path, state):
-        inputs = {}
-        if 'inputs' in ports and 'inputs' in wires:
-            inputs = self.types.project(
-                ports['inputs'],
-                wires['inputs'],
-                path,
-                state)
-
-        outputs = {}
-        if 'outputs' in ports and 'outputs' in wires:
-            outputs = self.types.project(
-                ports['outputs'],
-                wires['outputs'],
-                path,
-                state)
-
-        result = deep_merge(inputs, outputs)
-        
-        return result
 
 
     def invoke(self, state, _=None):
         update = self.update(state)
         sync = SyncUpdate(update)
         return sync
 
-    @abc.abstractmethod
+
     def update(self, state):
         return {}
 
 
 class Process(Edge):
     """Process parent class.
 
@@ -133,42 +104,28 @@
             config = {}
 
         self.config = self.types.fill(
             self.config_schema,
             config)
 
 
-    @abc.abstractmethod
     def schema(self):
         return {}
 
 
     def initial_state(self):
         return {}
-        # initial = {}
-        # return types.fill(
-        #     self.schema(),
-        #     initial)
-
-
-    def project_state(self, ports, wires, path, state):
-        return self.types.project(
-            ports,
-            wires,
-            path,
-            state)
 
 
     def invoke(self, state, interval):
         update = self.update(state, interval)
         sync = SyncUpdate(update)
         return sync
 
 
-    @abc.abstractmethod
     def update(self, state, interval):
         return {}
 
 
     # TODO: should we include run(interval) here?
     #   process would have to maintain state
 
@@ -200,26 +157,25 @@
             args
     ):
 
         self.defer = defer
         self.f = f
         self.args = args
 
+
     def get(self):
         """Perform the deferred computation.
 
         Returns:
             The result of calling the function.
         """
         return self.f(
             self.defer.get(),
             self.args)
 
-# TODO maybe keep wires as tuples/paths to distinguish them from schemas?
-
 
 def find_instances(state, instance_type='process_bigraph.composite.Process'):
     process_class = local_lookup_module(instance_type)
     found = {}
 
     for key, inner in state.items():
         if isinstance(inner, dict) and isinstance(inner.get('instance'), process_class):
@@ -240,15 +196,15 @@
     return hierarchy_depth(instances)
 
 
 def find_step_triggers(path, step):
     prefix = tuple(path[:-1])
     triggers = {}
     wire_paths = find_leaves(
-        step['wires']['inputs'])
+        step['inputs'])
 
     for wire in wire_paths:
         trigger_path = tuple(prefix) + tuple(wire)
         if trigger_path not in triggers:
             triggers[trigger_path] = []
         triggers[trigger_path].append(path)
 
@@ -306,39 +262,36 @@
 
     return leaves
 
 
 def build_step_network(steps):
     ancestors = {
         step_key: {
-            # 'ancestors': [],
             'input_paths': None,
             'output_paths': None}
         for step_key in steps}
 
     nodes = {}
 
     for step_key, step in steps.items():
         for other_key, other_step in steps.items():
             if step_key == other_key:
                 continue
 
             schema = step['instance'].schema()
-            wires = step['wires']
             other_schema = other_step['instance'].schema()
-            other_wires = other_step['wires']
 
             if ancestors[step_key]['input_paths'] is None:
                 ancestors[step_key]['input_paths'] = find_leaves(
-                    wires['inputs'])
+                    step['inputs'])
             input_paths = ancestors[step_key]['input_paths']
 
             if ancestors[step_key]['output_paths'] is None:
                 ancestors[step_key]['output_paths'] = find_leaves(
-                    wires.get('outputs', {}))
+                    step.get('outputs', {}))
             output_paths = ancestors[step_key]['output_paths']
 
             for input in input_paths:
                 path = tuple(input)
                 if not path in nodes:
                     nodes[path] = {
                         'before': set([]),
@@ -424,20 +377,23 @@
     """
 
 
     config_schema = {
         # TODO: add schema type
         'composition': 'tree[any]',
         'state': 'tree[any]',
-        'schema': 'tree[any]',
-        'bridge': 'wires',
+        'schema': {
+            'inputs': 'tree[any]',
+            'outputs': 'tree[any]'},
+        'bridge': {
+            'inputs': 'wires',
+            'outputs': 'wires'},
         'global_time_precision': 'maybe[float]'}
 
 
-    # TODO: if processes are serialized, deserialize them first
     def __init__(self, config=None, local_types=None):
         super().__init__(config, local_types)
 
         initial_composition = self.config.get('composition', {})
         if 'global_time' not in initial_composition:
             initial_composition['global_time'] = 'float'
         initial_composition = types.access(
@@ -456,14 +412,15 @@
         self.bridge = self.config.get('bridge', {})
 
         # fill in the parts of the composition schema
         # determined by the state
         composition, state = types.infer_schema(
             initial_composition,
             initial_state)
+
         # TODO: add flag to types.access(copy=True)
         composition_schema = types.access(composition)
         self.composition = copy.deepcopy(composition_schema)
 
         # find all processes, steps, and emitter in the state
         self.process_paths = find_instance_paths(
             state,
@@ -502,19 +459,21 @@
 
         # calling hydrate here assumes all processes have already been
         # deserialized in the call to infer_schema above.
         self.state = types.hydrate(
             self.composition,
             state)
 
-        self.process_schema = types.infer_edge(
-            self.composition,
-            self.bridge)
+        for port in ['inputs', 'outputs']:
+            self.process_schema = types.infer_edge(
+                self.composition,
+                self.bridge[port])
 
-        self.global_time_precision = self.config['global_time_precision']
+        self.global_time_precision = self.config[
+            'global_time_precision']
 
         self.step_triggers = {}
 
         for step_path, step in self.step_paths.items():
             step_triggers = find_step_triggers(
                 step_path, step)
             self.step_triggers = merge_collections(
@@ -560,16 +519,16 @@
 
     def process_update(
             self,
             path,
             process,
             states,
             interval,
-            ports_key=None,
-    ):
+            ports_key='outputs'):
+
         """Start generating a process's update.
 
         This function is similar to :py:meth:`_invoke_process` except in
         addition to triggering the computation of the process's update
         (by calling ``_invoke_process``), it also generates a
         :py:class:`Defer` object to transform the update into absolute
         terms.
@@ -605,14 +564,15 @@
 
         return absolute
 
 
     def run_process(self, path, process, end_time, full_step, force_complete):
         if path not in self.front:
             self.front[path] = empty_front(self.state['global_time'])
+
         process_time = self.front[path]['time']
         if process_time <= self.state['global_time']:
             if self.front[path].get('future'):
                 future_front = self.front[path]['future']
                 process_interval = future_front['interval']
                 store = future_front['store']
                 state = future_front['state']
@@ -620,15 +580,14 @@
             else:
                 state = types.view_edge(
                     self.composition,
                     self.state,
                     path)
 
                 process_interval = process['interval']
-                # process_timestep = process['instance'].calculate_timestep(state)
 
             if force_complete:
                 # force the process to complete at end_time
                 future = min(process_time + process_interval, end_time)
             else:
                 future = process_time + process_interval
 
@@ -682,15 +641,15 @@
                 self.state = types.apply_update(
                     self.composition,
                     self.state,
                     update)
 
                 bridge_update = types.view(
                     self.process_schema,
-                    self.bridge,
+                    self.bridge['outputs'],
                     (),
                     update)
 
                 if bridge_update:
                     self.bridge_updates.append(bridge_update)
 
         return update_paths
@@ -853,15 +812,15 @@
         return results
 
     def update(self, state, interval):
         # do everything
 
         projection = types.project(
             self.schema(),
-            self.bridge,
+            self.bridge['inputs'],
             [],
             state)
 
         self.state = types.set(
             self.composition,
             self.state,
             projection)
```

### Comparing `process-bigraph-0.0.8/process_bigraph/emitter.py` & `process-bigraph-0.0.9/process_bigraph/emitter.py`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/process_bigraph/experiments/minimal_gillespie.py` & `process-bigraph-0.0.9/process_bigraph/experiments/minimal_gillespie.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,14 @@
             '_default': '5e0'},
         'kdeg': {
             '_type': 'float',
             '_default': '1e-1'}}
 
 
     def schema(self):
-        # Step schemas always have 'inputs' and 'outputs' as top level keys
         return {
             'inputs': {
                 'DNA': {
                     'G': {
                         '_type': 'float',
                         '_default': '1.0'}},
                 'mRNA': {
@@ -86,25 +85,19 @@
             'mRNA': {'C': 11.111},
             'DNA': {
                 'G': 3.0}}
 
 
     def schema(self):
         return {
-            'DNA': 'tree[float]',
-            'mRNA': 'tree[float]'}
-
-            # 'DNA': {
-            #     'G': {
-            #         '_type': 'float',
-            #         '_default': '1.0'}},
-            # 'mRNA': {
-            #     'C': {
-            #         '_type': 'float',
-            #         '_default': '1.0'}}}
+            'inputs': {
+                'DNA': 'tree[float]',
+                'mRNA': 'tree[float]'},
+            'outputs': {
+                'mRNA': 'tree[float]'}}
 
 
     def next_reaction(self, x):
         """get the next reaction and return a new state"""
 
         propensities = [
             self.config['ktsc'] * x[0],
@@ -180,51 +173,55 @@
         # 'schema': {
         #     'DNA': {
         #         'G': 'float'},
         #     'mRNA': {
         #         'C': 'float'}},
 
         'bridge': {
-            'DNA': ['DNA'],
-            'mRNA': ['mRNA']},
+            'inputs': {
+                'DNA': ['DNA'],
+                'mRNA': ['mRNA']},
+            'outputs': {
+                'DNA': ['DNA'],
+                'mRNA': ['mRNA']}},
 
         'state': {
             'mRNA': {'C': 23.0},
             'interval': {
                 '_type': 'step',
                 'address': 'local:!process_bigraph.experiments.minimal_gillespie.GillespieInterval',
                 'config': {'ktsc': '6e0'},
-                'wires': {
-                    'inputs': {
-                        'DNA': ['DNA'],
-                        'mRNA': ['mRNA']},
-                    'outputs': {
-                        'interval': ['event', 'interval']}}},
+                'inputs': {
+                    'DNA': ['DNA'],
+                    'mRNA': ['mRNA']},
+                'outputs': {
+                    'interval': ['event', 'interval']}},
 
             'event': {
                 '_type': 'process',
                 'address': 'local:!process_bigraph.experiments.minimal_gillespie.GillespieEvent',
                 'config': {'ktsc': 6e0},
-                'wires': {
+                'inputs': {
                     'DNA': ['DNA'],
                     'mRNA': ['mRNA']},
+                'outputs': {
+                    'mRNA': ['mRNA']},
                 'interval': '3.0'},
 
             'emitter': {
                 '_type': 'step',
                 'address': 'local:ram-emitter',
                 'config': {
                     'ports': {
                         'inputs': {
                             'mRNA': 'tree[float]',
                             'interval': 'float'}}},
-                'wires': {
-                    'inputs': {
-                        'mRNA': ['mRNA'],
-                        'interval': ['event', 'interval']}}}}}
+                'inputs': {
+                    'mRNA': ['mRNA'],
+                    'interval': ['event', 'interval']}}}}
 
             # TODO: provide a way to emit everything:
             # 'emitter': emit_all(
             #     'console-emitter',
             #     exclusions={'DNA': {}}),
 
             # TODO: make us able to wire to the top with '**'
```

### Comparing `process-bigraph-0.0.8/process_bigraph/experiments/signal_modulation.py` & `process-bigraph-0.0.9/process_bigraph/experiments/signal_modulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -454,408 +454,410 @@
     })
     # run
     workflow.run(num_beats)
     # gather results
     return workflow.gather_results()
 
 
-def test_tremolo():
-    stop = 32
-    frequencies = [262, 294, 330, 349]
-    starting_signal = start_sine_wave(stop)
-
-    def tremolo_create_instance(starting_signal):
-        return {
-            'tremolo': {
-                '_type': 'process',
-                'address': 'local:tremolo',
-                'config': {
-                    'depth': 0.9,
-                    'rate': 9,
-                    'duration': stop,
-                    'input_signal': starting_signal
-                },
-                'wires': {  # this should return that which is in the schema
-                    'output_signal': ['output_signal_store'],
-                }
-            },
-            'emitter': {
-                '_type': 'step',
-                'address': 'local:ram-emitter',
-                'config': {
-                    'ports': {
-                        'inputs': {
-                            'output_signal': 'list[float]'
-                        },
-                    }
-                },
-                'wires': {
-                    'inputs': {
-                        'output_signal': ['output_signal_store'],
-                    }
-                }
-            }
-        }
-
-    def run_instance(instance, num_beats=stop):
-        # make the composite
-        workflow = Composite({
-            'state': instance
-        })
-
-        num_beats = 3
-        # run
-        workflow.run(num_beats)
-
-        # gather results
-        return workflow.gather_results()
-
-    instance = tremolo_create_instance(starting_signal)
-    result = run_instance(instance)
-
-
-def test_ring_mod():
-    duration = 8
-    pitch_frequency = 800
-    initial_signal = start_sine_wave(duration, pitch_frequency)
-
-    def ring_mod_create_instance():
-        return {
-            'ring_modulation': {
-                '_type': 'process',
-                'address': 'local:ring_modulation',
-                'config': {
-                    'mod_freq': 2000,
-                    'input_signal': initial_signal,
-                    'duration': duration
-                },
-                'wires': {  # this should return that which is in the schema
-                    'output_signal': ['output_signal_store'],
-                }
-            },
-            'emitter': {
-                '_type': 'step',
-                'address': 'local:ram-emitter',
-                'config': {
-                    'ports': {
-                        'inputs': {
-                            'output_signal': 'list[float]'
-                        },
-                    }
-                },
-                'wires': {
-                    'inputs': {
-                        'output_signal': ['output_signal_store'],
-                    }
-                }
-            }
-        }
-
-    instance = ring_mod_create_instance()
-    result = run_instance(instance, num_beats=8)[('emitter',)]
-    #array_to_wav(os.path.join('ring_mod_results', 'input_signal.wav'), input_signal=initial_signal)
-    #resulting_wave = np.array(result[('emitter',)])
-    print(len(result), type(result))
-    for r in result:
-        print(type(r))
-    #plot_signal(duration, resulting_wave, 'final_ring_mod_wave', fp='final_ring_mod_result')
-
-
-def test_phaser():
-    duration = 8
-    pitch_frequency = 800
-    rate = 3
-    depth = 0.75
-    initial_signal = start_sine_wave(duration, pitch_frequency)
-
-    def phaser_create_instance():
-        return {
-            'phaser': {
-                '_type': 'process',
-                'address': 'local:phaser',
-                'config': {
-                    'input_signal': initial_signal,
-                    'rate': rate,
-                    'depth': depth,
-                    'duration': duration
-                },
-                'wires': {  # this should return that which is in the schema
-                    'input_signal': ['input_signal_store'],
-                    'output_signal': ['output_signal_store'],
-                }
-            },
-            'emitter': {
-                '_type': 'step',
-                'address': 'local:ram-emitter',
-                'config': {
-                    'ports': {
-                        'inputs': {
-                            'output_signal': 'list[float]'
-                        },
-                    }
-                },
-                'wires': {
-                    'inputs': {
-                        'output_signal': ['output_signal_store'],
-                    }
-                }
-            }
-        }
-
-    instance = phaser_create_instance()
-    result = run_instance(instance, num_beats=8)[('emitter',)]
-    #array_to_wav(os.path.join('phaser_results', 'input_signal.wav'), input_signal=initial_signal)
-    #resulting_wave = np.array(result[('emitter',)])
-    print(len(result), type(result))
-    for r in result:
-        print(type(r))
-    #plot_signal(duration, resulting_wave, 'final_ring_mod_wave', fp='final_ring_mod_result')
-
-
-def test_delay():
-    duration = 8
-    b_flat = adjust_pitch_frequency(440.0, 1.0)
-    delay_time = 0.6
-    decay = 0.4
-    initial_signal = start_sine_wave(duration, b_flat)
-
-    def delay_create_instance():
-        return {
-            'phaser': {
-                '_type': 'process',
-                'address': 'local:delay',
-                'config': {
-                    'input_signal': initial_signal,
-                    'delay_time': delay_time,
-                    'decay': decay,
-                    'duration': duration
-                },
-                'wires': {  # this should return that which is in the schema
-                    'output_signal': ['output_signal_store'],
-                }
-            },
-            'emitter': {
-                '_type': 'step',
-                'address': 'local:ram-emitter',
-                'config': {
-                    'ports': {
-                        'inputs': {
-                            'output_signal': 'list[float]'
-                        },
-                    }
-                },
-                'wires': {
-                    'inputs': {
-                        'output_signal': ['output_signal_store'],
-                    }
-                }
-            }
-        }
-
-
-def create_instance(instance_type: str, wires: Dict[str, Any], **instance_config):
-    return {
-        instance_type: {
-            '_type': 'process',
-            'address': f'local:{instance_type}',
-            'config': instance_config,
-            'wires': wires
-        },
-        'emitter': {
-            '_type': 'step',
-            'address': 'local:ram-emitter',
-            'config': {
-                'ports': {
-                    'inputs': {
-                        'output_signal': 'list[float]'
-                    },
-                }
-            },
-            'wires': {
-                'inputs': {
-                    'output_signal': ['output_signal_store'],
-                }
-            }
-        }
-    }
-
-
-def create_modulation_instance(instance_type: str, **instance_config):
-    """Types to be expected are modeled in a meta-instance below:
-    ```
-         instance = {
-            'tremolo': {
-                'config': {
-                    'input_signal': initial_signal,
-                    'rate': tremolo_rate,
-                    'depth': tremolo_depth,
-                    'duration': duration
-                },
-            },
-            'ring_modulation': {
-                'config': {
-                    'input_signal': 'output_signal_store',
-                    'mod_freq': ring_mod_freq,
-                    'duration': duration
-                }
-            },
-            'delay': {
-                'config': {
-                    'input_signal': 'output_signal_store',
-                    'delay_time': delay_time,
-                    'decay': decay,
-                    'duration': duration
-                },
-            },
-    ```
-    """
-    wires = {'output_signal': ['output_signal_store']}
-    return create_instance(instance_type, wires, **instance_config)
-
-
-def modulate_signal(instance_type: str, duration: int, **instance_config):
-    instance = create_modulation_instance(instance_type, **instance_config)
-    result = run_instance(instance, duration)[('emitter',)]
-    return result[-1]['output_signal']
-
-
-def test_pedalboard_process():
-    """# set global parameters
-    duration = 8
-    b_flat = adjust_pitch_frequency(440.0, 1.0)
-    initial_signal = start_sine_wave(duration, b_flat)
-
-    # pedal-specific parameters
-    delay_time = 0.6
-    decay = 0.4
-    tremolo_rate = 3
-    tremolo_depth = 0.75
-    ring_mod_freq = 1000
-
-    # define pedal spec (must correspond to the process instance types)
-    pedals = {
-        'delay': {
-            'delay_time': delay_time,
-            'decay': decay
-        },
-        'tremolo': {
-            'rate': tremolo_rate,
-            'depth': tremolo_depth
-        },
-        'ring_modulation': {
-            'mod_freq': ring_mod_freq
-        }
-    }
-
-
-    instance = {
-        'pedalboard': {
-            '_type': 'process',
-            'address': 'local:pedalboard',
-            'config': {
-                'input_signal': initial_signal,
-                'duration': duration,
-                'pedals': pedals,
-            },
-            'wires': {  # this should return that which is in the schema
-                'input_signal': ['input_signal_store'],
-                'output_signal': ['output_signal_store'],
-            }
-        },
-        'emitter': {
-            '_type': 'step',
-            'address': 'local:ram-emitter',
-            'config': {
-                'ports': {
-                    'inputs': {
-                        'input_signal': 'list[float]',
-                        'output_signal': 'list[float]'
-                    },
-                }
-            },
-            'wires': {
-                'inputs': {
-                    'input_signal': ['input_signal_store'],
-                    'output_signal': ['output_signal_store'],
-                }
-            }
-        }
-    }
-
-    result = run_instance(instance, num_beats=8)[('emitter',)]
-    #array_to_wav('input_signal.wav', input_signal=initial_signal)
-    #resulting_wave = np.array(result[('emitter',)])
-    final_result = result[-1]['output_signal']
-    #plot_signal(duration, final_result, 'final_wave', fp='final_composite_wave')"""
-    pass
-
-
-def test_pedalboard():
-    # set global parameters
-    duration = 8
-    b_flat = adjust_pitch_frequency(440.0, 1.0)
-    initial_signal = start_sine_wave(duration, b_flat)
-
-    # pedal-specific parameters
-    delay_time = 0.6
-    decay = 0.4
-    tremolo_rate = 3
-    tremolo_depth = 0.75
-    ring_mod_freq = 1000
-
-    instance = {
-        'ring_modulation': {
-            '_type': 'process',
-            'address': 'local:ring_modulation',
-            'config': {
-                'mod_freq': 2000,
-                'input_signal': initial_signal,
-                'duration': duration
-            },
-            'wires': {  # this should return that which is in the schema
-                'input_signal': ['input_signal_store'],
-                'output_signal': ['output_signal_store'],
-            }
-        },
-        'tremolo': {
-            '_type': 'process',
-            'address': 'local:tremolo',
-            'config': {
-                'depth': 0.9,
-                'rate': 9,
-                'duration': duration,
-            },
-            'wires': {  # this should return that which is in the schema
-                'input_signal': 'input_signal_store',
-                'output_signal': ['output_signal_store'],
-            }
-        },
-        'emitter': {
-            '_type': 'step',
-            'address': 'local:ram-emitter',
-            'config': {
-                'ports': {
-                    'inputs': {
-                        'input_signal': 'list[float]',
-                        'output_signal': 'list[float]'
-                    },
-                }
-            },
-            'wires': {
-                'inputs': {
-                    'input_signal': ['input_signal_store'],
-                    'output_signal': ['output_signal_store'],
-                }
-            }
-        }
-    }
+# def test_tremolo():
+#     stop = 32
+#     frequencies = [262, 294, 330, 349]
+#     starting_signal = start_sine_wave(stop)
+
+#     def tremolo_create_instance(starting_signal):
+#         return {
+#             'tremolo': {
+#                 '_type': 'process',
+#                 'address': 'local:tremolo',
+#                 'config': {
+#                     'depth': 0.9,
+#                     'rate': 9,
+#                     'duration': stop,
+#                     'input_signal': starting_signal
+#                 },
+#                 'wires': {  # this should return that which is in the schema
+#                     'output_signal': ['output_signal_store'],
+#                 }
+#             },
+#             'emitter': {
+#                 '_type': 'step',
+#                 'address': 'local:ram-emitter',
+#                 'config': {
+#                     'ports': {
+#                         'inputs': {
+#                             'output_signal': 'list[float]'
+#                         },
+#                     }
+#                 },
+#                 'wires': {
+#                     'inputs': {
+#                         'output_signal': ['output_signal_store'],
+#                     }
+#                 }
+#             }
+#         }
+
+#     def run_instance(instance, num_beats=stop):
+#         # make the composite
+#         workflow = Composite({
+#             'state': instance
+#         })
+
+#         num_beats = 3
+#         # run
+#         workflow.run(num_beats)
+
+#         # gather results
+#         return workflow.gather_results()
+
+#     instance = tremolo_create_instance(starting_signal)
+#     result = run_instance(instance)
+
+
+# def test_ring_mod():
+#     duration = 8
+#     pitch_frequency = 800
+#     initial_signal = start_sine_wave(duration, pitch_frequency)
+
+#     def ring_mod_create_instance():
+#         return {
+#             'ring_modulation': {
+#                 '_type': 'process',
+#                 'address': 'local:ring_modulation',
+#                 'config': {
+#                     'mod_freq': 2000,
+#                     'input_signal': initial_signal,
+#                     'duration': duration
+#                 },
+#                 'wires': {  # this should return that which is in the schema
+#                     'output_signal': ['output_signal_store'],
+#                 }
+#             },
+#             'emitter': {
+#                 '_type': 'step',
+#                 'address': 'local:ram-emitter',
+#                 'config': {
+#                     'ports': {
+#                         'inputs': {
+#                             'output_signal': 'list[float]'
+#                         },
+#                     }
+#                 },
+#                 'wires': {
+#                     'inputs': {
+#                         'output_signal': ['output_signal_store'],
+#                     }
+#                 }
+#             }
+#         }
+
+#     instance = ring_mod_create_instance()
+#     result = run_instance(instance, num_beats=8)[('emitter',)]
+#     #array_to_wav(os.path.join('ring_mod_results', 'input_signal.wav'), input_signal=initial_signal)
+#     #resulting_wave = np.array(result[('emitter',)])
+#     print(len(result), type(result))
+#     for r in result:
+#         print(type(r))
+#     #plot_signal(duration, resulting_wave, 'final_ring_mod_wave', fp='final_ring_mod_result')
+
+
+# def test_phaser():
+#     duration = 8
+#     pitch_frequency = 800
+#     rate = 3
+#     depth = 0.75
+#     initial_signal = start_sine_wave(duration, pitch_frequency)
+
+#     def phaser_create_instance():
+#         return {
+#             'phaser': {
+#                 '_type': 'process',
+#                 'address': 'local:phaser',
+#                 'config': {
+#                     'input_signal': initial_signal,
+#                     'rate': rate,
+#                     'depth': depth,
+#                     'duration': duration
+#                 },
+#                 'wires': {  # this should return that which is in the schema
+#                     'input_signal': ['input_signal_store'],
+#                     'output_signal': ['output_signal_store'],
+#                 }
+#             },
+#             'emitter': {
+#                 '_type': 'step',
+#                 'address': 'local:ram-emitter',
+#                 'config': {
+#                     'ports': {
+#                         'inputs': {
+#                             'output_signal': 'list[float]'
+#                         },
+#                     }
+#                 },
+#                 'wires': {
+#                     'inputs': {
+#                         'output_signal': ['output_signal_store'],
+#                     }
+#                 }
+#             }
+#         }
+
+#     instance = phaser_create_instance()
+#     result = run_instance(instance, num_beats=8)[('emitter',)]
+#     #array_to_wav(os.path.join('phaser_results', 'input_signal.wav'), input_signal=initial_signal)
+#     #resulting_wave = np.array(result[('emitter',)])
+#     print(len(result), type(result))
+#     for r in result:
+#         print(type(r))
+#     #plot_signal(duration, resulting_wave, 'final_ring_mod_wave', fp='final_ring_mod_result')
+
+
+# def test_delay():
+#     duration = 8
+#     b_flat = adjust_pitch_frequency(440.0, 1.0)
+#     delay_time = 0.6
+#     decay = 0.4
+#     initial_signal = start_sine_wave(duration, b_flat)
+
+#     def delay_create_instance():
+#         return {
+#             'phaser': {
+#                 '_type': 'process',
+#                 'address': 'local:delay',
+#                 'config': {
+#                     'input_signal': initial_signal,
+#                     'delay_time': delay_time,
+#                     'decay': decay,
+#                     'duration': duration
+#                 },
+#                 'wires': {  # this should return that which is in the schema
+#                     'output_signal': ['output_signal_store'],
+#                 }
+#             },
+#             'emitter': {
+#                 '_type': 'step',
+#                 'address': 'local:ram-emitter',
+#                 'config': {
+#                     'ports': {
+#                         'inputs': {
+#                             'output_signal': 'list[float]'
+#                         },
+#                     }
+#                 },
+#                 'wires': {
+#                     'inputs': {
+#                         'output_signal': ['output_signal_store'],
+#                     }
+#                 }
+#             }
+#         }
+
+
+# def create_instance(instance_type: str, wires: Dict[str, Any], **instance_config):
+#     return {
+#         instance_type: {
+#             '_type': 'process',
+#             'address': f'local:{instance_type}',
+#             'config': instance_config,
+#             'wires': wires
+#         },
+#         'emitter': {
+#             '_type': 'step',
+#             'address': 'local:ram-emitter',
+#             'config': {
+#                 'ports': {
+#                     'inputs': {
+#                         'output_signal': 'list[float]'
+#                     },
+#                 }
+#             },
+#             'wires': {
+#                 'inputs': {
+#                     'output_signal': ['output_signal_store'],
+#                 }
+#             }
+#         }
+#     }
+
+
+# def create_modulation_instance(instance_type: str, **instance_config):
+#     """Types to be expected are modeled in a meta-instance below:
+#     ```
+#          instance = {
+#             'tremolo': {
+#                 'config': {
+#                     'input_signal': initial_signal,
+#                     'rate': tremolo_rate,
+#                     'depth': tremolo_depth,
+#                     'duration': duration
+#                 },
+#             },
+#             'ring_modulation': {
+#                 'config': {
+#                     'input_signal': 'output_signal_store',
+#                     'mod_freq': ring_mod_freq,
+#                     'duration': duration
+#                 }
+#             },
+#             'delay': {
+#                 'config': {
+#                     'input_signal': 'output_signal_store',
+#                     'delay_time': delay_time,
+#                     'decay': decay,
+#                     'duration': duration
+#                 },
+#             },
+#     ```
+#     """
+#     wires = {'output_signal': ['output_signal_store']}
+#     return create_instance(instance_type, wires, **instance_config)
+
+
+# def modulate_signal(instance_type: str, duration: int, **instance_config):
+#     instance = create_modulation_instance(instance_type, **instance_config)
+#     result = run_instance(instance, duration)[('emitter',)]
+#     return result[-1]['output_signal']
+
+
+# def test_pedalboard_process():
+#     """# set global parameters
+#     duration = 8
+#     b_flat = adjust_pitch_frequency(440.0, 1.0)
+#     initial_signal = start_sine_wave(duration, b_flat)
+
+#     # pedal-specific parameters
+#     delay_time = 0.6
+#     decay = 0.4
+#     tremolo_rate = 3
+#     tremolo_depth = 0.75
+#     ring_mod_freq = 1000
+
+#     # define pedal spec (must correspond to the process instance types)
+#     pedals = {
+#         'delay': {
+#             'delay_time': delay_time,
+#             'decay': decay
+#         },
+#         'tremolo': {
+#             'rate': tremolo_rate,
+#             'depth': tremolo_depth
+#         },
+#         'ring_modulation': {
+#             'mod_freq': ring_mod_freq
+#         }
+#     }
+
+
+#     instance = {
+#         'pedalboard': {
+#             '_type': 'process',
+#             'address': 'local:pedalboard',
+#             'config': {
+#                 'input_signal': initial_signal,
+#                 'duration': duration,
+#                 'pedals': pedals,
+#             },
+#             'wires': {  # this should return that which is in the schema
+#                 'input_signal': ['input_signal_store'],
+#                 'output_signal': ['output_signal_store'],
+#             }
+#         },
+#         'emitter': {
+#             '_type': 'step',
+#             'address': 'local:ram-emitter',
+#             'config': {
+#                 'ports': {
+#                     'inputs': {
+#                         'input_signal': 'list[float]',
+#                         'output_signal': 'list[float]'
+#                     },
+#                 }
+#             },
+#             'wires': {
+#                 'inputs': {
+#                     'input_signal': ['input_signal_store'],
+#                     'output_signal': ['output_signal_store'],
+#                 }
+#             }
+#         }
+#     }
+
+#     result = run_instance(instance, num_beats=8)[('emitter',)]
+#     #array_to_wav('input_signal.wav', input_signal=initial_signal)
+#     #resulting_wave = np.array(result[('emitter',)])
+#     final_result = result[-1]['output_signal']
+#     #plot_signal(duration, final_result, 'final_wave', fp='final_composite_wave')"""
+#     pass
+
+
+# def test_pedalboard():
+#     # set global parameters
+#     duration = 8
+#     b_flat = adjust_pitch_frequency(440.0, 1.0)
+#     initial_signal = start_sine_wave(duration, b_flat)
+
+#     # pedal-specific parameters
+#     delay_time = 0.6
+#     decay = 0.4
+#     tremolo_rate = 3
+#     tremolo_depth = 0.75
+#     ring_mod_freq = 1000
+
+#     instance = {
+#         'ring_modulation': {
+#             '_type': 'process',
+#             'address': 'local:ring_modulation',
+#             'config': {
+#                 'mod_freq': 2000,
+#                 'input_signal': initial_signal,
+#                 'duration': duration
+#             },
+#             'wires': {  # this should return that which is in the schema
+#                 'input_signal': ['input_signal_store'],
+#                 'output_signal': ['output_signal_store'],
+#             }
+#         },
+#         'tremolo': {
+#             '_type': 'process',
+#             'address': 'local:tremolo',
+#             'config': {
+#                 'depth': 0.9,
+#                 'rate': 9,
+#                 'duration': duration,
+#             },
+#             'wires': {  # this should return that which is in the schema
+#                 'input_signal': 'input_signal_store',
+#                 'output_signal': ['output_signal_store'],
+#             }
+#         },
+#         'emitter': {
+#             '_type': 'step',
+#             'address': 'local:ram-emitter',
+#             'config': {
+#                 'ports': {
+#                     'inputs': {
+#                         'input_signal': 'list[float]',
+#                         'output_signal': 'list[float]'
+#                     },
+#                 }
+#             },
+#             'wires': {
+#                 'inputs': {
+#                     'input_signal': ['input_signal_store'],
+#                     'output_signal': ['output_signal_store'],
+#                 }
+#             }
+#         }
+#     }
 
-    result = run_instance(instance, duration)
-    print(f'RESULT: {result}')
+#     result = run_instance(instance, duration)
+#     print(f'RESULT: {result}')
 
 
 if __name__ == '__main__':
-    test_pedalboard()
+    pass
+
+    # test_pedalboard()
     # test_delay()
     # test_phaser()
     # test_ring_mod()
     # test_tremolo()
```

### Comparing `process-bigraph-0.0.8/process_bigraph/protocols.py` & `process-bigraph-0.0.9/process_bigraph/protocols.py`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/process_bigraph/registry.py` & `process-bigraph-0.0.9/process_bigraph/registry.py`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/process_bigraph/testing/test_emitter.py` & `process-bigraph-0.0.9/process_bigraph/testing/test_emitter.py`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/process_bigraph/tests.py` & `process-bigraph-0.0.9/process_bigraph/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,20 +10,26 @@
 
 class IncreaseProcess(Process):
     config_schema = {
         'rate': {
             '_type': 'float',
             '_default': '0.1'}}
 
+
     def __init__(self, config=None):
         super().__init__(config)
 
+
     def schema(self):
         return {
-            'level': 'float'}
+            'inputs': {
+                'level': 'float'},
+            'outputs': {
+                'level': 'float'}}
+
 
     def update(self, state, interval):
         return {
             'level': state['level'] * self.config['rate']}
 
 
 def test_default_config():
@@ -39,42 +45,51 @@
 
     assert c[('what',)] == [1, 2, 3, 4, 5, 11]
 
 
 def test_process():
     process = IncreaseProcess({'rate': 0.2})
     schema = process.schema()
-    state = types.fill(schema)
+    state = types.fill(schema['inputs'])
+    state = types.fill(schema['outputs'])
     update = process.update({'level': 5.5}, 1.0)
-    new_state = types.apply(schema, state, update)
+
+    new_state = types.apply(schema['outputs'], state, update)
 
     assert new_state['level'] == 1.1
 
 
 def test_composite():
     # TODO: add support for the various vivarium emitter
 
     # increase = IncreaseProcess({'rate': 0.3})
     # TODO: This is the config of the composite,
     #   we also need a way to serialize the entire composite
 
     composite = Composite({
         'composition': {
-            'increase': 'process[level:float]',
+            'increase': 'process[level:float,level:float]',
             'value': 'float'},
         'schema': {
-            'exchange': 'float'},
+            'inputs': {
+                'exchange': 'float'},
+            'outputs': {
+                'exchange': 'float'}},
         'bridge': {
-            'exchange': ['value']},
+            'inputs': {
+                'exchange': ['value']},
+            'outputs': {
+                'exchange': ['value']}},
         'state': {
             'increase': {
                 'address': 'local:!process_bigraph.tests.IncreaseProcess',
                 'config': {'rate': 0.3},
                 'interval': 1.0,
-                'wires': {'level': ['value']}},
+                'inputs': {'level': ['value']},
+                'outputs': {'level': ['value']}},
             'value': 11.11}})
 
     initial_state = {'exchange': 3.33}
 
     updates = composite.update(initial_state, 10.0)
 
     final_exchange = sum([
@@ -89,15 +104,16 @@
 def test_infer():
     composite = Composite({
         'state': {
             'increase': {
                 '_type': 'process',
                 'address': 'local:!process_bigraph.tests.IncreaseProcess',
                 'config': {'rate': '0.3'},
-                'wires': {'level': ['value']}},
+                'inputs': {'level': ['value']},
+                'outputs': {'level': ['value']}},
             'value': '11.11'}})
 
     assert composite.composition['value']['_type'] == 'float'
     assert composite.state['value'] == 11.11
 
 
 class OperatorStep(Step):
@@ -134,32 +150,29 @@
             'A': 13,
             'B': 21,
             'step1': {
                 '_type': 'step',
                 'address': 'local:!process_bigraph.tests.OperatorStep',
                 'config': {
                     'operator': '+'},
-                # TODO: avoid inputs/outputs key in wires?
-                'wires': {
-                    'inputs': {
-                        'a': ['A'],
-                        'b': ['B']},
-                    'outputs': {
-                        'c': ['C']}}},
+                'inputs': {
+                    'a': ['A'],
+                    'b': ['B']},
+                'outputs': {
+                    'c': ['C']}},
             'step2': {
                 '_type': 'step',
                 'address': 'local:!process_bigraph.tests.OperatorStep',
                 'config': {
                     'operator': '*'},
-                'wires': {
-                    'inputs': {
-                        'a': ['B'],
-                        'b': ['C']},
-                    'outputs': {
-                        'c': ['D']}}}}})
+                'inputs': {
+                    'a': ['B'],
+                    'b': ['C']},
+                'outputs': {
+                    'c': ['D']}}}})
 
 
     assert composite.state['D'] == (13 + 21) * 21
 
 
 def test_dependencies():
     operation = {
@@ -168,64 +181,59 @@
         'c': 555.555,
 
         '1': {
             '_type': 'step',
             'address': 'local:!process_bigraph.tests.OperatorStep',
             'config': {
                 'operator': '+'},
-            'wires': {
-                'inputs': {
-                    'a': ['a'],
-                    'b': ['b']},
-                'outputs': {
-                    'c': ['e']}}},
+            'inputs': {
+                'a': ['a'],
+                'b': ['b']},
+            'outputs': {
+                'c': ['e']}},
         '2.1': {
             '_type': 'step',
             'address': 'local:!process_bigraph.tests.OperatorStep',
             'config': {
                 'operator': '-'},
-            'wires': {
-                'inputs': {
-                    'a': ['c'],
-                    'b': ['e']},
-                'outputs': {
-                    'c': ['f']}}},
+            'inputs': {
+                'a': ['c'],
+                'b': ['e']},
+            'outputs': {
+                'c': ['f']}},
         '2.2': {
             '_type': 'step',
             'address': 'local:!process_bigraph.tests.OperatorStep',
             'config': {
                 'operator': '-'},
-            'wires': {
-                'inputs': {
-                    'a': ['d'],
-                    'b': ['e']},
-                'outputs': {
-                    'c': ['g']}}},
+            'inputs': {
+                'a': ['d'],
+                'b': ['e']},
+            'outputs': {
+                'c': ['g']}},
         '3': {
             '_type': 'step',
             'address': 'local:!process_bigraph.tests.OperatorStep',
             'config': {
                 'operator': '*'},
-            'wires': {
-                'inputs': {
-                    'a': ['f'],
-                    'b': ['g']},
-                'outputs': {
-                    'c': ['h']}}},
+            'inputs': {
+                'a': ['f'],
+                'b': ['g']},
+            'outputs': {
+                'c': ['h']}},
         '4': {
             '_type': 'step',
             'address': 'local:!process_bigraph.tests.OperatorStep',
             'config': {
                 'operator': '+'},
-            'wires': {
-                'inputs': {
-                    'a': ['e'],
-                    'b': ['h']},
-                'outputs': {
-                    'c': ['i']}}}}
+            'inputs': {
+                'a': ['e'],
+                'b': ['h']},
+            'outputs': {
+                'c': ['i']}}}
 
     composite = Composite({'state': operation})
 
     assert composite.state['h'] == -17396.469884
 
 
 def test_dependency_cycle():
@@ -330,18 +338,24 @@
                         'concentrations': {},
                         'inner': {
                             'agent2': {
                                 '_type': 'process',
                                 'address': 'local:!process_bigraph.tests.SimpleCompartment',
                                 'config': {'id': '0'},
                                 'inner': {},
-                                'wires': {
+                                'inputs': {
+                                    'outer': ['..', '..'],
+                                    'inner': ['inner']},
+                                'outputs': {
                                     'outer': ['..', '..'],
                                     'inner': ['inner']}}},
-                        'wires': {
+                        'inputs': {
+                            'outer': ['..', '..'],
+                            'inner': ['inner']},
+                        'outputs': {
                             'outer': ['..', '..'],
                             'inner': ['inner']}}}}}}
 
 
 if __name__ == '__main__':
     test_default_config()
     test_merge_collections()
```

### Comparing `process-bigraph-0.0.8/process_bigraph/type_system.py` & `process-bigraph-0.0.9/process_bigraph/type_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-from bigraph_schema import TypeSystem, get_path, establish_path, set_path
+"""
+=============
+Process Types
+=============
+"""
+
+from bigraph_schema import Edge, TypeSystem, get_path, establish_path, set_path
 from process_bigraph.registry import protocol_registry
 
 
 process_interval_schema = {
     '_type': 'float',
     '_apply': 'set',
     '_default': '1.0'}
@@ -14,14 +20,20 @@
     process_schema.pop('_apply')
     return types.apply(
         process_schema,
         current,
         update)
 
 
+def check_process(state, bindings, types):
+    return 'instance' in state and isinstance(
+        state['instance'],
+        Edge)
+
+
 def divide_process(value, bindings=None, types=None):
     return value
 
 
 def serialize_process(value, bindings=None, types=None):
     # TODO -- need to get back the protocol: address and the config
     return value
@@ -95,106 +107,60 @@
     return deserialized
 
 
 process_types = {
     'protocol': {
         '_super': 'string'},
 
-    # TODO: step wires are directional ie, we make a distinction
-    #   between inputs and outputs, and the same wire cannot be both
-    #   an input and output at the same time
     'step': {
         '_super': ['edge'],
         '_apply': 'apply_process',
         '_serialize': 'serialize_process',
         '_deserialize': 'deserialize_step',
+        '_check': 'check_process',
         '_divide': 'divide_process',
         '_description': '',
         # TODO: support reference to type parameters from other states
         'address': 'protocol',
         'config': 'tree[any]'},
 
     'process': {
         '_super': ['edge'],
         '_apply': 'apply_process',
         '_serialize': 'serialize_process',
         '_deserialize': 'deserialize_process',
+        '_check': 'check_process',
         '_divide': 'divide_process',
         '_description': '',
         # TODO: support reference to type parameters from other states
-        'interval': process_interval_schema,
-        'address': 'protocol',
-        'config': 'tree[any]'},
+        'interval': process_interval_schema
+    }
 }
 
 
 def register_process_types(types):
     types.apply_registry.register('apply_process', apply_process)
     types.serialize_registry.register('serialize_process', serialize_process)
     types.deserialize_registry.register('deserialize_process', deserialize_process)
     types.divide_registry.register('divide_process', divide_process)
+    types.check_registry.register('check_process', check_process)
 
     types.deserialize_registry.register('deserialize_step', deserialize_step)
 
     for process_key, process_type in process_types.items():
         types.type_registry.register(process_key, process_type)
 
     return types
 
 
 class ProcessTypes(TypeSystem):
     def __init__(self):
         super().__init__()
         register_process_types(self)
 
-    # def serialize(self, schema, state):
-    #     return ''
-
-    # def deserialize(self, schema, encoded):
-    #     return {}
-
-    def infer_wires(self, ports, state, wires, top_schema=None, path=None):
-        top_schema = top_schema or {}
-        path = path or ()
-
-        for port_key, port_wires in wires.items():
-            if isinstance(ports, str):
-                import ipdb;
-                ipdb.set_trace()
-            port_schema = ports.get(port_key, {})
-            # port_wires = wires.get(port_key, ())
-            if isinstance(port_wires, dict):
-                top_schema = self.infer_wires(
-                    ports,
-                    state.get(port_key),
-                    port_wires,
-                    top_schema,
-                    path + (port_key,))
-            else:
-                peer = get_path(
-                    top_schema,
-                    path[:-1])
-
-                destination = establish_path(
-                    peer,
-                    port_wires[:-1],
-                    top=top_schema,
-                    cursor=path[:-1])
-
-                if len(port_wires) == 0:
-                    raise Exception(f'no wires at port "{port_key}" in ports {ports} with state {state}')
-
-                destination_key = port_wires[-1]
-                if destination_key in destination:
-                    # TODO: validate the schema/state
-                    pass
-                else:
-                    destination[destination_key] = port_schema
-
-        return top_schema
 
     def infer_schema(self, schema, state, top_state=None, path=None):
         '''
         Given a schema fragment and an existing state with _type keys,
         return the full schema required to describe that state,
         and whatever state was hydrated (processes/steps) during this process
         '''
@@ -224,45 +190,33 @@
                     {'_type': state_type})
 
                 # TODO: fix is_descendant
                 # if types.type_registry.is_descendant('process', state_schema) or types.registry.is_descendant('step', state_schema):
                 if state_type == 'process' or state_type == 'step':
                     port_schema = hydrated_state['instance'].schema()
 
-                    schema = set_path(
-                        schema,
-                        path + ('_ports',),
-                        port_schema)
-
-                    subwires = hydrated_state['wires']
-                    if state_type == 'step':
-                        input_subwires = subwires.get('inputs', {})
-                        input_port_schema = port_schema.get('inputs', {})
-                        schema = self.infer_wires(
-                            input_port_schema,
-                            hydrated_state,
-                            input_subwires,
-                            top_schema=schema,
-                            path=path[:-1])
+                    for port_key in ['inputs', 'outputs']:
+                        subschema = port_schema.get(
+                            port_key, {})
+
+                        schema = set_path(
+                            schema,
+                            path + (f'_{port_key}',),
+                            subschema)
+
+                        ports = hydrated_state.get(
+                            port_key, {})
 
-                        output_subwires = subwires.get('outputs', {})
-                        output_port_schema = port_schema.get('outputs', {})
-                        schema = self.infer_wires(
-                            output_port_schema,
-                            hydrated_state,
-                            output_subwires,
-                            top_schema=schema,
-                            path=path[:-1])
-                    else:
                         schema = self.infer_wires(
-                            port_schema,
+                            subschema,
                             hydrated_state,
-                            subwires,
+                            ports,
                             top_schema=schema,
                             path=path[:-1])
+
             elif '_type' in schema:
                 hydrated_state = self.deserialize(schema, state)
                 top_state = set_path(
                     top_state,
                     path,
                     hydrated_state)
             else:
@@ -317,17 +271,17 @@
 
         return edge
 
     def initialize_edge_state(self, schema, path, edge):
         initial_state = edge['instance'].initial_state()
         ports = get_path(schema, path + ('_ports',))
 
-        return edge['instance'].project_state(
+        return self.project_edge(
             ports,
-            edge['wires'],
+            edge,
             path[:-1],
             initial_state)
 
     def hydrate_state(self, schema, state):
         if isinstance(state, str) or '_deserialize' in schema:
             result = self.deserialize(schema, state)
         elif isinstance(state, dict):
```

### Comparing `process-bigraph-0.0.8/process_bigraph.egg-info/PKG-INFO` & `process-bigraph-0.0.9/process_bigraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: process-bigraph
-Version: 0.0.8
-Summary: UNKNOWN
+Version: 0.0.9
 Home-page: https://github.com/vivarium-collective/process-bigraph
 Author: Ryan Spangler, Eran Agmon
 Author-email: ryan.spangler@gmail.com, agmon.eran@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -140,9 +137,7 @@
 about how to adjust the final look of your bigraph figure.
 * [Ecoli](https://raw.githubusercontent.com/vivarium-collective/bigraph-viz/main/doc/_static/ecoli.png) for the wiring
 diagraph of a whole-cell E. coli model.
 
 ## License
 
 Bigraph-schema is open-source software released under the [Apache 2 License](https://github.com/vivarium-collective/process-bigraph/blob/main/LICENSE).
-
-
```

### Comparing `process-bigraph-0.0.8/process_bigraph.egg-info/SOURCES.txt` & `process-bigraph-0.0.9/process_bigraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `process-bigraph-0.0.8/setup.py` & `process-bigraph-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 
 with open("README.md", "r") as readme:
     description = readme.read()
     # Patch the relative links to absolute URLs that will work on PyPI.
     description2 = re.sub(
         r']\(([\w/.-]+\.png)\)',
```

