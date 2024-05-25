# Comparing `tmp/propar-1.0.1.tar.gz` & `tmp/propar-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propar-1.0.1.tar", last modified: Tue May 21 17:34:25 2024, max compression
+gzip compressed data, was "propar-1.0.2.tar", last modified: Sat May 25 09:56:44 2024, max compression
```

## Comparing `propar-1.0.1.tar` & `propar-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-21 17:34:25.370894 propar-1.0.1/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)    18072 2024-05-21 17:03:40.000000 propar-1.0.1/LICENSE
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2236 2024-05-21 17:34:25.369894 propar-1.0.1/PKG-INFO
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1633 2024-05-21 17:28:58.000000 propar-1.0.1/README.md
-drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-21 17:34:25.369894 propar-1.0.1/propar.egg-info/
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2236 2024-05-21 17:34:25.000000 propar-1.0.1/propar.egg-info/PKG-INFO
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      146 2024-05-21 17:34:25.000000 propar-1.0.1/propar.egg-info/SOURCES.txt
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-21 17:34:25.000000 propar-1.0.1/propar.egg-info/dependency_links.txt
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-21 17:34:25.000000 propar-1.0.1/propar.egg-info/top_level.txt
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)       38 2024-05-21 17:34:25.370894 propar-1.0.1/setup.cfg
--rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1013 2024-05-21 17:34:20.000000 propar-1.0.1/setup.py
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:56:44.618464 propar-1.0.2/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)    18072 2024-05-21 17:03:40.000000 propar-1.0.2/LICENSE
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2086 2024-05-25 09:56:44.618464 propar-1.0.2/PKG-INFO
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1483 2024-05-25 09:54:12.000000 propar-1.0.2/README.md
+drwxrwxr-x   0 thearchcoder  (1000) thearchcoder  (1000)        0 2024-05-25 09:56:44.618464 propar-1.0.2/propar.egg-info/
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     2086 2024-05-25 09:56:44.000000 propar-1.0.2/propar.egg-info/PKG-INFO
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)      146 2024-05-25 09:56:44.000000 propar-1.0.2/propar.egg-info/SOURCES.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-25 09:56:44.000000 propar-1.0.2/propar.egg-info/dependency_links.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)        1 2024-05-25 09:56:44.000000 propar-1.0.2/propar.egg-info/top_level.txt
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)       38 2024-05-25 09:56:44.618464 propar-1.0.2/setup.cfg
+-rw-rw-r--   0 thearchcoder  (1000) thearchcoder  (1000)     1013 2024-05-25 09:56:24.000000 propar-1.0.2/setup.py
```

### Comparing `propar-1.0.1/LICENSE` & `propar-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `propar-1.0.1/PKG-INFO` & `propar-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propar
-Version: 1.0.1
+Version: 1.0.2
 Summary: Run terminal commands easily!
 Author: Schkimansky
 Author-email: <ahmadchawla1432@gmail.com>
 Keywords: python,terminal,bash,command,commands,terminal command runner,execute command,run commands
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -17,25 +17,25 @@
 
 # Donations
 It takes me a long time to make these libraries. If you would like to support my work, Then you can follow my patreon :)
 
 https://www.patreon.com/Schkimansky
 
 # Library
-This is a easy to use python library that allows you to convert units of measurement to others. 
-For example, You can use the "time" function to convert seconds to minutes. 
+This is a easy to use python library that allows you to run terminal commands easily. 
+
 ```python
-import conversa
-result = conversa.time(90,  From="seconds",  To="minutes") # Output will be 1.5 minutes (1.5 as a integer)
+import propar
+result = propar.run_command('echo Hello, MG?')
 print(result)
 ```
 
 # Installation
 ```bash
-pip install conversa
+pip install propar
 ```
 
 # Documentation
 There are only 2 functions:
 ```python
 run_command(command: str, timeout=None, get_both_output_and_errors=False, get_return_code=False)
 run_commands(commands_array: list[str], timeout=None, get_both_output_and_errors=False, get_return_code=False)
```

### Comparing `propar-1.0.1/README.md` & `propar-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Donations
 It takes me a long time to make these libraries. If you would like to support my work, Then you can follow my patreon :)
 
 https://www.patreon.com/Schkimansky
 
 # Library
-This is a easy to use python library that allows you to convert units of measurement to others. 
-For example, You can use the "time" function to convert seconds to minutes. 
+This is a easy to use python library that allows you to run terminal commands easily. 
+
 ```python
-import conversa
-result = conversa.time(90,  From="seconds",  To="minutes") # Output will be 1.5 minutes (1.5 as a integer)
+import propar
+result = propar.run_command('echo Hello, MG?')
 print(result)
 ```
 
 # Installation
 ```bash
-pip install conversa
+pip install propar
 ```
 
 # Documentation
 There are only 2 functions:
 ```python
 run_command(command: str, timeout=None, get_both_output_and_errors=False, get_return_code=False)
 run_commands(commands_array: list[str], timeout=None, get_both_output_and_errors=False, get_return_code=False)
```

### Comparing `propar-1.0.1/propar.egg-info/PKG-INFO` & `propar-1.0.2/propar.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propar
-Version: 1.0.1
+Version: 1.0.2
 Summary: Run terminal commands easily!
 Author: Schkimansky
 Author-email: <ahmadchawla1432@gmail.com>
 Keywords: python,terminal,bash,command,commands,terminal command runner,execute command,run commands
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -17,25 +17,25 @@
 
 # Donations
 It takes me a long time to make these libraries. If you would like to support my work, Then you can follow my patreon :)
 
 https://www.patreon.com/Schkimansky
 
 # Library
-This is a easy to use python library that allows you to convert units of measurement to others. 
-For example, You can use the "time" function to convert seconds to minutes. 
+This is a easy to use python library that allows you to run terminal commands easily. 
+
 ```python
-import conversa
-result = conversa.time(90,  From="seconds",  To="minutes") # Output will be 1.5 minutes (1.5 as a integer)
+import propar
+result = propar.run_command('echo Hello, MG?')
 print(result)
 ```
 
 # Installation
 ```bash
-pip install conversa
+pip install propar
 ```
 
 # Documentation
 There are only 2 functions:
 ```python
 run_command(command: str, timeout=None, get_both_output_and_errors=False, get_return_code=False)
 run_commands(commands_array: list[str], timeout=None, get_both_output_and_errors=False, get_return_code=False)
```

### Comparing `propar-1.0.1/setup.py` & `propar-1.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     readme = "\n" + fh.read()
 
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'Run terminal commands easily!'
 
 setup(
     name="propar",
     version=VERSION,
     author="Schkimansky",
     author_email="<ahmadchawla1432@gmail.com>",
```

