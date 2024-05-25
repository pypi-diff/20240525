# Comparing `tmp/pygentic-0.1.1.tar.gz` & `tmp/pygentic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygentic-0.1.1.tar", last modified: Sat May 25 18:55:06 2024, max compression
+gzip compressed data, was "pygentic-0.1.2.tar", last modified: Sat May 25 19:03:42 2024, max compression
```

## Comparing `pygentic-0.1.1.tar` & `pygentic-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.845420 pygentic-0.1.1/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.1.1/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6624 2024-05-25 18:55:06.845420 pygentic-0.1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5545 2024-05-25 18:51:14.000000 pygentic-0.1.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.837420 pygentic-0.1.1/app/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/models.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.841420 pygentic-0.1.1/app/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/routes/runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/threads.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.841420 pygentic-0.1.1/app/services/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/services/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/database.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/llm_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/open_interpreter_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/serverless_service.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.841420 pygentic-0.1.1/pygentic.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)     6624 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      623 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 18:55:06.845420 pygentic-0.1.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1521 2024-05-25 18:54:57.000000 pygentic-0.1.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.845420 pygentic-0.1.1/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.761446 pygentic-0.1.2/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.1.2/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6495 2024-05-25 19:03:42.761446 pygentic-0.1.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5415 2024-05-25 19:02:47.000000 pygentic-0.1.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.753446 pygentic-0.1.2/app/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/models.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.757446 pygentic-0.1.2/app/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/routes/runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/routes/threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.757446 pygentic-0.1.2/app/services/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/app/services/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/database.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/llm_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/open_interpreter_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.1.2/app/services/serverless_service.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.761446 pygentic-0.1.2/pygentic.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6495 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      623 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 19:03:42.000000 pygentic-0.1.2/pygentic.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 19:03:42.761446 pygentic-0.1.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1521 2024-05-25 19:03:38.000000 pygentic-0.1.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 19:03:42.761446 pygentic-0.1.2/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.2/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.1.2/tests/test_threads.py
```

### Comparing `pygentic-0.1.1/LICENSE` & `pygentic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/PKG-INFO` & `pygentic-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.1.1
+Version: 0.1.2
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,17 @@
    ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
+    Created by rUv
 ```
+
 ### Introduction to Pygentic Framework
 
 Pygentic is an innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API. 
 
 Based on the robust architecture of the OpenAI Assistants API, Pygentic abstracts the complexities of integrating with different Large Language Models (LLMs), both local and remote. This abstraction ensures a consistent and seamless interaction regardless of the underlying model.
 
 ### What is the Pygentic Library?
@@ -68,15 +70,15 @@
 - **Customer Support**: Deploy intelligent agents to handle customer queries, providing instant and accurate responses.
 - **Content Generation**: Use AI to create engaging content in multiple languages, tailored to your audience.
 - **Data Analysis**: Leverage AI for interpreting and analyzing large datasets, extracting meaningful insights.
 - **Personal Assistants**: Develop personalized AI assistants to help with daily tasks, scheduling, and information retrieval.
 
 Pygentic empowers developers to harness the power of AI with ease, offering a flexible and scalable solution for integrating advanced language models into various applications. Its consistent API, multi-language support, and serverless capabilities make it a valuable tool for modern AI-driven projects.
 
-## Project Archicture
+## Project Architecture
 
 Here's a detailed breakdown of the directory structure and code blocks for each file.
 
 ### 1. **Directory Structure**
 
 ```
 pygentic/
