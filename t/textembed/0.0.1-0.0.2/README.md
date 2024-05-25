# Comparing `tmp/textembed-0.0.1.tar.gz` & `tmp/textembed-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textembed-0.0.1.tar", last modified: Mon May 20 16:23:17 2024, max compression
+gzip compressed data, was "textembed-0.0.2.tar", last modified: Sat May 25 20:06:32 2024, max compression
```

## Comparing `textembed-0.0.1.tar` & `textembed-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,43 @@
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.304434 textembed-0.0.1/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)    11357 2024-05-09 02:26:44.000000 textembed-0.0.1/LICENSE
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     4763 2024-05-20 16:23:17.304114 textembed-0.0.1/PKG-INFO
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1519 2024-05-20 16:14:21.000000 textembed-0.0.1/README.md
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       38 2024-05-20 16:23:17.304491 textembed-0.0.1/setup.cfg
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2784 2024-05-20 16:13:57.000000 textembed-0.0.1/setup.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.296931 textembed-0.0.1/src/
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.298940 textembed-0.0.1/src/textembed/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      173 2024-05-19 11:59:13.000000 textembed-0.0.1/src/textembed/__init__.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.300474 textembed-0.0.1/src/textembed/application/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-17 19:06:13.000000 textembed-0.0.1/src/textembed/application/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2038 2024-05-19 11:13:23.000000 textembed-0.0.1/src/textembed/application/application.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.301089 textembed-0.0.1/src/textembed/cache/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-18 19:12:00.000000 textembed-0.0.1/src/textembed/cache/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       28 2024-05-19 11:26:25.000000 textembed-0.0.1/src/textembed/cache/cache.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.301882 textembed-0.0.1/src/textembed/engine/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-05 17:38:30.000000 textembed-0.0.1/src/textembed/engine/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      844 2024-05-19 13:26:36.000000 textembed-0.0.1/src/textembed/engine/args.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     3491 2024-05-19 13:28:18.000000 textembed-0.0.1/src/textembed/engine/async_engine.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.302754 textembed-0.0.1/src/textembed/executor/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-18 19:35:33.000000 textembed-0.0.1/src/textembed/executor/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1731 2024-05-19 09:12:34.000000 textembed-0.0.1/src/textembed/executor/base.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.303256 textembed-0.0.1/src/textembed/executor/embedder/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-19 09:25:22.000000 textembed-0.0.1/src/textembed/executor/embedder/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     3476 2024-05-19 13:28:13.000000 textembed-0.0.1/src/textembed/executor/embedder/sentence_transformer.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      494 2024-05-19 04:53:46.000000 textembed-0.0.1/src/textembed/executor/primitives.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1584 2024-05-18 06:38:17.000000 textembed-0.0.1/src/textembed/log.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1918 2024-05-19 06:01:18.000000 textembed-0.0.1/src/textembed/server.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-20 16:23:17.300107 textembed-0.0.1/src/textembed.egg-info/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     4763 2024-05-20 16:23:17.000000 textembed-0.0.1/src/textembed.egg-info/PKG-INFO
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      723 2024-05-20 16:23:17.000000 textembed-0.0.1/src/textembed.egg-info/SOURCES.txt
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        1 2024-05-20 16:23:17.000000 textembed-0.0.1/src/textembed.egg-info/dependency_links.txt
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1062 2024-05-20 16:23:17.000000 textembed-0.0.1/src/textembed.egg-info/requires.txt
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       10 2024-05-20 16:23:17.000000 textembed-0.0.1/src/textembed.egg-info/top_level.txt
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.767008 textembed-0.0.2/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)    11357 2024-05-09 02:26:44.000000 textembed-0.0.2/LICENSE
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     5088 2024-05-25 20:06:32.766696 textembed-0.0.2/PKG-INFO
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1944 2024-05-21 18:08:40.000000 textembed-0.0.2/README.md
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       38 2024-05-25 20:06:32.767074 textembed-0.0.2/setup.cfg
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2783 2024-05-21 17:33:43.000000 textembed-0.0.2/setup.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.756629 textembed-0.0.2/src/
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.758988 textembed-0.0.2/src/textembed/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      173 2024-05-25 19:30:05.000000 textembed-0.0.2/src/textembed/__init__.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.761771 textembed-0.0.2/src/textembed/api/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:03:33.000000 textembed-0.0.2/src/textembed/api/__init__.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1480 2024-05-18 06:41:14.000000 textembed-0.0.2/src/textembed/api/docs.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2660 2024-05-25 19:12:49.000000 textembed-0.0.2/src/textembed/api/embed.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1603 2024-05-19 11:18:20.000000 textembed-0.0.2/src/textembed/api/monitor.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     3406 2024-05-18 19:33:48.000000 textembed-0.0.2/src/textembed/api/schemas.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.762363 textembed-0.0.2/src/textembed/application/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-17 19:06:13.000000 textembed-0.0.2/src/textembed/application/__init__.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2056 2024-05-24 18:21:49.000000 textembed-0.0.2/src/textembed/application/application.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.763089 textembed-0.0.2/src/textembed/batch/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      107 2024-05-23 17:30:42.000000 textembed-0.0.2/src/textembed/batch/__init__.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     4101 2024-05-25 19:12:58.000000 textembed-0.0.2/src/textembed/batch/batch_processor.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.763645 textembed-0.0.2/src/textembed/cache/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-18 19:12:00.000000 textembed-0.0.2/src/textembed/cache/__init__.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       28 2024-05-19 11:26:25.000000 textembed-0.0.2/src/textembed/cache/cache.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.764539 textembed-0.0.2/src/textembed/engine/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-05 17:38:30.000000 textembed-0.0.2/src/textembed/engine/__init__.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1862 2024-05-25 19:03:14.000000 textembed-0.0.2/src/textembed/engine/args.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     4210 2024-05-25 19:00:57.000000 textembed-0.0.2/src/textembed/engine/async_engine.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.765422 textembed-0.0.2/src/textembed/executor/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-18 19:35:33.000000 textembed-0.0.2/src/textembed/executor/__init__.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1731 2024-05-19 09:12:34.000000 textembed-0.0.2/src/textembed/executor/base.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.765931 textembed-0.0.2/src/textembed/executor/embedder/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-19 09:25:22.000000 textembed-0.0.2/src/textembed/executor/embedder/__init__.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2901 2024-05-25 18:40:21.000000 textembed-0.0.2/src/textembed/executor/embedder/sentence_transformer.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      494 2024-05-19 04:53:46.000000 textembed-0.0.2/src/textembed/executor/primitives.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1584 2024-05-25 19:11:54.000000 textembed-0.0.2/src/textembed/log.py
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2491 2024-05-25 19:22:38.000000 textembed-0.0.2/src/textembed/server.py
+drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.760332 textembed-0.0.2/src/textembed.egg-info/
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     5088 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/PKG-INFO
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      935 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/SOURCES.txt
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        1 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/dependency_links.txt
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1062 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/requires.txt
+-rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       10 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/top_level.txt
```

### Comparing `textembed-0.0.1/LICENSE` & `textembed-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `textembed-0.0.1/PKG-INFO` & `textembed-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: textembed
-Version: 0.0.1
+Version: 0.0.2
 Summary: TextEmbed provides a robust and scalable REST API for generating vector embeddings from text. Built for performance and flexibility, it supports various sentence-transformer models, allowing users to easily integrate state-of-the-art NLP techniques into their applications. Whether you need embeddings for search, recommendation, or other NLP tasks, TextEmbed delivers with high efficiency.
 Home-page: https://github.com/kevaldekivadiya2415/textembed
 Author: Keval Dekivadiya
 Author-email: kevaldekivadiya2415@gmail.com
 License: Apache License 2.0
 Keywords: Embedding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
@@ -32,15 +30,15 @@
 Requires-Dist: fastapi-cli==0.0.3
 Requires-Dist: filelock==3.14.0
 Requires-Dist: fsspec==2024.5.0
 Requires-Dist: h11==0.14.0
 Requires-Dist: httpcore==1.0.5
 Requires-Dist: httptools==0.6.1
 Requires-Dist: httpx==0.27.0
-Requires-Dist: huggingface-hub==0.23.0
+Requires-Dist: huggingface-hub==0.23.1
 Requires-Dist: idna==3.7
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: joblib==1.4.2
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mpmath==1.3.0
@@ -127,11 +125,23 @@
     Replace `<Model Name>` with the name of the model you want to use.
 
 3. For more information and additional options, run:
     ```bash
     python3 -m textembed.server --help
     ```
 
+### Running with Docker (Recommended)
+You can also run TextEmbed using Docker. The Docker image is available on Docker Hub.
+```bash
+docker run keval2415/textembed:0.0.1 --help
+```
+This command will show the help message for the TextEmbed server, detailing the available options and usage.
+
+For Example:
+```bash
+docker run -p 8000:8000 keval2415/textembed:0.0.1 --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
+```
+
 ### Accessing the API
 
 Once the server is running, you can access the API documentation via Swagger UI.
```

