# Comparing `tmp/toolforge_envvars_cli-0.0.5.tar.gz` & `tmp/toolforge_envvars_cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolforge_envvars_cli-0.0.5.tar", max compression
+gzip compressed data, was "toolforge_envvars_cli-0.0.6.tar", max compression
```

## Comparing `toolforge_envvars_cli-0.0.5.tar` & `toolforge_envvars_cli-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35121 2024-03-18 14:05:36.645111 toolforge_envvars_cli-0.0.5/LICENSE
--rw-r--r--   0        0        0     1049 2024-03-18 14:05:36.649111 toolforge_envvars_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 14:05:36.677111 toolforge_envvars_cli-0.0.5/toolforge_envvars_cli/__init__.py
--rw-r--r--   0        0        0     8156 2024-03-18 14:05:36.649111 toolforge_envvars_cli-0.0.5/toolforge_envvars_cli/cli.py
--rw-r--r--   0        0        0      671 2024-03-18 14:05:36.649111 toolforge_envvars_cli-0.0.5/toolforge_envvars_cli/config.py
--rw-r--r--   0        0        0     2692 2024-03-18 14:05:36.649111 toolforge_envvars_cli-0.0.5/toolforge_envvars_cli/envvars.py
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 toolforge_envvars_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35121 2024-05-25 20:52:30.758997 toolforge_envvars_cli-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1049 2024-05-25 20:52:30.758997 toolforge_envvars_cli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-25 20:52:30.786997 toolforge_envvars_cli-0.0.6/toolforge_envvars_cli/__init__.py
+-rw-r--r--   0        0        0     9948 2024-05-25 20:52:30.758997 toolforge_envvars_cli-0.0.6/toolforge_envvars_cli/cli.py
+-rw-r--r--   0        0        0      671 2024-05-25 20:52:30.758997 toolforge_envvars_cli-0.0.6/toolforge_envvars_cli/config.py
+-rw-r--r--   0        0        0     3117 2024-05-25 20:52:30.758997 toolforge_envvars_cli-0.0.6/toolforge_envvars_cli/envvars.py
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 toolforge_envvars_cli-0.0.6/PKG-INFO
```

### Comparing `toolforge_envvars_cli-0.0.5/LICENSE` & `toolforge_envvars_cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `toolforge_envvars_cli-0.0.5/pyproject.toml` & `toolforge_envvars_cli-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["David Caro <dcaro@wikimedia.org>"]
 description = "Toolforge envvars client"
 homepage = "https://gitlab.wikimedia.org/repos/cloud/toolforge/toolforge-envvars-cli"
 license = "GPLv3"
 name = "toolforge-envvars-cli"
-version = "0.0.5"
+version = "0.0.6"
 
 [tool.poetry.dependencies]
 click = "^8.0.3"
 python = "^3.7"
 requests = "^2.27.1"
 tabulate = "^0.9.0"
 toolforge-weld = ">=1.4,<2.0"
```

### Comparing `toolforge_envvars_cli-0.0.5/toolforge_envvars_cli/cli.py` & `toolforge_envvars_cli-0.0.6/toolforge_envvars_cli/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,29 @@
 
 from toolforge_envvars_cli.config import get_loaded_config
 from toolforge_envvars_cli.envvars import EnvvarsClient
 
 LOGGER = logging.getLogger("toolforge" if __name__ == "__main__" else __name__)
 
 
+def _display_messages(messages: dict[str, list[str]]) -> None:
+    # TODO: move this into toolforge-weld before using it in other clients once the POC is good to go
+    error_messages = messages.get("error", [])
+    for message in error_messages:
+        click.echo(click.style(message, fg="red"), err=True)
+
+    warning_messages = messages.get("warning", [])
+    for message in warning_messages:
+        click.echo(click.style(message, fg="yellow"), err=True)
+
+    info_messages = messages.get("info", [])
+    for message in info_messages:
+        click.echo(click.style(message, fg="blue"), err=True)
+
+
 def handle_error(e: Exception, debug: bool = False) -> None:
     user_error = isinstance(e, ToolforgeUserError)
 
     prefix = "Error: "
     if not user_error:
         prefix = f"{e.__class__.__name__}: "
 
@@ -97,15 +112,20 @@
 )
 def envvar_list(
     json: bool = False,
     truncate: bool = True,
 ) -> None:
     config = _load_config_from_ctx()
     envvars_client = EnvvarsClient.from_config(config=config)
