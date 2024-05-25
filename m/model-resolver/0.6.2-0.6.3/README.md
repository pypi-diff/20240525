# Comparing `tmp/model_resolver-0.6.2.tar.gz` & `tmp/model_resolver-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.6.2.tar", max compression
+gzip compressed data, was "model_resolver-0.6.3.tar", max compression
```

## Comparing `model_resolver-0.6.2.tar` & `model_resolver-0.6.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2024-05-24 20:44:21.871990 model_resolver-0.6.2/LICENSE
--rw-r--r--   0        0        0     1752 2024-05-24 20:44:21.871990 model_resolver-0.6.2/README.md
--rw-r--r--   0        0        0       36 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/__main__.py
--rw-r--r--   0        0        0     2200 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14936 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/plugin.py
--rw-r--r--   0        0        0    20256 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/render.py
--rw-r--r--   0        0        0      391 2024-05-24 20:44:21.875990 model_resolver-0.6.2/model_resolver/tests/special_filter.py
--rw-r--r--   0        0        0     1248 2024-05-24 20:44:21.875990 model_resolver-0.6.2/model_resolver/utils.py
--rw-r--r--   0        0        0      748 2024-05-24 20:44:37.348146 model_resolver-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-25 11:06:40.900815 model_resolver-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-25 11:06:40.900815 model_resolver-0.6.3/README.md
+-rw-r--r--   0        0        0       36 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/__main__.py
+-rw-r--r--   0        0        0     2301 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14936 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/plugin.py
+-rw-r--r--   0        0        0    20256 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/render.py
+-rw-r--r--   0        0        0      391 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/tests/special_filter.py
+-rw-r--r--   0        0        0     1248 2024-05-25 11:06:40.900815 model_resolver-0.6.3/model_resolver/utils.py
+-rw-r--r--   0        0        0      748 2024-05-25 11:06:57.364683 model_resolver-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.6.3/PKG-INFO
```

### Comparing `model_resolver-0.6.2/LICENSE` & `model_resolver-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.2/README.md` & `model_resolver-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.2/model_resolver/cli.py` & `model_resolver-0.6.3/model_resolver/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import typer
 from pathlib import Path
 from beet import run_beet, ProjectConfig
 from time import perf_counter
 from rich import print
+from typing import Annotated
 
 app = typer.Typer(
     rich_markup_mode="markdown",
 )
 
 
 # a simple command
 @app.command()
 def main(
     # fmt: off
-    render_size: int = typer.Option(256, help="Size of the rendered image"),
-    load_dir: Path = typer.Option(Path.cwd(), help="Directory where the resourcepack is located"),
-    output_dir: Path = typer.Option(Path.cwd() / "build", help="Where you want to save the new resourcepack, with new textures corresponding to the model"), 
-    filter: list[str] = typer.Option(None, help="Filter models in directory"),
-    use_cache: bool = typer.Option(False, help="Use cache for model rendering)"),
-    load_vanilla: bool = typer.Option(False, help="Load vanilla model"),
-    resolve_vanilla_atlas: bool = typer.Option(False, help="Resolve vanilla model textures, True if load_vanilla is True"),
-    minecraft_version: str = typer.Option("latest", help="Minecraft version to use for vanilla models"),
-    __special_filter__ = typer.Option(None, hidden=True),  # hidden option
+    render_size: Annotated[int, typer.Option(help="Size of the rendered image")] = 256,
+    load_dir:  Annotated[Path, typer.Option(help="Directory where the resourcepack is located")] = Path.cwd(),
+    output_dir: Annotated[Path, typer.Option(help="Where you want to save the new resourcepack, with new textures corresponding to the model")] = Path.cwd() / "build", 
+    filter: Annotated[list[str], typer.Option(help="Filter models in directory")] = None,
+    use_cache: Annotated[bool, typer.Option(help="Use cache for model rendering)")] = False,
+    load_vanilla: Annotated[bool, typer.Option(help="Load vanilla model")] = False,
+    resolve_vanilla_atlas: Annotated[bool, typer.Option(help="Resolve vanilla model textures, True if load_vanilla is True")] = False,
+    minecraft_version: Annotated[str, typer.Option(help="Minecraft version to use for vanilla models")] = "latest",
+    __special_filter__ = typer.Option(None, hidden=True),
     # fmt: on
 ):
     """
     A simple CLI to render models from a resourcepack, can also load vanilla models.
     """
     t_start = perf_counter()
     if isinstance(load_dir, str):
```

### Comparing `model_resolver-0.6.2/model_resolver/my_glutinit.py` & `model_resolver-0.6.3/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.2/model_resolver/plugin.py` & `model_resolver-0.6.3/model_resolver/plugin.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.2/model_resolver/render.py` & `model_resolver-0.6.3/model_resolver/render.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.2/model_resolver/utils.py` & `model_resolver-0.6.3/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.2/pyproject.toml` & `model_resolver-0.6.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-resolver"
-version = "0.6.2"
+version = "0.6.3"
 description = ""
 authors = ["edayot <pro.e.dayot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `model_resolver-0.6.2/PKG-INFO` & `model_resolver-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.6.2
+Version: 0.6.3
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