@@ -102,40 +104,29 @@
 │   ├── test_threads.py
 │   ├── test_messages.py
 │   ├── test_runs.py
 ├── requirements.txt
 └── README.md
 ```
 
-## Project Setup
+## Installation
+
+You can install the Pygentic library using pip:
+
+```bash
+pip install pygentic
+```
+
+## Running the Application
+
+After installing the library, you can run the application using the following command:
 
-1. **Setup Project Structure**
-    ```bash
-    ./setup.sh
-    ```
-
-2. **Install Dependencies**
-    ```bash
-    pip install -r requirements.txt
-    ```
-
-3. **Setup Virtual Environment**
-    ```bash
-    python -m venv venv
-    ```
-
-4. **Activate Virtual Environment**
-    ```bash
-    source venv/bin/activate
-    ```
-
-5. **Run the Application**
-    ```bash
-    uvicorn app.main:app --reload
-    ```
+```bash
+uvicorn app.main:app --reload
+```
 
 ## Endpoints
 
 ### Assistants
 - `POST /v1/assistants`: Create a new assistant.
 - `GET /v1/assistants/{assistant_id}`: Retrieve an assistant by ID.
 
@@ -146,7 +137,9 @@
 ### Messages
 - `POST /v1/threads/{thread_id}/messages`: Add a message to a thread.
 - `GET /v1/threads/{thread_id}/messages`: Retrieve messages in a thread.
 
 ### Runs
 - `POST /v1/threads/{thread_id}/runs`: Run a thread with an assistant.
 - `GET /v1/threads/{thread_id}/runs/{run_id}`: Retrieve a run by ID.
+```
+
```

### Comparing `pygentic-0.1.1/README.md` & `pygentic-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,17 @@
    ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
+    Created by rUv
 ```
+
 ### Introduction to Pygentic Framework
 
 Pygentic is an innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API. 
 
 Based on the robust architecture of the OpenAI Assistants API, Pygentic abstracts the complexities of integrating with different Large Language Models (LLMs), both local and remote. This abstraction ensures a consistent and seamless interaction regardless of the underlying model.
 
 ### What is the Pygentic Library?
@@ -39,15 +41,15 @@
 - **Customer Support**: Deploy intelligent agents to handle customer queries, providing instant and accurate responses.
 - **Content Generation**: Use AI to create engaging content in multiple languages, tailored to your audience.
 - **Data Analysis**: Leverage AI for interpreting and analyzing large datasets, extracting meaningful insights.
 - **Personal Assistants**: Develop personalized AI assistants to help with daily tasks, scheduling, and information retrieval.
 
 Pygentic empowers developers to harness the power of AI with ease, offering a flexible and scalable solution for integrating advanced language models into various applications. Its consistent API, multi-language support, and serverless capabilities make it a valuable tool for modern AI-driven projects.
 
-## Project Archicture
+## Project Architecture
 
 Here's a detailed breakdown of the directory structure and code blocks for each file.
 
 ### 1. **Directory Structure**
 
 ```
 pygentic/
@@ -73,40 +75,29 @@
 │   ├── test_threads.py
 │   ├── test_messages.py
 │   ├── test_runs.py
 ├── requirements.txt
 └── README.md
 ```
 
-## Project Setup
+## Installation
+
+You can install the Pygentic library using pip:
+
+```bash
+pip install pygentic
+```
+
+## Running the Application
+
+After installing the library, you can run the application using the following command:
 
-1. **Setup Project Structure**
-    ```bash
-    ./setup.sh
-    ```
-
-2. **Install Dependencies**
-    ```bash
-    pip install -r requirements.txt
-    ```
-
-3. **Setup Virtual Environment**
-    ```bash
-    python -m venv venv
-    ```
-
-4. **Activate Virtual Environment**
-    ```bash
-    source venv/bin/activate
-    ```
-
-5. **Run the Application**
-    ```bash
-    uvicorn app.main:app --reload
-    ```
+```bash
+uvicorn app.main:app --reload
+```
 
 ## Endpoints
 
 ### Assistants
 - `POST /v1/assistants`: Create a new assistant.
 - `GET /v1/assistants/{assistant_id}`: Retrieve an assistant by ID.
 
@@ -117,7 +108,9 @@
 ### Messages
 - `POST /v1/threads/{thread_id}/messages`: Add a message to a thread.
 - `GET /v1/threads/{thread_id}/messages`: Retrieve messages in a thread.
 
 ### Runs
 - `POST /v1/threads/{thread_id}/runs`: Run a thread with an assistant.
 - `GET /v1/threads/{thread_id}/runs/{run_id}`: Retrieve a run by ID.
+```
+
```

### Comparing `pygentic-0.1.1/app/models.py` & `pygentic-0.1.2/app/models.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/app/routes/assistants.py` & `pygentic-0.1.2/app/routes/assistants.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/app/routes/messages.py` & `pygentic-0.1.2/app/routes/messages.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/app/routes/runs.py` & `pygentic-0.1.2/app/routes/runs.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/app/routes/threads.py` & `pygentic-0.1.2/app/routes/threads.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/app/services/llm_service.py` & `pygentic-0.1.2/app/services/llm_service.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/pygentic.egg-info/PKG-INFO` & `pygentic-0.1.2/pygentic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygentic
-Version: 0.1.1
+Version: 0.1.2
 Summary: An innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API.
 Home-page: https://github.com/ruvnet/pygentic
 Author: Your Name
 Author-email: your-email@example.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -31,15 +31,17 @@
    ___                      _   _      
   / _ \/\_/\__ _  ___ _ __ | |_(_) ___ 
  / /_)/\_ _/ _` |/ _ \ '_ \| __| |/ __|
 / ___/  / \ (_| |  __/ | | | |_| | (__ 
 \/      \_/\__, |\___|_| |_|\__|_|\___|
            |___/                       
 
+    Created by rUv
 ```
