# Comparing `tmp/capslock-1.0.8.tar.gz` & `tmp/capslock-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/capslock-1.0.8.tar", last modified: Sat Mar  6 07:12:23 2021, max compression
+gzip compressed data, was "capslock-2.0.1.tar", last modified: Sat May 25 17:28:12 2024, max compression
```

## Comparing `capslock-1.0.8.tar` & `capslock-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 faruk     (1000) faruk     (1000)        0 2021-03-06 07:12:23.524384 capslock-1.0.8/
--rw-rw-r--   0 faruk     (1000) faruk     (1000)     5727 2021-03-06 07:12:23.520384 capslock-1.0.8/PKG-INFO
--rw-rw-r--   0 faruk     (1000) faruk     (1000)     4134 2021-03-06 07:09:49.000000 capslock-1.0.8/README.md
-drwxrwxr-x   0 faruk     (1000) faruk     (1000)        0 2021-03-06 07:12:23.520384 capslock-1.0.8/capslock/
--rw-rw-r--   0 faruk     (1000) faruk     (1000)      238 2021-03-06 07:09:49.000000 capslock-1.0.8/capslock/__init__.py
--rw-rw-r--   0 faruk     (1000) faruk     (1000)     3919 2021-03-06 07:09:49.000000 capslock-1.0.8/capslock/decorators.py
--rw-rw-r--   0 faruk     (1000) faruk     (1000)     2672 2021-03-06 07:09:49.000000 capslock-1.0.8/capslock/utils.py
-drwxrwxr-x   0 faruk     (1000) faruk     (1000)        0 2021-03-06 07:12:23.520384 capslock-1.0.8/capslock.egg-info/
--rw-rw-r--   0 faruk     (1000) faruk     (1000)     5727 2021-03-06 07:12:23.000000 capslock-1.0.8/capslock.egg-info/PKG-INFO
--rw-rw-r--   0 faruk     (1000) faruk     (1000)      239 2021-03-06 07:12:23.000000 capslock-1.0.8/capslock.egg-info/SOURCES.txt
--rw-rw-r--   0 faruk     (1000) faruk     (1000)        1 2021-03-06 07:12:23.000000 capslock-1.0.8/capslock.egg-info/dependency_links.txt
--rw-rw-r--   0 faruk     (1000) faruk     (1000)       17 2021-03-06 07:12:23.000000 capslock-1.0.8/capslock.egg-info/requires.txt
--rw-rw-r--   0 faruk     (1000) faruk     (1000)        9 2021-03-06 07:12:23.000000 capslock-1.0.8/capslock.egg-info/top_level.txt
--rw-rw-r--   0 faruk     (1000) faruk     (1000)       38 2021-03-06 07:12:23.524384 capslock-1.0.8/setup.cfg
--rw-rw-r--   0 faruk     (1000) faruk     (1000)      748 2021-03-06 07:11:27.000000 capslock-1.0.8/setup.py
+drwxr-xr-x   0 faruk      (501) staff       (20)        0 2024-05-25 17:28:12.952884 capslock-2.0.1/
+-rw-r--r--   0 faruk      (501) staff       (20)     1420 2024-05-25 17:00:34.000000 capslock-2.0.1/LICENSE
+-rw-r--r--   0 faruk      (501) staff       (20)       56 2024-05-25 17:26:14.000000 capslock-2.0.1/MANIFEST.in
+-rw-r--r--   0 faruk      (501) staff       (20)     5384 2024-05-25 17:28:12.952702 capslock-2.0.1/PKG-INFO
+-rw-r--r--   0 faruk      (501) staff       (20)     4819 2024-05-25 17:16:40.000000 capslock-2.0.1/README.md
+drwxr-xr-x   0 faruk      (501) staff       (20)        0 2024-05-25 17:28:12.951714 capslock-2.0.1/capslock/
+-rw-r--r--   0 faruk      (501) staff       (20)      283 2024-05-25 17:06:11.000000 capslock-2.0.1/capslock/__init__.py
+-rw-r--r--   0 faruk      (501) staff       (20)     4705 2024-05-25 17:22:12.000000 capslock-2.0.1/capslock/decorators.py
+-rw-r--r--   0 faruk      (501) staff       (20)     2672 2024-05-25 17:00:34.000000 capslock-2.0.1/capslock/utils.py
+drwxr-xr-x   0 faruk      (501) staff       (20)        0 2024-05-25 17:28:12.952492 capslock-2.0.1/capslock.egg-info/
+-rw-r--r--   0 faruk      (501) staff       (20)     5384 2024-05-25 17:28:12.000000 capslock-2.0.1/capslock.egg-info/PKG-INFO
+-rw-r--r--   0 faruk      (501) staff       (20)      259 2024-05-25 17:28:12.000000 capslock-2.0.1/capslock.egg-info/SOURCES.txt
+-rw-r--r--   0 faruk      (501) staff       (20)        1 2024-05-25 17:28:12.000000 capslock-2.0.1/capslock.egg-info/dependency_links.txt
+-rw-r--r--   0 faruk      (501) staff       (20)       24 2024-05-25 17:28:12.000000 capslock-2.0.1/capslock.egg-info/requires.txt
+-rw-r--r--   0 faruk      (501) staff       (20)        9 2024-05-25 17:28:12.000000 capslock-2.0.1/capslock.egg-info/top_level.txt
+-rw-r--r--   0 faruk      (501) staff       (20)       38 2024-05-25 17:28:12.952921 capslock-2.0.1/setup.cfg
+-rw-r--r--   0 faruk      (501) staff       (20)      758 2024-05-25 17:27:37.000000 capslock-2.0.1/setup.py
```

### Comparing `capslock-1.0.8/PKG-INFO` & `capslock-2.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,173 @@
 Metadata-Version: 2.1
 Name: capslock
