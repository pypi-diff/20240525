# Comparing `tmp/mkdocs_ai_summary-0.2.2.tar.gz` & `tmp/mkdocs_ai_summary-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ai_summary-0.2.2.tar", last modified: Thu May 23 05:41:00 2024, max compression
+gzip compressed data, was "mkdocs_ai_summary-0.2.3.tar", last modified: Sat May 25 02:05:45 2024, max compression
```

## Comparing `mkdocs_ai_summary-0.2.2.tar` & `mkdocs_ai_summary-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:41:00.236763 mkdocs_ai_summary-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-23 05:40:51.000000 mkdocs_ai_summary-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-23 05:41:00.236763 mkdocs_ai_summary-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:41:00.232763 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:40:51.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-23 05:40:51.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/chatgpt_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-23 05:40:51.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-23 05:40:51.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/tongyi_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:41:00.236763 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-23 05:41:00.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-23 05:41:00.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:41:00.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 05:41:00.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-23 05:41:00.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-23 05:41:00.000000 mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 05:40:51.000000 mkdocs_ai_summary-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-23 05:40:51.000000 mkdocs_ai_summary-0.2.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:41:00.236763 mkdocs_ai_summary-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:45.001359 mkdocs_ai_summary-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-25 02:05:45.001359 mkdocs_ai_summary-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:44.997359 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/tongyi_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:05:44.997359 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-25 02:05:44.000000 mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-25 02:05:35.000000 mkdocs_ai_summary-0.2.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:05:45.001359 mkdocs_ai_summary-0.2.3/setup.cfg
```

### Comparing `mkdocs_ai_summary-0.2.2/LICENSE` & `mkdocs_ai_summary-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.2.2/PKG-INFO` & `mkdocs_ai_summary-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.2.2
+Version: 0.2.3
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/chatgpt_api.py` & `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/chatgpt_api.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/plugin.py` & `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from mkdocs import plugins
 from mkdocs.config import config_options
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.exceptions import ConfigurationError
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
 
@@ -9,15 +10,15 @@
 import logging
 
 logger = logging.getLogger("mkdocs.plugins.ai-summary")
 
 
 class AiSummaryPlugin(BasePlugin):
     config_scheme = (
-        ("api", config_options.Type(str, default="chatgpt")),
+        ("api", config_options.Choice(["chatgpt", "tongyi"], default="chatgpt")),
         ("ignore_code", config_options.Type(bool, default=True)),
         ("cache", config_options.Type(bool, default=True)),
         ("cache_dir", config_options.Type(str, default="./")),
         (
             "model",
             config_options.Type(str, default="gpt-3.5-turbo"),
         ),
@@ -27,14 +28,15 @@
                 str,
                 default="Please help me summarize the following content into an"
                 "abstract within 200 words: ",
             ),
         ),
     )
 
+    @plugins.event_priority(50)
     def on_page_markdown(
         self, markdown: str, *, page: Page, config: MkDocsConfig, files: Files
     ) -> str | None:
         # add ai-summary only when meta info say it is included
         if page.meta:
             if "ai-summary" not in page.meta.get("include", {}):
                 return markdown
@@ -56,15 +58,15 @@
             case "tongyi":
                 try:
                     from .tongyi_api import get_summary_tongyi, AiSummaryError
                 except ImportError as e:
                     logger.warning("tongyi is not available", repr(e))
                     return markdown
 
-                logger.info(f"Asking AI summary for page {page.title}")
+                logger.info(f"Asking AI summary for page {page.title}({page.url})")
                 try:
                     summary = get_summary_tongyi(
                         page=str(page.title),
                         prompt=prompt,
                         markdown=markdown_to_summary,
                         cache=cache,
                         cache_dir=cache_dir,
@@ -80,15 +82,15 @@
             case "chatgpt":
                 try:
                     from .chatgpt_api import get_summary_chatgpt
                 except ImportError as e:
                     logger.warning("chatgpt is not available", repr(e))
                     return markdown
 
-                logger.info(f"Asking AI summary for page {page.title}")
+                logger.info(f"Asking AI summary for page {page.title}({page.url})")
                 try:
                     summary = get_summary_chatgpt(
                         page=str(page.title),
                         prompt=prompt,
                         markdown=markdown_to_summary,
                         cache=cache,
                         cache_dir=cache_dir,
```

### Comparing `mkdocs_ai_summary-0.2.2/mkdocs_ai_summary/tongyi_api.py` & `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary/tongyi_api.py`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.2.2/mkdocs_ai_summary.egg-info/PKG-INFO` & `mkdocs_ai_summary-0.2.3/mkdocs_ai_summary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.2.2
+Version: 0.2.3
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `mkdocs_ai_summary-0.2.2/pyproject.toml` & `mkdocs_ai_summary-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [project]
 name = "mkdocs-ai-summary"
-version = "0.2.2"
+version = "0.2.3"
 requires-python = ">=3.10"
 dependencies = [
     "mkdocs>=1.5.3",
 ]
 authors = [
   { name="Yang Zhang", email="mail@yangzhang.site" },
 ]
```

### Comparing `mkdocs_ai_summary-0.2.2/readme.md` & `mkdocs_ai_summary-0.2.3/readme.md`

 * *Files identical despite different names*

