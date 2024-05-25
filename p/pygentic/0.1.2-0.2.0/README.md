# Comparing `tmp/pygentic-0.1.2.tar.gz` & `tmp/pygentic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygentic-0.1.2.tar", last modified: Sat May 25 19:03:42 2024, max compression
+gzip compressed data, was "pygentic-0.2.0.tar", last modified: Sat May 25 19:17:03 2024, max compression
```

## Comparing `pygentic-0.1.2.tar` & `pygentic-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.761446 pygentic-0.1.2/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.1.2/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6495 2024-05-25 19:03:42.761446 pygentic-0.1.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5415 2024-05-25 19:02:47.000000 pygentic-0.1.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.753446 pygentic-0.1.2/app/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/models.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.757446 pygentic-0.1.2/app/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/routes/runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/threads.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.757446 pygentic-0.1.2/app/services/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/services/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/database.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/llm_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/open_interpreter_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/serverless_service.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.761446 pygentic-0.1.2/pygentic.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6495 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      623 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 19:03:42.761446 pygentic-0.1.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1521 2024-05-25 19:03:38.000000 pygentic-0.1.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.761446 pygentic-0.1.2/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.673486 pygentic-0.2.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.2.0/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6469 2024-05-25 19:17:03.673486 pygentic-0.2.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5389 2024-05-25 19:16:40.000000 pygentic-0.2.0/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.665486 pygentic-0.2.0/app/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      812 2024-05-25 19:14:49.000000 pygentic-0.2.0/app/main.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/models.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.669486 pygentic-0.2.0/app/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/routes/runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/routes/threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.669486 pygentic-0.2.0/app/services/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/app/services/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/database.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/llm_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/open_interpreter_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.2.0/app/services/serverless_service.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.669486 pygentic-0.2.0/pygentic.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6469 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      635 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 19:17:03.000000 pygentic-0.2.0/pygentic.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 19:17:03.673486 pygentic-0.2.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1480 2024-05-25 19:16:56.000000 pygentic-0.2.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:17:03.673486 pygentic-0.2.0/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.2.0/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.2.0/tests/test_threads.py
```

### Comparing `pygentic-0.1.2/LICENSE` & `pygentic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.2/PKG-INFO` & `pygentic-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.1.2
+Version: 0.2.0
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,16 +23,15 @@
 Requires-Dist: uvicorn
 Requires-Dist: liteLLM
 Requires-Dist: pydbantic
 Requires-Dist: databases[sqlite]
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 
-```
-   ___                      _   _      
+```   ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
     Created by rUv
@@ -117,15 +116,15 @@
 ```
 
 ## Running the Application
 
 After installing the library, you can run the application using the following command:
 
 ```bash
-uvicorn app.main:app --reload
+pygentic
 ```
 
 ## Endpoints
 
 ### Assistants
 - `POST /v1/assistants`: Create a new assistant.
 - `GET /v1/assistants/{assistant_id}`: Retrieve an assistant by ID.
@@ -137,9 +136,8 @@
 ### Messages
 - `POST /v1/threads/{thread_id}/messages`: Add a message to a thread.
 - `GET /v1/threads/{thread_id}/messages`: Retrieve messages in a thread.
 
 ### Runs
 - `POST /v1/threads/{thread_id}/runs`: Run a thread with an assistant.
 - `GET /v1/threads/{thread_id}/runs/{run_id}`: Retrieve a run by ID.
-```
```

### Comparing `pygentic-0.1.2/README.md` & `pygentic-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-```
-   ___                      _   _      
+```   ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
     Created by rUv
@@ -88,15 +87,15 @@
 ```
 
 ## Running the Application
 
 After installing the library, you can run the application using the following command:
 
 ```bash
-uvicorn app.main:app --reload
+pygentic
 ```
 
 ## Endpoints
 
 ### Assistants
 - `POST /v1/assistants`: Create a new assistant.
 - `GET /v1/assistants/{assistant_id}`: Retrieve an assistant by ID.
@@ -108,9 +107,8 @@
 ### Messages
 - `POST /v1/threads/{thread_id}/messages`: Add a message to a thread.
 - `GET /v1/threads/{thread_id}/messages`: Retrieve messages in a thread.
 
 ### Runs
 - `POST /v1/threads/{thread_id}/runs`: Run a thread with an assistant.
 - `GET /v1/threads/{thread_id}/runs/{run_id}`: Retrieve a run by ID.
-```
```

### Comparing `pygentic-0.1.2/app/models.py` & `pygentic-0.2.0/app/models.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.2/app/routes/assistants.py` & `pygentic-0.2.0/app/routes/assistants.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.2/app/routes/messages.py` & `pygentic-0.2.0/app/routes/messages.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.2/app/routes/runs.py` & `pygentic-0.2.0/app/routes/runs.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.2/app/routes/threads.py` & `pygentic-0.2.0/app/routes/threads.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.2/app/services/llm_service.py` & `pygentic-0.2.0/app/services/llm_service.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.2/pygentic.egg-info/PKG-INFO` & `pygentic-0.2.0/pygentic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.1.2
+Version: 0.2.0
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,16 +23,15 @@
 Requires-Dist: uvicorn
 Requires-Dist: liteLLM
 Requires-Dist: pydbantic
 Requires-Dist: databases[sqlite]
 Requires-Dist: pytest
 Requires-Dist: pytest-asyncio
 
-```
-   ___                      _   _      
+```   ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
     Created by rUv
@@ -117,15 +116,15 @@
 ```
 
 ## Running the Application
 
 After installing the library, you can run the application using the following command:
 
 ```bash
-uvicorn app.main:app --reload
+pygentic
 ```
 
 ## Endpoints
 
 ### Assistants
 - `POST /v1/assistants`: Create a new assistant.
 - `GET /v1/assistants/{assistant_id}`: Retrieve an assistant by ID.
@@ -137,9 +136,8 @@
 ### Messages
 - `POST /v1/threads/{thread_id}/messages`: Add a message to a thread.
 - `GET /v1/threads/{thread_id}/messages`: Retrieve messages in a thread.
 
 ### Runs
 - `POST /v1/threads/{thread_id}/runs`: Run a thread with an assistant.
 - `GET /v1/threads/{thread_id}/runs/{run_id}`: Retrieve a run by ID.
-```
```

### Comparing `pygentic-0.1.2/pygentic.egg-info/SOURCES.txt` & `pygentic-0.2.0/pygentic.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 app/__init__.py
+app/main.py
 app/models.py
 app/routes/__init__.py
 app/routes/assistants.py
 app/routes/messages.py
 app/routes/runs.py
 app/routes/threads.py
 app/services/__init__.py
```

### Comparing `pygentic-0.1.2/setup.py` & `pygentic-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pygentic',
-    version='0.1.2',  # Incremented version number
+    version='0.2.0',
     packages=find_packages(),
     install_requires=[
         'fastapi',
         'pydantic',
         'httpx',
         'uvicorn',
         'liteLLM',
         'pydbantic',
         'databases[sqlite]',
         'pytest',
         'pytest-asyncio',
     ],
     entry_points={
         'console_scripts': [
-            'pygentic=pygentic.__main__:main',
+            'pygentic=app.main:run'
         ],
     },
     author='Your Name',
     author_email='your-email@example.com',
     description='An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

