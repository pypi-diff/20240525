# Comparing `tmp/telegramify_markdown-0.1.2.tar.gz` & `tmp/telegramify_markdown-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegramify_markdown-0.1.2.tar", last modified: Sun Mar 17 06:45:42 2024, max compression
+gzip compressed data, was "telegramify_markdown-0.1.3.tar", last modified: Sat May 25 10:43:37 2024, max compression
```

## Comparing `telegramify_markdown-0.1.2.tar` & `telegramify_markdown-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/LICENSE
--rw-r--r--   0        0        0     1971 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/README.md
--rw-r--r--   0        0        0      653 2024-03-17 06:45:42.376406 telegramify_markdown-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1368 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/src/telegramify_markdown/__init__.py
--rw-r--r--   0        0        0      336 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/src/telegramify_markdown/customize.py
--rw-r--r--   0        0        0     5578 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/src/telegramify_markdown/render.py
--rw-r--r--   0        0        0      941 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/tests/exp1.md
--rw-r--r--   0        0        0      437 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/tests/exp_test.py
--rw-r--r--   0        0        0      608 2024-03-17 06:45:31.124341 telegramify_markdown-0.1.2/tests/server.py
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 telegramify_markdown-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2581 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/README.md
+-rw-r--r--   0        0        0      653 2024-05-25 10:43:37.866512 telegramify_markdown-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1656 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/src/telegramify_markdown/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/src/telegramify_markdown/customize.py
+-rw-r--r--   0        0        0     6062 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/src/telegramify_markdown/render.py
+-rw-r--r--   0        0        0     1908 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/tests/exp1.md
+-rw-r--r--   0        0        0      437 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/tests/exp_test.py
+-rw-r--r--   0        0        0      608 2024-05-25 10:43:24.418334 telegramify_markdown-0.1.3/tests/server.py
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 telegramify_markdown-0.1.3/PKG-INFO
```

### Comparing `telegramify_markdown-0.1.2/LICENSE` & `telegramify_markdown-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `telegramify_markdown-0.1.2/pyproject.toml` & `telegramify_markdown-0.1.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "telegramify-markdown"
-version = "0.1.2"
+version = "0.1.3"
 description = "Convert Markdown to a format usable by Telegram."
 authors = [
     { name = "sudoskys", email = "coldlando@hotmail.com" },
 ]
 dependencies = [
-    "mistletoe>=1.3.0",
+    "mistletoe==1.3.0",
     "pytelegrambotapi>=4.16.1",
     "emoji>=2.10.1",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
```

### Comparing `telegramify_markdown-0.1.2/src/telegramify_markdown/render.py` & `telegramify_markdown-0.1.3/src/telegramify_markdown/render.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Iterable
 
 from mistletoe import block_token, span_token
 from mistletoe.markdown_renderer import MarkdownRenderer, LinkReferenceDefinition, Fragment
 from telebot import formatting
+
 from .customize import markdown_symbol
 
 
 class TelegramMarkdownRenderer(MarkdownRenderer):
 
     def render_heading(
             self, token: block_token.Heading, max_line_length: int
@@ -60,19 +61,22 @@
     def render_setext_heading(
             self, token: block_token.SetextHeading, max_line_length: int
     ) -> Iterable[str]:
         yield from self.span_to_lines(token.children, max_line_length=max_line_length)
         yield formatting.escape_markdown("——" * 5)
 
     def render_emphasis(self, token: span_token.Emphasis) -> Iterable[Fragment]:
-        token.delimiter = "_"
         return super().render_emphasis(token)
 
     def render_strong(self, token: span_token.Strong) -> Iterable[Fragment]:
-        return self.embed_span(Fragment(token.delimiter * 1), token.children)
+        # Telegram strong: *text* but __text__ for emphasis, so we need to check the delimiter
+        if token.delimiter == "*":
+            return self.embed_span(Fragment(token.delimiter * 1), token.children)
+        # __
+        return self.embed_span(Fragment(token.delimiter * 2), token.children)
 
     def render_strikethrough(
             self, token: span_token.Strikethrough
     ) -> Iterable[Fragment]:
         return self.embed_span(Fragment("~"), token.children)
 
     def render_list_item(
@@ -125,13 +129,20 @@
         else:
             # "[" description "]"
             pass
 
     def render_auto_link(self, token: span_token.AutoLink) -> Iterable[Fragment]:
         yield Fragment(formatting.escape_markdown("<") + token.children[0].content + formatting.escape_markdown(">"))
 
+    def render_escape_sequence(
+            self, token: span_token.EscapeSequence
+    ) -> Iterable[Fragment]:
+        # 渲染转义字符
+        # because the escape_markdown already happened in the parser, we can skip it here.
+        yield Fragment("" + token.children[0].content)
+
     def render_table(
             self, token: block_token.Table, max_line_length: int
     ) -> Iterable[str]:
         # note: column widths are not preserved; they are automatically adjusted to fit the contents.
         fs = super().render_table(token, max_line_length)
         return [formatting.mcode("\n".join(fs))]
```

### Comparing `telegramify_markdown-0.1.2/tests/server.py` & `telegramify_markdown-0.1.3/tests/server.py`

 * *Files identical despite different names*

