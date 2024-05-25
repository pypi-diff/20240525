# Comparing `tmp/burrow_cli-0.1.6.tar.gz` & `tmp/burrow_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burrow_cli-0.1.6.tar", max compression
+gzip compressed data, was "burrow_cli-0.1.7.tar", max compression
```

## Comparing `burrow_cli-0.1.6.tar` & `burrow_cli-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-05-24 03:38:27.323179 burrow_cli-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.6/burrow_cli/__init__.py
--rw-r--r--   0        0        0     6811 2024-05-24 08:35:14.086251 burrow_cli-0.1.6/burrow_cli/main.py
--rw-r--r--   0        0        0      602 2024-05-24 08:35:43.914925 burrow_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 burrow_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-24 03:38:27.323179 burrow_cli-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-23 13:49:53.573442 burrow_cli-0.1.7/burrow_cli/__init__.py
+-rw-r--r--   0        0        0     7415 2024-05-24 14:47:03.700623 burrow_cli-0.1.7/burrow_cli/main.py
+-rw-r--r--   0        0        0      602 2024-05-24 14:47:24.774970 burrow_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 burrow_cli-0.1.7/PKG-INFO
```

### Comparing `burrow_cli-0.1.6/README.md` & `burrow_cli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `burrow_cli-0.1.6/burrow_cli/main.py` & `burrow_cli-0.1.7/burrow_cli/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -87,58 +87,72 @@
     if bool(re.match(pattern, gram)):
         # client = docker.DockerClient(base_url='unix://var/run/docker.sock',version='1.45')
         client = docker.from_env()
         env = ["GENV_GPUS={}".format(1), "GENV_GPU_MEMORY={}".format(gram)]
         gpu_container = None
         if split_gpu:
             typer.echo("Start a shared GPU with GRAM size of {}".format(gram[0:-2]))
-            gpu_container = client.containers.run(
-                "jyzisgod/python3:latest",
-                detach=True,
-                remove=True,
-                stdout=True,
-                environment=env,
-                runtime="genv",
-                labels={"burrow-cli-container": uuid.uuid4().hex},
-            )
+            with Progress(
+                SpinnerColumn(),
+                TextColumn("[progress.description]{task.description}"),
+                transient=True,
+            ) as progress:
+                progress.add_task(description="Downloading docker image", total=None)
+                gpu_container = client.containers.run(
+                    "jyzisgod/python3:latest",
+                    detach=True,
+                    remove=True,
+                    stdout=True,
+                    environment=env,
+                    runtime="genv",
+                    labels={"burrow-cli-container": uuid.uuid4().hex},
+                )
         else:
             typer.echo(
                 "Start a shared container without splitting GPU {}".format(gram[0:-2])
             )
-            gpu_container = client.containers.run(
-                "jyzisgod/python3:latest",
-                detach=True,
-                remove=True,
-                stdout=True,
-                environment=env,
-                labels={"burrow-cli-container": uuid.uuid4().hex},
-            )
+            with Progress(
+                SpinnerColumn(),
+                TextColumn("[progress.description]{task.description}"),
+                transient=True,
+            ) as progress:
+                progress.add_task(description="Downloading docker image", total=None)
+                gpu_container = client.containers.run(
+                    "jyzisgod/python3:latest",
+                    detach=True,
+                    remove=True,
+                    stdout=True,
+                    environment=env,
+                    labels={"burrow-cli-container": uuid.uuid4().hex},
+                )
+
         f = open("./sh_bin.tar", "wb")
         with Progress(
             SpinnerColumn(),
             TextColumn("[progress.description]{task.description}"),
             transient=True,
         ) as progress:
             progress.add_task(
-                description="Creating GPU fractional container...usually take about 5 seconds", total=None
+                description="Creating GPU fractional container...usually take about 5 seconds",
+                total=None,
             )
             time.sleep(5)
 
         bits, stat = gpu_container.get_archive("/workspace/server.txt")
         # print(stat)
         # print(type(bits))
         for chunk in bits:
             f.write(chunk)
         f.close()
         untar_and_list_files("./sh_bin.tar")
         sshx_url = print_file_content("./server.txt")
         print("[bold green]GPU fractional container created successfully![/bold green]")
         print(
-            "Now you can send this link [bold blue]{}[/bold blue] or click [link={}]here[/link] to your friends, and start sharing GPU 🚀💻✨".format(
-                sshx_url, sshx_url
+            "Now you can send this link [bold blue]{}[/bold blue] to your friends, and start sharing the GPU 🚀💻✨".format(
+                sshx_url
             )
         )
     else:
         typer.echo("Wrong memory size format, size should be like 512mi or 2gi")
 
 
 @app.command(name="stop")
```

### Comparing `burrow_cli-0.1.6/pyproject.toml` & `burrow_cli-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burrow-cli"
-version = "0.1.6"
+version = "0.1.7"
 description = "Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together"
 authors = ["Vurtne Saerdna <vurtnesaerdna@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 burrow = "burrow_cli.main:app"
```

### Comparing `burrow_cli-0.1.6/PKG-INFO` & `burrow_cli-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burrow-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: Burrow command line app, you can launch a fractional GPU contaienr with this app, and share a link of the container to your friends, you and your friends can work colloratively together
 Author: Vurtne Saerdna
 Author-email: vurtnesaerdna@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

