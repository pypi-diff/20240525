# Comparing `tmp/kumaone-0.0.1a6.tar.gz` & `tmp/kumaone-0.0.1a7.tar.gz`

## Comparing `kumaone-0.0.1a6.tar` & `kumaone-0.0.1a7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/__init__.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/configs.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/connection.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/event_handlers.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/ioevents.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/main.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/monitors.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/notification_settings.py
--rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/notifications.py
--rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/payload_handler.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/settings.py
--rw-r--r--   0        0        0     9537 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/status_pages.py
--rw-r--r--   0        0        0     7693 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/utils.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/cli/__init__.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/cli/config_cli.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/cli/monitor_cli.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/cli/notification_cli.py
--rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/src/kumaone/cli/status_page_cli.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/.gitignore
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/AUTHORS.md
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/LICENSE
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/README.md
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/pyproject.toml
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 kumaone-0.0.1a6/PKG-INFO
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/__init__.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/configs.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/connection.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/event_handlers.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/ioevents.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/main.py
+-rw-r--r--   0        0        0    12564 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/monitors.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/notification_settings.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/notifications.py
+-rw-r--r--   0        0        0    11113 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/payload_handler.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/settings.py
+-rw-r--r--   0        0        0     9514 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/status_pages.py
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/cli/__init__.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/cli/config_cli.py
+-rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/cli/monitor_cli.py
+-rw-r--r--   0        0        0     8712 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/cli/notification_cli.py
+-rw-r--r--   0        0        0     7133 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/src/kumaone/cli/status_page_cli.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/.gitignore
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/AUTHORS.md
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/LICENSE
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/README.md
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/pyproject.toml
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 kumaone-0.0.1a7/PKG-INFO
```

### Comparing `kumaone-0.0.1a6/src/kumaone/configs.py` & `kumaone-0.0.1a7/src/kumaone/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import sys
 from types import SimpleNamespace
 import yaml
 
 # Import external python libraries
 from rich.console import Console
 from rich.prompt import Prompt
-from rich.rule import Rule
 import validators
 
 # Import custom (local) python packages
 from src.kumaone.utils import log_manager
 
 # Source code meta data
 __author__ = "Dalwar Hossain"
@@ -42,15 +41,15 @@
 
     try:
         with open(file_path, "w") as kuma_config:
             yaml.safe_dump(data_to_write, kuma_config)
             return True
     except Exception as err:
         console.print(f":x: {err} Exception occurred.", style="logging.level.error")
-        exit(1)
+        sys.exit(1)
 
 
 def check_config(config_path=None, log_level=None, logger=None, get_url=False):
     """
     Checks for uptime kuma config
 
     :param config_path: (Path) configuration yaml file path
@@ -87,19 +86,19 @@
                     logger.info(f"Config file {config_file} found!")
                     logger.debug(f"{config_data}")
                 console.print(f":partying_face: Uptime kuma config file found at: {config_file}", style="green")
                 return SimpleNamespace(**config_data["kuma"])
             else:
                 logger.error(f"Config path is not a file.")
                 console.print(f":x: {config_file} is not a file.", style="red")
-                exit(1)
+                sys.exit(1)
         else:
             logger.error(f"Provided config path doesn't exists.")
             console.print(f":x: {config_file} doesn't exists.", style="red")
-            exit(1)
+            sys.exit(1)
 
 
 def create_config(config_path=None, log_level=None):
     """
     Create a new config for kumaone with necessary info about uptime kuma
 
     :param config_path: (Path) Custom configuration path.
@@ -159,15 +158,15 @@
             console.print(f":pencil: Creating configuration file.", style="logging.level.info")
             if __write_config_file(data_to_write=config_data_to_write, file_path=config_file_path):
                 logger.info("Configuration file creation was successful.")
                 console.print(f":white_heavy_check_mark:  Successfully created the configuration file!", style="green")
         except Exception as err:
             logger.error(f"{err} exception occurred.")
             console.print(f":x: {err} exception occurred.", style="logging.level.error")
