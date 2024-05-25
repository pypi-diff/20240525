# Comparing `tmp/FlowVisor-0.2.2.tar.gz` & `tmp/FlowVisor-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.2.2.tar", last modified: Wed May 22 11:33:23 2024, max compression
+gzip compressed data, was "FlowVisor-0.2.3.tar", last modified: Sat May 25 13:19:45 2024, max compression
```

## Comparing `FlowVisor-0.2.2.tar` & `FlowVisor-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 11:33:23.414352 FlowVisor-0.2.2/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 11:33:23.410351 FlowVisor-0.2.2/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-22 11:33:23.000000 FlowVisor-0.2.2/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-22 11:33:23.000000 FlowVisor-0.2.2/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-22 11:33:23.000000 FlowVisor-0.2.2/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-22 11:33:23.000000 FlowVisor-0.2.2/FlowVisor.egg-info/entry_points.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-05-22 11:33:23.000000 FlowVisor-0.2.2/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-22 11:33:23.000000 FlowVisor-0.2.2/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.2.2/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-22 11:33:23.414352 FlowVisor-0.2.2/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     3055 2024-05-13 12:49:23.000000 FlowVisor-0.2.2/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 11:33:23.410351 FlowVisor-0.2.2/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.2.2/flowvisor/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-22 11:33:23.414352 FlowVisor-0.2.2/flowvisor/cli/
--rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.2.2/flowvisor/cli/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3199 2024-04-25 13:10:53.000000 FlowVisor-0.2.2/flowvisor/cli/add_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.2.2/flowvisor/cli/remove_vis.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     1194 2024-05-22 11:32:42.000000 FlowVisor-0.2.2/flowvisor/cli/vis_file.py
--rw-rw-r--   0 phil      (1000) phil      (1000)    15190 2024-05-22 11:32:32.000000 FlowVisor-0.2.2/flowvisor/flowvisor.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2350 2024-05-20 17:44:05.000000 FlowVisor-0.2.2/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8076 2024-05-22 09:41:15.000000 FlowVisor-0.2.2/flowvisor/flowvisor_verifier.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     8494 2024-05-13 10:38:59.000000 FlowVisor-0.2.2/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.2.2/flowvisor/logger.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.2.2/flowvisor/sankey.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.2.2/flowvisor/time_tracker.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2288 2024-05-20 18:08:09.000000 FlowVisor-0.2.2/flowvisor/time_value.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.2.2/flowvisor/timer.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.2.2/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-22 11:33:23.414352 FlowVisor-0.2.2/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.2.2/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:19:45.118070 FlowVisor-0.2.3/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:19:45.114070 FlowVisor-0.2.3/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-25 13:19:45.000000 FlowVisor-0.2.3/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      593 2024-05-25 13:19:45.000000 FlowVisor-0.2.3/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-05-25 13:19:45.000000 FlowVisor-0.2.3/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)      138 2024-05-25 13:19:45.000000 FlowVisor-0.2.3/FlowVisor.egg-info/entry_points.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-05-25 13:19:45.000000 FlowVisor-0.2.3/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-05-25 13:19:45.000000 FlowVisor-0.2.3/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.2.3/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3736 2024-05-25 13:19:45.118070 FlowVisor-0.2.3/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3055 2024-05-13 12:49:23.000000 FlowVisor-0.2.3/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:19:45.118070 FlowVisor-0.2.3/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)      221 2024-05-08 20:53:18.000000 FlowVisor-0.2.3/flowvisor/__init__.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-05-25 13:19:45.118070 FlowVisor-0.2.3/flowvisor/cli/
+-rw-rw-r--   0 phil      (1000) phil      (1000)        0 2024-04-25 10:31:43.000000 FlowVisor-0.2.3/flowvisor/cli/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3409 2024-05-25 13:12:32.000000 FlowVisor-0.2.3/flowvisor/cli/add_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2270 2024-04-25 13:16:50.000000 FlowVisor-0.2.3/flowvisor/cli/remove_vis.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1194 2024-05-22 11:32:42.000000 FlowVisor-0.2.3/flowvisor/cli/vis_file.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)    16152 2024-05-25 13:19:07.000000 FlowVisor-0.2.3/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2350 2024-05-20 17:44:05.000000 FlowVisor-0.2.3/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8076 2024-05-22 09:41:15.000000 FlowVisor-0.2.3/flowvisor/flowvisor_verifier.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     8494 2024-05-13 10:38:59.000000 FlowVisor-0.2.3/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      887 2024-05-13 06:45:56.000000 FlowVisor-0.2.3/flowvisor/logger.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2181 2024-05-08 16:32:50.000000 FlowVisor-0.2.3/flowvisor/sankey.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2732 2024-04-25 11:15:11.000000 FlowVisor-0.2.3/flowvisor/time_tracker.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2288 2024-05-20 18:08:09.000000 FlowVisor-0.2.3/flowvisor/time_value.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      300 2024-05-08 13:28:52.000000 FlowVisor-0.2.3/flowvisor/timer.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     3132 2024-05-09 07:27:11.000000 FlowVisor-0.2.3/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-05-25 13:19:45.118070 FlowVisor-0.2.3/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1585 2024-04-25 13:18:25.000000 FlowVisor-0.2.3/setup.py
```

### Comparing `FlowVisor-0.2.2/FlowVisor.egg-info/PKG-INFO` & `FlowVisor-0.2.3/FlowVisor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.2.2
+Version: 0.2.3
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.2.2/FlowVisor.egg-info/SOURCES.txt` & `FlowVisor-0.2.3/FlowVisor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/LICENSE` & `FlowVisor-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/PKG-INFO` & `FlowVisor-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowVisor
-Version: 0.2.2
+Version: 0.2.3
 Summary: Visualize and profile your python code with FlowVisor.
 Home-page: https://github.com/cophilot/FlowVisor
 Author: cophilot (Philipp B.)
 Author-email: <info@philipp-bonin.com>
 License: MIT
 Keywords: python,flow,visualize,code,flowvisor,profiling,profile,decorator
 Platform: UNKNOWN
