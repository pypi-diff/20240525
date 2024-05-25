# Comparing `tmp/arch_flow-0.1.8.2.tar.gz` & `tmp/arch_flow-0.1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.1.8.2.tar", last modified: Thu May 23 08:06:26 2024, max compression
+gzip compressed data, was "arch_flow-0.1.8.3.tar", last modified: Sat May 25 05:05:28 2024, max compression
```

## Comparing `arch_flow-0.1.8.2.tar` & `arch_flow-0.1.8.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 08:06:26.987673 arch_flow-0.1.8.2/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.8.2/LICENCE
--rw-rw-rw-   0        0        0     1004 2024-05-23 08:06:26.986673 arch_flow-0.1.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 08:06:26.965670 arch_flow-0.1.8.2/arch_flow/
--rw-rw-rw-   0        0        0     5165 2024-05-21 02:24:38.000000 arch_flow-0.1.8.2/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      260 2024-05-21 02:57:55.000000 arch_flow-0.1.8.2/arch_flow/ArchFlowCli.py
--rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.8.2/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.8.2/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0      363 2024-05-21 01:57:35.000000 arch_flow-0.1.8.2/arch_flow/Run.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.8.2/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.8.2/arch_flow/__init__.py
--rw-rw-rw-   0        0        0      102 2024-05-21 02:57:55.000000 arch_flow-0.1.8.2/arch_flow/db.json
-drwxrwxrwx   0        0        0        0 2024-05-23 08:06:26.978670 arch_flow-0.1.8.2/arch_flow/exceptions/
--rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.8.2/arch_flow/exceptions/ExceptionHandler.py
--rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.8.2/arch_flow/exceptions/FileOrDirectoryExistsError.py
--rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.8.2/arch_flow/exceptions/NotFoundException.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:06:26.981670 arch_flow-0.1.8.2/arch_flow/implementations/
--rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.8.2/arch_flow/implementations/DirectoryCreatorImplementation.py
--rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.8.2/arch_flow/implementations/DirectoryExplorerImplementation.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.8.2/arch_flow/implementations/StringManipulatorImplementation.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:06:26.982670 arch_flow-0.1.8.2/arch_flow/output/
--rw-rw-rw-   0        0        0     4712 2024-05-23 08:06:24.000000 arch_flow-0.1.8.2/arch_flow/output/OutputHandler.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:06:26.984670 arch_flow-0.1.8.2/arch_flow/utils/
--rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.8.2/arch_flow/utils/DirectoryExplorerUtil.py
--rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.8.2/arch_flow/utils/Filter.py
-drwxrwxrwx   0        0        0        0 2024-05-23 08:06:26.985671 arch_flow-0.1.8.2/arch_flow.egg-info/
--rw-rw-rw-   0        0        0     1004 2024-05-23 08:06:26.000000 arch_flow-0.1.8.2/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2024-05-23 08:06:26.000000 arch_flow-0.1.8.2/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 08:06:26.000000 arch_flow-0.1.8.2/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 08:06:26.000000 arch_flow-0.1.8.2/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 08:06:26.000000 arch_flow-0.1.8.2/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 08:06:26.987673 arch_flow-0.1.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1254 2024-05-23 08:06:24.000000 arch_flow-0.1.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:05:28.428678 arch_flow-0.1.8.3/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.8.3/LICENCE
+-rw-rw-rw-   0        0        0     1004 2024-05-25 05:05:28.427671 arch_flow-0.1.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.8.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 05:05:28.346676 arch_flow-0.1.8.3/arch_flow/
+-rw-rw-rw-   0        0        0     6124 2024-05-25 05:05:15.000000 arch_flow-0.1.8.3/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      260 2024-05-21 02:57:55.000000 arch_flow-0.1.8.3/arch_flow/ArchFlowCli.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.8.3/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.8.3/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0      363 2024-05-21 01:57:35.000000 arch_flow-0.1.8.3/arch_flow/Run.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.8.3/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.8.3/arch_flow/__init__.py
+-rw-rw-rw-   0        0        0      102 2024-05-21 02:57:55.000000 arch_flow-0.1.8.3/arch_flow/db.json
+drwxrwxrwx   0        0        0        0 2024-05-25 05:05:28.384042 arch_flow-0.1.8.3/arch_flow/exceptions/
+-rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.8.3/arch_flow/exceptions/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.8.3/arch_flow/exceptions/FileOrDirectoryExistsError.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.8.3/arch_flow/exceptions/NotFoundException.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:05:28.412570 arch_flow-0.1.8.3/arch_flow/implementations/
+-rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.8.3/arch_flow/implementations/DirectoryCreatorImplementation.py
+-rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.8.3/arch_flow/implementations/DirectoryExplorerImplementation.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.8.3/arch_flow/implementations/StringManipulatorImplementation.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:05:28.413645 arch_flow-0.1.8.3/arch_flow/output/
+-rw-rw-rw-   0        0        0     4744 2024-05-25 05:05:15.000000 arch_flow-0.1.8.3/arch_flow/output/OutputHandler.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:05:28.425162 arch_flow-0.1.8.3/arch_flow/utils/
+-rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.8.3/arch_flow/utils/DirectoryExplorerUtil.py
+-rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.8.3/arch_flow/utils/Filter.py
+drwxrwxrwx   0        0        0        0 2024-05-25 05:05:28.426165 arch_flow-0.1.8.3/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0     1004 2024-05-25 05:05:28.000000 arch_flow-0.1.8.3/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-05-25 05:05:28.000000 arch_flow-0.1.8.3/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 05:05:28.000000 arch_flow-0.1.8.3/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-25 05:05:28.000000 arch_flow-0.1.8.3/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-25 05:05:28.000000 arch_flow-0.1.8.3/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 05:05:28.428678 arch_flow-0.1.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-05-25 05:05:15.000000 arch_flow-0.1.8.3/setup.py
```

### Comparing `arch_flow-0.1.8.2/LICENCE` & `arch_flow-0.1.8.3/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/PKG-INFO` & `arch_flow-0.1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.8.2
+Version: 0.1.8.3
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.8.2/README.md` & `arch_flow-0.1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/ArchFlow.py` & `arch_flow-0.1.8.3/arch_flow/ArchFlow.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from arch_flow.DirectoryCreator import DirectoryCreator
 from arch_flow.DirectoryExplorer import DirectoryExplorer
 from arch_flow.StringManipulator import StringManipulator
 from arch_flow.utils.Filter import Filter
 from arch_flow.output.OutputHandler import OutputHandler
 import sys
 import os