-            exit(1)
+            sys.exit(1)
 
 
 def delete_config(config_path=None, remove_parent=False, log_level=None):
     """
     Delete uptime kuma config
 
     :param config_path: (Path) Custom configuration path.
```

### Comparing `kumaone-0.0.1a6/src/kumaone/connection.py` & `kumaone-0.0.1a7/src/kumaone/connection.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/src/kumaone/event_handlers.py` & `kumaone-0.0.1a7/src/kumaone/event_handlers.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/src/kumaone/ioevents.py` & `kumaone-0.0.1a7/src/kumaone/ioevents.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/src/kumaone/main.py` & `kumaone-0.0.1a7/src/kumaone/main.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/src/kumaone/monitors.py` & `kumaone-0.0.1a7/src/kumaone/monitors.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,21 +141,17 @@
     if process_monitor_check["exists"]:
         # console.print(f":wastebasket: Deleting process monitor '{process_monitor_name}'.", style="logging.level.info")
         monitor_id = process_monitor_check["id"]
         monitor_name = process_monitor_check["name"]
         delete_event_response = _sio_call("deleteMonitor", monitor_id)
         if isinstance(delete_event_response, dict):
             if delete_event_response["ok"]:
-                console.print(
-                    f":ghost: '{monitor_name}' monitor deletion successful!", style="logging.level.info"
-                )
+                console.print(f":ghost: '{monitor_name}' monitor deletion successful!", style="logging.level.info")
             else:
-                console.print(
-                    f":crab: '{monitor_name}' monitor deletion unsuccessful!", style="logging.level.warning"
-                )
+                console.print(f":crab: '{monitor_name}' monitor deletion unsuccessful!", style="logging.level.warning")
         else:
             console.print(
                 f":red_circle: Something went wrong! {delete_event_response['msg']}", style="logging.level.error"
             )
             return False
     else:
         console.print(
```

### Comparing `kumaone-0.0.1a6/src/kumaone/notifications.py` & `kumaone-0.0.1a7/src/kumaone/notifications.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 # Import external python libraries
 from rich.console import Console
 from rich.table import Table
 
 # Import custom (local) python packages
 from .event_handlers import get_event_data, wait_for_event
+from .notification_settings import notification_types, notification_providers
 from . import ioevents
 from .utils import _sio_call
 
 # Source code meta data
 __author__ = "Dalwar Hossain"
 __email__ = "dalwar23@pm.me"
 
@@ -71,37 +72,51 @@
     """
 
     if notifications_file_path is not None and Path(notifications_file_path).is_file():
         with open(notifications_file_path) as notification_config_file:
             notification_configs = yaml.safe_load(notification_config_file)["notifications"]
         logger.debug(notification_configs)
     for notification_config in notification_configs:
-        for payload in notification_config.values():
+        required_args = ["name", "type", "isDefault", "applyExisting"]
+        for notification_type, payload in notification_config.items():
+            payload['type'] = notification_types[notification_type.lower()]
             logger.debug(f"Payload for '{payload['type']}': {payload}")
+            # Check if necessary arguments are provided
+            for key, val in notification_providers[notification_type.lower()].items():
+                if val["required"]:
+                    required_args.append(key)
+            logger.debug(f"Required args: {required_args}")
+            logger.debug(f"Payload args: {payload.keys()}")
+            missing_keys = []
+            for key in required_args:
+                if key not in payload.keys():
+                    missing_keys.append(key)
+            if missing_keys:
+                raise TypeError(f"'{payload['type']}' notification type is missing required arguments: {missing_keys}.")
             notification_provider_exists = list_notifications(
                 notification_title=payload["name"], logger=logger, check_existence=True
             )
             if not notification_provider_exists:
                 with wait_for_event(ioevents.notification_list):
                     response = _sio_call("addNotification", (payload, None))
                     if verbose:
                         print(f"{payload['type']}: {response}")
                     else:
                         if response["ok"]:
                             console.print(
-                                f":floppy_disk: Notification provider '{payload['type']}' added successfully.",
+                                f":floppy_disk: Notification provider '{payload['type'].title()}' added successfully.",
                                 style="logging.level.info",
                             )
                         else:
                             console.print(
                                 f":orange_circle: '{payload['type']}' notification provider addition failed. Response: {response['msg']}",
                                 style="logging.level.warning",
                             )
             else:
