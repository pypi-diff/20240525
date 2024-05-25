# Comparing `tmp/aihorde-0.1.tar.gz` & `tmp/aihorde-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihorde-0.1.tar", last modified: Wed May  8 10:20:44 2024, max compression
+gzip compressed data, was "aihorde-0.3.tar", last modified: Sat May 25 21:32:12 2024, max compression
```

## Comparing `aihorde-0.1.tar` & `aihorde-0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:20:44.705855 aihorde-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-08 10:20:39.000000 aihorde-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-08 10:20:44.705855 aihorde-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-08 10:20:39.000000 aihorde-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:20:44.705855 aihorde-0.1/aihorde/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 10:20:39.000000 aihorde-0.1/aihorde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-08 10:20:39.000000 aihorde-0.1/aihorde/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-08 10:20:39.000000 aihorde-0.1/aihorde/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:20:44.705855 aihorde-0.1/aihorde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-08 10:20:44.000000 aihorde-0.1/aihorde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-08 10:20:44.000000 aihorde-0.1/aihorde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:20:44.000000 aihorde-0.1/aihorde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 10:20:44.000000 aihorde-0.1/aihorde.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-08 10:20:39.000000 aihorde-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:20:44.705855 aihorde-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:32:12.150939 aihorde-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-25 21:32:07.000000 aihorde-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-25 21:32:12.150939 aihorde-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-25 21:32:07.000000 aihorde-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:32:12.150939 aihorde-0.3/aihorde/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-25 21:32:07.000000 aihorde-0.3/aihorde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-25 21:32:07.000000 aihorde-0.3/aihorde/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14894 2024-05-25 21:32:07.000000 aihorde-0.3/aihorde/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 21:32:12.150939 aihorde-0.3/aihorde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-25 21:32:12.000000 aihorde-0.3/aihorde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-25 21:32:12.000000 aihorde-0.3/aihorde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 21:32:12.000000 aihorde-0.3/aihorde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 21:32:12.000000 aihorde-0.3/aihorde.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-25 21:32:12.000000 aihorde-0.3/aihorde.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-25 21:32:07.000000 aihorde-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 21:32:12.150939 aihorde-0.3/setup.cfg
```

### Comparing `aihorde-0.1/LICENSE` & `aihorde-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aihorde-0.1/PKG-INFO` & `aihorde-0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: aihorde
-Version: 0.1
+Version: 0.3
 Summary: Python client for AI Horde API
-Author-email: "LapisMYT (Nikita Gavrilin)" <nikitagavrilin005@gmail.com>
+Author-email: "LapisMYT (Nikita Ugnich)" <nikitagavrilin005@gmail.com>
 Project-URL: Homepage, https://github.com/lapismyt/pyAIHorde
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: msgspec
 
 # Async Python client library for AI Horde
 
-## Usage examples:
-Here you can find some usage examples of library
+## Installation:
+Warning: supports only Python 3.11 or later
+```bash
+python3.11 -m pip install aihorde
+```
+
+## Usage examples
 
 ### Image generation
 ```python
 import asyncio
 from aihorde.client import AIHordeClient
 from aihorde import models
 
@@ -39,15 +45,15 @@
     client = AIHordeClient(API_KEY)
     generation_input = models.GenerationInputStable(
         q,
         models=['Anything v5', 'Anything v3', 'MeinaMix', 'Cetus-Mix', 'Anything Diffusion',
                 'AAM XL', 'AlbedoBase XL (SDXL)', 'Animagine XL', 'Anime Illust Diffusion', 'DreamShaper XL',
                 'ICBINP XL', 'Juggernaut XL', 'Quiet Goodnight XL', 'Unstable Diffusers XL']
     )
-    generations: list[models.GenerationStable] = await client.generate_image(generation_input)
+    generations: list[models.GenerationStable] = (await client.generate_image(generation_input)).generations
     for generation in generations:
         print(f'{generation.model}: {generation.img}')
 
 asyncio.run(image())
 ```
 
 ### Text generation
@@ -66,14 +72,29 @@
         max_length=160
     )
     generation_input = models.GenerationInputKobold(
         f' Human: {q}/n AI:',
         params=params,
         models=['koboldcpp/Kunoichi-DPO-v2-7B-Q8_0-imatrix'] # i dont know which models are good for text :D
     )
-    results: list[models.GenerationKobold] = await client.generate_text(generation_input)
+    results: list[models.GenerationKobold] = (await client.generate_text(generation_input)).generations
     for result in results:
         print(result.text.strip())
 
 asyncio.run(text())
 ```
 
+### Get active models list
+```python
+import asyncio
+from aihorde.client import AIHordeClient
+from aihorde import models
+
+API_KEY = '0000000000' # Your API key from aihorde.net/register. You can also use 0000000000.
+
+async def models():
+    client = AIHordeClient(API_KEY)
+    active_models: list[models.ActiveModel] = await client.get_models(type='image') # or 'text'
+    print(repr(active_models))
+
+asyncio.run(models())
+```
```

### Comparing `aihorde-0.1/README.md` & `aihorde-0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Async Python client library for AI Horde
 
-## Usage examples:
-Here you can find some usage examples of library
+## Installation:
+Warning: supports only Python 3.11 or later
+```bash
+python3.11 -m pip install aihorde
+```
+
+## Usage examples
 
 ### Image generation
 ```python
 import asyncio
 from aihorde.client import AIHordeClient
 from aihorde import models
 
@@ -16,15 +21,15 @@
     client = AIHordeClient(API_KEY)
     generation_input = models.GenerationInputStable(
         q,
         models=['Anything v5', 'Anything v3', 'MeinaMix', 'Cetus-Mix', 'Anything Diffusion',
                 'AAM XL', 'AlbedoBase XL (SDXL)', 'Animagine XL', 'Anime Illust Diffusion', 'DreamShaper XL',
                 'ICBINP XL', 'Juggernaut XL', 'Quiet Goodnight XL', 'Unstable Diffusers XL']
     )
-    generations: list[models.GenerationStable] = await client.generate_image(generation_input)
+    generations: list[models.GenerationStable] = (await client.generate_image(generation_input)).generations
     for generation in generations:
         print(f'{generation.model}: {generation.img}')
 
 asyncio.run(image())
 ```
 
 ### Text generation