-    envvars = envvars_client.get("/envvar")
+    list_response = envvars_client.get("/envvar")
+    envvars = list_response
+    # TODO: refactor when the API is updated to return the new format
+    if "messages" in list_response:
+        _display_messages(list_response["messages"])
+        envvars = list_response["envvars"]
 
     if json:
         click.echo(json_mod.dumps(envvars, indent=4))
     else:
         formatted_envvars = [
             [
                 envvar["name"],
@@ -131,15 +151,20 @@
 )
 def envvar_show(
     envvar_name: str,
     json: bool = False,
 ) -> None:
     config = _load_config_from_ctx()
     envvars_client = EnvvarsClient.from_config(config=config)
-    envvar = envvars_client.get(f"/envvar/{envvar_name}")
+    get_response = envvars_client.get(f"/envvar/{envvar_name}")
+    envvar = get_response
+    # TODO: refactor when the API is updated to return the new format
+    if "messages" in get_response:
+        envvar = get_response["envvar"]
+        _display_messages(get_response["messages"])
 
     if json:
         click.echo(json_mod.dumps(envvar, indent=4))
     else:
         click.echo(
             tabulate(
                 [[envvar["name"], envvar["value"]]],
@@ -177,15 +202,20 @@
 def envvar_create(
     envvar_name: str,
     envvar_value: str | None,
     json: bool = False,
 ) -> None:
     config = _load_config_from_ctx()
     envvars_client = EnvvarsClient.from_config(config=config)
-    envvar = envvars_client.post(f"/envvar/{envvar_name}", json={"value": envvar_value})
+    create_response = envvars_client.post(f"/envvar/{envvar_name}", json={"value": envvar_value})
+    envvar = create_response
+    # TODO: refactor when the API is updated to return the new format
+    if "messages" in create_response:
+        envvar = create_response["envvar"]
+        _display_messages(create_response["messages"])
 
     if json:
         click.echo(json_mod.dumps(envvar, indent=4))
     else:
         click.echo(
             tabulate(
                 [[envvar["name"], envvar["value"]]],
@@ -221,20 +251,25 @@
             show_default=False,
             type=lambda val: val.lower() in ["y", "Y", "1", "yes", "true"],
         ):
             click.echo("Aborting at user's request")
             sys.exit(1)
 
     envvars_client = EnvvarsClient.from_config(config=config)
-    envvar = envvars_client.delete(f"/envvar/{envvar_name}")
+    delete_response = envvars_client.delete(f"/envvar/{envvar_name}")
+    envvar = delete_response
+    # TODO: refactor when the API is updated to return the new format
+    if "messages" in delete_response:
+        envvar = delete_response["envvar"]
+        _display_messages(delete_response["messages"])
 
     if json:
         click.echo(json_mod.dumps(envvar, indent=4))
     else:
-        click.echo(f"Deleted {envvar_name}, here it's it's last value: ")
+        click.echo(f"Deleted {envvar_name}, here is its last value: ")
         click.echo(
             tabulate(
                 [[envvar["name"], envvar["value"]]],
                 headers=_format_headers(["name", "value"]),
                 tablefmt="plain",
             )
         )
@@ -247,15 +282,20 @@
     is_flag=True,
 )
 def envvar_quota(
     json: bool = False,
 ) -> None:
     config = _load_config_from_ctx()
     envvars_client = EnvvarsClient.from_config(config=config)
-    quota = envvars_client.get("/quota")
+    quota_response = envvars_client.get("/quota")
+    quota = quota_response
+    # TODO: refactor when the API is updated to return the new format
+    if "messages" in quota_response:
+        quota = quota_response["quota"]
+        _display_messages(quota_response["messages"])
 
     if json:
         click.echo(json_mod.dumps(quota, indent=4))
     else:
         formatted_quota = [[quota["quota"], quota["used"], quota["quota"] - quota["used"]]]
 
         click.echo(
```

### Comparing `toolforge_envvars_cli-0.0.5/toolforge_envvars_cli/config.py` & `toolforge_envvars_cli-0.0.6/toolforge_envvars_cli/config.py`

 * *Files identical despite different names*

### Comparing `toolforge_envvars_cli-0.0.5/toolforge_envvars_cli/envvars.py` & `toolforge_envvars_cli-0.0.6/toolforge_envvars_cli/envvars.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,17 +38,25 @@
         error_class = EnvvarsClientError
 
     context = {}
     message = e.response.text
     try:
         data = e.response.json()
         if isinstance(data, dict):
+            # TODO: remove once api has been updated to return the new error format
             if "message" in data:
                 message = data["message"]
                 context = data
+            # ignoring warning and info fields that might be in data for now.
+            # TODO: look for warning and info messages and log them out with click ?
+            elif "error" in data:
+                message = ""
+                for msg in data["error"]:
+                    message += f"{msg}\n"
+                context = data
         elif isinstance(data, str):
             message = data
     except requests.exceptions.InvalidJSONError:
         pass
 
     return error_class(message=message, context=context)
```

### Comparing `toolforge_envvars_cli-0.0.5/PKG-INFO` & `toolforge_envvars_cli-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolforge-envvars-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Toolforge envvars client
 Home-page: https://gitlab.wikimedia.org/repos/cloud/toolforge/toolforge-envvars-cli
 License: GPLv3
 Author: David Caro
 Author-email: dcaro@wikimedia.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