-                console.print(f":sunflower: '{payload['type']}' notification provider already exists.")
+                console.print(f":sunflower: '{payload['type'].title()}' notification provider already exists.")
 
 
 def list_notifications(verbose=None, notification_title=None, notification_id=None, logger=None, check_existence=False):
     """
     Show list of notification processes
 
     :param verbose: (bool) Enable verbose output.
@@ -145,14 +160,48 @@
                 console.print(f":four_leaf_clover: No data available.", style="logging.level.info")
     else:
         if check_existence:
             return False
         console.print(f":four_leaf_clover: No data available.", style="logging.level.info")
 
 
+def list_notification_providers(verbose=None, logger=None):
+    """
+    Show list of notification processes
+
+    :param verbose: (bool) Enable verbose output.
+    :param logger: (object) Logging object.
+    :return: (dict) Dictionary of arguments for a notification provider
+    """
+
+    table = Table("Supported Providers")
+    for key in notification_types.keys():
+        table.add_row(key.lower())
+    if table.rows:
+        console.print(table, style="green")
+
+
+def list_notification_provider_args(verbose=None, notification_type=None, logger=None, check_existence=False):
+    """
+    Show list of notification processes
+
+    :param verbose: (bool) Enable verbose output.
+    :param notification_type: (str) Uptime kuma notification process name.
+    :param logger: (object) Logging object.
+    :param check_existence: (bool) Check existence of notification provider by name.
+    :return: (dict) Dictionary of arguments for a notification provider
+    """
+
+    table = Table("Argument Key", "Required?")
+    for key, val in notification_providers[notification_type.lower()].items():
+        table.add_row(key, str(val["required"]))
+    if table.rows:
+        console.print(table, style="green")
+
+
 def delete_notification(notifications_file_path=None, notification_title=None, logger=None, verbose=None):
     """
     Delete a notification provider.
 
     :param notifications_file_path: (Path) Path to the notification provider definition file.
     :param notification_title: (str) Whether the notification provider should be added interactively or not.
     :param logger: (object) Logger object instance.
```

### Comparing `kumaone-0.0.1a6/src/kumaone/payload_handler.py` & `kumaone-0.0.1a7/src/kumaone/payload_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 #!/usr/bin/env python3
 
 """Payload handler module for kumaone"""
 
-# Import builtin python libraries
-import logging
-import sys
-
 # Import external python libraries
 from rich.console import Console
 
 # Import custom (local) python packages
-from .notification_settings import notification_providers
 from .settings import authentication_methods
 
 # Source code meta data
 __author__ = "Dalwar Hossain"
 __email__ = "dalwar23@pm.me"
 
 console = Console()
```

### Comparing `kumaone-0.0.1a6/src/kumaone/settings.py` & `kumaone-0.0.1a7/src/kumaone/settings.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/src/kumaone/status_pages.py` & `kumaone-0.0.1a7/src/kumaone/status_pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 # Import custom (local) python packages
 from .event_handlers import get_event_data, wait_for_event
 from . import ioevents
 from .monitors import _check_monitor
 from .payload_handler import _get_status_page_data_payload
-from .settings import get_missing_arguments, timeout
+from .settings import timeout
 from .utils import _sio_call
 
 # Source code meta data
 __author__ = "Dalwar Hossain"
 __email__ = "dalwar23@pm.me"
 
 console = Console()
```

### Comparing `kumaone-0.0.1a6/src/kumaone/utils.py` & `kumaone-0.0.1a7/src/kumaone/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                 raw_data = yaml.safe_load(tmp_read_file)
                 logger.debug(raw_data)
                 logger.debug(key_to_check_for)
                 if key_to_check_for in raw_data:
                     return sorted([data_path])
                 else:
                     console.print(
-                        f":orange_circle: Provided data file might not contain necessary data. Missing {key_to_check_for} key.",
+                        f":orange_circle: Provided data file is missing necessary data. Missing {key_to_check_for} key.",
                         style="logging.level.warning",
                     )
                     sys.exit(1)
     else:
         console.print(f":x:  Data path: '{data_path}', does not exists!", style="logging.level.error")
         sys.exit(1)
