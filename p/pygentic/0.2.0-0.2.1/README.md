# Comparing `tmp/pygentic-0.2.0.tar.gz` & `tmp/pygentic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygentic-0.2.0.tar", last modified: Sat May 25 19:17:03 2024, max compression
+gzip compressed data, was "pygentic-0.2.1.tar", last modified: Sat May 25 19:25:28 2024, max compression
```

## Comparing `pygentic-0.2.0.tar` & `pygentic-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.673486 pygentic-0.2.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.2.0/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6469 2024-05-25 19:17:03.673486 pygentic-0.2.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5389 2024-05-25 19:16:40.000000 pygentic-0.2.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.665486 pygentic-0.2.0/app/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      812 2024-05-25 19:14:49.000000 pygentic-0.2.0/app/main.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/models.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.669486 pygentic-0.2.0/app/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/routes/runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/threads.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.669486 pygentic-0.2.0/app/services/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/services/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/database.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/llm_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/open_interpreter_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/serverless_service.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.669486 pygentic-0.2.0/pygentic.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6469 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 19:17:03.673486 pygentic-0.2.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1480 2024-05-25 19:16:56.000000 pygentic-0.2.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.673486 pygentic-0.2.0/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:25:28.189512 pygentic-0.2.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.2.1/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6470 2024-05-25 19:25:28.189512 pygentic-0.2.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5390 2024-05-25 19:24:32.000000 pygentic-0.2.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:25:28.181512 pygentic-0.2.1/app/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.1/app/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      812 2024-05-25 19:14:49.000000 pygentic-0.2.1/app/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.2.1/app/models.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:25:28.185512 pygentic-0.2.1/app/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.1/app/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.2.1/app/routes/assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.2.1/app/routes/messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.2.1/app/routes/runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.2.1/app/routes/threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:25:28.185512 pygentic-0.2.1/app/services/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.1/app/services/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.2.1/app/services/database.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.2.1/app/services/llm_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.2.1/app/services/open_interpreter_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.2.1/app/services/serverless_service.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:25:28.189512 pygentic-0.2.1/pygentic.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6470 2024-05-25 19:25:28.000000 pygentic-0.2.1/pygentic.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2024-05-25 19:25:28.000000 pygentic-0.2.1/pygentic.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 19:25:28.000000 pygentic-0.2.1/pygentic.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2024-05-25 19:25:28.000000 pygentic-0.2.1/pygentic.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 19:25:28.000000 pygentic-0.2.1/pygentic.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 19:25:28.000000 pygentic-0.2.1/pygentic.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 19:25:28.189512 pygentic-0.2.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1480 2024-05-25 19:25:07.000000 pygentic-0.2.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:25:28.189512 pygentic-0.2.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.1/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.2.1/tests/test_assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.2.1/tests/test_messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.2.1/tests/test_runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.2.1/tests/test_threads.py
```

### Comparing `pygentic-0.2.0/LICENSE` & `pygentic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/PKG-INFO` & `pygentic-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.2.0
+Version: 0.2.1
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,16 @@
 Requires-Dist: uvicorn
 Requires-Dist: liteLLM
 Requires-Dist: pydbantic
 Requires-Dist: databases[sqlite]
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 
-```   ___                      _   _      
+```
+   ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
     Created by rUv
```

### Comparing `pygentic-0.2.0/README.md` & `pygentic-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-```   ___                      _   _      
+```
+   ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
     Created by rUv
```

### Comparing `pygentic-0.2.0/app/main.py` & `pygentic-0.2.1/app/main.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/app/models.py` & `pygentic-0.2.1/app/models.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/app/routes/assistants.py` & `pygentic-0.2.1/app/routes/assistants.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/app/routes/messages.py` & `pygentic-0.2.1/app/routes/messages.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/app/routes/runs.py` & `pygentic-0.2.1/app/routes/runs.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/app/routes/threads.py` & `pygentic-0.2.1/app/routes/threads.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/app/services/llm_service.py` & `pygentic-0.2.1/app/services/llm_service.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/pygentic.egg-info/PKG-INFO` & `pygentic-0.2.1/pygentic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.2.0
+Version: 0.2.1
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,16 @@
 Requires-Dist: uvicorn
 Requires-Dist: liteLLM
 Requires-Dist: pydbantic
 Requires-Dist: databases[sqlite]
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 
-```   ___                      _   _      
+```
+   ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
     Created by rUv
```

### Comparing `pygentic-0.2.0/pygentic.egg-info/SOURCES.txt` & `pygentic-0.2.1/pygentic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygentic-0.2.0/setup.py` & `pygentic-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pygentic',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         'fastapi',
         'pydantic',
         'httpx',
         'uvicorn',
         'liteLLM',
```