-import json
+
 
 filter = Filter()
 
 
 class ArchFlow(ABC):
     def __init__(self):
         self.DirectoryCreator = DirectoryCreator()
@@ -58,18 +58,33 @@
             return None
         name_function = args[0]
 
         func = filter.find_key_in_dictionaries(json_content, name_function)
         if func is not None:
             steps_funcao = filter.find_key_in_dictionaries(func, 'steps')
             dictonary_functions = self.dictionary_of_standard_functions()
+            self.count_steps(steps_funcao, args, dictonary_functions, json_content)
             self.execute_step(steps_funcao, args, dictonary_functions, json_content)
         else:
             self.OutputHandler.alert_message(f"function '{name_function}' is not valid, try another one or try --help ")
 
+    def count_steps(self, steps_function, args, dictonary_functions, functions_json):
+        for dic in steps_function:
+            for step in dic:
+                args_function = filter.find_key_in_dictionaries(dic, step)
+                function = filter.find_key_in_dictionaries(dictonary_functions, step)
+                self.OutputHandler.messages_qtde +=1
+                if function is None:
+                    function = filter.find_key_in_dictionaries(functions_json, step)
+                    steps_functions = filter.find_key_in_dictionaries(function, 'steps')
+                    args_function_ = filter.find_key_in_dictionaries(dic, step)
+                    args_mapped = filter.map_args(args_function_, args[0:], "args[")
+                    self.count_steps(steps_functions, args_mapped, dictonary_functions, functions_json)
+                    break
+
     def execute_step(self, steps_function, args, dictonary_functions, functions_json):
         for dic in steps_function:
             for step in dic:
                 args_function = filter.find_key_in_dictionaries(dic, step)
                 function = filter.find_key_in_dictionaries(dictonary_functions, step)
                 if function is None:
                     function = filter.find_key_in_dictionaries(functions_json, step)