+
 ### Introduction to Pygentic Framework
 
 Pygentic is an innovative system designed to enhance the capabilities of AI assistants by providing a flexible and standardized API. 
 
 Based on the robust architecture of the OpenAI Assistants API, Pygentic abstracts the complexities of integrating with different Large Language Models (LLMs), both local and remote. This abstraction ensures a consistent and seamless interaction regardless of the underlying model.
 
 ### What is the Pygentic Library?
@@ -68,15 +70,15 @@
 - **Customer Support**: Deploy intelligent agents to handle customer queries, providing instant and accurate responses.
 - **Content Generation**: Use AI to create engaging content in multiple languages, tailored to your audience.
 - **Data Analysis**: Leverage AI for interpreting and analyzing large datasets, extracting meaningful insights.
 - **Personal Assistants**: Develop personalized AI assistants to help with daily tasks, scheduling, and information retrieval.
 
 Pygentic empowers developers to harness the power of AI with ease, offering a flexible and scalable solution for integrating advanced language models into various applications. Its consistent API, multi-language support, and serverless capabilities make it a valuable tool for modern AI-driven projects.
 
-## Project Archicture
+## Project Architecture
 
 Here's a detailed breakdown of the directory structure and code blocks for each file.
 
 ### 1. **Directory Structure**
 
 ```
 pygentic/
@@ -102,40 +104,29 @@
 │   ├── test_threads.py
 │   ├── test_messages.py
 │   ├── test_runs.py
 ├── requirements.txt
 └── README.md
 ```
 
-## Project Setup
+## Installation
+
+You can install the Pygentic library using pip:
+
+```bash
+pip install pygentic
+```
+
+## Running the Application
+
+After installing the library, you can run the application using the following command:
 
-1. **Setup Project Structure**
-    ```bash
-    ./setup.sh
-    ```
-
-2. **Install Dependencies**
-    ```bash
-    pip install -r requirements.txt
-    ```
-
-3. **Setup Virtual Environment**
-    ```bash
-    python -m venv venv
-    ```
-
-4. **Activate Virtual Environment**
-    ```bash
-    source venv/bin/activate
-    ```
-
-5. **Run the Application**
-    ```bash
-    uvicorn app.main:app --reload
-    ```
+```bash
+uvicorn app.main:app --reload
+```
 
 ## Endpoints
 
 ### Assistants
 - `POST /v1/assistants`: Create a new assistant.
 - `GET /v1/assistants/{assistant_id}`: Retrieve an assistant by ID.
 
@@ -146,7 +137,9 @@
 ### Messages
 - `POST /v1/threads/{thread_id}/messages`: Add a message to a thread.
 - `GET /v1/threads/{thread_id}/messages`: Retrieve messages in a thread.
 
 ### Runs
 - `POST /v1/threads/{thread_id}/runs`: Run a thread with an assistant.
 - `GET /v1/threads/{thread_id}/runs/{run_id}`: Retrieve a run by ID.
+```
+
```

### Comparing `pygentic-0.1.1/pygentic.egg-info/SOURCES.txt` & `pygentic-0.1.2/pygentic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.1/setup.py` & `pygentic-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='pygentic',
-    version='0.1.1',  # Incremented version number
+    version='0.1.2',  # Incremented version number
     packages=find_packages(),
     install_requires=[
         'fastapi',
         'pydantic',
         'httpx',
         'uvicorn',
         'liteLLM',
```

