# Comparing `tmp/model_resolver-0.6.1.tar.gz` & `tmp/model_resolver-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_resolver-0.6.1.tar", max compression
+gzip compressed data, was "model_resolver-0.6.2.tar", max compression
```

## Comparing `model_resolver-0.6.1.tar` & `model_resolver-0.6.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1067 2024-05-24 19:34:26.531158 model_resolver-0.6.1/LICENSE
--rw-r--r--   0        0        0     1752 2024-05-24 19:34:26.531158 model_resolver-0.6.1/README.md
--rw-r--r--   0        0        0       36 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/__init__.py
--rw-r--r--   0        0        0       59 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/__main__.py
--rw-r--r--   0        0        0     1924 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/cli.py
--rw-r--r--   0        0        0     1474 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/my_glutinit.py
--rw-r--r--   0        0        0    14762 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/plugin.py
--rw-r--r--   0        0        0    19793 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/render.py
--rw-r--r--   0        0        0     1248 2024-05-24 19:34:26.531158 model_resolver-0.6.1/model_resolver/utils.py
--rw-r--r--   0        0        0      748 2024-05-24 19:34:43.443154 model_resolver-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-24 20:44:21.871990 model_resolver-0.6.2/LICENSE
+-rw-r--r--   0        0        0     1752 2024-05-24 20:44:21.871990 model_resolver-0.6.2/README.md
+-rw-r--r--   0        0        0       36 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/__main__.py
+-rw-r--r--   0        0        0     2200 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/cli.py
+-rw-r--r--   0        0        0     1474 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/my_glutinit.py
+-rw-r--r--   0        0        0    14936 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/plugin.py
+-rw-r--r--   0        0        0    20256 2024-05-24 20:44:21.871990 model_resolver-0.6.2/model_resolver/render.py
+-rw-r--r--   0        0        0      391 2024-05-24 20:44:21.875990 model_resolver-0.6.2/model_resolver/tests/special_filter.py
+-rw-r--r--   0        0        0     1248 2024-05-24 20:44:21.875990 model_resolver-0.6.2/model_resolver/utils.py
+-rw-r--r--   0        0        0      748 2024-05-24 20:44:37.348146 model_resolver-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 model_resolver-0.6.2/PKG-INFO
```

### Comparing `model_resolver-0.6.1/LICENSE` & `model_resolver-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.1/README.md` & `model_resolver-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.1/model_resolver/cli.py` & `model_resolver-0.6.2/model_resolver/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,33 +16,39 @@
     render_size: int = typer.Option(256, help="Size of the rendered image"),
     load_dir: Path = typer.Option(Path.cwd(), help="Directory where the resourcepack is located"),
     output_dir: Path = typer.Option(Path.cwd() / "build", help="Where you want to save the new resourcepack, with new textures corresponding to the model"), 
     filter: list[str] = typer.Option(None, help="Filter models in directory"),
     use_cache: bool = typer.Option(False, help="Use cache for model rendering)"),
     load_vanilla: bool = typer.Option(False, help="Load vanilla model"),
     resolve_vanilla_atlas: bool = typer.Option(False, help="Resolve vanilla model textures, True if load_vanilla is True"),
-    minecraft_version: str = typer.Option("latest", help="Minecraft version to use for vanilla models")
+    minecraft_version: str = typer.Option("latest", help="Minecraft version to use for vanilla models"),
+    __special_filter__ = typer.Option(None, hidden=True),  # hidden option
     # fmt: on
 ):
     """
     A simple CLI to render models from a resourcepack, can also load vanilla models.
     """
     t_start = perf_counter()