```

### Comparing `arch_flow-0.1.8.2/arch_flow/DirectoryCreator.py` & `arch_flow-0.1.8.3/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/DirectoryExplorer.py` & `arch_flow-0.1.8.3/arch_flow/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/StringManipulator.py` & `arch_flow-0.1.8.3/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/exceptions/ExceptionHandler.py` & `arch_flow-0.1.8.3/arch_flow/exceptions/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/exceptions/FileOrDirectoryExistsError.py` & `arch_flow-0.1.8.3/arch_flow/exceptions/FileOrDirectoryExistsError.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/exceptions/NotFoundException.py` & `arch_flow-0.1.8.3/arch_flow/exceptions/NotFoundException.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/implementations/DirectoryCreatorImplementation.py` & `arch_flow-0.1.8.3/arch_flow/implementations/DirectoryCreatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/implementations/DirectoryExplorerImplementation.py` & `arch_flow-0.1.8.3/arch_flow/implementations/DirectoryExplorerImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/implementations/StringManipulatorImplementation.py` & `arch_flow-0.1.8.3/arch_flow/implementations/StringManipulatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow/output/OutputHandler.py` & `arch_flow-0.1.8.3/arch_flow/output/OutputHandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 from rich.table import Table
 import os
 import shutil
 
 init(autoreset=True)
 
 console = Console()
+
+
 class SingletonMeta(type):
     _instances = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
             instance = super().__call__(*args, **kwargs)
             cls._instances[cls] = instance
         return cls._instances[cls]
 
+
 class OutputHandler(metaclass=SingletonMeta):
     messages = []
+
     def __init__(self):
         self.message_model = True
+        self.messages_qtde = 0
 
     @staticmethod
     def format_message(type_message, message, color_type=Fore.RED, identification=2):
         character_limit = 100
         formatted_message = f"{color_type} {type_message}: {message} {Style.RESET_ALL}"
 
         if len(formatted_message) > character_limit:
@@ -80,29 +85,28 @@
     def message_red(message):
         console.print(f"[bold red]{message}[/bold red]")
 
     @staticmethod
     def message_yellow(message):
         console.print(f"[bold yellow]{message}[/bold yellow]")
 
-    @staticmethod
-    def update_content(live, messages):
+    def update_content(self, live, messages):
         terminal_size = shutil.get_terminal_size()
         table_width = terminal_size.columns
         max_message_length = max(len(message['message']) for message in messages)
 
         description_width = min(max_message_length, table_width - 30)
 
         table = Table(show_header=True, header_style="bold magenta")
         table.add_column("Steps", style="dim", width=description_width)
         table.add_column("Status", width=10, justify="center")
         table.add_column("Step", justify="center", width=10)
 
         for step, message in enumerate(messages, start=1):
-            table.add_row(message['message'], message['status'], f"{step}/{len(messages)}")
+            table.add_row(message['message'], message['status'], f"{step}/{self.messages_qtde}")
 
         live.update(table)
 
     def generate_output(self, new_message, status, previous_messages):
         messages = previous_messages[:]
         new_message = {"message": new_message, "status": status}
         messages.append(new_message)
```

### Comparing `arch_flow-0.1.8.2/arch_flow/utils/Filter.py` & `arch_flow-0.1.8.3/arch_flow/utils/Filter.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/arch_flow.egg-info/PKG-INFO` & `arch_flow-0.1.8.3/arch_flow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.8.2
+Version: 0.1.8.3
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.8.2/arch_flow.egg-info/SOURCES.txt` & `arch_flow-0.1.8.3/arch_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.8.2/setup.py` & `arch_flow-0.1.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='arch-flow',
-    version='0.1.8.2',
+    version='0.1.8.3',
     license='MIT License',
     author='Carlos Vinicius Da Silva',
     long_description="O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='arch flow',
     description=u'O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.',
```