```

### Comparing `FlowVisor-0.2.2/README.md` & `FlowVisor-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/cli/add_vis.py` & `FlowVisor-0.2.3/flowvisor/cli/add_vis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 import os
 import sys
 
 IMPORT_STATEMENT = "from flowvisor import vis"
 DECORATOR = "@vis"
 
+
 def add_decorator(dir_path="."):
     for root, dirs, files in os.walk(dir_path):
         if ignore_dir(os.path.basename(root)):
             continue
 
         for file in files:
             if not file.endswith(".py"):
                 continue
             handle_file(root, file)
     print("Done")
 
+
 def handle_file(root, file):
     # read contents of the file
     file_path = os.path.join(root, file)
     with open(file_path, "r") as f:
         lines = f.readlines()
-    
+
     found_function = False
     found_import = False
     for line in lines:
         if is_function(line):
             found_function = True
         if IMPORT_STATEMENT in line:
             found_import = True
-    
+
     if not found_function:
         print(f"No function found in {file_path}")
         return
-    
+
     new_content = []
 
     # iterate in reverse
     adding_existing_decorator = False
+    found_vis = False
     spacing = ""
     for index, line in enumerate(lines[::-1]):
         if adding_existing_decorator:
             new_content.append(line)
+            if lines.strip().startswith(DECORATOR):
+                found_vis = True
             if not lines[-index - 1].strip().startswith("@"):
                 adding_existing_decorator = False
-                new_content.append(f"{spacing}{DECORATOR}\n")
+                if not found_vis:
+                    new_content.append(f"{spacing}{DECORATOR}\n")
+                found_vis = False
         elif is_function(line):
             new_content.append(line)
             spacing = line.split("def")[0]
             if lines[-index - 1].strip().startswith("@"):
                 adding_existing_decorator = True
             else:
                 new_content.append(f"{spacing}{DECORATOR}\n")
@@ -59,49 +66,57 @@
 
     new_content.reverse()
 
     with open(file_path, "w") as f:
         f.writelines(new_content)
     print(f"Added vis to {file_path}")
 
+
 def ignore_dir(dir_name):
     if dir_name.endswith("__pycache__"):
         return True
     if dir_name.endswith("venv"):
         return True
     if dir_name.endswith(".git"):
         return True
     if dir_name.endswith(".vscode"):
         return True
-    if dir_name.startswith(".") and dir_name != ".": # ignore hidden directories
+    if dir_name.startswith(".") and dir_name != ".":  # ignore hidden directories
         return True
     return False
 
+
 def is_function(line):
     return line.strip().startswith("def ") and line.strip().endswith(":")
 
+
 def main():
-    print("This script will add the vis decorator to all python files in the provided directory.")
+    print(
+        "This script will add the vis decorator to all python files in the provided directory."
+    )
     print("Visit https://github.com/cophilot/FlowVisor#cli for more information.")
     # check if the path is provided as an argument
     args = sys.argv
     for index, arg in enumerate(args):
         if arg == "-path" or arg == "-p":
             dir_path = args[index + 1]
             if os.path.exists(dir_path):
                 add_decorator(dir_path)
                 return
 
     while True:
-        dir_path = input("Enter the directory path where you want to add the decorator (default: current directory): ")
+        dir_path = input(
+            "Enter the directory path where you want to add the decorator (default: current directory): "
+        )
         if dir_path == "":
             dir_path = "."
 
         # check if the path is valid
         if not os.path.exists(dir_path):
             print("Invalid path")
             continue
         break
     add_decorator(dir_path)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `FlowVisor-0.2.2/flowvisor/cli/remove_vis.py` & `FlowVisor-0.2.3/flowvisor/cli/remove_vis.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/cli/vis_file.py` & `FlowVisor-0.2.3/flowvisor/cli/vis_file.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/flowvisor.py` & `FlowVisor-0.2.3/flowvisor/flowvisor.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,47 +60,78 @@
 
         TimeTracker.start(reduce_overhead)
         return result
 
     return wrapper
 
 
+def do_nothing(func):
+    """
+    Decorator that does nothing.
+    """
+
+    def wrapper(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 class FlowVisor:
     """
     The FlowVisor class is responsible for managing the flow of the functions
     and generating the graph.
     """
 
     VIS_FUNCTION = vis_impl
+    VIS_FUNCTION_CACHE = vis_impl
 
     NODES: List[FunctionNode] = []
     ROOTS: List[FunctionNode] = []
     STACK: List[FunctionNode] = []
     CONFIG = FlowVisorConfig()
 
     EXCLUDE_FUNCTIONS = []
     VERIFIER_MODE = False
+    DISABLED = False
 
     SYS_INFO = None
 
     @staticmethod
     def reset():
         """
         Resets the flowvisor.
         """
         FlowVisor.VIS_FUNCTION = vis_impl
+        FlowVisor.VIS_FUNCTION_CACHE = vis_impl
         FlowVisor.NODES = []
         FlowVisor.ROOTS = []
         FlowVisor.STACK = []
         FlowVisor.CONFIG = FlowVisorConfig()
         FlowVisor.EXCLUDE_FUNCTIONS = []
         FlowVisor.VERIFIER_MODE = False
+        FlowVisor.DISABLED = False
         FlowVisor.SYS_INFO = None
 
     @staticmethod
+    def disable():
+        """
+        Disables the flowvisor.
+        """
+        FlowVisor.VIS_FUNCTION = do_nothing
+        FlowVisor.DISABLED = True
+
+    @staticmethod
+    def enable():
+        """
+        Enables the flowvisor.
+        """
+        FlowVisor.VIS_FUNCTION = FlowVisor.VIS_FUNCTION_CACHE
+        FlowVisor.DISABLED = False
+
+    @staticmethod
     def add_function_node(func):
         """
         Adds a function node to the list of nodes if it does not exist.
         """
         func_id = function_to_id(func)
         for node in FlowVisor.NODES:
             if node.id == func_id:
@@ -458,20 +489,26 @@
             FlowVisor.enable_verifier_mode()
             return
         Logger.log(
             f"Verifier mode not enabled. Count of calls is {count} and the limit is {verifier_limit}"
         )
 
     @staticmethod
-    def enable_verifier_mode():
+    def enable_verifier_mode(force=False):
         """
         Enables the verifier mode.
+
+        :param force: If True, the verifier mode will be enabled even if the FlowVisor is disabled.
         """
+        if FlowVisor.DISABLED and not force:
+            Logger.log("Can not enable verifier mode when disabled!")
+            return
         FlowVisor.VERIFIER_MODE = True
         FlowVisor.VIS_FUNCTION = vis_verifier
+        FlowVisor.VIS_FUNCTION_CACHE = vis_verifier
         Logger.log("*** Running FlowVisor in verify mode ***")
 
     @staticmethod
     def verify_export(file_name="flowvisor_verifier.json"):
         """
         Exports the verifier.
         """
```

### Comparing `FlowVisor-0.2.2/flowvisor/flowvisor_config.py` & `FlowVisor-0.2.3/flowvisor/flowvisor_config.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/flowvisor_verifier.py` & `FlowVisor-0.2.3/flowvisor/flowvisor_verifier.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/function_node.py` & `FlowVisor-0.2.3/flowvisor/function_node.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/logger.py` & `FlowVisor-0.2.3/flowvisor/logger.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/sankey.py` & `FlowVisor-0.2.3/flowvisor/sankey.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/time_tracker.py` & `FlowVisor-0.2.3/flowvisor/time_tracker.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/time_value.py` & `FlowVisor-0.2.3/flowvisor/time_value.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/flowvisor/utils.py` & `FlowVisor-0.2.3/flowvisor/utils.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.2.2/setup.py` & `FlowVisor-0.2.3/setup.py`

 * *Files identical despite different names*