@@ -43,14 +48,29 @@
         max_length=160
     )
     generation_input = models.GenerationInputKobold(
         f' Human: {q}/n AI:',
         params=params,
         models=['koboldcpp/Kunoichi-DPO-v2-7B-Q8_0-imatrix'] # i dont know which models are good for text :D
     )
-    results: list[models.GenerationKobold] = await client.generate_text(generation_input)
+    results: list[models.GenerationKobold] = (await client.generate_text(generation_input)).generations
     for result in results:
         print(result.text.strip())
 
 asyncio.run(text())
 ```
 
+### Get active models list
+```python
+import asyncio
+from aihorde.client import AIHordeClient
+from aihorde import models
+
+API_KEY = '0000000000' # Your API key from aihorde.net/register. You can also use 0000000000.
+
+async def models():
+    client = AIHordeClient(API_KEY)
+    active_models: list[models.ActiveModel] = await client.get_models(type='image') # or 'text'
+    print(repr(active_models))
+
+asyncio.run(models())
+```
```

### Comparing `aihorde-0.1/aihorde/models.py` & `aihorde-0.3/aihorde/models.py`

 * *Files identical despite different names*

### Comparing `aihorde-0.1/aihorde.egg-info/PKG-INFO` & `aihorde-0.3/aihorde.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: aihorde
-Version: 0.1
+Version: 0.3
 Summary: Python client for AI Horde API
-Author-email: "LapisMYT (Nikita Gavrilin)" <nikitagavrilin005@gmail.com>
+Author-email: "LapisMYT (Nikita Ugnich)" <nikitagavrilin005@gmail.com>
 Project-URL: Homepage, https://github.com/lapismyt/pyAIHorde
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: aiohttp
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
+Requires-Dist: msgspec
 
 # Async Python client library for AI Horde
 
-## Usage examples:
-Here you can find some usage examples of library
+## Installation:
+Warning: supports only Python 3.11 or later
+```bash
+python3.11 -m pip install aihorde
+```
+
+## Usage examples
 
 ### Image generation
 ```python
 import asyncio
 from aihorde.client import AIHordeClient
 from aihorde import models
 
@@ -39,15 +45,15 @@
     client = AIHordeClient(API_KEY)
     generation_input = models.GenerationInputStable(
         q,
         models=['Anything v5', 'Anything v3', 'MeinaMix', 'Cetus-Mix', 'Anything Diffusion',
                 'AAM XL', 'AlbedoBase XL (SDXL)', 'Animagine XL', 'Anime Illust Diffusion', 'DreamShaper XL',
                 'ICBINP XL', 'Juggernaut XL', 'Quiet Goodnight XL', 'Unstable Diffusers XL']
     )
-    generations: list[models.GenerationStable] = await client.generate_image(generation_input)
+    generations: list[models.GenerationStable] = (await client.generate_image(generation_input)).generations
     for generation in generations:
         print(f'{generation.model}: {generation.img}')
 
 asyncio.run(image())
 ```
 
 ### Text generation
@@ -66,14 +72,29 @@
         max_length=160
     )
     generation_input = models.GenerationInputKobold(
         f' Human: {q}/n AI:',
         params=params,
         models=['koboldcpp/Kunoichi-DPO-v2-7B-Q8_0-imatrix'] # i dont know which models are good for text :D
     )
-    results: list[models.GenerationKobold] = await client.generate_text(generation_input)
+    results: list[models.GenerationKobold] = (await client.generate_text(generation_input)).generations
     for result in results:
         print(result.text.strip())
 
 asyncio.run(text())
 ```
 
+### Get active models list
+```python
+import asyncio
+from aihorde.client import AIHordeClient
+from aihorde import models
+
+API_KEY = '0000000000' # Your API key from aihorde.net/register. You can also use 0000000000.
+
+async def models():
+    client = AIHordeClient(API_KEY)
+    active_models: list[models.ActiveModel] = await client.get_models(type='image') # or 'text'
+    print(repr(active_models))
+
+asyncio.run(models())
+```
```

### Comparing `aihorde-0.1/pyproject.toml` & `aihorde-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
-requires = ["setuptools>=42", "wheel"]
+requires = ["setuptools>=62", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aihorde"
-version = "0.1"
+version = "0.3"
 description = "Python client for AI Horde API"
+dependencies = ["aiohttp", "msgspec"]
 authors = [
-    {name = "LapisMYT (Nikita Gavrilin)", email = "nikitagavrilin005@gmail.com"}
+    {name = "LapisMYT (Nikita Ugnich)", email = "nikitagavrilin005@gmail.com"}
 ]
 readme = "README.md"
 classifiers = ["Development Status :: 4 - Beta",
               "Framework :: aiohttp",
               "Intended Audience :: Developers",
-              "Programming Language :: Python :: 3.10",
               "Programming Language :: Python :: 3.11",
               "Programming Language :: Python :: 3.12",
               "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
               "Topic :: Scientific/Engineering :: Artificial Intelligence",
               "Topic :: Scientific/Engineering :: Image Processing",
               "Topic :: Scientific/Engineering :: Visualization",
               "Topic :: Software Development :: Libraries",
```

