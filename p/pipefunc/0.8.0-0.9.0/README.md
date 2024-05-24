# Comparing `tmp/pipefunc-0.8.0.tar.gz` & `tmp/pipefunc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipefunc-0.8.0.tar", last modified: Fri May 17 00:21:22 2024, max compression
+gzip compressed data, was "pipefunc-0.9.0.tar", last modified: Wed May 22 22:43:26 2024, max compression
```

## Comparing `pipefunc-0.8.0.tar` & `pipefunc-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.765198 pipefunc-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 00:21:09.000000 pipefunc-0.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-17 00:21:09.000000 pipefunc-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 00:21:09.000000 pipefunc-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-17 00:21:22.765198 pipefunc-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2024-05-17 00:21:09.000000 pipefunc-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.769198 pipefunc-0.8.0/pipefunc/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12831 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)    47314 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    25220 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 00:21:22.769198 pipefunc-0.8.0/pipefunc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.761198 pipefunc-0.8.0/pipefunc/map/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/_filearray.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/_mapspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    16101 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8387 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pipefunc/map/adaptive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.765198 pipefunc-0.8.0/pipefunc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 00:21:22.000000 pipefunc-0.8.0/pipefunc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-17 00:21:09.000000 pipefunc-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 00:21:22.765198 pipefunc-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:21:22.765198 pipefunc-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17939 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_pipefunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)    13132 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-17 00:21:09.000000 pipefunc-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:43:26.047414 pipefunc-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 22:43:20.000000 pipefunc-0.9.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-22 22:43:20.000000 pipefunc-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 22:43:20.000000 pipefunc-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-22 22:43:26.047414 pipefunc-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-22 22:43:20.000000 pipefunc-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:43:26.051414 pipefunc-0.9.0/pipefunc/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16467 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54836 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25190 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 22:43:26.051414 pipefunc-0.9.0/pipefunc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:43:26.043414 pipefunc-0.9.0/pipefunc/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11949 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/map/_filearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16715 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/map/_mapspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21440 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/map/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pipefunc/map/adaptive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:43:26.047414 pipefunc-0.9.0/pipefunc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-05-22 22:43:26.000000 pipefunc-0.9.0/pipefunc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-22 22:43:26.000000 pipefunc-0.9.0/pipefunc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:43:26.000000 pipefunc-0.9.0/pipefunc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-22 22:43:26.000000 pipefunc-0.9.0/pipefunc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 22:43:26.000000 pipefunc-0.9.0/pipefunc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-22 22:43:20.000000 pipefunc-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:43:26.047414 pipefunc-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:43:26.047414 pipefunc-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-05-22 22:43:20.000000 pipefunc-0.9.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-22 22:43:20.000000 pipefunc-0.9.0/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-22 22:43:20.000000 pipefunc-0.9.0/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-05-22 22:43:20.000000 pipefunc-0.9.0/tests/test_pipefunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-22 22:43:20.000000 pipefunc-0.9.0/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13107 2024-05-22 22:43:20.000000 pipefunc-0.9.0/tests/test_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-22 22:43:20.000000 pipefunc-0.9.0/tests/test_utils.py
```

### Comparing `pipefunc-0.8.0/LICENSE` & `pipefunc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/PKG-INFO` & `pipefunc-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
@@ -90,38 +90,36 @@
 - [:hammer_and_wrench: Development](#hammer_and_wrench-development)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 <!-- toc-end -->
 
 ## :thinking: What is this?
 
-`pipefunc` is a Python library that simplifies the creation and management of complex function pipelines. It allows you to declare the dependencies between functions and automatically organizes the execution order to satisfy these dependencies.
-
-`pipefunc` provides a range of features to streamline your workflow, including pipeline visualization, flexible function arguments, support for multiple outputs, pipeline simplification, resource usage profiling, parallel execution, caching, and parameter sweep utilities.
+`pipefunc` is a Python library for creating and running function pipelines. By annotating functions and specifying their outputs, it forms a pipeline that automatically organizes the execution order to satisfy dependencies. Just specify the names of the outputs you want to compute, and `pipefunc` will handle the rest by leveraging the parameter names of the annotated functions.
 
 Whether you're working with data processing, scientific computations, machine learning (AI) workflows, or any other scenario involving interdependent functions, `pipefunc` helps you focus on the logic of your code while it handles the intricacies of function dependencies and execution order.
 
 ## :rocket: Key Features
 
-1. 🚀 **Function Composition and Pipelining**: Create pipelines where the output of one function feeds into another, with `pipefunc` handling the execution order.
+1. 🚀 **Function Composition and Pipelining**: Create pipelines by using the `@pipefunc` decorator; execution order is automatically handled.
 2. 📊 **Pipeline Visualization**: Generate visual graphs of your pipelines to better understand the flow of data.
-3. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
-4. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
-5. 🔁 **Map-Reduce Support**: Utilize "fan-out" to distribute tasks and "fan-in" to aggregate results, streamlining data processing in distributed environments.
-6. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
-7. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
-8. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
-9. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
-10. 🛠️ **Flexibility and Ease of Use**: Manage complex function dependencies in a clear, intuitive way with this lightweight yet powerful tool.
+3. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
+4. 🔁 **Map-Reduce Support**: Perform "map" operations to apply functions over data and "reduce" operations to aggregate results, allowing n-dimensional mappings.
+5. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
+6. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
+7. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
+8. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
+9. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
+10. 🏗️ **Leverages giants**: Builds on top of [NetworkX](https://networkx.org/) for graph algorithms and [NumPy](https://numpy.org/) for n-dimensional arrays.
 
 ## :test_tube: How does it work?
 
 pipefunc provides a Pipeline class that you use to define your function pipeline.
-You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify a function's output name and dependencies.
-Once your pipeline is defined, you can execute it for specific output values, simplify it by combining functions with the same root arguments, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
+You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify the function's output name.
+Once your pipeline is defined, you can execute it for specific output values, simplify it by combining function nodes, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
 For more detailed usage instructions and examples, please check the usage example provided in the package.
 
 Here is a simple example usage of pipefunc to illustrate its primary features:
 
 ```python
 from pipefunc import pipefunc, Pipeline
 
@@ -135,38 +133,66 @@
     return b * c
 
 @pipefunc(output_name="e")
 def f_e(c, d, x=1):
     return c * d * x
 
 # Create a pipeline with these functions
-funcs = [f_c, f_d, f_e]
-pipeline = Pipeline(funcs, profile=True)
+pipeline = Pipeline([f_c, f_d, f_e], profile=True)  # `profile=True` enables resource profiling
+
+# Call the pipeline directly for different outputs:
+assert pipeline("d", a=2, b=3) == 15
+assert pipeline("e", a=2, b=3, x=1) == 75
 
-# You can access and call these functions using the func method
+# Or create a new function for a specific output
 h_d = pipeline.func("d")
 assert h_d(a=2, b=3) == 15
 
 h_e = pipeline.func("e")
 assert h_e(a=2, b=3, x=1) == 75
+# Instead of providing the root arguments, you can also provide the intermediate results directly
 assert h_e(c=5, d=15, x=1) == 75
 
 # Visualize the pipeline
 pipeline.visualize()
 
 # Get all possible argument mappings for each function
 all_args = pipeline.all_arg_combinations
 print(all_args)
 
 # Show resource reporting (only works if profile=True)
 pipeline.resources_report()
 ```
 
 This example demonstrates defining a pipeline with `f_c`, `f_d`, `f_e` functions, accessing and executing these functions using the pipeline, visualizing the pipeline graph, getting all possible argument mappings, and reporting on the resource usage.
-This basic example should give you an idea of how to use pipefunc to construct and manage function pipelines.
+This basic example should give you an idea of how to use `pipefunc` to construct and manage function pipelines.
+
+The following example demonstrates how to perform a map-reduce operation using `pipefunc`:
+
+```python
+from pipefunc import pipefunc, Pipeline
+from pipefunc.map import load_outputs
+import numpy as np
+
+@pipefunc(output_name="c", mapspec="a[i], b[j] -> c[i, j]")  # the mapspec is used to specify the mapping
+def f(a: int, b: int):
+    return a + b
+
+@pipefunc(output_name="mean")  # there is no mapspec, so this function takes the full 2D array
+def g(c: np.ndarray):
+    return np.mean(c)
+
+pipeline = Pipeline([f, g])
+inputs = {"a": [1, 2, 3], "b": [4, 5, 6]}
+pipeline.map(inputs, run_folder="my_run_folder", parallel=True)
+result = load_outputs("mean", run_folder="my_run_folder")
+print(result)  # prints 7.0
+```
+
+Here the `mapspec` argument is used to specify the mapping between the inputs and outputs of the `f` function, it creates the product of the `a` and `b` input lists and computes the sum of each pair. The `g` function then computes the mean of the resulting 2D array. The `map` method executes the pipeline for the `inputs`, and the `load_outputs` function is used to load the results of the `g` function from the specified run folder.
 
 ## :notebook: Jupyter Notebook Example
 
 See the detailed usage example and more in our [example.ipynb](https://github.com/basnijholt/pipefunc/blob/main/example.ipynb).
 
 ## :computer: Installation
```

### Comparing `pipefunc-0.8.0/README.md` & `pipefunc-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -28,38 +28,36 @@
 - [:hammer_and_wrench: Development](#hammer_and_wrench-development)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 <!-- toc-end -->
 
 ## :thinking: What is this?
 
-`pipefunc` is a Python library that simplifies the creation and management of complex function pipelines. It allows you to declare the dependencies between functions and automatically organizes the execution order to satisfy these dependencies.
-
-`pipefunc` provides a range of features to streamline your workflow, including pipeline visualization, flexible function arguments, support for multiple outputs, pipeline simplification, resource usage profiling, parallel execution, caching, and parameter sweep utilities.
+`pipefunc` is a Python library for creating and running function pipelines. By annotating functions and specifying their outputs, it forms a pipeline that automatically organizes the execution order to satisfy dependencies. Just specify the names of the outputs you want to compute, and `pipefunc` will handle the rest by leveraging the parameter names of the annotated functions.
 
 Whether you're working with data processing, scientific computations, machine learning (AI) workflows, or any other scenario involving interdependent functions, `pipefunc` helps you focus on the logic of your code while it handles the intricacies of function dependencies and execution order.
 
 ## :rocket: Key Features
 
-1. 🚀 **Function Composition and Pipelining**: Create pipelines where the output of one function feeds into another, with `pipefunc` handling the execution order.
+1. 🚀 **Function Composition and Pipelining**: Create pipelines by using the `@pipefunc` decorator; execution order is automatically handled.
 2. 📊 **Pipeline Visualization**: Generate visual graphs of your pipelines to better understand the flow of data.
-3. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
-4. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
-5. 🔁 **Map-Reduce Support**: Utilize "fan-out" to distribute tasks and "fan-in" to aggregate results, streamlining data processing in distributed environments.
-6. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
-7. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
-8. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
-9. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
-10. 🛠️ **Flexibility and Ease of Use**: Manage complex function dependencies in a clear, intuitive way with this lightweight yet powerful tool.
+3. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
+4. 🔁 **Map-Reduce Support**: Perform "map" operations to apply functions over data and "reduce" operations to aggregate results, allowing n-dimensional mappings.
+5. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
+6. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
+7. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
+8. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
+9. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
+10. 🏗️ **Leverages giants**: Builds on top of [NetworkX](https://networkx.org/) for graph algorithms and [NumPy](https://numpy.org/) for n-dimensional arrays.
 
 ## :test_tube: How does it work?
 
 pipefunc provides a Pipeline class that you use to define your function pipeline.
-You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify a function's output name and dependencies.
-Once your pipeline is defined, you can execute it for specific output values, simplify it by combining functions with the same root arguments, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
+You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify the function's output name.
+Once your pipeline is defined, you can execute it for specific output values, simplify it by combining function nodes, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
 For more detailed usage instructions and examples, please check the usage example provided in the package.
 
 Here is a simple example usage of pipefunc to illustrate its primary features:
 
 ```python
 from pipefunc import pipefunc, Pipeline
 
@@ -73,38 +71,66 @@
     return b * c
 
 @pipefunc(output_name="e")
 def f_e(c, d, x=1):
     return c * d * x
 
 # Create a pipeline with these functions
-funcs = [f_c, f_d, f_e]
-pipeline = Pipeline(funcs, profile=True)
+pipeline = Pipeline([f_c, f_d, f_e], profile=True)  # `profile=True` enables resource profiling
+
+# Call the pipeline directly for different outputs:
+assert pipeline("d", a=2, b=3) == 15
+assert pipeline("e", a=2, b=3, x=1) == 75
 
-# You can access and call these functions using the func method
+# Or create a new function for a specific output
 h_d = pipeline.func("d")
 assert h_d(a=2, b=3) == 15
 
 h_e = pipeline.func("e")
 assert h_e(a=2, b=3, x=1) == 75
+# Instead of providing the root arguments, you can also provide the intermediate results directly
 assert h_e(c=5, d=15, x=1) == 75
 
 # Visualize the pipeline
 pipeline.visualize()
 
 # Get all possible argument mappings for each function
 all_args = pipeline.all_arg_combinations
 print(all_args)
 
 # Show resource reporting (only works if profile=True)
 pipeline.resources_report()
 ```
 
 This example demonstrates defining a pipeline with `f_c`, `f_d`, `f_e` functions, accessing and executing these functions using the pipeline, visualizing the pipeline graph, getting all possible argument mappings, and reporting on the resource usage.
-This basic example should give you an idea of how to use pipefunc to construct and manage function pipelines.
+This basic example should give you an idea of how to use `pipefunc` to construct and manage function pipelines.
+
+The following example demonstrates how to perform a map-reduce operation using `pipefunc`:
+
+```python
+from pipefunc import pipefunc, Pipeline
+from pipefunc.map import load_outputs
+import numpy as np
+
+@pipefunc(output_name="c", mapspec="a[i], b[j] -> c[i, j]")  # the mapspec is used to specify the mapping
+def f(a: int, b: int):
+    return a + b
+
+@pipefunc(output_name="mean")  # there is no mapspec, so this function takes the full 2D array
+def g(c: np.ndarray):
+    return np.mean(c)
+
+pipeline = Pipeline([f, g])
+inputs = {"a": [1, 2, 3], "b": [4, 5, 6]}
+pipeline.map(inputs, run_folder="my_run_folder", parallel=True)
+result = load_outputs("mean", run_folder="my_run_folder")
+print(result)  # prints 7.0
+```
+
+Here the `mapspec` argument is used to specify the mapping between the inputs and outputs of the `f` function, it creates the product of the `a` and `b` input lists and computes the sum of each pair. The `g` function then computes the mean of the resulting 2D array. The `map` method executes the pipeline for the `inputs`, and the `load_outputs` function is used to load the results of the `g` function from the specified run folder.
 
 ## :notebook: Jupyter Notebook Example
 
 See the detailed usage example and more in our [example.ipynb](https://github.com/basnijholt/pipefunc/blob/main/example.ipynb).
 
 ## :computer: Installation
```

### Comparing `pipefunc-0.8.0/pipefunc/__init__.py` & `pipefunc-0.9.0/pipefunc/__init__.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/pipefunc/_cache.py` & `pipefunc-0.9.0/pipefunc/_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 from typing import TYPE_CHECKING, Any, Hashable
 
 import cloudpickle
 
 if TYPE_CHECKING:
     from collections.abc import Hashable
 
-_NONE_RETURN_STR = "__ReturnsNone__"
-
 
 class _CacheBase(abc.ABC):
     @abc.abstractmethod
     def get(self, key: Hashable) -> Any:
         raise NotImplementedError
 
     @abc.abstractmethod
@@ -102,15 +100,15 @@
     @property
     def cache(self) -> dict[Hashable, Any]:
         """Return the cache entries."""
         if not self.shared:
             assert isinstance(self._cache_dict, dict)
             return self._cache_dict
         with self._cache_lock:
-            return dict(self._cache_dict.items())
+            return {k: _maybe_load(v, self._allow_cloudpickle) for k, v in self._cache_dict.items()}
 
     @property
     def access_counts(self) -> dict[Hashable, int]:
         """Return the access counts of the cache entries."""
         if not self.shared:
             assert isinstance(self._access_counts, dict)
             return self._access_counts
@@ -139,22 +137,22 @@
         Returns
         -------
         Any
             The value associated with the key if the key is present in the cache,
             otherwise None.
 
         """
+        if key not in self._cache_dict:
+            return None
         with self._cache_lock:
-            if key in self._cache_dict:
-                self._access_counts[key] += 1
-                value = self._cache_dict[key]
-                if self._allow_cloudpickle and self.shared:
-                    value = cloudpickle.loads(value)
-                return value
-        return None  # pragma: no cover
+            self._access_counts[key] += 1
+        value = self._cache_dict[key]
+        if self._allow_cloudpickle and self.shared:
+            value = cloudpickle.loads(value)
+        return value
 
     def put(self, key: Hashable, value: Any, duration: float) -> None:  # type: ignore[override]
         """Add a value to the cache with its associated key and computation duration.
 
         If the cache is full, the entry with the lowest score based on the access
         frequency and computation duration will be invalidated.
 
@@ -243,14 +241,18 @@
         return cache_str + access_counts_str + computation_durations_str
 
     def __len__(self) -> int:
         """Return the number of entries in the cache."""
         return len(self._cache_dict)
 
 
+def _maybe_load(value: bytes | str, allow_cloudpickle: bool) -> Any:  # noqa: FBT001
+    return cloudpickle.loads(value) if allow_cloudpickle else value
+
+
 class LRUCache(_CacheBase):
     """A shared memory LRU cache implementation.
 
     Parameters
     ----------
     max_size
         Cache size of the LRU cache, by default 128.
@@ -283,31 +285,28 @@
         else:
             self._cache_dict = {}  # type: ignore[assignment]
             self._cache_queue = []  # type: ignore[assignment]
             self._cache_lock = nullcontext()  # type: ignore[assignment]
 
     def get(self, key: Hashable) -> Any:
         """Get a value from the cache by key."""
+        if key not in self._cache_dict:
+            return None
         with self._cache_lock:
-            value = self._cache_dict.get(key)
-            if value is not None:  # Move key to back of queue
-                self._cache_queue.remove(key)
-                self._cache_queue.append(key)
-        if value is not None:
-            if value == _NONE_RETURN_STR:
-                value = None
-            elif self._allow_cloudpickle and self.shared:
-                value = cloudpickle.loads(value)
+            value = self._cache_dict[key]
+            # Move key to back of queue
+            self._cache_queue.remove(key)
+            self._cache_queue.append(key)
+        if self._allow_cloudpickle and self.shared:
+            return cloudpickle.loads(value)
         return value
 
     def put(self, key: Hashable, value: Any) -> None:
         """Insert a key value pair into the cache."""
-        if value is None:
-            value = _NONE_RETURN_STR
-        elif self._allow_cloudpickle and self.shared:
+        if self._allow_cloudpickle and self.shared:
             value = cloudpickle.dumps(value)
         with self._cache_lock:
             self._cache_dict[key] = value
             cache_size = len(self._cache_queue)
             if cache_size < self.max_size:
                 self._cache_queue.append(key)
             else:
@@ -322,15 +321,15 @@
     @property
     def cache(self) -> dict:
         """Returns a copy of the cache."""
         if not self.shared:
             assert isinstance(self._cache_dict, dict)
             return self._cache_dict
         with self._cache_lock:
-            return dict(self._cache_dict.items())
+            return {k: _maybe_load(v, self._allow_cloudpickle) for k, v in self._cache_dict.items()}
 
     def __len__(self) -> int:
         """Return the number of entries in the cache."""
         return len(self._cache_dict)
 
     def clear(self) -> None:
         """Clear the cache."""
```

### Comparing `pipefunc-0.8.0/pipefunc/_lazy.py` & `pipefunc-0.9.0/pipefunc/_lazy.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/pipefunc/_perf.py` & `pipefunc-0.9.0/pipefunc/_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/pipefunc/_pipefunc.py` & `pipefunc-0.9.0/pipefunc/_pipefunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,27 @@
             for k, v in parameters.items()
             if v.default is not inspect.Parameter.empty
         }
         self.profiling_stats: ProfilingStats | None
         self.set_profiling(enable=profile)
         self._validate_mapspec()
 
+    def copy(self) -> PipeFunc:
+        return PipeFunc(
+            self.func,
+            self.output_name,
+            output_picker=self.output_picker,
+            renames=self.renames,
+            profile=self.profile,
+            debug=self.debug,
+            cache=self.cache,
+            save_function=self.save_function,
+            mapspec=self.mapspec,
+        )
+
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Call the wrapped function with the given arguments.
 
         Returns
         -------
         Any
             The return value of the wrapped function.
@@ -282,25 +295,25 @@
         if not isinstance(self.mapspec, MapSpec):  # pragma: no cover
             msg = (
                 "The 'mapspec' argument should be an instance of MapSpec,"
                 f" not {type(self.mapspec)}."
             )
             raise TypeError(msg)
 
-        mapspec_input_names = {x.name for x in self.mapspec.inputs}
+        mapspec_input_names = set(self.mapspec.input_names)
         input_names = set(self.parameters)
         if extra := mapspec_input_names - input_names:
             msg = (
                 f"The input of the function `{self.__name__}` should match"
                 f" the input of the MapSpec `{self.mapspec}`:"
                 f" `{extra} not in {input_names}`."
             )
             raise ValueError(msg)
 
-        mapspec_output_names = {x.name for x in self.mapspec.outputs}
+        mapspec_output_names = set(self.mapspec.output_names)
         output_names = set(at_least_tuple(self.output_name))
         if mapspec_output_names != output_names:
             msg = (
                 f"The output of the function `{self.__name__}` should match"
                 f" the output of the MapSpec `{self.mapspec}`:"
                 f" `{mapspec_output_names} != {output_names}`."
             )
```

### Comparing `pipefunc-0.8.0/pipefunc/_pipeline.py` & `pipefunc-0.9.0/pipefunc/_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 import contextlib
 import functools
 import inspect
 import sys
 import time
 import warnings
 from collections import defaultdict
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Iterable,
-    Literal,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Iterable, Literal, Tuple, Union
 
 import networkx as nx
 from tabulate import tabulate
 
 from pipefunc._cache import DiskCache, HybridCache, LRUCache, SimpleCache
 from pipefunc._lazy import _LazyFunction, task_graph
 from pipefunc._pipefunc import PipeFunc
 from pipefunc._plotting import visualize, visualize_holoviews
 from pipefunc._simplify import _combine_nodes, _get_signature, _wrap_dict_to_tuple
 from pipefunc._utils import at_least_tuple, generate_filename_from_dict, handle_error
 from pipefunc.exceptions import UnusedParametersError
-from pipefunc.map._mapspec import MapSpec
+from pipefunc.map._mapspec import (
+    ArraySpec,
+    MapSpec,
+    mapspec_axes,
+    mapspec_dimensions,
+    validate_consistent_axes,
+)
+from pipefunc.map._run import run
 
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import TypeAlias
 else:
     from typing import TypeAlias
 
 if TYPE_CHECKING:
@@ -224,14 +224,15 @@
             else:
                 mapspec = None
             self.add(f, mapspec=mapspec)
         self._init_internal_cache()
         self._cache_type = cache_type
         self._cache_kwargs = cache_kwargs
         self.cache = _create_cache(cache_type, lazy, cache_kwargs)
+        self._validate_mapspec()
 
     def _init_internal_cache(self) -> None:
         # Internal Pipeline cache
         self._arg_combinations: dict[_OUTPUT_TYPE, set[tuple[str, ...]]] = {}
         self._root_args: dict[_OUTPUT_TYPE, tuple[str, ...]] = {}
         self._func: dict[_OUTPUT_TYPE, _Function] = {}
         with contextlib.suppress(AttributeError):
@@ -251,14 +252,18 @@
         with contextlib.suppress(AttributeError):
             del self.all_arg_combinations
         with contextlib.suppress(AttributeError):
             del self.all_root_args
         with contextlib.suppress(AttributeError):
             del self.topological_generations
 
+    def _validate_mapspec(self) -> None:
+        validate_consistent_axes(self.mapspecs(ordered=False))
+        self._autogen_mapspec_axes()
+
     def _current_cache(self) -> LRUCache | HybridCache | DiskCache | SimpleCache | None:
         """Return the cache used by the pipeline."""
         if not isinstance(self.cache, SimpleCache) and (tg := task_graph()) is not None:
             return tg.cache
         return self.cache
 
     @property
@@ -283,19 +288,15 @@
     def debug(self, value: bool | None) -> None:
         """Set the debug flag for the pipeline and all functions."""
         self._debug = value
         if value is not None:
             for f in self.functions:
                 f.debug = value
 
-    def add(
-        self,
-        f: PipeFunc | Callable,
-        mapspec: str | MapSpec | None = None,
-    ) -> PipeFunc:
+    def add(self, f: PipeFunc | Callable, mapspec: str | MapSpec | None = None) -> PipeFunc:
         """Add a function to the pipeline.
 
         Parameters
         ----------
         f
             The function to add to the pipeline.
         profile
@@ -303,23 +304,22 @@
         mapspec
             This is a specification for mapping that dictates how input values should
             be merged together. If None, the default behavior is that the input directly
             maps to the output.
 
         """
         if not isinstance(f, PipeFunc):
-            f = PipeFunc(f, output_name=f.__name__)
+            f = PipeFunc(f, output_name=f.__name__, mapspec=mapspec)
         elif mapspec is not None:
             msg = (
-                "Initializing the `Pipeline` using `MapSpec`s and"
-                " `PipeFunc`s modifies the `PipeFunc`s inplace."
+                "Initializing the `Pipeline` using tuples of `PipeFunc`s and `MapSpec`s"
+                " will create a copy of the `PipeFunc`."
             )
             warnings.warn(msg, UserWarning, stacklevel=3)
-
-        if mapspec is not None:
+            f: PipeFunc = f.copy()  # type: ignore[no-redef]
             if isinstance(mapspec, str):
                 mapspec = MapSpec.from_string(mapspec)
             f.mapspec = mapspec
             f._validate_mapspec()
 
         self.functions.append(f)
 
@@ -333,20 +333,15 @@
 
         if self.debug is not None:
             f.debug = self.debug
 
         self._init_internal_cache()  # reset cache
         return f
 
-    def drop(
-        self,
-        *,
-        f: PipeFunc | None = None,
-        output_name: _OUTPUT_TYPE | None = None,
-    ) -> None:
+    def drop(self, *, f: PipeFunc | None = None, output_name: _OUTPUT_TYPE | None = None) -> None:
         """Drop a function from the pipeline.
 
         Parameters
         ----------
         f
             The function to drop from the pipeline.
         output_name
@@ -420,20 +415,15 @@
             return f
         root_args = self.root_args(output_name)
         assert isinstance(root_args, tuple)
         f = _Function(self, output_name, root_args=root_args)
         self._func[output_name] = f
         return f
 
-    def __call__(
-        self,
-        __output_name__: _OUTPUT_TYPE | None = None,
-        /,
-        **kwargs: Any,
-    ) -> Any:
+    def __call__(self, __output_name__: _OUTPUT_TYPE | None = None, /, **kwargs: Any) -> Any:
         """Call the pipeline for a specific return value.
 
         Parameters
         ----------
         __output_name__
             The identifier for the return value of the pipeline.
             Is None by default, in which case the unique leaf node is used.
@@ -556,17 +546,18 @@
         -------
         Any
             The return value of the pipeline or a dictionary mapping function
             names to their return values if full_output is True.
 
         """
         if p := self.map_parameters & set(self.func_dependencies(output_name)):
+            inputs = self.map_parameters & set(self.root_args(output_name))
             msg = (
                 f"Cannot execute pipeline to get `{output_name}` because `{p}`"
-                f" have `MapSpec`(s). Use `Pipeline.map` instead."
+                f" (depends on `{inputs=}`) have `MapSpec`(s). Use `Pipeline.map` instead."
             )
             raise RuntimeError(msg)
 
         if output_name in kwargs:
             msg = f"The `output_name='{output_name}'` argument cannot be provided in `kwargs={kwargs}`."
             raise ValueError(msg)
 
@@ -578,33 +569,52 @@
             kwargs=kwargs,
             all_results=all_results,
             full_output=full_output,
             used_parameters=used_parameters,
         )
 
         # if has None, result was from cache, so we don't know which parameters were used
-        if None not in used_parameters and (unused := set(kwargs) - set(used_parameters)):
+        if None not in used_parameters and (unused := kwargs.keys() - set(used_parameters)):
             unused_str = ", ".join(sorted(unused))
             msg = f"Unused keyword arguments: `{unused_str}`. {kwargs=}, {used_parameters=}"
             raise UnusedParametersError(msg)
 
         return all_results if full_output else all_results[output_name]
 
     def map(
         self,
         inputs: dict[str, Any],
-        run_folder: str | Path,
-        manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
+        run_folder: str | Path | None,
+        internal_shapes: dict[str, int | tuple[int, ...]] | None = None,
         *,
-        cleanup: bool = True,
         parallel: bool = True,
+        cleanup: bool = True,
     ) -> list[Result]:
-        from pipefunc.map import run
+        """Run a pipeline with `MapSpec` functions for given `inputs`.
 
-        return run(self, inputs, run_folder, manual_shapes, cleanup=cleanup, parallel=parallel)
+        Parameters
+        ----------
+        inputs
+            The inputs to the pipeline. The keys should be the names of the input
+            parameters of the pipeline functions and the values should be the
+            corresponding input data, these are either single values for functions without `mapspec`
+            or lists of values or `numpy.ndarray`s for functions with `mapspec`.
+        run_folder
+            The folder to store the run information. If `None`, a temporary folder
+            is created.
+        internal_shapes
+            The shapes for intermediary outputs that cannot be inferred from the inputs.
+            You will receive an exception if the shapes cannot be inferred and need to be provided.
+        parallel
+            Whether to run the functions in parallel.
+        cleanup
+            Whether to clean up the `run_folder` before running the pipeline.
+
+        """
+        return run(self, inputs, run_folder, internal_shapes, cleanup=cleanup, parallel=parallel)
 
     @functools.cached_property
     def node_mapping(self) -> dict[_OUTPUT_TYPE, PipeFunc | str]:
         """Return a mapping from node names to nodes.
 
         Returns
         -------
@@ -698,29 +708,44 @@
             node.output_name: self.root_args(node.output_name)
             for node in self.graph.nodes
             if isinstance(node, PipeFunc)
         }
 
     @functools.cached_property
     def map_parameters(self) -> set[str]:
-        map_parameters: set[str] = set()
-        for func in self.functions:
-            if func.mapspec:
-                map_parameters.update(func.mapspec.parameters)
-                for output in func.mapspec.outputs:
-                    map_parameters.add(output.name)
-        return map_parameters
+        return {
+            name
+            for mapspec in self.mapspecs()
+            for name in mapspec.input_names + mapspec.output_names
+        }
 
     @functools.cached_property
     def defaults(self) -> dict[str, Any]:
         defaults = {}
         for func in self.functions:
             defaults.update(func.defaults)
         return defaults
 
+    def mapspecs(self, *, ordered: bool = True) -> list[MapSpec]:
+        """Return the MapSpecs for all functions in the pipeline."""
+        functions = self.sorted_functions if ordered else self.functions
+        return [f.mapspec for f in functions if f.mapspec]
+
+    def mapspecs_as_strings(self) -> list[str]:
+        """Return the MapSpecs for all functions in the pipeline as strings."""
+        return [str(mapspec) for mapspec in self.mapspecs(ordered=True)]
+
+    def mapspec_dimensions(self: Pipeline) -> dict[str, int]:
+        """Return the number of dimensions for each array parameter in the pipeline."""
+        return mapspec_dimensions(self.mapspecs())
+
+    def mapspec_axes(self: Pipeline) -> dict[str, tuple[str, ...]]:
+        """Return the axes for each array parameter in the pipeline."""
+        return mapspec_axes(self.mapspecs())
+
     @functools.cached_property
     def unique_leaf_node(self) -> PipeFunc:
         """Return the unique leaf node of the pipeline graph."""
         leaf_nodes = self.leaf_nodes
         if len(leaf_nodes) != 1:  # pragma: no cover
             msg = (
                 "The pipeline has multiple leaf nodes. Please specify the output_name"
@@ -732,14 +757,47 @@
     @functools.cached_property
     def topological_generations(self) -> tuple[list[str], list[list[PipeFunc]]]:
         generations = list(nx.topological_generations(self.graph))
         assert all(isinstance(x, str) for x in generations[0])
         assert all(isinstance(x, PipeFunc) for gen in generations[1:] for x in gen)
         return generations[0], generations[1:]
 
+    @property
+    def sorted_functions(self) -> list[PipeFunc]:
+        """Return the functions in the pipeline in topological order."""
+        return [f for gen in self.topological_generations[1] for f in gen]
+
+    def _autogen_mapspec_axes(self) -> set[PipeFunc]:
+        """Generate `MapSpec`s for functions that return arrays with `internal_shapes`."""
+        root_args = self.topological_generations[0]
+        mapspecs = self.mapspecs(ordered=False)
+        non_root_inputs = _find_non_root_axes(mapspecs, root_args)
+        output_names = {at_least_tuple(f.output_name) for f in self.functions}
+        multi_output_mapping = {n: names for names in output_names for n in names if len(names) > 1}
+        _replace_none_in_axes(mapspecs, non_root_inputs, multi_output_mapping)  # type: ignore[arg-type]
+        return _create_missing_mapspecs(self.functions, non_root_inputs)  # type: ignore[arg-type]
+
+    def add_mapspec_axis(self, *parameter: str, axis: str) -> None:
+        """Add a new axis to `parameter`'s MapSpec.
+
+        Parameters
+        ----------
+        parameter
+            The parameter to add an axis to.
+        axis
+            The axis to add to the `MapSpec` of all functions that depends on
+            `parameter`. Provide a new axis name to add a new axis or an
+            existing axis name to zip the parameter with the existing axis.
+
+        """
+        self._autogen_mapspec_axes()
+        for p in parameter:
+            _add_mapspec_axis(p, dims={}, axis=axis, functions=self.sorted_functions)
+        self._init_internal_cache()  # reset cache because mapspecs have changed
+
     def _func_node_colors(
         self,
         *,
         conservatively_combine: bool = False,
         output_name: _OUTPUT_TYPE | None = None,
     ) -> list[str]:
         if output_name is None:
@@ -1275,23 +1333,19 @@
     if isinstance(node, PipeFunc):
         if isinstance(node.output_name, tuple):
             return ",".join(node.output_name)
         return node.output_name
     return node
 
 
-def _unique(
-    nodes: Iterable[PipeFunc | str],
-) -> tuple[PipeFunc | str, ...]:
+def _unique(nodes: Iterable[PipeFunc | str]) -> tuple[PipeFunc | str, ...]:
     return tuple(sorted(set(nodes), key=_sort_key))
 
 
-def _filter_funcs(
-    funcs: Iterable[PipeFunc | str],
-) -> list[PipeFunc]:
+def _filter_funcs(funcs: Iterable[PipeFunc | str]) -> list[PipeFunc]:
     return [f for f in funcs if isinstance(f, PipeFunc)]
 
 
 def _compute_arg_mapping(
     graph: nx.DiGraph,
     node: PipeFunc,
     head: PipeFunc,
@@ -1305,7 +1359,106 @@
     if deps_names in arg_set:
         return
     arg_set.add(deps_names)
 
     for func in _filter_funcs(deps):
         new_args = [dep for dep in deps if dep != func]
         _compute_arg_mapping(graph, func, head, new_args, [*replaced, node], arg_set)
+
+
+def _axes_from_dims(p: str, dims: dict[str, int], axis: str) -> tuple[str | None, ...]:
+    n = dims.get(p, 1) - 1
+    return n * (None,) + (axis,)
+
+
+def _add_mapspec_axis(p: str, dims: dict[str, int], axis: str, functions: list[PipeFunc]) -> None:
+    for f in functions:
+        if p not in f.parameters:
+            continue
+        if f.mapspec is None:
+            axes = _axes_from_dims(p, dims, axis)
+            input_specs = [ArraySpec(p, axes)]
+            output_specs = [ArraySpec(name, (axis,)) for name in at_least_tuple(f.output_name)]
+        else:
+            existing_inputs = set(f.mapspec.input_names)
+            if p in existing_inputs:
+                input_specs = [
+                    s.add_axes(axis) if s.name == p and axis not in s.axes else s
+                    for s in f.mapspec.inputs
+                ]
+            else:
+                axes = _axes_from_dims(p, dims, axis)
+                input_specs = [*f.mapspec.inputs, ArraySpec(p, axes)]
+            output_specs = [
+                s.add_axes(axis) if axis not in s.axes else s for s in f.mapspec.outputs
+            ]
+        f.mapspec = MapSpec(tuple(input_specs), tuple(output_specs))
+        for o in output_specs:
+            dims[o.name] = len(o.axes)
+            _add_mapspec_axis(o.name, dims, axis, functions)
+
+
+def _find_non_root_axes(
+    mapspecs: list[MapSpec],
+    root_args: list[str],
+) -> dict[str, list[str | None]]:
+    non_root_inputs: dict[str, list[str | None]] = {}
+    for mapspec in mapspecs:
+        for spec in mapspec.inputs:
+            if spec.name not in root_args:
+                if spec.name not in non_root_inputs:
+                    non_root_inputs[spec.name] = spec.rank * [None]  # type: ignore[assignment]
+                for i, axis in enumerate(spec.axes):
+                    if axis is not None:
+                        non_root_inputs[spec.name][i] = axis
+    return non_root_inputs
+
+
+def _replace_none_in_axes(
+    mapspecs: list[MapSpec],
+    non_root_inputs: dict[str, list[str]],
+    multi_output_mapping: dict[str, tuple[str, ...]],
+) -> None:
+    all_axes_names = {
+        axis.name for mapspec in mapspecs for axis in mapspec.inputs + mapspec.outputs
+    }
+
+    i = 0
+    axis_template = "unnamed_{}"
+    for name, axes in non_root_inputs.items():
+        for j, axis in enumerate(axes):
+            if axis is None:
+                while (new_axis := axis_template.format(i)) in all_axes_names:
+                    i += 1
+                non_root_inputs[name][j] = new_axis
+                all_axes_names.add(new_axis)
+                if name in multi_output_mapping:
+                    # If output is a tuple, update its axes with the new axis.
+                    for output_name in multi_output_mapping[name]:
+                        non_root_inputs[output_name][j] = new_axis
+    assert not any(None in axes for axes in non_root_inputs.values())
+
+
+def _create_missing_mapspecs(
+    functions: list[PipeFunc],
+    non_root_inputs: dict[str, set[str]],
+) -> set[PipeFunc]:
+    # Mapping from output_name to PipeFunc for functions without a MapSpec
+    outputs_without_mapspec: dict[str, PipeFunc] = {
+        name: func
+        for func in functions
+        if func.mapspec is None
+        for name in at_least_tuple(func.output_name)
+    }
+
+    missing: set[str] = non_root_inputs.keys() & outputs_without_mapspec.keys()
+    func_with_new_mapspecs = set()
+    for p in missing:
+        func = outputs_without_mapspec[p]
+        if func in func_with_new_mapspecs:
+            continue  # already added a MapSpec because of multiple outputs
+        axes = tuple(non_root_inputs[p])
+        outputs = tuple(ArraySpec(x, axes) for x in at_least_tuple(func.output_name))
+        func.mapspec = MapSpec(inputs=(), outputs=outputs)
+        func_with_new_mapspecs.add(func)
+        print(f"Autogenerated MapSpec for `{func}`: `{func.mapspec}`")
+    return func_with_new_mapspecs
```

### Comparing `pipefunc-0.8.0/pipefunc/_plotting.py` & `pipefunc-0.9.0/pipefunc/_plotting.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/pipefunc/_simplify.py` & `pipefunc-0.9.0/pipefunc/_simplify.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/pipefunc/_sweep.py` & `pipefunc-0.9.0/pipefunc/_sweep.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,15 @@
     if len(funcs) == 0:
         return None
     if len(funcs) == 1:
         return funcs[0]
     return lambda x: any(func(x) for func in funcs)
 
 
-def _combine_dicts(
-    *maybe_dict: dict[str, Any] | None,
-) -> dict[str, Any] | None:
+def _combine_dicts(*maybe_dict: dict[str, Any] | None) -> dict[str, Any] | None:
     """Combine multiple dictionaries into one."""
     dicts = [d for d in maybe_dict if d is not None]
     if len(dicts) == 0:
         return None
     if len(dicts) == 1:
         return dicts[0]
     # make sure no keys are repeated
@@ -270,18 +268,15 @@
             items,
             dims=dims,
             exclude=_combined_exclude(self.exclude, other.exclude),
             constants=_combine_dicts(self.constants, other.constants),  # type: ignore[arg-type]
             derivers=_combine_dicts(self.derivers, other.derivers),  # type: ignore[arg-type]
         )
 
-    def add_derivers(
-        self,
-        **derivers: Callable[[dict[str, Any]], Any],
-    ) -> Sweep:
+    def add_derivers(self, **derivers: Callable[[dict[str, Any]], Any]) -> Sweep:
         """Add derivers to the sweep, which are functions that modify the sweep items.
 
         Parameters
         ----------
         derivers
             A dictionary of functions to be applied to each
             dict. The dictionary keys are attribute names and the
```

### Comparing `pipefunc-0.8.0/pipefunc/_utils.py` & `pipefunc-0.9.0/pipefunc/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     Returns True if the dictionaries are equal, False if they are not equal,
     and None if there are errors comparing keys and values.
     """
     if len(d1) != len(d2):
         return False
 
-    if set(d1.keys()) != set(d2.keys()):
+    if d1.keys() != d2.keys():
         return False
 
     errors = []
     for k, v1 in d1.items():
         v2 = d2[k]
         try:
             equal = _is_equal(v1, v2)
```

### Comparing `pipefunc-0.8.0/pipefunc/map/_mapspec.py` & `pipefunc-0.9.0/pipefunc/map/_mapspec.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # This file is part of the pipefunc package.
 # Originally, it is based on code from the `aiida-dynamic-workflows` package.
 # Its license can be found in the LICENSE file in this folder.
 
 from __future__ import annotations
 
+import itertools
 import re
+from collections import defaultdict
 from dataclasses import dataclass
 from typing import Any
 
 import numpy as np
 import numpy.typing as npt
 
 
@@ -44,15 +46,15 @@
 
     def __post_init__(self) -> None:
         if not self.name.isidentifier():
             msg = f"Array name '{self.name}' is not a valid Python identifier"
             raise ValueError(msg)
         for i in self.axes:
             if not (i is None or i.isidentifier()):
-                msg = f"Index name '{i}' is not a valid Python identifier"
+                msg = f"Index name '{i}' is not a valid Python identifier."
                 raise ValueError(msg)
 
     def __str__(self) -> str:
         indices = (":" if x is None else x for x in self.axes)
         return f"{self.name}[{', '.join(indices)}]"
 
     @property
@@ -64,17 +66,27 @@
     def rank(self) -> int:
         """Return the rank of this array spec."""
         return len(self.axes)
 
     def validate(self, shape: tuple[int, ...]) -> None:
         """Raise an exception if 'shape' is not compatible with this array spec."""
         if len(shape) != self.rank:
-            msg = f"Expecting array of rank {self.rank}, but got array of shape {shape}"
+            msg = (
+                f"Expecting array of rank {self.rank}, but got array of shape {shape} for `{self}`."
+            )
             raise ValueError(msg)
 
+    def add_axes(self, *axis: str | None) -> ArraySpec:
+        """Return a new ArraySpec with additional axes."""
+        # check for no duplicate axes
+        if any(ax in self.axes for ax in axis if ax is not None):
+            msg = f"Duplicate axes are not allowed: {axis}"
+            raise ValueError(msg)
+        return ArraySpec(self.name, self.axes + axis)
+
 
 @dataclass(frozen=True)
 class MapSpec:
     """Specification for how to map input axes to output axes.
 
     Examples
     --------
@@ -94,69 +106,75 @@
         if not all(x.indices == self.outputs[0].indices for x in self.outputs[1:]):
             msg = "All output arrays must have identical indices."
             raise ValueError(msg)
 
         output_indices = set(self.outputs[0].indices)
         input_indices: set[str] = {index for x in self.inputs for index in x.indices}
 
-        if extra_indices := output_indices - input_indices:
-            msg = f"Output array has indices that do not appear in the input: {extra_indices}"
-            raise ValueError(msg)
         if unused_indices := input_indices - output_indices:
             msg = f"Input array have indices that do not appear in the output: {unused_indices}"
             raise ValueError(msg)
 
     @property
-    def parameters(self) -> tuple[str, ...]:
+    def input_names(self) -> tuple[str, ...]:
         """Return the parameter names of this mapspec."""
         return tuple(x.name for x in self.inputs)
 
     @property
-    def indices(self) -> tuple[str, ...]:
-        """Return the index names for this MapSpec."""
+    def output_names(self) -> tuple[str, ...]:
+        """Return the names of the output arrays."""
+        return tuple(x.name for x in self.outputs)
+
+    @property
+    def output_indices(self) -> tuple[str, ...]:
+        """Return the index names of the output array."""
         return self.outputs[0].indices  # All outputs have the same indices
 
-    def shape(self, shapes: dict[str, tuple[int, ...]]) -> tuple[int, ...]:
+    @property
+    def input_indices(self) -> set[str]:
+        """Return the index names of the input arrays."""
+        return {index for x in self.inputs for index in x.indices}
+
+    def shape(
+        self,
+        input_shapes: dict[str, tuple[int, ...]],
+        internal_shapes: dict[str, tuple[int, ...]] | None = None,
+    ) -> tuple[tuple[int, ...], tuple[bool, ...]]:
         """Return the shape of the output of this MapSpec.
 
         Parameters
         ----------
-        shapes
+        input_shapes
             Shapes of the inputs, keyed by name.
+        internal_shapes
+            Shapes of the outputs, keyed by name. Provide this only if the output
+            has an axis not shared with any input.
 
         """
-        input_names = {x.name for x in self.inputs}
-
-        if extra_names := set(shapes.keys()) - input_names:
-            msg = f"Got extra array {extra_names} that are not accepted by this map."
-            raise ValueError(msg)
-        if missing_names := input_names - set(shapes.keys()):
-            msg = f"Inputs expected by this map were not provided: {missing_names}"
-            raise ValueError(msg)
-
-        # Each individual array is of the appropriate rank
-        for x in self.inputs:
-            x.validate(shapes[x.name])
-
-        # Shapes match between array sharing a named index
-
-        def get_dim(array: ArraySpec, index: str) -> int:
-            axis = array.axes.index(index)
-            return shapes[array.name][axis]
+        input_names = set(self.input_names)
+        _validate_shapes(input_names, input_shapes, self.inputs, internal_shapes, self.output_names)
 
+        internal_shapes = internal_shapes or {}
         shape = []
-        for index in self.outputs[0].indices:  # All outputs have the same indices
+        mask = []
+        internal_shape_index = 0
+        output = self.outputs[0]  # All outputs have the same shape
+        for index in output.axes:
+            assert isinstance(index, str)
             relevant_arrays = [x for x in self.inputs if index in x.indices]
-            dim, *rest = (get_dim(x, index) for x in relevant_arrays)
-            if any(dim != x for x in rest):
-                msg = f"Dimension mismatch for arrays {relevant_arrays} along {index} axis."
-                raise ValueError(msg)
-            shape.append(dim)
-
-        return tuple(shape)
+            if relevant_arrays:
+                dim = _get_common_dim(relevant_arrays, index, input_shapes)
+                shape.append(dim)
+                mask.append(True)
+            else:
+                dim = _get_output_dim(output, internal_shapes, internal_shape_index)
+                shape.append(dim)
+                mask.append(False)
+                internal_shape_index += 1
+        return tuple(shape), tuple(mask)
 
     def output_key(self, shape: tuple[int, ...], linear_index: int) -> tuple[int, ...]:
         """Return a key used for indexing the output of this map.
 
         Parameters
         ----------
         shape
@@ -167,20 +185,18 @@
         Examples
         --------
         >>> spec = MapSpec.from_string("x[i, j], y[j, :, k] -> z[i, j, k]")
         >>> spec.output_key((5, 2, 3), 23)
         (3, 1, 2)
 
         """
-        if len(shape) != len(self.indices):
-            msg = f"Expected a shape of length {len(self.indices)}, got {shape}"
+        if len(shape) != len(self.input_indices):
+            msg = f"Expected a shape of length {len(self.input_indices)}, got {shape}"
             raise ValueError(msg)
-        return tuple(
-            (linear_index // stride) % dim for stride, dim in zip(shape_to_strides(shape), shape)
-        )
+        return _shape_to_key(shape, linear_index)
 
     def input_keys(
         self,
         shape: tuple[int, ...],
         linear_index: int,
     ) -> dict[str, tuple[slice | int, ...]]:
         """Return keys for indexing inputs of this map.
@@ -195,23 +211,26 @@
         Examples
         --------
         >>> spec = MapSpec("x[i, j], y[j, :, k] -> z[i, j, k]")
         >>> spec.input_keys((5, 2, 3), 23)
         {'x': (3, 1), 'y': (1, slice(None, None, None), 2)}
 
         """
-        output_key = self.output_key(shape, linear_index)
-        ids = dict(zip(self.indices, output_key))
+        if len(shape) != len(self.output_indices):
+            msg = f"Expected a shape of length {len(self.input_indices)}, got {shape}"
+            raise ValueError(msg)
+        key = _shape_to_key(shape, linear_index)
+        ids = dict(zip(self.output_indices, key))
         return {
             x.name: tuple(slice(None) if ax is None else ids[ax] for ax in x.axes)
             for x in self.inputs
         }
 
     def __str__(self) -> str:
-        inputs = ", ".join(map(str, self.inputs))
+        inputs = ", ".join(map(str, self.inputs)) if self.inputs else "..."
         outputs = ", ".join(map(str, self.outputs))
         return f"{inputs} -> {outputs}"
 
     @classmethod
     def from_string(cls: type[MapSpec], expr: str) -> MapSpec:
         """Construct an MapSpec from a string."""
         try:
@@ -225,21 +244,36 @@
 
         return cls(inputs, outputs)
 
     def to_string(self) -> str:
         """Return a faithful representation of a MapSpec as a string."""
         return str(self)
 
+    def add_axes(self, *axis: str | None) -> MapSpec:
+        """Return a new MapSpec with additional axes."""
+        return MapSpec(
+            tuple(x.add_axes(*axis) for x in self.inputs),
+            tuple(x.add_axes(*axis) for x in self.outputs),
+        )
+
+
+def _shape_to_key(shape: tuple[int, ...], linear_index: int) -> tuple[int, ...]:
+    return tuple(
+        (linear_index // stride) % dim for stride, dim in zip(shape_to_strides(shape), shape)
+    )
+
 
 def _parse_index_string(index_string: str) -> tuple[str | None, ...]:
     indices = (idx.strip() for idx in index_string.split(","))
     return tuple(i if i != ":" else None for i in indices)
 
 
 def _parse_indexed_arrays(expr: str) -> tuple[ArraySpec, ...]:
+    if expr.strip() == "...":
+        return ()
     if "[" not in expr or "]" not in expr:
         msg = (
             f"Invalid expression '{expr.strip()}'. Expected an expression that includes "
             "array indices in square brackets. For example, 'a[i]' or 'b[i, j]'. "
             "Please check your syntax and try again."
         )
         raise ValueError(msg)
@@ -313,15 +347,15 @@
     msg = f"No array shape defined for type {type(x)}"
     raise TypeError(msg)
 
 
 def expected_mask(mapspec: MapSpec, inputs: dict[str, Any]) -> npt.NDArray[np.bool_]:
     kwarg_shapes = {k: array_shape(v) for k, v in inputs.items()}
     kwarg_masks = {k: array_mask(v) for k, v in inputs.items()}
-    map_shape = mapspec.shape(kwarg_shapes)
+    map_shape, _ = mapspec.shape(kwarg_shapes)
     map_size = np.prod(map_shape)
 
     def is_masked(i: int) -> bool:
         return any(kwarg_masks[k][v] for k, v in mapspec.input_keys(map_shape, i).items())
 
     return np.array([is_masked(x) for x in range(map_size)]).reshape(map_shape)
 
@@ -331,10 +365,118 @@
     return np.sum(~mask)  # type: ignore[return-value]
 
 
 def num_tasks(kwargs: dict[str, Any], mapspec: str | MapSpec) -> int:
     """Return the number of tasks."""
     if isinstance(mapspec, str):
         mapspec = MapSpec.from_string(mapspec)
-    mapped_kwargs = {k: v for k, v in kwargs.items() if k in mapspec.parameters}
+    mapped_kwargs = {k: v for k, v in kwargs.items() if k in mapspec.input_names}
     mask = expected_mask(mapspec, mapped_kwargs)
     return num_tasks_from_mask(mask)
+
+
+def validate_consistent_axes(mapspecs: list[MapSpec]) -> None:
+    """Raise an exception if the axes of the mapspecs are inconsistent."""
+    indices: dict[str, set[ArraySpec]] = defaultdict(set)
+    for mapspec in mapspecs:
+        for spec in mapspec.inputs:
+            indices[spec.name].add(spec)
+        for spec in mapspec.outputs:
+            indices[spec.name].add(spec)
+
+    for name, specs in indices.items():
+        specs_str = ", ".join(str(spec) for spec in specs)
+        lengths = {len(spec.axes) for spec in specs}
+        if len(lengths) > 1:
+            msg = (
+                f"MapSpec axes for `{name}` are inconsistent: {specs_str}."
+                " All axes should have the same length."
+            )
+            raise ValueError(msg)
+        axes: dict[int, str] = {}
+        for spec in specs:
+            for i, axis in enumerate(spec.axes):
+                if axis is not None:
+                    if i in axes and axes[i] != axis:
+                        msg = (
+                            f"MapSpec axes for `{name}` are inconsistent: {specs_str}."
+                            " All axes should have the same name at the same index."
+                        )
+                        raise ValueError(msg)
+                    axes[i] = axis
+
+
+def mapspec_dimensions(mapspecs: list[MapSpec]) -> dict[str, int]:
+    """Return the number of dimensions for each array parameter in the pipeline."""
+    return {
+        arrayspec.name: len(arrayspec.axes)
+        for mapspec in mapspecs
+        for arrayspec in itertools.chain(mapspec.inputs, mapspec.outputs)
+    }
+
+
+def mapspec_axes(mapspecs: list[MapSpec]) -> dict[str, tuple[str, ...]]:
+    """Return the axes for each array parameter in the pipeline."""
+    axes: dict[str, dict[int, str]] = defaultdict(dict)
+    for mapspec in mapspecs:
+        for arrayspec in itertools.chain(mapspec.inputs, mapspec.outputs):
+            for i, axis in enumerate(arrayspec.axes):
+                if axis is not None:
+                    axes[arrayspec.name][i] = axis
+    return {name: tuple(dct[i] for i in range(len(dct))) for name, dct in axes.items()}
+
+
+def _validate_shapes(
+    input_names: set[str],
+    input_shapes: dict[str, tuple[int, ...]],
+    inputs: tuple[ArraySpec, ...],
+    internal_shapes: dict[str, tuple[int, ...]] | None,
+    output_names: tuple[str, ...],
+) -> None:
+    if extra_names := input_shapes.keys() - input_names:
+        msg = f"Got extra array {extra_names} that are not accepted by this map."
+        raise ValueError(msg)
+    if missing_names := input_names - input_shapes.keys():
+        msg = f"Inputs expected by this map were not provided: {missing_names}"
+        raise ValueError(msg)
+    for x in inputs:
+        x.validate(input_shapes[x.name])
+    if internal_shapes:
+        for output_name in internal_shapes:
+            if output_name not in output_names:
+                msg = f"Internal shape of `{output_name}` is not accepted by this map."
+                raise ValueError(msg)
+
+
+def _get_common_dim(
+    arrays: list[ArraySpec],
+    index: str,
+    input_shapes: dict[str, tuple[int, ...]],
+) -> int:
+    def _get_dim(array: ArraySpec, index: str) -> int:
+        axis = array.axes.index(index)
+        return input_shapes[array.name][axis]
+
+    dim, *rest = (_get_dim(x, index) for x in arrays)
+    if any(dim != x for x in rest):
+        arrs = ", ".join(x.name for x in arrays)
+        msg = f"Dimension mismatch for arrays `{arrs}` along `{index}` axis."
+        raise ValueError(msg)
+    return dim
+
+
+def _get_output_dim(
+    output: ArraySpec,
+    internal_shapes: dict[str, tuple[int, ...]],
+    internal_shape_index: int,
+) -> int:
+    if output.name not in internal_shapes:
+        msg = f"Internal shape for '{output.name}' is missing."
+        raise ValueError(msg)
+    if internal_shape_index >= len(internal_shapes[output.name]):
+        msg = f"Internal shape for '{output.name}' is too short."
+        raise ValueError(msg)
+    dim = internal_shapes[output.name][internal_shape_index]
+    if not isinstance(dim, int):
+        msg = f"Internal shape for '{output.name}' must be a tuple of integers."
+        raise TypeError(msg)
+    return dim
```

### Comparing `pipefunc-0.8.0/pipefunc/map/_run.py` & `pipefunc-0.9.0/pipefunc/map/_run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from __future__ import annotations
 
 import shutil
+import tempfile
 from concurrent.futures import ProcessPoolExecutor
 from dataclasses import dataclass
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, NamedTuple, Tuple, Union
 
 import numpy as np
 
 from pipefunc._utils import at_least_tuple, dump, equal_dicts, handle_error, load, prod
-from pipefunc.map._filearray import FileArray
-from pipefunc.map._mapspec import MapSpec, array_shape
+from pipefunc._version import __version__
+from pipefunc.map._filearray import FileArray, _iterate_shape_indices, _select_by_mask
+from pipefunc.map._mapspec import (
+    MapSpec,
+    _shape_to_key,
+    array_shape,
+    mapspec_dimensions,
+    validate_consistent_axes,
+)
 
 if TYPE_CHECKING:
     import sys
 
     from pipefunc import PipeFunc, Pipeline
 
     if sys.version_info < (3, 10):  # pragma: no cover
         from typing_extensions import TypeAlias
     else:
         from typing import TypeAlias
 
-    if sys.version_info < (3, 11):  # pragma: no cover
-        pass
-    else:
-        pass
-
 _OUTPUT_TYPE: TypeAlias = Union[str, Tuple[str, ...]]
 
 
 @dataclass
 class _MockPipeline:
     """An object that contains all information required to run a pipeline.
 
@@ -46,14 +49,33 @@
     def from_pipeline(cls: type[_MockPipeline], pipeline: Pipeline) -> _MockPipeline:  # noqa: PYI019
         return cls(
             defaults=pipeline.defaults,
             map_parameters=pipeline.map_parameters,
             topological_generations=pipeline.topological_generations,
         )
 
+    @property
+    def functions(self) -> list[PipeFunc]:
+        # Return all functions in topological order
+        return [f for gen in self.topological_generations[1] for f in gen]
+
+    def mapspecs(self, *, ordered: bool = True) -> list[MapSpec]:  # noqa: ARG002
+        """Return the MapSpecs for all functions in the pipeline."""
+        functions = self.functions  # topologically ordered
+        return [f.mapspec for f in functions if f.mapspec]
+
+    @property
+    def sorted_functions(self) -> list[PipeFunc]:
+        """Return the functions in the pipeline in topological order."""
+        return self.functions
+
+    def mapspec_dimensions(self) -> dict[str, int]:
+        """Return the number of dimensions for each array parameter in the pipeline."""
+        return mapspec_dimensions(self.mapspecs())
+
 
 def _dump_inputs(
     inputs: dict[str, Any],
     defaults: dict[str, Any],
     run_folder: Path,
 ) -> dict[str, Path]:
     folder = run_folder / "inputs"
@@ -83,15 +105,15 @@
     if isinstance(func.output_name, tuple):
         new_output = []  # output in same order as func.output_name
         for output_name in func.output_name:
             assert func.output_picker is not None
             _output = func.output_picker(output, output_name)
             new_output.append(_output)
             path = _output_path(output_name, run_folder)
-            dump(output, path)
+            dump(_output, path)
         output = new_output
     else:
         path = _output_path(func.output_name, run_folder)
         dump(output, path)
 
     return output
 
@@ -107,23 +129,24 @@
     shutil.rmtree(run_folder, ignore_errors=True)
 
 
 def _compare_to_previous_run_info(
     pipeline: Pipeline,
     run_folder: Path,
     inputs: dict[str, Any],
-    manual_shapes: dict[str, int | tuple[int, ...]],
+    internal_shapes: dict[str, int | tuple[int, ...]] | None = None,
 ) -> None:
     if not RunInfo.path(run_folder).is_file():
         return
     old = RunInfo.load(run_folder, cache=False)
-    if manual_shapes != old.manual_shapes:
-        msg = "Manual shapes do not match previous run, cannot use `cleanup=False`."
+    if internal_shapes != old.internal_shapes:
+        msg = "Internal shapes do not match previous run, cannot use `cleanup=False`."
         raise ValueError(msg)
-    if map_shapes(pipeline, inputs, manual_shapes) != old.shapes:
+    shapes, masks = map_shapes(pipeline, inputs, internal_shapes)
+    if shapes != old.shapes:
         msg = "Shapes do not match previous run, cannot use `cleanup=False`."
         raise ValueError(msg)
     old_inputs = {k: _load_input(k, old.input_paths) for k in inputs}
     equal_inputs = equal_dicts(inputs, old_inputs, verbose=True)
     if equal_inputs is None:
         print(
             "Could not compare new `inputs` to `inputs` from previous run."
@@ -131,56 +154,62 @@
         )
         return
     if not equal_inputs:
         msg = "Inputs do not match previous run, cannot use `cleanup=False`."
         raise ValueError(msg)
 
 
+def _check_inputs(pipeline: Pipeline, inputs: dict[str, Any]) -> None:
+    input_dimensions = pipeline.mapspec_dimensions()
+    for name, value in inputs.items():
+        if (dim := input_dimensions.get(name, 0)) > 1 and isinstance(value, (list, tuple)):
+            msg = f"Expected {dim}D `numpy.ndarray` for input `{name}`, got {type(value)}."
+            raise ValueError(msg)
+
+
 class RunInfo(NamedTuple):
     input_paths: dict[str, Path]
     shapes: dict[_OUTPUT_TYPE, tuple[int, ...]]
-    manual_shapes: dict[str, int | tuple[int, ...]]
+    internal_shapes: dict[str, int | tuple[int, ...]] | None
+    shape_masks: dict[_OUTPUT_TYPE, tuple[bool, ...]]
     run_folder: Path
+    pipefunc_version: str = __version__
 
     @classmethod
     def create(
         cls: type[RunInfo],
         run_folder: str | Path,
         pipeline: Pipeline,
         inputs: dict[str, Any],
-        manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
+        internal_shapes: dict[str, int | tuple[int, ...]] | None = None,
         *,
         cleanup: bool = True,
     ) -> RunInfo:
         run_folder = Path(run_folder)
-        manual_shapes = manual_shapes or {}
         if cleanup:
             cleanup_run_folder(run_folder)
         else:
-            _compare_to_previous_run_info(pipeline, run_folder, inputs, manual_shapes)
+            _compare_to_previous_run_info(pipeline, run_folder, inputs, internal_shapes)
+        _check_inputs(pipeline, inputs)
         input_paths = _dump_inputs(inputs, pipeline.defaults, run_folder)
-        shapes = map_shapes(pipeline, inputs, manual_shapes)
+        shapes, masks = map_shapes(pipeline, inputs, internal_shapes or {})
         return cls(
             input_paths=input_paths,
             shapes=shapes,
-            manual_shapes=manual_shapes,
+            internal_shapes=internal_shapes,
+            shape_masks=masks,
             run_folder=run_folder,
         )
 
     def dump(self, run_folder: str | Path) -> None:
         path = self.path(run_folder)
         dump(self._asdict(), path)
 
     @classmethod
-    def load(
-        cls: type[RunInfo],
-        run_folder: str | Path,
-        *,
-        cache: bool = True,
-    ) -> RunInfo:
+    def load(cls: type[RunInfo], run_folder: str | Path, *, cache: bool = True) -> RunInfo:
         path = cls.path(run_folder)
         dct = load(path, cache=cache)
         return cls(**dct)
 
     @staticmethod
     def path(run_folder: str | Path) -> Path:
         return Path(run_folder) / "run_info.cloudpickle"
@@ -191,36 +220,41 @@
     return run_folder / "outputs" / output_name
 
 
 def _load_parameter(
     parameter: str,
     input_paths: dict[str, Path],
     shapes: dict[_OUTPUT_TYPE, tuple[int, ...]],
-    manual_shapes: dict[str, int | tuple[int, ...]],
+    shape_masks: dict[_OUTPUT_TYPE, tuple[bool, ...]],
     run_folder: Path,
 ) -> Any:
     if parameter in input_paths:
         return _load_input(parameter, input_paths)
-    if parameter in manual_shapes or parameter not in shapes:
+    if parameter not in shapes or not any(shape_masks[parameter]):
         return _load_output(parameter, run_folder)
     file_array_path = _file_array_path(parameter, run_folder)
-    shape = shapes[parameter]
-    return FileArray(file_array_path, shape)
+    external_shape = _external_shape(shapes[parameter], shape_masks[parameter])
+    internal_shape = _internal_shape(shapes[parameter], shape_masks[parameter])
+    return FileArray(
+        file_array_path,
+        external_shape,
+        internal_shape,
+        shape_masks[parameter],
+    )
 
 
 def _func_kwargs(
     func: PipeFunc,
     input_paths: dict[str, Path],
     shapes: dict[_OUTPUT_TYPE, tuple[int, ...]],
-    manual_shapes: dict[str, int | tuple[int, ...]],
+    shape_masks: dict[_OUTPUT_TYPE, tuple[bool, ...]],
     run_folder: Path,
 ) -> dict[str, Any]:
     return {
-        p: _load_parameter(p, input_paths, shapes, manual_shapes, run_folder)
-        for p in func.parameters
+        p: _load_parameter(p, input_paths, shapes, shape_masks, run_folder) for p in func.parameters
     }
 
 
 def _select_kwargs(
     func: PipeFunc,
     kwargs: dict[str, Any],
     shape: tuple[int, ...],
@@ -231,29 +265,42 @@
         k: v[0] if len(v) == 1 else v for k, v in func.mapspec.input_keys(shape, index).items()
     }
     selected = {k: v[input_keys[k]] if k in input_keys else v for k, v in kwargs.items()}
     _load_file_array(selected)
     return selected
 
 
+def _internal_shape(shape: tuple[int, ...], mask: tuple[bool, ...]) -> tuple[int, ...]:
+    return tuple(s for s, m in zip(shape, mask) if not m)
+
+
+def _external_shape(shape: tuple[int, ...], mask: tuple[bool, ...]) -> tuple[int, ...]:
+    return tuple(s for s, m in zip(shape, mask) if m)
+
+
 def _init_file_arrays(
     output_name: _OUTPUT_TYPE,
     shape: tuple[int, ...],
+    mask: tuple[bool, ...],
     run_folder: Path,
 ) -> list[FileArray]:
+    external_shape = _external_shape(shape, mask)
+    internal_shape = _internal_shape(shape, mask)
     return [
-        FileArray(_file_array_path(output_name, run_folder), shape)
+        FileArray(
+            _file_array_path(output_name, run_folder),
+            external_shape,
+            internal_shape,
+            mask,
+        )
         for output_name in at_least_tuple(output_name)
     ]
 
 
-def _init_result_arrays(
-    output_name: _OUTPUT_TYPE,
-    shape: tuple[int, ...],
-) -> list[np.ndarray]:
+def _init_result_arrays(output_name: _OUTPUT_TYPE, shape: tuple[int, ...]) -> list[np.ndarray]:
     return [np.empty(prod(shape), dtype=object) for _ in at_least_tuple(output_name)]
 
 
 def _pick_output(func: PipeFunc, output: Any) -> list[Any]:
     return [
         (func.output_picker(output, output_name) if func.output_picker is not None else output)
         for output_name in at_least_tuple(func.output_name)
@@ -270,44 +317,89 @@
     try:
         return func(**selected)
     except Exception as e:
         handle_error(e, func, selected)
         raise  # handle_error raises but mypy doesn't know that
 
 
-def _run_iteration_and_pick_output(
+def _run_iteration_and_process(
     index: int,
     func: PipeFunc,
     kwargs: dict[str, Any],
     shape: tuple[int, ...],
+    shape_mask: tuple[bool, ...],
+    file_arrays: list[FileArray],
 ) -> list[Any]:
     output = _run_iteration(func, kwargs, shape, index)
-    return _pick_output(func, output)
+    outputs = _pick_output(func, output)
+    _update_file_array(func, file_arrays, shape, shape_mask, index, outputs)
+    return outputs
 
 
 def _update_file_array(
     func: PipeFunc,
     file_arrays: list[FileArray],
     shape: tuple[int, ...],
+    shape_mask: tuple[bool, ...],
     index: int,
-    output: list[Any],
+    outputs: list[Any],
 ) -> None:
     assert isinstance(func.mapspec, MapSpec)
-    output_key = func.mapspec.output_key(shape, index)
-    for file_array, _output in zip(file_arrays, output):
+    external_shape = _external_shape(shape, shape_mask)
+    output_key = func.mapspec.output_key(external_shape, index)
+    for file_array, _output in zip(file_arrays, outputs):
         file_array.dump(output_key, _output)
 
 
+def _indices_to_flat_index(
+    shape: tuple[int, ...],
+    internal_shape: tuple[int, ...],
+    shape_mask: tuple[bool, ...],
+    external_index: tuple[int, ...],
+    internal_index: tuple[int, ...],
+) -> np.int_:
+    full_index = _select_by_mask(shape_mask, external_index, internal_index)
+    full_shape = _select_by_mask(shape_mask, shape, internal_shape)
+    return np.ravel_multi_index(full_index, full_shape)
+
+
+def _set_output(
+    arr: np.ndarray,
+    output: np.ndarray,
+    linear_index: int,
+    shape: tuple[int, ...],
+    shape_mask: tuple[bool, ...],
+) -> None:
+    external_shape = _external_shape(shape, shape_mask)
+    internal_shape = _internal_shape(shape, shape_mask)
+    external_index = _shape_to_key(external_shape, linear_index)
+    for internal_index in _iterate_shape_indices(internal_shape):
+        flat_index = _indices_to_flat_index(
+            external_shape,
+            internal_shape,
+            shape_mask,
+            external_index,
+            internal_index,
+        )
+        arr[flat_index] = output[internal_index]
+
+
 def _update_result_array(
     result_arrays: list[np.ndarray],
     index: int,
     output: list[Any],
+    shape: tuple[int, ...],
+    mask: tuple[bool, ...],
 ) -> None:
     for result_array, _output in zip(result_arrays, output):
-        result_array[index] = _output
+        if not all(mask):
+            _output = np.asarray(_output)  # In case _output is a list
+            _set_output(result_array, _output, index, shape, mask)
+        else:
+            result_array[index] = _output
 
 
 def _existing_and_missing_indices(file_arrays: list[FileArray]) -> tuple[list[int], list[int]]:
     masks = (arr._mask_list() for arr in file_arrays)
     existing_indices = []
     missing_indices = []
     for i, mask_values in enumerate(zip(*masks)):
@@ -318,37 +410,45 @@
     return existing_indices, missing_indices
 
 
 def _execute_map_spec(
     func: PipeFunc,
     kwargs: dict[str, Any],
     shapes: dict[_OUTPUT_TYPE, tuple[int, ...]],
+    shape_masks: dict[_OUTPUT_TYPE, tuple[bool, ...]],
     run_folder: Path,
     parallel: bool,  # noqa: FBT001
 ) -> np.ndarray | list[np.ndarray]:
     assert isinstance(func.mapspec, MapSpec)
     shape = shapes[func.output_name]
-    file_arrays = _init_file_arrays(func.output_name, shape, run_folder)
+    mask = shape_masks[func.output_name]
+    file_arrays = _init_file_arrays(func.output_name, shape, mask, run_folder)
     result_arrays = _init_result_arrays(func.output_name, shape)
-    process_index = partial(_run_iteration_and_pick_output, func=func, kwargs=kwargs, shape=shape)
+    process_index = partial(
+        _run_iteration_and_process,
+        func=func,
+        kwargs=kwargs,
+        shape=shape,
+        shape_mask=mask,
+        file_arrays=file_arrays,
+    )
     existing, missing = _existing_and_missing_indices(file_arrays)
     n = len(missing)
     if parallel and n > 1:
         with ProcessPoolExecutor() as ex:
             outputs_list = list(ex.map(process_index, missing))
     else:
         outputs_list = [process_index(index) for index in missing]
 
     for index, outputs in zip(missing, outputs_list):
-        _update_file_array(func, file_arrays, shape, index, outputs)
-        _update_result_array(result_arrays, index, outputs)
+        _update_result_array(result_arrays, index, outputs, shape, mask)
 
     for index in existing:
         outputs = [file_array.get_from_index(index) for file_array in file_arrays]
-        _update_result_array(result_arrays, index, outputs)
+        _update_result_array(result_arrays, index, outputs, shape, mask)
 
     result_arrays = [x.reshape(shape) for x in result_arrays]
     return result_arrays if isinstance(func.output_name, tuple) else result_arrays[0]
 
 
 def _maybe_load_single_output(
     func: PipeFunc,
@@ -383,52 +483,51 @@
         output = func(**kwargs)
     except Exception as e:
         handle_error(e, func, kwargs)
         raise  # handle_error raises but mypy doesn't know that
     return _dump_output(func, output, run_folder)
 
 
+class Shapes(NamedTuple):
+    shapes: dict[_OUTPUT_TYPE, tuple[int, ...]]
+    masks: dict[_OUTPUT_TYPE, tuple[bool, ...]]
+
+
 def map_shapes(
     pipeline: Pipeline,
     inputs: dict[str, Any],
-    manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
-) -> dict[_OUTPUT_TYPE, tuple[int, ...]]:
-    if manual_shapes is None:
-        manual_shapes = {}
+    internal_shapes: dict[str, int | tuple[int, ...]] | None = None,
+) -> Shapes:
+    if internal_shapes is None:
+        internal_shapes = {}
+    internal = {k: at_least_tuple(v) for k, v in internal_shapes.items()}
+
     map_parameters: set[str] = pipeline.map_parameters
 
     input_parameters = set(pipeline.topological_generations[0])
 
     shapes: dict[_OUTPUT_TYPE, tuple[int, ...]] = {
         p: array_shape(inputs[p]) for p in input_parameters if p in map_parameters
     }
-    mapspec_funcs = [f for gen in pipeline.topological_generations[1] for f in gen if f.mapspec]
+    masks = {name: len(shape) * (True,) for name, shape in shapes.items()}
+    mapspec_funcs = [f for f in pipeline.sorted_functions if f.mapspec]
     for func in mapspec_funcs:
-        assert func.mapspec is not None
-        input_shapes = {}
-        for p in func.mapspec.parameters:
-            if shape := shapes.get(p):
-                input_shapes[p] = shape
-            elif p in manual_shapes:
-                input_shapes[p] = at_least_tuple(manual_shapes[p])
-            else:
-                msg = (
-                    f"Parameter `{p}` is used in map but its shape"
-                    " cannot be inferred from the inputs."
-                    " Provide the shape manually in `manual_shapes`."
-                )
-                raise ValueError(msg)
-        output_shape = func.mapspec.shape(input_shapes)
+        assert func.mapspec is not None  # mypy
+        input_shapes = {p: shapes[p] for p in func.mapspec.input_names if p in shapes}
+        output_shapes = {p: internal[p] for p in func.mapspec.output_names if p in internal}
+        output_shape, mask = func.mapspec.shape(input_shapes, output_shapes)  # type: ignore[arg-type]
         shapes[func.output_name] = output_shape
+        masks[func.output_name] = mask
         if isinstance(func.output_name, tuple):
             for output_name in func.output_name:
                 shapes[output_name] = output_shape
+                masks[output_name] = mask
 
-    assert all(k in shapes for k in map_parameters if k not in manual_shapes)
-    return shapes
+    assert all(k in shapes for k in map_parameters if k not in internal)
+    return Shapes(shapes, masks)
 
 
 def _maybe_load_file_array(x: Any) -> Any:
     if isinstance(x, FileArray):
         return x.to_array()
     return x
 
@@ -447,22 +546,31 @@
 
 def _run_function(func: PipeFunc, run_folder: Path, parallel: bool) -> list[Result]:  # noqa: FBT001
     run_info = RunInfo.load(run_folder)
     kwargs = _func_kwargs(
         func,
         run_info.input_paths,
         run_info.shapes,
-        run_info.manual_shapes,
+        run_info.shape_masks,
         run_folder,
     )
-    if func.mapspec:
-        output = _execute_map_spec(func, kwargs, run_info.shapes, run_folder, parallel)
+    if func.mapspec and func.mapspec.inputs:
+        output = _execute_map_spec(
+            func,
+            kwargs,
+            run_info.shapes,
+            run_info.shape_masks,
+            run_folder,
+            parallel,
+        )
     else:
         output = _execute_single(func, kwargs, run_folder)
 
+    # Note that the kwargs still contain the FileArray objects if _execute_map_spec
+    # was used.
     if isinstance(func.output_name, str):
         return [
             Result(
                 function=func.__name__,
                 kwargs=kwargs,
                 output_name=func.output_name,
                 output=output,
@@ -471,47 +579,75 @@
 
     return [
         Result(function=func.__name__, kwargs=kwargs, output_name=output_name, output=_output)
         for output_name, _output in zip(func.output_name, output)
     ]
 
 
+def _ensure_run_folder(run_folder: str | Path | None) -> Path:
+    if run_folder is None:
+        tmp_dir = tempfile.mkdtemp()
+        run_folder = Path(tmp_dir)
+    return Path(run_folder)
+
+
 def run(
     pipeline: Pipeline,
     inputs: dict[str, Any],
-    run_folder: str | Path,
-    manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
+    run_folder: str | Path | None,
+    internal_shapes: dict[str, int | tuple[int, ...]] | None = None,
     *,
     parallel: bool = True,
     cleanup: bool = True,
 ) -> list[Result]:
-    run_folder = Path(run_folder)
-    run_info = RunInfo.create(run_folder, pipeline, inputs, manual_shapes, cleanup=cleanup)
+    """Run a pipeline with `MapSpec` functions for given `inputs`.
+
+    Parameters
+    ----------
+    pipeline
+        The pipeline to run.
+    inputs
+        The inputs to the pipeline. The keys should be the names of the input
+        parameters of the pipeline functions and the values should be the
+        corresponding input data, these are either single values for functions without `mapspec`
+        or lists of values or `numpy.ndarray`s for functions with `mapspec`.
+    run_folder
+        The folder to store the run information. If `None`, a temporary folder
+        is created.
+    internal_shapes
+        The shapes for intermediary outputs that cannot be inferred from the inputs.
+        You will receive an exception if the shapes cannot be inferred and need to be provided.
+    parallel
+        Whether to run the functions in parallel.
+    cleanup
+        Whether to clean up the `run_folder` before running the pipeline.
+
+    """
+    validate_consistent_axes(pipeline.mapspecs(ordered=False))
+    run_folder = _ensure_run_folder(run_folder)
+    run_info = RunInfo.create(run_folder, pipeline, inputs, internal_shapes, cleanup=cleanup)
     run_info.dump(run_folder)
     outputs = []
     for gen in pipeline.topological_generations[1]:
         # These evaluations *can* happen in parallel
         for func in gen:
             _outputs = _run_function(func, run_folder, parallel)
             outputs.extend(_outputs)
     return outputs
 
 
-def load_outputs(
-    *output_names: str,
-    run_folder: str | Path,
-) -> Any:
+def load_outputs(*output_names: str, run_folder: str | Path) -> Any:
     """Load the outputs of a run."""
     run_folder = Path(run_folder)
     run_info = RunInfo.load(run_folder)
     outputs = [
         _load_parameter(
             on,
             run_info.input_paths,
             run_info.shapes,
-            run_info.manual_shapes,
+            run_info.shape_masks,
             run_folder,
         )
         for on in output_names
     ]
     outputs = [_maybe_load_file_array(o) for o in outputs]
     return outputs[0] if len(output_names) == 1 else outputs
```

### Comparing `pipefunc-0.8.0/pipefunc/map/adaptive.py` & `pipefunc-0.9.0/pipefunc/map/adaptive.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 from pipefunc.map._run import (
     RunInfo,
     _execute_single,
     _func_kwargs,
     _init_file_arrays,
     _maybe_load_single_output,
     _MockPipeline,
-    _run_iteration_and_pick_output,
-    _update_file_array,
+    _run_iteration_and_process,
     run,
 )
 
 if TYPE_CHECKING:
     import sys
 
     from pipefunc import PipeFunc, Pipeline, Sweep
@@ -37,15 +36,15 @@
 _OUTPUT_TYPE: TypeAlias = Union[str, Tuple[str, ...]]
 
 
 def create_learners(
     pipeline: Pipeline,
     inputs: dict[str, Any],
     run_folder: str | Path,
-    manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
+    internal_shapes: dict[str, int | tuple[int, ...]] | None = None,
     *,
     return_output: bool = False,
     cleanup: bool = True,
 ) -> list[dict[_OUTPUT_TYPE, adaptive.SequenceLearner]]:
     """Create adaptive learners for a single `Pipeline.map` call.
 
     Creates a learner for each function node in the graph. Which means that
@@ -57,36 +56,36 @@
     ----------
     pipeline
         The pipeline to create learners for.
     inputs
         The inputs to the pipeline, the same as passed to `pipeline.map`.
     run_folder
         The folder to store the run information.
-    manual_shapes
-        The manual shapes to use for the run.
+    internal_shapes
+        The internal shapes to use for the run.
     return_output
         Whether to return the output of the function in the learner.
     cleanup
         Whether to clean up the `run_folder`.
 
     Returns
     -------
     A list of dictionaries where the keys are the output names of the
     functions and the values are the corresponding adaptive learners. As noted
     above, the learners have to be executed in order.
 
     """
     run_folder = Path(run_folder)
-    run_info = RunInfo.create(run_folder, pipeline, inputs, manual_shapes, cleanup=cleanup)
+    run_info = RunInfo.create(run_folder, pipeline, inputs, internal_shapes, cleanup=cleanup)
     run_info.dump(run_folder)
     learners = []
     for gen in pipeline.topological_generations[1]:
         _learners = {}
         for func in gen:
-            if func.mapspec:
+            if func.mapspec and func.mapspec.inputs:
                 f = functools.partial(
                     _execute_iteration_in_map_spec,
                     func=func,
                     run_info=run_info,
                     run_folder=run_folder,
                     return_output=return_output,
                 )
@@ -128,15 +127,15 @@
     output, exists = _maybe_load_single_output(func, run_folder, return_output=return_output)
     if exists:
         return output
     kwargs = _func_kwargs(
         func,
         run_info.input_paths,
         run_info.shapes,
-        run_info.manual_shapes,
+        run_info.shape_masks,
         run_folder,
     )
     result = _execute_single(func, kwargs, run_folder)
     return result if return_output else None
 
 
 def _execute_iteration_in_map_spec(
@@ -152,66 +151,66 @@
     Performs a single iteration of the code in `_execute_map_spec`, however,
     it does not keep and return the output. This is meant to be used in the
     parallel execution of the map spec.
 
     Meets the requirements of `adaptive.SequenceLearner`.
     """
     shape = run_info.shapes[func.output_name]
-    file_arrays = _init_file_arrays(func.output_name, shape, run_folder)
+    mask = run_info.shape_masks[func.output_name]
+    file_arrays = _init_file_arrays(func.output_name, shape, mask, run_folder)
     # Load the data if it exists
     if all(arr.has_index(index) for arr in file_arrays):
         if not return_output:
             return None
         return [arr.get_from_index(index) for arr in file_arrays]
     # Otherwise, run the function
     assert isinstance(func.mapspec, MapSpec)
     kwargs = _func_kwargs(
         func,
         run_info.input_paths,
         run_info.shapes,
-        run_info.manual_shapes,
+        run_info.shape_masks,
         run_folder,
     )
-    outputs = _run_iteration_and_pick_output(index, func, kwargs, shape)
-    _update_file_array(func, file_arrays, shape, index, outputs)
+    outputs = _run_iteration_and_process(index, func, kwargs, shape, mask, file_arrays)
     return outputs if return_output else None
 
 
 @dataclass
 class _MapWrapper:
     """Wraps the `pipefunc.map.run` function and makes it a callable with a single unused argument.
 
     Uses a `_MockPipeline` that contains all the required information to run the pipeline but is
     cheaper to serialize and pass around.
     """
 
     mock_pipeline: _MockPipeline
     inputs: dict[str, Any]
     run_folder: Path
-    manual_shapes: dict[str, int | tuple[int, ...]] | None
+    internal_shapes: dict[str, int | tuple[int, ...]] | None
     parallel: bool
     cleanup: bool
 
     def __call__(self, _: Any) -> None:
         """Run the pipeline."""
         run(
             self.mock_pipeline,  # type: ignore[arg-type]
             self.inputs,
             self.run_folder,
-            self.manual_shapes,
+            self.internal_shapes,
             parallel=self.parallel,
             cleanup=self.cleanup,
         )
 
 
 def create_learners_from_sweep(
     pipeline: Pipeline,
     sweep: Sweep,
     run_folder: str | Path,
-    manual_shapes: dict[str, int | tuple[int, ...]] | None = None,
+    internal_shapes: dict[str, int | tuple[int, ...]] | None = None,
     *,
     parallel: bool = True,
     cleanup: bool = True,
 ) -> tuple[list[adaptive.SequenceLearner], list[Path]]:
     """Create adaptive learners for a sweep.
 
     Creates an `adaptive.SequenceLearner` for each sweep run. These learners
@@ -230,16 +229,16 @@
         The pipeline to create learners for.
     sweep
         The sweep to create learners for, must generate `input` dictionaries as
         expected by `pipeline.map`.
     run_folder
         The folder to store the run information. Each sweep run will be stored in
         a subfolder of this folder.
-    manual_shapes
-        The manual shapes to use for the run, as expected by `pipeline.map`.
+    internal_shapes
+        The internal shapes to use for the run, as expected by `pipeline.map`.
     parallel
         Whether to run the map in parallel.
     cleanup
         Whether to clean up the `run_folder`.
 
     Returns
     -------
@@ -250,12 +249,12 @@
     run_folder = Path(run_folder)
     learners = []
     folders = []
     max_digits = len(str(len(sweep) - 1))
     for i, inputs in enumerate(sweep):
         sweep_run = run_folder / f"sweep_{str(i).zfill(max_digits)}"
         mock_pipeline = _MockPipeline.from_pipeline(pipeline)
-        f = _MapWrapper(mock_pipeline, inputs, sweep_run, manual_shapes, parallel, cleanup)
+        f = _MapWrapper(mock_pipeline, inputs, sweep_run, internal_shapes, parallel, cleanup)
         learner = adaptive.SequenceLearner(f, sequence=[None])
         learners.append(learner)
         folders.append(sweep_run)
     return learners, folders
```

### Comparing `pipefunc-0.8.0/pipefunc.egg-info/PKG-INFO` & `pipefunc-0.9.0/pipefunc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipefunc
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Python library for defining, managing, and executing function pipelines.
 Maintainer-email: Bas Nijholt <bas@nijho.lt>
 License: MIT
 Project-URL: homepage, https://pipefunc.readthedocs.io/
 Project-URL: documentation, https://pipefunc.readthedocs.io/
 Project-URL: repository, https://github.com/basnijholt/pipefunc
 Classifier: Development Status :: 4 - Beta
@@ -90,38 +90,36 @@
 - [:hammer_and_wrench: Development](#hammer_and_wrench-development)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 <!-- toc-end -->
 
 ## :thinking: What is this?
 
-`pipefunc` is a Python library that simplifies the creation and management of complex function pipelines. It allows you to declare the dependencies between functions and automatically organizes the execution order to satisfy these dependencies.
-
-`pipefunc` provides a range of features to streamline your workflow, including pipeline visualization, flexible function arguments, support for multiple outputs, pipeline simplification, resource usage profiling, parallel execution, caching, and parameter sweep utilities.
+`pipefunc` is a Python library for creating and running function pipelines. By annotating functions and specifying their outputs, it forms a pipeline that automatically organizes the execution order to satisfy dependencies. Just specify the names of the outputs you want to compute, and `pipefunc` will handle the rest by leveraging the parameter names of the annotated functions.
 
 Whether you're working with data processing, scientific computations, machine learning (AI) workflows, or any other scenario involving interdependent functions, `pipefunc` helps you focus on the logic of your code while it handles the intricacies of function dependencies and execution order.
 
 ## :rocket: Key Features
 
-1. 🚀 **Function Composition and Pipelining**: Create pipelines where the output of one function feeds into another, with `pipefunc` handling the execution order.
+1. 🚀 **Function Composition and Pipelining**: Create pipelines by using the `@pipefunc` decorator; execution order is automatically handled.
 2. 📊 **Pipeline Visualization**: Generate visual graphs of your pipelines to better understand the flow of data.
-3. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
-4. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
-5. 🔁 **Map-Reduce Support**: Utilize "fan-out" to distribute tasks and "fan-in" to aggregate results, streamlining data processing in distributed environments.
-6. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
-7. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
-8. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
-9. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
-10. 🛠️ **Flexibility and Ease of Use**: Manage complex function dependencies in a clear, intuitive way with this lightweight yet powerful tool.
+3. 👥 **Multiple Outputs**: Handle functions that return multiple results, allowing each result to be used as input to other functions.
+4. 🔁 **Map-Reduce Support**: Perform "map" operations to apply functions over data and "reduce" operations to aggregate results, allowing n-dimensional mappings.
+5. ➡️ **Pipeline Simplification**: Merge nodes in complex pipelines to improve computational efficiency, trading off visibility into intermediate steps.
+6. 🎛️ **Resource Usage Profiling**: Get reports on CPU usage, memory consumption, and execution time to identify bottlenecks and optimize your code.
+7. 🔄 **Parallel Execution and Caching**: Run functions in parallel and cache results to avoid redundant computations.
+8. 🔍 **Parameter Sweep Utilities**: Generate parameter combinations for parameter sweeps and optimize the sweeps with result caching.
+9. 💡 **Flexible Function Arguments**: Call functions with different argument combinations, letting `pipefunc` determine which other functions to call based on the provided arguments.
+10. 🏗️ **Leverages giants**: Builds on top of [NetworkX](https://networkx.org/) for graph algorithms and [NumPy](https://numpy.org/) for n-dimensional arrays.
 
 ## :test_tube: How does it work?
 
 pipefunc provides a Pipeline class that you use to define your function pipeline.
-You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify a function's output name and dependencies.
-Once your pipeline is defined, you can execute it for specific output values, simplify it by combining functions with the same root arguments, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
+You add functions to the pipeline using the `pipefunc` decorator, which also lets you specify the function's output name.
+Once your pipeline is defined, you can execute it for specific output values, simplify it by combining function nodes, visualize it as a directed graph, and profile the resource usage of the pipeline functions.
 For more detailed usage instructions and examples, please check the usage example provided in the package.
 
 Here is a simple example usage of pipefunc to illustrate its primary features:
 
 ```python
 from pipefunc import pipefunc, Pipeline
 
@@ -135,38 +133,66 @@
     return b * c
 
 @pipefunc(output_name="e")
 def f_e(c, d, x=1):
     return c * d * x
 
 # Create a pipeline with these functions
-funcs = [f_c, f_d, f_e]
-pipeline = Pipeline(funcs, profile=True)
+pipeline = Pipeline([f_c, f_d, f_e], profile=True)  # `profile=True` enables resource profiling
+
+# Call the pipeline directly for different outputs:
+assert pipeline("d", a=2, b=3) == 15
+assert pipeline("e", a=2, b=3, x=1) == 75
 
-# You can access and call these functions using the func method
+# Or create a new function for a specific output
 h_d = pipeline.func("d")
 assert h_d(a=2, b=3) == 15
 
 h_e = pipeline.func("e")
 assert h_e(a=2, b=3, x=1) == 75
+# Instead of providing the root arguments, you can also provide the intermediate results directly
 assert h_e(c=5, d=15, x=1) == 75
 
 # Visualize the pipeline
 pipeline.visualize()
 
 # Get all possible argument mappings for each function
 all_args = pipeline.all_arg_combinations
 print(all_args)
 
 # Show resource reporting (only works if profile=True)
 pipeline.resources_report()
 ```
 
 This example demonstrates defining a pipeline with `f_c`, `f_d`, `f_e` functions, accessing and executing these functions using the pipeline, visualizing the pipeline graph, getting all possible argument mappings, and reporting on the resource usage.
-This basic example should give you an idea of how to use pipefunc to construct and manage function pipelines.
+This basic example should give you an idea of how to use `pipefunc` to construct and manage function pipelines.
+
+The following example demonstrates how to perform a map-reduce operation using `pipefunc`:
+
+```python
+from pipefunc import pipefunc, Pipeline
+from pipefunc.map import load_outputs
+import numpy as np
+
+@pipefunc(output_name="c", mapspec="a[i], b[j] -> c[i, j]")  # the mapspec is used to specify the mapping
+def f(a: int, b: int):
+    return a + b
+
+@pipefunc(output_name="mean")  # there is no mapspec, so this function takes the full 2D array
+def g(c: np.ndarray):
+    return np.mean(c)
+
+pipeline = Pipeline([f, g])
+inputs = {"a": [1, 2, 3], "b": [4, 5, 6]}
+pipeline.map(inputs, run_folder="my_run_folder", parallel=True)
+result = load_outputs("mean", run_folder="my_run_folder")
+print(result)  # prints 7.0
+```
+
+Here the `mapspec` argument is used to specify the mapping between the inputs and outputs of the `f` function, it creates the product of the `a` and `b` input lists and computes the sum of each pair. The `g` function then computes the mean of the resulting 2D array. The `map` method executes the pipeline for the `inputs`, and the `load_outputs` function is used to load the results of the `g` function from the specified run folder.
 
 ## :notebook: Jupyter Notebook Example
 
 See the detailed usage example and more in our [example.ipynb](https://github.com/basnijholt/pipefunc/blob/main/example.ipynb).
 
 ## :computer: Installation
```

### Comparing `pipefunc-0.8.0/pipefunc.egg-info/SOURCES.txt` & `pipefunc-0.9.0/pipefunc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/pyproject.toml` & `pipefunc-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/tests/test_cache.py` & `pipefunc-0.9.0/tests/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,18 @@
 @pytest.mark.parametrize("shared", [True, False])
 def test_hybrid_cache_expire(shared):
     cache = HybridCache(max_size=3, shared=shared)
     cache.put("key1", "value1", 1.0)
     cache.put("key2", "value2", 2.0)
     cache.put("key3", "value3", 3.0)
     cache.put("key4", "value4", 4.0)
-    assert "key1" not in cache, cache.cache
-    assert "key4" in cache, cache.cache
+    assert "key1" not in cache
+    assert "key4" in cache
+    assert len(cache) == 3
+    assert len(cache.cache) == 3
 
 
 @pytest.mark.parametrize("shared", [True, False])
 def test_hybrid_cache_str(shared):
     cache = HybridCache(max_size=3, shared=shared, allow_cloudpickle=False)
     cache.put("key1", "value1", 2.0)
     assert "Cache: {'key1': 'value1'}" in str(cache)
@@ -137,15 +139,15 @@
     cache = LRUCache(max_size=2, shared=shared)
     cache.put("test", "value")
     assert "test" in cache
 
 
 @pytest.mark.parametrize("shared", [True, False])
 def test_cache_property(shared):
-    cache = LRUCache(max_size=2, shared=shared, allow_cloudpickle=False)
+    cache = LRUCache(max_size=2, shared=shared, allow_cloudpickle=True)
     cache.put("test", "value")
     cache_dict = cache.cache
     assert cache_dict == {"test": "value"}
 
 
 @pytest.fixture()
 def cache_dir(tmp_path):
@@ -256,21 +258,22 @@
     assert len(cache) == 2
     assert len(cache.lru_cache) == 2
     cache.clear()
     assert len(cache) == 0
     assert len(cache.lru_cache) == 0
 
 
-def test_file_cache_put_and_get_none(cache_dir):
-    cache = DiskCache(cache_dir=str(cache_dir), with_lru_cache=True)
+@pytest.mark.parametrize("shared", [True, False])
+def test_file_cache_put_and_get_none(cache_dir, shared: bool):  # noqa: FBT001
+    cache = DiskCache(cache_dir=str(cache_dir), with_lru_cache=True, lru_shared=shared)
     cache.put("key1", None)
     assert cache.get("key1") is None
     assert "key1" in cache
     assert "key1" in cache.lru_cache
-    assert cache.cache["key1"] == "__ReturnsNone__"
+    assert cache.cache["key1"] is None
 
 
 @pytest.mark.parametrize("shared", [True, False])
 def test_hybrid_cache_clear(shared):
     cache = HybridCache(max_size=3, shared=shared)
     cache.put("key1", "value1", 2.0)
     cache.put("key2", "value2", 3.0)
```

### Comparing `pipefunc-0.8.0/tests/test_dag.py` & `pipefunc-0.9.0/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/tests/test_perf.py` & `pipefunc-0.9.0/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/tests/test_pipefunc.py` & `pipefunc-0.9.0/tests/test_pipefunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,15 @@
 import inspect
 import pickle
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 import pytest
 
-from pipefunc import (
-    PipeFunc,
-    Pipeline,
-    Sweep,
-    count_sweep,
-    get_precalculation_order,
-    pipefunc,
-)
+from pipefunc import PipeFunc, Pipeline, Sweep, count_sweep, get_precalculation_order, pipefunc
 from pipefunc.exceptions import UnusedParametersError
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 def test_pipeline_and_all_arg_combinations() -> None:
@@ -177,17 +170,16 @@
     def f(a, b=1):
         return a + b
 
     @pipefunc(output_name="y")
     def g(c, b=2):
         return c * b
 
-    p = Pipeline([f, g])
     with pytest.raises(ValueError, match="Inconsistent default values"):
-        _ = p.graph
+        Pipeline([f, g])
 
 
 def test_output_name_in_kwargs():
     @pipefunc(output_name="c")
     def f(a, b):
         return a + b
 
@@ -677,7 +669,33 @@
     func2 = pickle.loads(p)  # noqa: S301
     assert func(1, 2) == func2(1, 2)
 
     func = PipeFunc(DataClass, output_name="c")
     p = pickle.dumps(func)
     func2 = pickle.loads(p)  # noqa: S301
     assert func(a=1) == func2(a=1)
+
+
+def test_independent_axes_in_mapspecs_with_disconnected_chains():
+    @pipefunc(output_name="c", mapspec="a[i] -> c[i]")
+    def f(a: int, b: int):
+        return a + b
+
+    @pipefunc(output_name="z", mapspec="x[i], y[i] -> z[i]")
+    def g(x, y):
+        return x + y
+
+    pipeline = Pipeline([f, g])
+    assert pipeline.mapspecs_as_strings() == [
+        "a[i] -> c[i]",
+        "x[i], y[i] -> z[i]",
+    ]
+
+    pipeline.add_mapspec_axis("b", axis="j")
+    assert pipeline.mapspecs_as_strings() == ["a[i], b[j] -> c[i, j]", "x[i], y[i] -> z[i]"]
+
+    pipeline.add_mapspec_axis("x", axis="j")
+    pipeline.add_mapspec_axis("y", axis="j")
+    assert pipeline.mapspecs_as_strings() == [
+        "a[i], b[j] -> c[i, j]",
+        "x[i, j], y[i, j] -> z[i, j]",
+    ]
```

### Comparing `pipefunc-0.8.0/tests/test_simplify.py` & `pipefunc-0.9.0/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `pipefunc-0.8.0/tests/test_sweep.py` & `pipefunc-0.9.0/tests/test_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from itertools import product
 
 import pytest
 
 from pipefunc import Pipeline, pipefunc
-from pipefunc._sweep import (
-    MultiSweep,
-    Sweep,
-    count_sweep,
-    generate_sweep,
-    set_cache_for_sweep,
-)
+from pipefunc._sweep import MultiSweep, Sweep, count_sweep, generate_sweep, set_cache_for_sweep
 
 
 @pytest.fixture()
 def pipeline():
     @pipefunc(output_name="c")
     def f1(a, b):
         return a + b
```

### Comparing `pipefunc-0.8.0/tests/test_utils.py` & `pipefunc-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