### Comparing `textembed-0.0.1/setup.py` & `textembed-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Setup script for the TextEmbed package."""
 
 import os
 import re
 
 from setuptools import find_packages, setup
 
+this_directory = os.path.abspath(os.path.dirname(__file__))
+
 
 def get_version():
     """
     Reads the version of the package from the __init__.py file.
 
     Returns:
         str: The version string.
@@ -25,15 +27,17 @@
 def get_requires():
     """
     Reads the list of dependencies from the requirements.txt file.
 
     Returns:
         list: A list of dependency strings.
     """
-    with open("requirements.txt", "r", encoding="utf-8") as f:
+    with open(
+        os.path.join(this_directory, "requirements.txt"), "r", encoding="utf-8"
+    ) as f:
         file_content = f.read()
         lines = [
             line.strip()
             for line in file_content.strip().split("\n")
             if line and not line.startswith("#")
         ]
         return lines
@@ -60,25 +64,23 @@
         long_description=open("README.md", "r", encoding="utf-8").read(),
         long_description_content_type="text/markdown",
         keywords=["Embedding"],
         license="Apache License 2.0",
         url="https://github.com/kevaldekivadiya2415/textembed",
         package_dir={"": "src"},
         packages=find_packages("src"),
-        python_requires=">=3.10.0",
+        python_requires=">=3.11.0",
         install_requires=get_requires(),
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Developers",
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
-            "Programming Language :: Python :: 3.8",
-            "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Topic :: Scientific/Engineering :: Artificial Intelligence",
         ],
     )
```

### Comparing `textembed-0.0.1/src/textembed/application/application.py` & `textembed-0.0.2/src/textembed/application/application.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,18 @@
         """
         logger.info(
             docs.startup_message(
                 host=doc_extra.get("host", "localhost"),
                 port=doc_extra.get("port", 8000),
             )
         )