-Version: 1.0.8
+Version: 2.0.1
 Summary: A utility python library for writing certain tasks in python easily & elegantly.
 Home-page: https://github.com/faruk-ahmad/capslock
 Author: Faruk Ahmad
 Author-email: faruk.csebrur@gmail.com
 License: MIT
-Description: # CAPSLOCK
-        ----------------------------------------------
-        #### A utility python library for writing certain tasks in python easily & elegantly.
-        -----------------------------------------------
-        [The library is still in development. The doc is not completed yet. You can contribute to improve the library.]
-        ## Background
-        <p align= "justify">
-        
-        ```capslock``` is a high level utility library written in python for writing certain frequently needed task in faster & efficient way. For example, if you want to keep track of the execution time of one of your method while optimizing it, witing code for tracking execution time can be done easily using capslock.
-        </p>
-        
-        --------------------------------------------------
-        
-        
-        ## Installation
-        Install using the following command - 
-        ```bash
-        pip install capslock
-        ```
-        
-        Uninstall using the following command - 
-        ```bash
-        pip uninstall capslock
-        ```
-        
-        ## Getting Started
-        
-        ### How to use decorators from capslock
-        
-        Capslock defines different decorators that can be used out of the box for certain frequent tasks. E.g. getting the run time of certain function over the period of optimization in development phase.
-        
-        ### Timing Decorator
-        
-        To keep track of the execution time of a function in your project for optimizing it over the time, just put the "timing" decorator in your desired function. Capslock will keep track of different run of that function and will plot a well visualized graph for last five execution time of that function.
-        
-        ```python
-        from capslock import timing
-        
-        @timing(plot=True)
-        def say_hello():
-            print("Hello World")
-        
-        if __name__ == '__main__':
-            say_hello()
-        ```
-        This will generate output like bellow: 
-        
-        ![Output of Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/output_1.png)
-        
-        And it will also keep track of runtime for different runs of the ```say_hello()``` function. and will plot a graph in the same directory of your python script if you set ```plot=True```, otherwise the plot flag is by default ```False```.
-        
-        ![Runtime tracking using Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/say_hello.png)
-        
-        
-        ### Debug Decorator
-        
-        To get debug information of anyof your function, follow the bellow instruction-
-        
-        ```python
-        from capslock import debug
-        
-        @debug
-        def add(number1, number2):
-            return number1 + number2
-        
-        if __name__ == '__main__':
-            print(add(20, 30))
-        ```
-        
-        will provide you the following output with some debug information-
-        
-        ![Debug Information using Capslock Debug Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/debug.png)
-        
-        
-        ### Run Multiple Times Decorator
-        
-        To run a function multiple times, use the ```run_multiple_times``` decorator from capslock package.
-        
-        ```python
-        from datetime import datetime
-        from capslock import run_multiple_times
-        
-        @run_multiple_times(times=10)
-        def current_time():
-            now = datetime.now()
-            return now.strftime("%H:%M:%S.%f")
-        
-        if __name__ == '__main__':
-            print(current_time())
-        ```
-        
-        will run the current time function 10 times.
-        
-        
-        ### Require Root previllege Decorator
-        
-        If you want to prevent some accidental execution of a certain part of code
-        that might cause system-wide changes and you wish the user to have root
-        previllege before running that part of the python code, just use the
-        ```require_root``` decorator from capslock.
-        
-        ```python
-        from capslock import require_root
-        
-        @require_root
-        def say_hello():
-            for _ in range(10):
-                print("Hello World")
-        
-        
-        if __name__ == '__main__':
-            say_hello()
-        ```
-        
-        Now, ```say_hello()``` will only run, if the user is root.
-        
-        ### Color your function output decorator
-        If you want to see your function output as colorful this method might help you to color your function output.
-        At present this method support these colors `BLUE, CYAN, GREEN, YELLOW, RED, BOLD, UNDERLINE`
-        
-        ```py
-        from capslock import color_output
-        
-        @color_output("RED")
-        def hello_color():
-            return "Hey! How are you!"
-        
-        if __name__ == '__main__':
-            hello_color()
-        
-        ```
-        
-        
-        ## How to Contribute
-        
-        You can contribute in different ways. You can add more decorators for frequently used tasks in day to day development works.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: psutil
+
+# CAPSLOCK
+----------------------------------------------
+#### A utility python library for writing certain tasks in python easily & elegantly.
+-----------------------------------------------
+[The library is still in development. The doc is not completed yet. You can contribute to improve the library.]
+## Background
+<p align= "justify">
+
+```capslock``` is a high level utility library written in python for writing certain frequently needed task in faster & efficient way. For example, if you want to keep track of the execution time of one of your method while optimizing it, witing code for tracking execution time can be done easily using capslock.
+</p>
+
+--------------------------------------------------
+
+
+## Installation
+Install using the following command - 
+```bash
+pip install capslock
+```
+
+Uninstall using the following command - 
+```bash
+pip uninstall capslock
+```
+
+## Getting Started
+
+### How to use decorators from capslock
+
+Capslock defines different decorators that can be used out of the box for certain frequent tasks. E.g. getting the run time of certain function over the period of optimization in development phase.
+
+### Timing Decorator
+
+To keep track of the execution time of a function in your project for optimizing it over the time, just put the "timing" decorator in your desired function. Capslock will keep track of different run of that function and will plot a well visualized graph for last five execution time of that function.
+
+```python
+from capslock import timing
+
+@timing(plot=True)
+def say_hello():
+    print("Hello World")
+
+if __name__ == '__main__':
+    say_hello()
+```
+This will generate output like bellow: 
+
+![Output of Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/output_1.png)
+
+And it will also keep track of runtime for different runs of the ```say_hello()``` function. and will plot a graph in the same directory of your python script if you set ```plot=True```, otherwise the plot flag is by default ```False```.
+
+![Runtime tracking using Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/say_hello.png)
+
+
+### Debug Decorator
+
+To get debug information of anyof your function, follow the bellow instruction-
+
+```python
+from capslock import debug
+
+@debug
+def add(number1, number2):
+    return number1 + number2
+
+if __name__ == '__main__':
+    print(add(20, 30))
+```
+
+will provide you the following output with some debug information-
+
+![Debug Information using Capslock Debug Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/debug.png)
+
+
+### Run Multiple Times Decorator
+
+To run a function multiple times, use the ```run_multiple_times``` decorator from capslock package.
+
+```python
+from datetime import datetime
+from capslock import run_multiple_times
+
+@run_multiple_times(times=10)
+def current_time():
+    now = datetime.now()
+    return now.strftime("%H:%M:%S.%f")
+
+if __name__ == '__main__':
+    print(current_time())
+```
+
+will run the current time function 10 times.
+
+
+### Require Root previllege Decorator
+
+If you want to prevent some accidental execution of a certain part of code
+that might cause system-wide changes and you wish the user to have root
+previllege before running that part of the python code, just use the
+```require_root``` decorator from capslock.
+
+```python
+from capslock import require_root
+
+@require_root
+def say_hello():
+    for _ in range(10):
+        print("Hello World")
+
+
+if __name__ == '__main__':
+    say_hello()
+```
+
+Now, ```say_hello()``` will only run, if the user is root.
+
+### Color your function output decorator
+If you want to see your function output as colorful this method might help you to color your function output.
+At present this method support these colors `BLUE, CYAN, GREEN, YELLOW, RED, BOLD, UNDERLINE`
+
+```py
+from capslock import color_output
+
+@color_output("RED")
+def hello_color():
+    return "Hey! How are you!"
+
+if __name__ == '__main__':
+    hello_color()
+
+```
+
+### Restrict Memory check before Memory intensive workload function execution
+If you have a memory intensive workload function and you know the minimum memory requriement, 
+you can restrict the fucntion execution by checking the available memory in that system beforehand
+by using this decorator.
+
+```py
+from capslock import requires_ram
+
+@requires_ram(8)
+def memory_intensive_task():
+    print("Running a memory-intensive task...")
+
+
+if __name__ == '__main__':
+    memory_intensive_task()
+
+```
+If the system has less memory than mentioned in the decorator, the function will not execute.
+E.g., in the above example, if the system has 8 GB or more RAM, then the function will execute.
+
+## How to Contribute
+
+You can contribute in different ways. You can add more decorators for frequently used tasks in day to day development works.
```

### Comparing `capslock-1.0.8/capslock/decorators.py` & `capslock-2.0.1/capslock/decorators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 This module introduces some decorators that can
 be used for some frequent tasks.
 """
 
 import os
 import sys
+import psutil
 import functools
 import time
 import numpy as np
 from datetime import datetime
 
 from capslock.utils import BCOLOR
 from capslock.utils import read_timing_db, write_timing_db, plot_time
 
 
-
-
 def timing(_func=None, *, plot=False):
     """Return the runtime/execution time of the decorated function
     """
     def timing_decorator(func):
         @functools.wraps(func)
         def timing_decorator_wrapper(*args, **kwargs):
             start_time = time.perf_counter()
@@ -118,9 +117,29 @@
                 print(f"{mycolor}{str(value)}{bcolors.ENDC}")
             return value
         return color_decorator_wrapper
     if color is None:
         return color_decorator
     return color_decorator
 
+def requires_ram(min_ram_gb):
+    """
+    Decorator to check if the system has at least `min_ram_gb` GB of RAM.
+    If the system has less RAM, the function will not be executed.
+    
+    Parameters:
+    min_ram_gb (float): The minimum amount of RAM in gigabytes required to run the function.
+    """
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            total_ram_gb = psutil.virtual_memory().total / (1024 ** 3)
+            if total_ram_gb >= min_ram_gb:
+                return func(*args, **kwargs)
+            else:
+                print(f"Function '{func.__name__}' requires at least {min_ram_gb} GB of RAM. System has {total_ram_gb:.2f} GB.")
+                return None
+        return wrapper
+    return decorator
+
 if __name__ == '__main__':
     pass
```

### Comparing `capslock-1.0.8/capslock/utils.py` & `capslock-2.0.1/capslock/utils.py`

 * *Files identical despite different names*

### Comparing `capslock-1.0.8/capslock.egg-info/PKG-INFO` & `capslock-2.0.1/capslock.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,173 @@
 Metadata-Version: 2.1
 Name: capslock
-Version: 1.0.8
+Version: 2.0.1
 Summary: A utility python library for writing certain tasks in python easily & elegantly.
 Home-page: https://github.com/faruk-ahmad/capslock
 Author: Faruk Ahmad
 Author-email: faruk.csebrur@gmail.com
 License: MIT
-Description: # CAPSLOCK
-        ----------------------------------------------
-        #### A utility python library for writing certain tasks in python easily & elegantly.
-        -----------------------------------------------
-        [The library is still in development. The doc is not completed yet. You can contribute to improve the library.]
-        ## Background
-        <p align= "justify">
-        
-        ```capslock``` is a high level utility library written in python for writing certain frequently needed task in faster & efficient way. For example, if you want to keep track of the execution time of one of your method while optimizing it, witing code for tracking execution time can be done easily using capslock.
-        </p>
-        
-        --------------------------------------------------
-        
-        
-        ## Installation
-        Install using the following command - 
-        ```bash
-        pip install capslock
-        ```
-        
-        Uninstall using the following command - 
-        ```bash
-        pip uninstall capslock
-        ```
-        
-        ## Getting Started
-        
-        ### How to use decorators from capslock
-        
-        Capslock defines different decorators that can be used out of the box for certain frequent tasks. E.g. getting the run time of certain function over the period of optimization in development phase.
-        
-        ### Timing Decorator
-        
-        To keep track of the execution time of a function in your project for optimizing it over the time, just put the "timing" decorator in your desired function. Capslock will keep track of different run of that function and will plot a well visualized graph for last five execution time of that function.
-        
-        ```python
-        from capslock import timing
-        
-        @timing(plot=True)
-        def say_hello():
-            print("Hello World")
-        
-        if __name__ == '__main__':
-            say_hello()
-        ```
-        This will generate output like bellow: 
-        
-        ![Output of Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/output_1.png)
-        
-        And it will also keep track of runtime for different runs of the ```say_hello()``` function. and will plot a graph in the same directory of your python script if you set ```plot=True```, otherwise the plot flag is by default ```False```.
-        
-        ![Runtime tracking using Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/say_hello.png)
-        
-        
-        ### Debug Decorator
-        
-        To get debug information of anyof your function, follow the bellow instruction-
-        
-        ```python
-        from capslock import debug
-        
-        @debug
-        def add(number1, number2):
-            return number1 + number2
-        
-        if __name__ == '__main__':
-            print(add(20, 30))
-        ```
-        
-        will provide you the following output with some debug information-
-        
-        ![Debug Information using Capslock Debug Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/debug.png)
-        
-        
-        ### Run Multiple Times Decorator
-        
-        To run a function multiple times, use the ```run_multiple_times``` decorator from capslock package.
-        
-        ```python
-        from datetime import datetime
-        from capslock import run_multiple_times
-        
-        @run_multiple_times(times=10)
-        def current_time():
-            now = datetime.now()
-            return now.strftime("%H:%M:%S.%f")
-        
-        if __name__ == '__main__':
-            print(current_time())
-        ```
-        
-        will run the current time function 10 times.
-        
-        
-        ### Require Root previllege Decorator
-        
-        If you want to prevent some accidental execution of a certain part of code
-        that might cause system-wide changes and you wish the user to have root
-        previllege before running that part of the python code, just use the
-        ```require_root``` decorator from capslock.
-        
-        ```python
-        from capslock import require_root
-        
-        @require_root
-        def say_hello():
-            for _ in range(10):
-                print("Hello World")
-        
-        
-        if __name__ == '__main__':
-            say_hello()
-        ```
-        
-        Now, ```say_hello()``` will only run, if the user is root.
-        
-        ### Color your function output decorator
-        If you want to see your function output as colorful this method might help you to color your function output.
-        At present this method support these colors `BLUE, CYAN, GREEN, YELLOW, RED, BOLD, UNDERLINE`
-        
-        ```py
-        from capslock import color_output
-        
-        @color_output("RED")
-        def hello_color():
-            return "Hey! How are you!"
-        
-        if __name__ == '__main__':
-            hello_color()
-        
-        ```
-        
-        
-        ## How to Contribute
-        
-        You can contribute in different ways. You can add more decorators for frequently used tasks in day to day development works.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: matplotlib
+Requires-Dist: psutil
+
+# CAPSLOCK
+----------------------------------------------
+#### A utility python library for writing certain tasks in python easily & elegantly.
+-----------------------------------------------
+[The library is still in development. The doc is not completed yet. You can contribute to improve the library.]
+## Background
+<p align= "justify">
+
+```capslock``` is a high level utility library written in python for writing certain frequently needed task in faster & efficient way. For example, if you want to keep track of the execution time of one of your method while optimizing it, witing code for tracking execution time can be done easily using capslock.
+</p>
+
+--------------------------------------------------
+
+
+## Installation
+Install using the following command - 
+```bash
+pip install capslock
+```
+
+Uninstall using the following command - 
+```bash
+pip uninstall capslock
+```
+
+## Getting Started
+
+### How to use decorators from capslock
+
+Capslock defines different decorators that can be used out of the box for certain frequent tasks. E.g. getting the run time of certain function over the period of optimization in development phase.
+
+### Timing Decorator
+
+To keep track of the execution time of a function in your project for optimizing it over the time, just put the "timing" decorator in your desired function. Capslock will keep track of different run of that function and will plot a well visualized graph for last five execution time of that function.
+
+```python
+from capslock import timing
+
+@timing(plot=True)
+def say_hello():
+    print("Hello World")
+
+if __name__ == '__main__':
+    say_hello()
+```
+This will generate output like bellow: 
+
+![Output of Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/output_1.png)
+
+And it will also keep track of runtime for different runs of the ```say_hello()``` function. and will plot a graph in the same directory of your python script if you set ```plot=True```, otherwise the plot flag is by default ```False```.
+
+![Runtime tracking using Capslock Timing Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/say_hello.png)
+
+
+### Debug Decorator
+
+To get debug information of anyof your function, follow the bellow instruction-
+
+```python
+from capslock import debug
+
+@debug
+def add(number1, number2):
+    return number1 + number2
+
+if __name__ == '__main__':
+    print(add(20, 30))
+```
+
+will provide you the following output with some debug information-
+
+![Debug Information using Capslock Debug Decorator](https://raw.githubusercontent.com/faruk-ahmad/capslock/main/docs/debug.png)
+
+
+### Run Multiple Times Decorator
+
+To run a function multiple times, use the ```run_multiple_times``` decorator from capslock package.
+
+```python
+from datetime import datetime
+from capslock import run_multiple_times
+
+@run_multiple_times(times=10)
+def current_time():
+    now = datetime.now()
+    return now.strftime("%H:%M:%S.%f")
+
+if __name__ == '__main__':
+    print(current_time())
+```
+
+will run the current time function 10 times.
+
+
+### Require Root previllege Decorator
+
+If you want to prevent some accidental execution of a certain part of code
+that might cause system-wide changes and you wish the user to have root
+previllege before running that part of the python code, just use the
+```require_root``` decorator from capslock.
+
+```python
+from capslock import require_root
+
+@require_root
+def say_hello():
+    for _ in range(10):
+        print("Hello World")
+
+
+if __name__ == '__main__':
+    say_hello()
+```
+
+Now, ```say_hello()``` will only run, if the user is root.
+
+### Color your function output decorator
+If you want to see your function output as colorful this method might help you to color your function output.
+At present this method support these colors `BLUE, CYAN, GREEN, YELLOW, RED, BOLD, UNDERLINE`
+
+```py
+from capslock import color_output
+
+@color_output("RED")
+def hello_color():
+    return "Hey! How are you!"
+
+if __name__ == '__main__':
+    hello_color()
+
+```
+
+### Restrict Memory check before Memory intensive workload function execution
+If you have a memory intensive workload function and you know the minimum memory requriement, 
+you can restrict the fucntion execution by checking the available memory in that system beforehand
+by using this decorator.
+
+```py
+from capslock import requires_ram
+
+@requires_ram(8)
+def memory_intensive_task():
+    print("Running a memory-intensive task...")
+
+
+if __name__ == '__main__':
+    memory_intensive_task()
+
+```
+If the system has less memory than mentioned in the decorator, the function will not execute.
+E.g., in the above example, if the system has 8 GB or more RAM, then the function will execute.
+
+## How to Contribute
+
+You can contribute in different ways. You can add more decorators for frequently used tasks in day to day development works.
```

### Comparing `capslock-1.0.8/setup.py` & `capslock-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import codecs
 import setuptools
 
 
 setuptools.setup(
     name="capslock",
-    version="1.0.8",
+    version="2.0.1",
     author="Faruk Ahmad",
     author_email="faruk.csebrur@gmail.com",
     description="A utility python library for writing certain tasks in python easily & elegantly.",
     long_description=codecs.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/faruk-ahmad/capslock",
     license="MIT",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=['numpy', 'matplotlib'],
+    install_requires=['numpy', 'matplotlib', 'psutil'],
     python_requires='>=3.5',
     
 )
```

