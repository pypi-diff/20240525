# Comparing `tmp/pygentic-0.1.0.tar.gz` & `tmp/pygentic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygentic-0.1.0.tar", last modified: Sat May 25 18:45:19 2024, max compression
+gzip compressed data, was "pygentic-0.1.1.tar", last modified: Sat May 25 18:55:06 2024, max compression
```

## Comparing `pygentic-0.1.0.tar` & `pygentic-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:45:19.637390 pygentic-0.1.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.1.0/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)      298 2024-05-25 18:45:19.637390 pygentic-0.1.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1241 2024-05-25 18:25:15.000000 pygentic-0.1.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:45:19.629390 pygentic-0.1.0/app/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.0/app/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.1.0/app/models.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:45:19.629390 pygentic-0.1.0/app/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.0/app/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.1.0/app/routes/assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.1.0/app/routes/messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.1.0/app/routes/runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.1.0/app/routes/threads.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:45:19.633391 pygentic-0.1.0/app/services/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.0/app/services/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.1.0/app/services/database.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.1.0/app/services/llm_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.1.0/app/services/open_interpreter_service.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.1.0/app/services/serverless_service.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:45:19.633391 pygentic-0.1.0/pygentic.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)      298 2024-05-25 18:45:19.000000 pygentic-0.1.0/pygentic.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      623 2024-05-25 18:45:19.000000 pygentic-0.1.0/pygentic.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 18:45:19.000000 pygentic-0.1.0/pygentic.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2024-05-25 18:45:19.000000 pygentic-0.1.0/pygentic.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 18:45:19.000000 pygentic-0.1.0/pygentic.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 18:45:19.000000 pygentic-0.1.0/pygentic.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 18:45:19.637390 pygentic-0.1.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      456 2024-05-25 18:28:35.000000 pygentic-0.1.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:45:19.637390 pygentic-0.1.0/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.0/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.1.0/tests/test_assistants.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.1.0/tests/test_messages.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.1.0/tests/test_runs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.1.0/tests/test_threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.845420 pygentic-0.1.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11357 2024-05-25 18:24:15.000000 pygentic-0.1.1/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6624 2024-05-25 18:55:06.845420 pygentic-0.1.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5545 2024-05-25 18:51:14.000000 pygentic-0.1.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.837420 pygentic-0.1.1/app/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1149 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/models.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.841420 pygentic-0.1.1/app/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      603 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      548 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      537 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/routes/runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      534 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/routes/threads.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.841420 pygentic-0.1.1/app/services/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/app/services/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      217 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/database.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1845 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/llm_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      135 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/open_interpreter_service.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      119 2024-05-25 18:25:15.000000 pygentic-0.1.1/app/services/serverless_service.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.841420 pygentic-0.1.1/pygentic.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     6624 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      623 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       52 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       89 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       10 2024-05-25 18:55:06.000000 pygentic-0.1.1/pygentic.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-25 18:55:06.845420 pygentic-0.1.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1521 2024-05-25 18:54:57.000000 pygentic-0.1.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:55:06.845420 pygentic-0.1.1/tests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-25 18:25:14.000000 pygentic-0.1.1/tests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      406 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_assistants.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      413 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_messages.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      415 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_runs.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      388 2024-05-25 18:25:15.000000 pygentic-0.1.1/tests/test_threads.py
```

### Comparing `pygentic-0.1.0/LICENSE` & `pygentic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.0/app/models.py` & `pygentic-0.1.1/app/models.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.0/app/routes/assistants.py` & `pygentic-0.1.1/app/routes/assistants.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.0/app/routes/messages.py` & `pygentic-0.1.1/app/routes/messages.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.0/app/routes/runs.py` & `pygentic-0.1.1/app/routes/runs.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.0/app/routes/threads.py` & `pygentic-0.1.1/app/routes/threads.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.0/app/services/llm_service.py` & `pygentic-0.1.1/app/services/llm_service.py`

 * *Files identical despite different names*

### Comparing `pygentic-0.1.0/pygentic.egg-info/SOURCES.txt` & `pygentic-0.1.1/pygentic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