+    if isinstance(load_dir, str):
+        load_dir = Path(load_dir)
+    if isinstance(output_dir, str):
+        output_dir = Path(output_dir)
     config = ProjectConfig(
         pipeline=["model_resolver"],
         output=output_dir,
         resource_pack={"load": load_dir, "name": load_dir.name},
         meta={
             "model_resolver": {
                 "load_vanilla": load_vanilla,
                 "use_cache": use_cache,
                 "render_size": render_size,
                 "minecraft_version": minecraft_version,
                 "resolve_vanilla_atlas": resolve_vanilla_atlas,
                 "filter": filter,
+                "__special_filter__": __special_filter__,
             },
         },
     )
     with run_beet(config=config) as ctx:
         pass
     t_end = perf_counter()
     print(f"[green][bold]✔️[/bold]  Finished in {t_end - t_start:.2f} seconds [/green]")
```

### Comparing `model_resolver-0.6.1/model_resolver/my_glutinit.py` & `model_resolver-0.6.2/model_resolver/my_glutinit.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.1/model_resolver/plugin.py` & `model_resolver-0.6.2/model_resolver/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         resolve_vanilla_atlas = True
     use_cache = ctx.meta.get("model_resolver", {}).get("use_cache", False)
     render_size = ctx.meta.get("model_resolver", {}).get("render_size", 1024)
     minecraft_version = ctx.meta.get("model_resolver", {}).get(
         "minecraft_version", "latest"
     )
     filter = ctx.meta.get("model_resolver", {}).get("filter", None)
+    __special_filter__ = ctx.meta.get("model_resolver", {}).get("__special_filter__", None)
+    if __special_filter__ is not None:
+        filter = __special_filter__.keys()
 
     vanilla = ctx.inject(Vanilla)
     if not minecraft_version == "latest":
         vanilla = vanilla.releases[minecraft_version]
     generated_models = set()
     generated_textures = set()
```

### Comparing `model_resolver-0.6.1/model_resolver/render.py` & `model_resolver-0.6.2/model_resolver/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,16 @@
             self.ctx,
             self.vanilla,
         )
         self.reset_camera()
         self.frame_count = 0
         self.logger = logging.getLogger("model_resolver")
 
+        self.__special_filter__ = ctx.meta.get("model_resolver", {}).get("__special_filter__", None)
+
     def reset_camera(self):
         self.translate = [0, 0, 0]
         self.rotate = [0, 0, 0]
 
     def reload(self):
         self.textures_bindings = {}
         self.textures = load_textures(
@@ -174,17 +176,24 @@
         with open(save_path, "wb") as f:
             img.save(f, "PNG")
 
     def display(self):
         try:
             glClearColor(0.0, 0.0, 0.0, 0.0)
             img = self.draw_buffer()
-            model_name = self.model_list[self.current_model_index].split(":")
-            texture_path = f"{model_name[0]}:render/{model_name[1]}"
-            self.ctx.assets.textures[texture_path] = Texture(img)
+            if self.__special_filter__ is None:
+                model_name = self.model_list[self.current_model_index].split(":")
+                texture_path = f"{model_name[0]}:render/{model_name[1]}"
+                self.ctx.assets.textures[texture_path] = Texture(img)
+            else:
+                model_name = self.model_list[self.current_model_index]
+                path_save = self.__special_filter__.get(model_name, None)
+                if path_save is not None:
+                    with open(path_save, "wb") as f:
+                        img.save(f, "PNG")
 
             self.cache_in_ctx(img)
             self.current_model_index += 1
             if self.current_model_index >= len(self.model_list):
                 glutLeaveMainLoop()
                 return
             self.logger.info(f"Rendering {self.model_list[self.current_model_index]}")
```

### Comparing `model_resolver-0.6.1/model_resolver/utils.py` & `model_resolver-0.6.2/model_resolver/utils.py`

 * *Files identical despite different names*

### Comparing `model_resolver-0.6.1/pyproject.toml` & `model_resolver-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-resolver"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["edayot <pro.e.dayot@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `model_resolver-0.6.1/PKG-INFO` & `model_resolver-0.6.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-resolver
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 License: MIT
 Author: edayot
 Author-email: pro.e.dayot@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