```

### Comparing `kumaone-0.0.1a6/src/kumaone/cli/config_cli.py` & `kumaone-0.0.1a7/src/kumaone/cli/config_cli.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/src/kumaone/cli/monitor_cli.py` & `kumaone-0.0.1a7/src/kumaone/cli/monitor_cli.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/src/kumaone/cli/notification_cli.py` & `kumaone-0.0.1a7/src/kumaone/cli/notification_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from rich.console import Console
 import typer
 from typing_extensions import Annotated
 
 # Import custom (local) python packages
 from src.kumaone.configs import check_config
 from src.kumaone.connection import connect_login, disconnect
-from src.kumaone.notifications import add_notification, delete_notification, list_notifications
+from src.kumaone.notifications import add_notification, delete_notification, list_notifications, list_notification_providers, list_notification_provider_args
 from src.kumaone.utils import log_manager, _mutual_exclusivity_check
 
 # Source code meta data
 __author__ = "Dalwar Hossain"
 __email__ = "dalwar23@pm.me"
 
 # Create typer app and turn off debug mode by default
@@ -121,14 +121,70 @@
     connect_login(config_data=config_data)
     list_notifications(
         verbose=verbose, notification_title=notification_title, notification_id=notification_id, logger=logger
     )
     disconnect()
 
 
+@app.command(name="providers", help="Show all supported uptime kuma notification providers.")
+def notification_list_providers(
+    config_file: Annotated[
+        Optional[Path], typer.Option(..., "--config", "-c", help="Uptime kuma configuration file path.")
+    ] = Path.home().joinpath(".config/kumaone/kuma.yaml"),
+    verbose: Annotated[bool, typer.Option(help="Show verbose output.")] = False,
+    log_level: Annotated[str, typer.Option(help="Set log level.")] = "NOTSET",
+):
+    """
+    List all uptime kuma notification provider.
+
+    :return: None
+    """
+
+    if log_level:
+        state["log_level"] = log_level
+        logger = log_manager(log_level=log_level)
+    config_data = check_config(config_path=config_file, logger=logger)
+    connect_login(config_data=config_data)
+    list_notification_providers(verbose=verbose, logger=logger)
+    disconnect()
+
+
+@app.command(name="provider-args", help="Show all arguments of an uptime kuma notification provider by notification type.")
+def notification_show_args(
+    notificaton_type: Annotated[
+        str,
+        typer.Option(
+            ..., "--type", "-t", help="Uptime kuma notification type.", callback=_mutual_exclusivity_check(size=2)
+        ),
+    ] = None,
+    config_file: Annotated[
+        Optional[Path], typer.Option(..., "--config", "-c", help="Uptime kuma configuration file path.")
+    ] = Path.home().joinpath(".config/kumaone/kuma.yaml"),
+    verbose: Annotated[bool, typer.Option(help="Show verbose output.")] = False,
+    log_level: Annotated[str, typer.Option(help="Set log level.")] = "NOTSET",
+):
+    """
+    List all uptime kuma notification provider.
+
+    :return: None
+    """
+
+    if log_level:
+        state["log_level"] = log_level
+        logger = log_manager(log_level=log_level)
+    if notificaton_type is None:
+        raise typer.BadParameter("Notification type '--type' / '-n' parameter is required.")
+    config_data = check_config(config_path=config_file, logger=logger)
+    connect_login(config_data=config_data)
+    list_notification_provider_args(
+        verbose=verbose, notification_type=notificaton_type, logger=logger
+    )
+    disconnect()
+
+
 @app.command(name="delete", help="Delete a notification provider.")
 def notification_delete(
     notifications: Annotated[
         Optional[Path],
         typer.Option(..., "--notifications", "-n", help="Notification(s) data."),
     ] = None,
     config_file: Annotated[
```

### Comparing `kumaone-0.0.1a6/src/kumaone/cli/status_page_cli.py` & `kumaone-0.0.1a7/src/kumaone/cli/status_page_cli.py`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/.gitignore` & `kumaone-0.0.1a7/.gitignore`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/LICENSE` & `kumaone-0.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `kumaone-0.0.1a6/README.md` & `kumaone-0.0.1a7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 [uptime kuma](https://github.com/louislam/uptime-kuma) and `uptime-kuma-api` project.
 
 `kumaone` is a CLI application. Designed for bulk operations mainly from reading configuration files. `kumaone` is very
 early in development. Contribution and constructive feedbacks are always welcome.
 
 ## Virtualenv
 
-- Install `pipenv` from [here](https://pipenv.pypa.io/en/latest/installation/)
+- Install `pipenv` from [here](https://pipenv.pypa.io/en/latest/)
 
 - Activate virtual environment
 
   ```shell
   pipenv shell
   ```
 
@@ -99,15 +99,18 @@
 - [x] Add status pages from file(s).
 - [x] Delete single status page by slug.
 - [x] Delete status page from file(s).
 
 ### Notification
 
 - Supported notification providers (tested)
+  - [x] Discord
+  - [x] Email(SMTP)
   - [x] Opsgenie
+  - [x] PagerDuty
   - [x] Rocket.Chat
   - [x] Slack
   - [x] Teams
   - [x] Webhook
 - [x] List all `notification`(s).
 - [x] See details of a `single notification` by name/id.
 - [ ] Add new notification (interactive).
```

### Comparing `kumaone-0.0.1a6/pyproject.toml` & `kumaone-0.0.1a7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.12.1",
   "mypy>=1.8.0",
   "ruff>=0.1.14",
+  "flake8>=7.0.0",
 ]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive {args:src/kumaone tests}"
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
 ]