-        app.state.engine = AsyncEngine.from_args(engine_args=engine_args)
-        await app.state.engine.start()
+        app.state.async_engine = AsyncEngine.from_args(engine_args=engine_args)
+        await app.state.async_engine.start()
         yield
-        await app.state.engine.stop()
+        await app.state.async_engine.stop()
 
     app = FastAPI(
         title=docs.FASTAPI_TITLE,
         summary=docs.FASTAPI_SUMMARY,
         description=docs.FASTAPI_DESCRIPTION,
         lifespan=lifespan,
         version=textembed.__version__,
```

### Comparing `textembed-0.0.1/src/textembed/engine/async_engine.py` & `textembed-0.0.2/src/textembed/engine/async_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Asynchronous engine creation."""
 
 from typing import List
 
-import numpy as np
-
+from textembed.batch import BatchProcessor
 from textembed.engine.args import AsyncEngineArgs
 from textembed.executor.embedder.sentence_transformer import SentenceTransformerEmbedder
 from textembed.log import logger
 
 
 class AsyncEngine:
     """Asynchronous engine for embedding text data.
 
     This class provides functionality to asynchronously handle and process
     text data using an underlying engine defined by `AsyncEngineArgs`.
 
     Attributes:
         engine_args (AsyncEngineArgs): Arguments required to initialize the engine.
         running (bool): Flag indicating if the engine is currently running.
+        batch_processor (BatchProcessor): Processor for handling batch requests.
+        model (SentenceTransformerEmbedder): Model for generating embeddings.
     """
 
     def __init__(self, engine_args: AsyncEngineArgs) -> None:
         """
         Initialize the asynchronous engine.
 
         Args:
             engine_args (AsyncEngineArgs): Arguments required to initialize the engine.
         """
         self._engine_args = engine_args
         self.running = False
+        self.batch_processor = None
         self.model = None
 
     @classmethod
     def from_args(cls, engine_args: AsyncEngineArgs) -> "AsyncEngine":
         """Create an engine instance from `AsyncEngineArgs`.
 
         Args:
@@ -42,35 +44,44 @@
             AsyncEngine: An instance of the `AsyncEngine` class.
         """
         return cls(engine_args)
 
     async def start(self):
         """Start the engine.
 
-        This method sets the running flag to True, indicating that the engine
-        is active and ready to process requests.
+        This method initializes the model and batch processor, and sets the
+        running flag to True, indicating that the engine is active and ready
+        to process requests.
         """
         if self.running:
             logger.warning("The engine is already running.")
+            return
 
-        self.model = SentenceTransformerEmbedder(engine_args=self.engine_args)
+        self.model = SentenceTransformerEmbedder(engine_args=self._engine_args)
+        self.batch_processor = BatchProcessor(
+            model=self.model,
+            workers=self._engine_args.workers,
+            batch_size=self._engine_args.batch_size,
+        )
         self.running = True
         logger.info("Engine started.")
 
     async def stop(self):
         """Stop the engine.
 
         This method sets the running flag to False, indicating that the engine
         is no longer active and will not process requests.
 
         Raises:
             ValueError: If the engine is not running when this method is called.
         """
         self._check_running()
         self.running = False
+        if self.batch_processor is not None:
+            await self.batch_processor.shutdown()
         logger.info("Engine stopped.")
 
     def _check_running(self):
         """Check if the engine is running.
 
         This method verifies the running status of the engine and raises an
         error if the engine is not running.
@@ -89,22 +100,24 @@
         """Get the engine arguments.
 
         Returns:
             AsyncEngineArgs: The arguments required to initialize the engine.
         """
         return self._engine_args
 
-    async def aembed(self, sentences: List[str]) -> List[np.ndarray]:
+    async def aembed(self, sentences: List[str], future):
         """Asynchronously embed a list of sentences.
 
         This method processes the input sentences using the underlying engine.
         It should only be called when the engine is running.
 
         Args:
             sentences (List[str]): List of sentences to be embedded.
+            future (asyncio.Future): A future object to set the result of embeddings.
 
         Raises:
             ValueError: If the engine is not running when this method is called.
         """
         self._check_running()
-        embeddings = await self.model.generate_embeddings(sentences=sentences)
-        return embeddings
+        if self.batch_processor is None:
+            raise ValueError("Batch processor is not initialized.")
+        await self.batch_processor.add_request(sentences, future)
```

### Comparing `textembed-0.0.1/src/textembed/executor/base.py` & `textembed-0.0.2/src/textembed/executor/base.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.1/src/textembed/executor/embedder/sentence_transformer.py` & `textembed-0.0.2/src/textembed/executor/embedder/sentence_transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Sentence Transformers"""
 
-import asyncio
 from typing import Any, Dict, List
 
 import numpy as np
 import torch
 from sentence_transformers import SentenceTransformer, util
 from torch import Tensor
 
@@ -55,49 +54,34 @@
             Tensor: Raw embeddings from the model.
         """
         with torch.inference_mode():
             features = util.batch_to_device(features, self.device)
             out_features = self.forward(features)["sentence_embedding"]
         return out_features
 
-    async def postprocess(self, out_features: Tensor) -> np.ndarray:
+    async def postprocess(self, out_features: Tensor) -> List[np.ndarray]:
         """Postprocesses the raw embeddings to the final format.
 
         Args:
             out_features (Tensor): Raw embeddings from the model.
 
         Returns:
             np.ndarray: Postprocessed embeddings in numpy array format.
         """
         with torch.inference_mode():
             embeddings = out_features.detach().cpu().numpy()
         return embeddings
 
-    async def _generate_embedding_for_sentence(self, sentence: str) -> np.ndarray:
-        """Helper function to generate embedding for a single sentence.
-
-        Args:
-            sentence (str): A single input sentence to generate embedding for.
-
-        Returns:
-            np.ndarray: Generated embedding for the sentence.
-        """
-        features = await self.preprocess([sentence])
-        out_features = await self.core_process(features)
-        embedding = await self.postprocess(out_features)
-        return embedding[0]
-
     async def generate_embeddings(self, sentences: List[str]) -> List[np.ndarray]:
         """Generates embeddings for the input sentences.
 
         Args:
             sentences (List[str]): Input sentences to generate embeddings for.
 
         Returns:
             List[np.ndarray]: Generated embeddings.
         """
-        tasks = [
-            asyncio.create_task(self._generate_embedding_for_sentence(sentence))
-            for sentence in sentences
-        ]
-        embeddings = await asyncio.gather(*tasks)
+        features = await self.preprocess(sentences)
+        out_features = await self.core_process(features)
+        embeddings = await self.postprocess(out_features)
+
         return embeddings
```

### Comparing `textembed-0.0.1/src/textembed/log.py` & `textembed-0.0.2/src/textembed/log.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.1/src/textembed.egg-info/PKG-INFO` & `textembed-0.0.2/src/textembed.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: textembed
-Version: 0.0.1
+Version: 0.0.2
 Summary: TextEmbed provides a robust and scalable REST API for generating vector embeddings from text. Built for performance and flexibility, it supports various sentence-transformer models, allowing users to easily integrate state-of-the-art NLP techniques into their applications. Whether you need embeddings for search, recommendation, or other NLP tasks, TextEmbed delivers with high efficiency.
 Home-page: https://github.com/kevaldekivadiya2415/textembed
 Author: Keval Dekivadiya
 Author-email: kevaldekivadiya2415@gmail.com
 License: Apache License 2.0
 Keywords: Embedding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.10.0
+Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
@@ -32,15 +30,15 @@
 Requires-Dist: fastapi-cli==0.0.3
 Requires-Dist: filelock==3.14.0
 Requires-Dist: fsspec==2024.5.0
 Requires-Dist: h11==0.14.0
 Requires-Dist: httpcore==1.0.5
 Requires-Dist: httptools==0.6.1
 Requires-Dist: httpx==0.27.0
-Requires-Dist: huggingface-hub==0.23.0
+Requires-Dist: huggingface-hub==0.23.1
 Requires-Dist: idna==3.7
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: joblib==1.4.2
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mpmath==1.3.0
@@ -127,11 +125,23 @@
     Replace `<Model Name>` with the name of the model you want to use.
 
 3. For more information and additional options, run:
     ```bash
     python3 -m textembed.server --help
     ```
 
+### Running with Docker (Recommended)
+You can also run TextEmbed using Docker. The Docker image is available on Docker Hub.
+```bash
+docker run keval2415/textembed:0.0.1 --help
+```
+This command will show the help message for the TextEmbed server, detailing the available options and usage.
+
+For Example:
+```bash
+docker run -p 8000:8000 keval2415/textembed:0.0.1 --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
+```
+
 ### Accessing the API
 
 Once the server is running, you can access the API documentation via Swagger UI.
```

### Comparing `textembed-0.0.1/src/textembed.egg-info/requires.txt` & `textembed-0.0.2/src/textembed.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 fastapi-cli==0.0.3
 filelock==3.14.0
 fsspec==2024.5.0
 h11==0.14.0
 httpcore==1.0.5
 httptools==0.6.1
 httpx==0.27.0
-huggingface-hub==0.23.0
+huggingface-hub==0.23.1
 idna==3.7
 Jinja2==3.1.4
 joblib==1.4.2
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 mdurl==0.1.2
 mpmath==1.3.0
```

