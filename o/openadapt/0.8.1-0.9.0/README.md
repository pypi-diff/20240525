# Comparing `tmp/openadapt-0.8.1.tar.gz` & `tmp/openadapt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openadapt-0.8.1.tar", max compression
+gzip compressed data, was "openadapt-0.9.0.tar", max compression
```

## Comparing `openadapt-0.8.1.tar` & `openadapt-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
--rw-r--r--   0        0        0        0 2023-08-21 17:45:14.759613 openadapt-0.8.1/LICENSE
--rw-r--r--   0        0        0    11129 2023-08-21 17:45:14.759613 openadapt-0.8.1/README.md
--rw-r--r--   0        0        0      106 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/__init__.py
--rw-r--r--   0        0        0       49 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/__init__.py
--rw-r--r--   0        0        0   102300 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/assets/logo.ico
--rw-r--r--   0        0        0     4001 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/assets/logo.png
--rw-r--r--   0        0        0     5318 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/assets/logo_inverted.png
--rw-r--r--   0        0        0     1113 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/build.py
--rw-r--r--   0        0        0     4352 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/cards.py
--rw-r--r--   0        0        0     3029 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/main.py
--rw-r--r--   0        0        0     1014 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/objects/console.py
--rw-r--r--   0        0        0     4382 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/objects/local_file_picker.py
--rw-r--r--   0        0        0     6188 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/tray.py
--rw-r--r--   0        0        0     3325 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/app/util.py
--rw-r--r--   0        0        0     2192 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/cache.py
--rw-r--r--   0        0        0      478 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/common.py
--rw-r--r--   0        0        0     6334 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/config.py
--rw-r--r--   0        0        0    12204 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/crud.py
--rw-r--r--   0        0        0     1864 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/db.py
--rw-r--r--   0        0        0    27938 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/events.py
--rw-r--r--   0        0        0     4809 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/extensions/synchronized_queue.py
--rw-r--r--   0        0        0      887 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/extensions/thread.py
--rw-r--r--   0        0        0     1357 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/logging.py
--rw-r--r--   0        0        0    13431 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/models.py
--rw-r--r--   0        0        0     3358 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/playback.py
--rw-r--r--   0        0        0        0 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/privacy/__init__.py
--rw-r--r--   0        0        0     3218 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/privacy/base.py
--rw-r--r--   0        0        0        0 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/privacy/providers/__init__.py
--rw-r--r--   0        0        0    10893 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/privacy/providers/presidio.py
--rw-r--r--   0        0        0    30461 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/record.py
--rw-r--r--   0        0        0     1951 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/replay.py
--rw-r--r--   0        0        0       98 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/scripts/__init__.py
--rw-r--r--   0        0        0      862 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/scripts/reset_db.py
--rw-r--r--   0        0        0     3949 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/scripts/scrub.py
--rw-r--r--   0        0        0      734 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/start.py
--rw-r--r--   0        0        0      293 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/__init__.py
--rw-r--r--   0        0        0     3363 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/base.py
--rw-r--r--   0        0        0     3156 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/demo.py
--rw-r--r--   0        0        0     1708 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/mixins/ascii.py
--rw-r--r--   0        0        0     2785 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/mixins/huggingface.py
--rw-r--r--   0        0        0     7096 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/mixins/ocr.py
--rw-r--r--   0        0        0     7154 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/mixins/openai.py
--rw-r--r--   0        0        0    10434 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/mixins/sam.py
--rw-r--r--   0        0        0     2007 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/mixins/summary.py
--rw-r--r--   0        0        0     3352 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/naive.py
--rw-r--r--   0        0        0     7668 2023-08-21 17:45:14.767613 openadapt-0.8.1/openadapt/strategies/stateful.py
--rw-r--r--   0        0        0    24843 2023-08-21 17:45:14.771613 openadapt-0.8.1/openadapt/utils.py
--rw-r--r--   0        0        0     9401 2023-08-21 17:45:14.771613 openadapt-0.8.1/openadapt/visualize.py
--rw-r--r--   0        0        0     2092 2023-08-21 17:45:14.771613 openadapt-0.8.1/openadapt/window/__init__.py
--rw-r--r--   0        0        0     9593 2023-08-21 17:45:14.771613 openadapt-0.8.1/openadapt/window/_macos.py
--rw-r--r--   0        0        0     6055 2023-08-21 17:45:14.771613 openadapt-0.8.1/openadapt/window/_windows.py
--rw-r--r--   0        0        0     2917 2023-08-21 17:45:14.771613 openadapt-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    14060 1970-01-01 00:00:00.000000 openadapt-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-28 21:51:42.164709 openadapt-0.9.0/LICENSE
+-rw-r--r--   0        0        0    11721 2023-08-28 21:51:42.164709 openadapt-0.9.0/README.md
+-rw-r--r--   0        0        0      106 2023-08-28 21:51:42.172709 openadapt-0.9.0/openadapt/__init__.py
+-rw-r--r--   0        0        0       49 2023-08-28 21:51:42.172709 openadapt-0.9.0/openadapt/app/__init__.py
+-rw-r--r--   0        0        0   102300 2023-08-28 21:51:42.172709 openadapt-0.9.0/openadapt/app/assets/logo.ico
+-rw-r--r--   0        0        0     4001 2023-08-28 21:51:42.172709 openadapt-0.9.0/openadapt/app/assets/logo.png
+-rw-r--r--   0        0        0     5318 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/assets/logo_inverted.png
+-rw-r--r--   0        0        0     1113 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/build.py
+-rw-r--r--   0        0        0     4352 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/cards.py
+-rw-r--r--   0        0        0     3226 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/main.py
+-rw-r--r--   0        0        0     1014 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/objects/console.py
+-rw-r--r--   0        0        0     4382 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/objects/local_file_picker.py
+-rw-r--r--   0        0        0     6332 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/tray.py
+-rw-r--r--   0        0        0     3325 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/app/util.py
+-rw-r--r--   0        0        0     2192 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/cache.py
+-rw-r--r--   0        0        0      478 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/common.py
+-rw-r--r--   0        0        0     6690 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/config.py
+-rw-r--r--   0        0        0    12204 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/crud.py
+-rw-r--r--   0        0        0     1864 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/db.py
+-rw-r--r--   0        0        0       48 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/deprecated/__init__.py
+-rw-r--r--   0        0        0     9401 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/deprecated/visualize.py
+-rw-r--r--   0        0        0    27938 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/events.py
+-rw-r--r--   0        0        0     4809 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/extensions/synchronized_queue.py
+-rw-r--r--   0        0        0      916 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/extensions/thread.py
+-rw-r--r--   0        0        0     1357 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/logging.py
+-rw-r--r--   0        0        0    13431 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/models.py
+-rw-r--r--   0        0        0     3358 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/playback.py
+-rw-r--r--   0        0        0       57 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/privacy/__init__.py
+-rw-r--r--   0        0        0     3218 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/privacy/base.py
+-rw-r--r--   0        0        0       55 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/privacy/providers/__init__.py
+-rw-r--r--   0        0        0    10893 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/privacy/providers/presidio.py
+-rw-r--r--   0        0        0    22731 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/productivity.py
+-rw-r--r--   0        0        0    30461 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/record.py
+-rw-r--r--   0        0        0     1951 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/replay.py
+-rw-r--r--   0        0        0       98 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/scripts/__init__.py
+-rw-r--r--   0        0        0      862 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/scripts/reset_db.py
+-rw-r--r--   0        0        0     3949 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/scripts/scrub.py
+-rw-r--r--   0        0        0      734 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/start.py
+-rw-r--r--   0        0        0      293 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/__init__.py
+-rw-r--r--   0        0        0     3363 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/base.py
+-rw-r--r--   0        0        0     3156 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/demo.py
+-rw-r--r--   0        0        0     1708 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/mixins/ascii.py
+-rw-r--r--   0        0        0     2785 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/mixins/huggingface.py
+-rw-r--r--   0        0        0     7096 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/mixins/ocr.py
+-rw-r--r--   0        0        0     7154 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/mixins/openai.py
+-rw-r--r--   0        0        0    10434 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/mixins/sam.py
+-rw-r--r--   0        0        0     2007 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/mixins/summary.py
+-rw-r--r--   0        0        0     3412 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/naive.py
+-rw-r--r--   0        0        0     7668 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/strategies/stateful.py
+-rw-r--r--   0        0        0    25603 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/utils.py
+-rw-r--r--   0        0        0    13238 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/visualize.py
+-rw-r--r--   0        0        0     2092 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/window/__init__.py
+-rw-r--r--   0        0        0     9593 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/window/_macos.py
+-rw-r--r--   0        0        0     6055 2023-08-28 21:51:42.176709 openadapt-0.9.0/openadapt/window/_windows.py
+-rw-r--r--   0        0        0     3227 2023-08-28 21:51:42.180709 openadapt-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14781 1970-01-01 00:00:00.000000 openadapt-0.9.0/PKG-INFO
```

### Comparing `openadapt-0.8.1/README.md` & `openadapt-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -260,29 +260,37 @@
 validations on your codebase.
 
 The following pre-commit hooks are used in OpenAdapt:
 
 - [check-yaml](https://github.com/pre-commit/pre-commit-hooks#check-yaml): Validates the syntax and structure of YAML files.
 - [end-of-file-fixer](https://github.com/pre-commit/pre-commit-hooks#end-of-file-fixer): Ensures that files end with a newline character.
 - [trailing-whitespace](https://github.com/pre-commit/pre-commit-hooks#trailing-whitespace): Detects and removes trailing whitespace at the end of lines.
-- [black](https://github.com/psf/black): Formats Python code to adhere to the Black code style.
+- [black](https://github.com/psf/black): Formats Python code to adhere to the Black code style. Notably, the `--preview` feature is used.
 - [isort](https://github.com/PyCQA/isort): Sorts Python import statements in a consistent and standardized manner.
 
 To set up the pre-commit hooks, follow these steps:
 
 1. Navigate to the root directory of your OpenAdapt repository.
 
 2. Run the following command to install the hooks:
 
 ```
 pre-commit install
 ```
 
 Now, the pre-commit hooks are installed and will run automatically before each commit. They will enforce code quality standards and prevent committing code that doesn't pass the defined checks.
 
+### Status Checks
+
+When you submit a PR, the "Python CI" workflow is triggered for code consistency. It follows organized steps to review your code:
+
+1. **Python Black Check** : This step verifies code formatting using Python Black style, with the `--preview` flag for style.
+
+2. **Flake8 Review** : Next, Flake8 tool thoroughly checks code structure, including flake8-annotations and flake8-docstrings. Though GitHub Actions automates checks, it's wise to locally run `flake8 .` before finalizing changes for quicker issue spotting and resolution.
+
 # Submitting an Issue
 
 Please submit any issues to https://github.com/OpenAdaptAI/OpenAdapt/issues with the
 following information:
 
 - Problem description (please include any relevant console output and/or screenshots)
 - Steps to reproduce (please help others to help you!)
```

### Comparing `openadapt-0.8.1/openadapt/app/assets/logo.ico` & `openadapt-0.9.0/openadapt/app/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/app/assets/logo.png` & `openadapt-0.9.0/openadapt/app/assets/logo.png`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/app/assets/logo_inverted.png` & `openadapt-0.9.0/openadapt/app/assets/logo_inverted.png`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/app/build.py` & `openadapt-0.9.0/openadapt/app/build.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/app/cards.py` & `openadapt-0.9.0/openadapt/app/cards.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/app/main.py` & `openadapt-0.9.0/openadapt/app/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 
 Example usage:
     from openadapt.app import run_app
 
     run_app()
 """
 
+from functools import partial
+from subprocess import Popen
 import base64
 import os
 
 from nicegui import app, ui
 
-from openadapt import config, replay, visualize
+from openadapt import config, replay
 from openadapt.app.cards import recording_prompt, select_import, settings
 from openadapt.app.objects.console import Console
 from openadapt.app.util import clear_db, on_export, on_import
 
 SERVER = "127.0.0.1:8000/upload"
 FPATH = os.path.dirname(__file__)
 
@@ -27,70 +29,65 @@
 app.native.start_args["debug"] = False
 
 dark = ui.dark_mode()
 dark.value = config.APP_DARK_MODE
 
 logger = None
 
-# Add logo
-# right align icon
-with ui.row().classes("w-full justify-right"):
-    # settings
-
-    # alignment trick
-    with ui.avatar(color="white" if dark else "black", size=128):
-        logo_base64 = base64.b64encode(
-            open(os.path.join(FPATH, "assets/logo.png"), "rb").read()
+
+def start(fullscreen: bool = False) -> None:
+    """Start the OpenAdapt application."""
+    with ui.row().classes("w-full justify-right"):
+        with ui.avatar(color="white" if dark else "black", size=128):
+            logo_base64 = base64.b64encode(
+                open(os.path.join(FPATH, "assets/logo.png"), "rb").read()
+            )
+            img = bytes(
+                f"data:image/png;base64,{(logo_base64.decode('utf-8'))}",
+                encoding="utf-8",
+            )
+            ui.image(img.decode("utf-8"))
+        ui.icon("settings").tooltip("Settings").on("click", lambda: settings(dark))
+        ui.icon("delete").on("click", lambda: clear_db(log=logger)).tooltip(
+            "Clear all recorded data"
         )
-        img = bytes(
-            f"data:image/png;base64,{(logo_base64.decode('utf-8'))}",
-            encoding="utf-8",
+        ui.icon("upload").tooltip("Export Data").on("click", lambda: on_export(SERVER))
+        ui.icon("download").tooltip("Import Data").on(
+            "click", lambda: select_import(on_import)
         )
-        ui.image(img.decode("utf-8"))
-    ui.icon("settings").tooltip("Settings").on("click", lambda: settings(dark))
-    ui.icon("delete").on("click", lambda: clear_db(log=logger)).tooltip(
-        "Clear all recorded data"
-    )
-    ui.icon("upload").tooltip("Export Data").on("click", lambda: on_export(SERVER))
-    ui.icon("download").tooltip("Import Data").on(
-        "click", lambda: select_import(on_import)
-    )
-    ui.icon("share").tooltip("Share").on(
-        "click", lambda: (_ for _ in ()).throw(Exception(NotImplementedError))
-    )
-
-    with ui.splitter(value=20) as splitter:
-        splitter.classes("w-full h-full")
-        with splitter.before:
-            with ui.column().classes("w-full h-full"):
-                record_button = (
-                    ui.icon("radio_button_checked", size="64px")
-                    .on(
-                        "click",
-                        lambda: recording_prompt(OPTIONS, record_button),
+        ui.icon("share").tooltip("Share").on(
+            "click", lambda: (_ for _ in ()).throw(Exception(NotImplementedError))
+        )
+
+        with ui.splitter(value=20) as splitter:
+            splitter.classes("w-full h-full")
+            with splitter.before:
+                with ui.column().classes("w-full h-full"):
+                    record_button = (
+                        ui.icon("radio_button_checked", size="64px")
+                        .on(
+                            "click",
+                            lambda: recording_prompt(OPTIONS, record_button),
+                        )
+                        .tooltip("Record a new replay / Stop recording")
                     )
-                    .tooltip("Record a new replay / Stop recording")
-                )
-                ui.icon("visibility", size="64px").on("click", visualize.main).tooltip(
-                    "Visualize the latest replay"
-                )
-
-                ui.icon("play_arrow", size="64px").on(
-                    "click",
-                    lambda: replay.replay("NaiveReplayStrategy"),
-                ).tooltip("Play the latest replay")
-        with splitter.after:
-            logger = Console()
-            logger.log.style("height: 250px;, width: 300px;")
+                    ui.icon("visibility", size="64px").on(
+                        "click", partial(Popen, ["python", "-m", "openadapt.visualize"])
+                    ).tooltip("Visualize the latest replay")
 
-        splitter.enabled = False
+                    ui.icon("play_arrow", size="64px").on(
+                        "click",
+                        lambda: replay.replay("NaiveReplayStrategy"),
+                    ).tooltip("Play the latest replay")
+            with splitter.after:
+                logger = Console()
+                logger.log.style("height: 250px;, width: 300px;")
 
+            splitter.enabled = False
 
-def start(fullscreen: bool = False) -> None:
-    """Start the OpenAdapt application."""
     ui.run(
         title="OpenAdapt Client",
         native=True,
         window_size=(400, 400),
         fullscreen=fullscreen,
         reload=False,
         show=False,
```

### Comparing `openadapt-0.8.1/openadapt/app/objects/console.py` & `openadapt-0.9.0/openadapt/app/objects/console.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/app/objects/local_file_picker.py` & `openadapt-0.9.0/openadapt/app/objects/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/app/tray.py` & `openadapt-0.9.0/openadapt/app/tray.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Implementation of the system tray icon for OpenAdapt.
 
 usage: `python -m openadapt.app.tray` or `poetry run app`
 """
+
 from functools import partial
-from threading import Thread
+from subprocess import Popen
 import os
 import sys
 
+from loguru import logger
 from notifypy import Notify
 from PySide6.QtCore import QTimer
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QApplication, QMenu, QSystemTrayIcon
 
 from openadapt.app.cards import quick_record, stop_record
 from openadapt.app.main import FPATH, start
 from openadapt.crud import get_all_recordings
 from openadapt.extensions.thread import Thread as oaThread
 from openadapt.models import Recording
 from openadapt.replay import replay
-from openadapt.visualize import main as visualize
 
 # hide dock icon on macos
 if sys.platform == "darwin":
     import AppKit
 
     info = AppKit.NSBundle.mainBundle().infoDictionary()
     info["LSBackgroundOnly"] = "1"
@@ -74,14 +75,16 @@
         self.tray.setContextMenu(self.menu)
 
         self.timer = QTimer()
         self.timer.setInterval(1000)  # update every second
         self.timer.timeout.connect(self.update_tray_icon)
         self.timer.start()
 
+        self.visualize_proc = None
+
         Notify("Status", "OpenAdapt is running in the background.", "OpenAdapt").send()
 
     def update_tray_icon(self) -> None:
         """Update the tray icon."""
         try:
             if self.recording:
                 self.record_action.setText("Stop recording")
@@ -113,19 +116,24 @@
     def _visualize(self, recording: Recording) -> None:
         """Visualize a recording.
 
         Args:
             recording (Recording): The recording to visualize.
         """
         Notify("Status", "Starting visualization...", "OpenAdapt").send()
-        vthread = oaThread(target=visualize, args=(recording,))
-        vthread.run()
-        if vthread.join():
-            Notify("Status", "Visualization finished", "OpenAdapt").send()
-        else:
+        try:
+            if self.visualize_proc is not None:
+                self.visualize_proc.kill()
+            self.visualize_proc = Popen(
+                f"python -m openadapt.visualize --timestamp {recording.timestamp}",
+                shell=True,
+            )
+
+        except Exception as e:
+            logger.error(e)
             Notify("Status", "Visualization failed", "OpenAdapt").send()
 
     def _replay(self, recording: Recording) -> None:
         """Replay a recording.
 
         Args:
             recording (Recording): The recording to replay.
@@ -159,15 +167,15 @@
                 partial(action, recording)
             )
             menu.addAction(self.recording_actions[action_type][idx])
 
     def show_app(self) -> None:
         """Show the main application window."""
         if self.app_thread is None or not self.app_thread.is_alive():
-            self.app_thread = Thread(target=start, daemon=True, args=(True,))
+            self.app_thread = oaThread(target=start, daemon=True, args=(True,))
             self.app_thread.start()
 
     def run(self) -> None:
         """Run the system tray icon."""
         self.app.exec_()
```

### Comparing `openadapt-0.8.1/openadapt/app/util.py` & `openadapt-0.9.0/openadapt/app/util.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/cache.py` & `openadapt-0.9.0/openadapt/cache.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/config.py` & `openadapt-0.9.0/openadapt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,21 @@
         "task_description",
         "key_char",
         "canonical_key_char",
         "key_vk",
         "children",
     ],
     "PLOT_PERFORMANCE": True,
+    # VISUALIZATION CONFIGURATIONS
+    "VISUALIZE_DARK_MODE": False,
+    "VISUALIZE_RUN_NATIVELY": True,
+    "VISUALIZE_DENSE_TREES": True,
+    "VISUALIZE_ANIMATIONS": True,
+    "VISUALIZE_EXPAND_ALL": False,  # not recommended for large trees
+    "VISUALIZE_MAX_TABLE_CHILDREN": 10,
     # Calculate and save the difference between 2 neighboring screenshots
     "SAVE_SCREENSHOT_DIFF": False,
     "SPACY_MODEL_NAME": "en_core_web_trf",
     "SCRUB_PROVIDER_NAME": ["Presidio"],
 }
 
 # each string in STOP_STRS should only contain strings
@@ -128,14 +135,16 @@
     if type(rval) is str and rval.lower() in (
         "true",
         "false",
         "1",
         "0",
     ):
         rval = rval.lower() == "true" or rval == "1"
+    if type(rval) is str and rval.isnumeric():
+        rval = int(rval)
     if rval is None:
         raise ValueError(f"{var_name=} not defined")
     return rval
 
 
 def persist_env(var_name: str, val: str, env_file_path: str = ENV_FILE_PATH) -> None:
     """Persist an environment variable to a .env file.
```

### Comparing `openadapt-0.8.1/openadapt/crud.py` & `openadapt-0.9.0/openadapt/crud.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/db.py` & `openadapt-0.9.0/openadapt/db.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/events.py` & `openadapt-0.9.0/openadapt/events.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/extensions/synchronized_queue.py` & `openadapt-0.9.0/openadapt/extensions/synchronized_queue.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/logging.py` & `openadapt-0.9.0/openadapt/logging.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/models.py` & `openadapt-0.9.0/openadapt/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module defines the models used in the OpenAdapt system."""
 
 from typing import Union
 import io
 
 from loguru import logger
-from PIL import Image, ImageChops
 from oa_pynput import keyboard
+from PIL import Image, ImageChops
 import numpy as np
 import sqlalchemy as sa
 
 from openadapt import config, db, window
 
 
 # https://groups.google.com/g/sqlalchemy/c/wlr7sShU6-k
```

### Comparing `openadapt-0.8.1/openadapt/playback.py` & `openadapt-0.9.0/openadapt/playback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utilities for playing back ActionEvents."""
 
 from loguru import logger
-from oa_pynput import mouse, keyboard
+from oa_pynput import keyboard, mouse
 
 from openadapt.common import KEY_EVENTS, MOUSE_EVENTS
 from openadapt.models import ActionEvent
 
 
 def play_mouse_event(event: ActionEvent, mouse_controller: mouse.Controller) -> None:
     """Play a mouse event.
```

### Comparing `openadapt-0.8.1/openadapt/privacy/base.py` & `openadapt-0.9.0/openadapt/privacy/base.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/privacy/providers/presidio.py` & `openadapt-0.9.0/openadapt/privacy/providers/presidio.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/record.py` & `openadapt-0.9.0/openadapt/record.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import signal
 import sys
 import threading
 import time
 import tracemalloc
 
 from loguru import logger
-from pympler import tracker
 from oa_pynput import keyboard, mouse
+from pympler import tracker
 from tqdm import tqdm
 import fire
 import mss.tools
 import psutil
 
 from openadapt import config, crud, utils, window
 from openadapt.extensions import synchronized_queue as sq
```

### Comparing `openadapt-0.8.1/openadapt/replay.py` & `openadapt-0.9.0/openadapt/replay.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/scripts/reset_db.py` & `openadapt-0.9.0/openadapt/scripts/reset_db.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/scripts/scrub.py` & `openadapt-0.9.0/openadapt/scripts/scrub.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/start.py` & `openadapt-0.9.0/openadapt/start.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/base.py` & `openadapt-0.9.0/openadapt/strategies/base.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/demo.py` & `openadapt-0.9.0/openadapt/strategies/demo.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/mixins/ascii.py` & `openadapt-0.9.0/openadapt/strategies/mixins/ascii.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/mixins/huggingface.py` & `openadapt-0.9.0/openadapt/strategies/mixins/huggingface.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/mixins/ocr.py` & `openadapt-0.9.0/openadapt/strategies/mixins/ocr.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/mixins/openai.py` & `openadapt-0.9.0/openadapt/strategies/mixins/openai.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/mixins/sam.py` & `openadapt-0.9.0/openadapt/strategies/mixins/sam.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from pathlib import Path
 import urllib
 
 from loguru import logger
 from PIL import Image
 from segment_anything import (
-    modeling,
     SamAutomaticMaskGenerator,
     SamPredictor,
+    modeling,
     sam_model_registry,
 )
 import matplotlib.axes as axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 from openadapt.models import Recording, Screenshot
```

### Comparing `openadapt-0.8.1/openadapt/strategies/mixins/summary.py` & `openadapt-0.9.0/openadapt/strategies/mixins/summary.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/strategies/naive.py` & `openadapt-0.9.0/openadapt/strategies/naive.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from openadapt import config, models, strategies, utils
 
 DISPLAY_EVENTS = False
 PROCESS_EVENTS = True
 REPLAY_EVENTS = True
 SLEEP = False
+assert PROCESS_EVENTS or not SLEEP, "invalid configuration"
 
 
 class NaiveReplayStrategy(strategies.base.BaseReplayStrategy):
     """Naive playback strategy that replays ActionEvents directly."""
 
     def __init__(
         self,
```

### Comparing `openadapt-0.8.1/openadapt/strategies/stateful.py` & `openadapt-0.9.0/openadapt/strategies/stateful.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/utils.py` & `openadapt-0.9.0/openadapt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -651,25 +651,38 @@
 
     strategy_classes = BaseReplayStrategy.__subclasses__()
     class_by_name = {cls.__name__: cls for cls in strategy_classes}
     logger.debug(f"{class_by_name=}")
     return class_by_name
 
 
-def plot_performance(recording_timestamp: float = None) -> None:
+def plot_performance(
+    recording_timestamp: float = None,
+    view_file: bool = True,
+    save_file: bool = True,
+    dark_mode: bool = False,
+) -> str:
     """Plot the performance of the event processing and writing.
 
     Args:
-        recording_timestamp (float): The timestamp of the recording
-          (defaults to latest).
+        recording_timestamp: The timestamp of the recording (defaults to latest)
+        view_file: Whether to view the file after saving it.
+        save_file: Whether to save the file.
+        dark_mode: Whether to use dark mode.
+
+    Returns:
+        str: a base64-encoded image of the plot, if not viewing the file
     """
     type_to_proc_times = defaultdict(list)
     type_to_timestamps = defaultdict(list)
     event_types = set()
 
+    if dark_mode:
+        plt.style.use("dark_background")
+
     # avoid circular import
     from openadapt import crud
 
     if not recording_timestamp:
         recording_timestamp = crud.get_latest_recording().timestamp
     perf_stats = crud.get_perf_stats(recording_timestamp)
     for perf_stat in perf_stats:
@@ -714,21 +727,34 @@
         all_labels = labels1 + labels2
 
         ax.legend(all_handles, all_labels)
 
     ax.set_title(f"{recording_timestamp=}")
 
     # TODO: add PROC_WRITE_BY_EVENT_TYPE
-    fname_parts = ["performance", str(recording_timestamp)]
-    fname = "-".join(fname_parts) + ".png"
-    os.makedirs(config.DIRNAME_PERFORMANCE_PLOTS, exist_ok=True)
-    fpath = os.path.join(config.DIRNAME_PERFORMANCE_PLOTS, fname)
-    logger.info(f"{fpath=}")
-    plt.savefig(fpath)
-    os.system(f"open {fpath}")
+    if save_file:
+        fname_parts = ["performance", str(recording_timestamp)]
+        fname = "-".join(fname_parts) + ".png"
+        os.makedirs(config.DIRNAME_PERFORMANCE_PLOTS, exist_ok=True)
+        fpath = os.path.join(config.DIRNAME_PERFORMANCE_PLOTS, fname)
+        logger.info(f"{fpath=}")
+        plt.savefig(fpath)
+        if view_file:
+            os.system(f"open {fpath}")
+    else:
+        plt.savefig(BytesIO(), format="png")  # save fig to void
+        if view_file:
+            plt.show()
+        else:
+            plt.close()
+        return image2utf8(
+            Image.frombytes(
+                "RGB", fig.canvas.get_width_height(), fig.canvas.tostring_rgb()
+            )
+        )
 
 
 def strip_element_state(action_event: ActionEvent) -> ActionEvent:
     """Strip the element state from the action event and its children.
 
     Args:
         action_event (ActionEvent): The action event to strip.
```

### Comparing `openadapt-0.8.1/openadapt/visualize.py` & `openadapt-0.9.0/openadapt/deprecated/visualize.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/window/__init__.py` & `openadapt-0.9.0/openadapt/window/__init__.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/openadapt/window/_macos.py` & `openadapt-0.9.0/openadapt/window/_macos.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import pickle
 import plistlib
 import re
 
 from loguru import logger
 import AppKit
 import ApplicationServices
-import oa_atomacos
 import Foundation
+import oa_atomacos
 import Quartz
 
 
 def get_active_window_state() -> dict | None:
     """Get the state of the active window.
 
     Returns:
```

### Comparing `openadapt-0.8.1/openadapt/window/_windows.py` & `openadapt-0.9.0/openadapt/window/_windows.py`

 * *Files identical despite different names*

### Comparing `openadapt-0.8.1/pyproject.toml` & `openadapt-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "openadapt"
-version = "0.8.1"
+version = "0.9.0"
 description = "GUI Process Automation with Transformers"
 authors = [
     'OpenAdapt.AI Team <richard.abrich@mldsai.com>',
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Operating System :: OS Independent"
+    "Operating System :: OS Independent",
 ]
 
 readme = "README.md"
 
 repository = "https://github.com/mldsai/openadapt"
 homepage = "https://openadapt.ai/"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MLDSAI/OpenAdapt/issues"
 
 [tool.poetry.dependencies]
 python = "3.10.x"
 alembic = "1.8.1"
 black = "23.3.0"
-pygetwindow = {version = "<0.0.5", markers = "sys_platform == 'win32'"}
-pywin32 = {version = "306", markers = "sys_platform == 'win32'"}
+pygetwindow = { version = "<0.0.5", markers = "sys_platform == 'win32'" }
+pywin32 = { version = "306", markers = "sys_platform == 'win32'" }
 ascii-magic = "2.3.0"
 bokeh = "2.4.3"
 clipboard = "0.0.4"
-deepdiff = {extras = ["optimize"], version = "^6.3.0"}
+deepdiff = { extras = ["optimize"], version = "^6.3.0" }
 ascii_magic = "2.3.0"
 dictalchemy3 = "1.0.0"
 fire = "0.4.0"
 ipdb = "0.13.11"
 loguru = "0.6.0"
 matplotlib = "3.6.2"
 mss = "6.1.0"
@@ -49,15 +49,15 @@
 torch = "^2.0.0"
 tqdm = "4.64.0"
 transformers = "4.29.2"
 python-dotenv = "1.0.0"
 pyinstaller = "^5.12.0"
 setuptools-lint = "^0.6.0"
 sphinx = "7.0.1"
-nicegui = "1.2.24"
+nicegui = "^1.2.24"
 spacy = "^3.5.3"
 fuzzywuzzy = "0.18.0"
 segment-anything = "^1.0"
 torchvision = "^0.15.2"
 sumy = "0.11.0"
 nltk = "3.8.1"
 pillow = "9.5.0"
@@ -68,21 +68,31 @@
 python-levenshtein = "^0.21.1"
 pyside6 = "^6.5.1.1"
 notify-py = "^0.3.42"
 flake8-annotations = "^3.0.1"
 pre-commit = "^3.3.3"
 pympler = "^1.0.1"
 psutil = "^5.9.5"
-pyobjc-framework-avfoundation = {version = "^9.2", markers = "sys_platform == 'darwin'"}
+tomlkit = "^0.11.8"
+pyobjc-framework-avfoundation = { version = "^9.2", markers = "sys_platform == 'darwin'" }
 fastapi = "0.98.0"
 oa-pynput = "^1.7.7"
 oa-atomacos = {version = "3.2.0", markers = "sys_platform == 'darwin'"}
 presidio-image-redactor = "^0.0.48"
+pywebview = "^4.2.2"
+click = "^8.1.6"
 spacy-transformers = "^1.2.5"
 
+[tool.pytest.ini_options]
+filterwarnings = [
+    # suppress warnings starting from "setuptools>=67.3"
+    "ignore:Deprecated call to `pkg_resources\\.declare_namespace\\('.*'\\):DeprecationWarning",
+    "ignore:pkg_resources is deprecated as an API",
+]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 group_by_package = true
@@ -100,20 +110,16 @@
 /(
   | venv
   | alembic
 )/
 '''
 
 [tool.semantic_release]
-version_variable = [
-    "openadapt/__init__.py:__version__"
-]
-version_toml = [
-    "pyproject.toml:tool.poetry.version"
-]
+version_variable = ["openadapt/__init__.py:__version__"]
+version_toml = ["pyproject.toml:tool.poetry.version"]
 major_on_zero = false
 branch = "main"
 commit_subject = "chore(release): v{version}"
 commit_version_number = true
 upload_to_PyPI = false
 upload_to_release = true
 upload_to_repository = false
```

### Comparing `openadapt-0.8.1/PKG-INFO` & `openadapt-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: openadapt
-Version: 0.8.1
+Version: 0.9.0
 Summary: GUI Process Automation with Transformers
 Home-page: https://openadapt.ai/
 Author: OpenAdapt.AI Team
 Author-email: richard.abrich@mldsai.com
 Requires-Python: ==3.10.*
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: alembic (==1.8.1)
 Requires-Dist: ascii-magic (==2.3.0)
 Requires-Dist: ascii_magic (==2.3.0)
 Requires-Dist: black (==23.3.0)
 Requires-Dist: bokeh (==2.4.3)
+Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: clipboard (==0.0.4)
 Requires-Dist: deepdiff[optimize] (>=6.3.0,<7.0.0)
 Requires-Dist: dictalchemy3 (==1.0.0)
 Requires-Dist: fastapi (==0.98.0)
 Requires-Dist: fire (==0.4.0)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: flake8-annotations (>=3.0.1,<4.0.0)
 Requires-Dist: flake8-docstrings (>=1.7.0,<2.0.0)
 Requires-Dist: fuzzywuzzy (==0.18.0)
 Requires-Dist: ipdb (==0.13.11)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: matplotlib (==3.6.2)
 Requires-Dist: moviepy (==1.0.3)
 Requires-Dist: mss (==6.1.0)
-Requires-Dist: nicegui (==1.2.24)
+Requires-Dist: nicegui (>=1.2.24,<2.0.0)
 Requires-Dist: nltk (==3.8.1)
 Requires-Dist: notify-py (>=0.3.42,<0.4.0)
 Requires-Dist: oa-atomacos (==3.2.0) ; sys_platform == "darwin"
 Requires-Dist: oa-pynput (>=1.7.7,<2.0.0)
 Requires-Dist: openai (==0.27.5)
 Requires-Dist: pandas (==2.0.0)
 Requires-Dist: pillow (==9.5.0)
@@ -46,27 +47,29 @@
 Requires-Dist: pympler (>=1.0.1,<2.0.0)
 Requires-Dist: pyobjc-framework-avfoundation (>=9.2,<10.0) ; sys_platform == "darwin"
 Requires-Dist: pyside6 (>=6.5.1.1,<7.0.0.0)
 Requires-Dist: pytesseract (==0.3.7)
 Requires-Dist: pytest (==7.1.3)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: python-levenshtein (>=0.21.1,<0.22.0)
+Requires-Dist: pywebview (>=4.2.2,<5.0.0)
 Requires-Dist: pywin32 (==306) ; sys_platform == "win32"
 Requires-Dist: pywinauto (>=0.6.8,<0.7.0) ; sys_platform == "win32"
 Requires-Dist: rapidocr-onnxruntime (==1.2.3)
 Requires-Dist: scikit-learn (==1.2.2)
 Requires-Dist: scipy (==1.9.3)
 Requires-Dist: segment-anything (>=1.0,<2.0)
 Requires-Dist: setuptools-lint (>=0.6.0,<0.7.0)
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: spacy-transformers (>=1.2.5,<2.0.0)
 Requires-Dist: sphinx (==7.0.1)
 Requires-Dist: sqlalchemy (==1.4.43)
 Requires-Dist: sumy (==0.11.0)
 Requires-Dist: tiktoken (==0.4.0)
+Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Requires-Dist: tqdm (==4.64.0)
 Requires-Dist: transformers (==4.29.2)
 Project-URL: Bug Tracker, https://github.com/MLDSAI/OpenAdapt/issues
 Project-URL: Repository, https://github.com/mldsai/openadapt
 Description-Content-Type: text/markdown
@@ -333,29 +336,37 @@
 validations on your codebase.
 
 The following pre-commit hooks are used in OpenAdapt:
 
 - [check-yaml](https://github.com/pre-commit/pre-commit-hooks#check-yaml): Validates the syntax and structure of YAML files.
 - [end-of-file-fixer](https://github.com/pre-commit/pre-commit-hooks#end-of-file-fixer): Ensures that files end with a newline character.
 - [trailing-whitespace](https://github.com/pre-commit/pre-commit-hooks#trailing-whitespace): Detects and removes trailing whitespace at the end of lines.
-- [black](https://github.com/psf/black): Formats Python code to adhere to the Black code style.
+- [black](https://github.com/psf/black): Formats Python code to adhere to the Black code style. Notably, the `--preview` feature is used.
 - [isort](https://github.com/PyCQA/isort): Sorts Python import statements in a consistent and standardized manner.
 
 To set up the pre-commit hooks, follow these steps:
 
 1. Navigate to the root directory of your OpenAdapt repository.
 
 2. Run the following command to install the hooks:
 
 ```
 pre-commit install
 ```
 
 Now, the pre-commit hooks are installed and will run automatically before each commit. They will enforce code quality standards and prevent committing code that doesn't pass the defined checks.
 
+### Status Checks
+
+When you submit a PR, the "Python CI" workflow is triggered for code consistency. It follows organized steps to review your code:
+
+1. **Python Black Check** : This step verifies code formatting using Python Black style, with the `--preview` flag for style.
+
+2. **Flake8 Review** : Next, Flake8 tool thoroughly checks code structure, including flake8-annotations and flake8-docstrings. Though GitHub Actions automates checks, it's wise to locally run `flake8 .` before finalizing changes for quicker issue spotting and resolution.
+
 # Submitting an Issue
 
 Please submit any issues to https://github.com/OpenAdaptAI/OpenAdapt/issues with the
 following information:
 
 - Problem description (please include any relevant console output and/or screenshots)
 - Steps to reproduce (please help others to help you!)
```