@@ -101,15 +102,15 @@
 [tool.black]
 target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py38"
-line-length = 120
+line-length = 130
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -142,14 +143,18 @@
   "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
   # Argument name should be lowercase
   "N803",
   # fString without a placeholder
   "F541",
+  # Prefer absolute imports over relative imports
+  "TID252",
+  # Boolean default positional argument in function definition
+  "FBT001", "FBT002",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.isort]
@@ -178,15 +183,15 @@
 exclude_lines = [
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.bumpversion]
-current_version = "0.0.1-alpha.6"
+current_version = "0.0.1-alpha.7"
 #parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 #serialize = ["{major}.{minor}.{patch}"]
 parse = """(?x)
     (?P<major>[0-9]+)
     \\.(?P<minor>[0-9]+)
     \\.(?P<patch>[0-9]+)
     (?:
```

### Comparing `kumaone-0.0.1a6/PKG-INFO` & `kumaone-0.0.1a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kumaone
-Version: 0.0.1a6
+Version: 0.0.1a7
 Summary: Automation friendly bulk action CLI helper for Uptime Kuma.
 Project-URL: Documentation, https://kumaone.rtfd.io/
 Project-URL: Issues, https://github.com/dalwar23/kumaone/issues
 Project-URL: Source, https://github.com/dalwar23/kumaone
 Author-email: Dalwar Hossain <dalwar23@pm.me>
 License-Expression: BSD-3-Clause
 License-File: AUTHORS.md
@@ -52,15 +52,15 @@
 [uptime kuma](https://github.com/louislam/uptime-kuma) and `uptime-kuma-api` project.
 
 `kumaone` is a CLI application. Designed for bulk operations mainly from reading configuration files. `kumaone` is very
 early in development. Contribution and constructive feedbacks are always welcome.
 
 ## Virtualenv
 
-- Install `pipenv` from [here](https://pipenv.pypa.io/en/latest/installation/)
+- Install `pipenv` from [here](https://pipenv.pypa.io/en/latest/)
 
 - Activate virtual environment
 
   ```shell
   pipenv shell
   ```
 
@@ -129,15 +129,18 @@
 - [x] Add status pages from file(s).
 - [x] Delete single status page by slug.
 - [x] Delete status page from file(s).
 
 ### Notification
 
 - Supported notification providers (tested)
+  - [x] Discord
+  - [x] Email(SMTP)
   - [x] Opsgenie
+  - [x] PagerDuty
   - [x] Rocket.Chat
   - [x] Slack
   - [x] Teams
   - [x] Webhook
 - [x] List all `notification`(s).
 - [x] See details of a `single notification` by name/id.
 - [ ] Add new notification (interactive).
```

