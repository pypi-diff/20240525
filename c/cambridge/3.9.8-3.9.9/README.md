# Comparing `tmp/cambridge-3.9.8.tar.gz` & `tmp/cambridge-3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cambridge-3.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cambridge-3.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cambridge-3.9.8.tar` & `cambridge-3.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.8/.gitignore
--rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.8/LICENSE
--rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.8/README.md
--rw-r--r--   0        0        0      266 2024-05-24 04:32:32.406246 cambridge-3.9.8/cambridge/__init__.py
--rw-r--r--   0        0        0     8610 2024-05-24 04:12:20.868957 cambridge-3.9.8/cambridge/args.py
--rw-r--r--   0        0        0     2306 2024-04-02 14:57:17.675678 cambridge-3.9.8/cambridge/cache.py
--rw-r--r--   0        0        0     1769 2024-05-23 14:16:50.775853 cambridge-3.9.8/cambridge/color.py
--rw-r--r--   0        0        0     3159 2024-05-24 02:25:10.074112 cambridge-3.9.8/cambridge/console.py
--rw-r--r--   0        0        0    18593 2024-05-24 02:25:10.076072 cambridge-3.9.8/cambridge/dicts/cambridge.py
--rw-r--r--   0        0        0     5597 2024-05-24 02:25:10.077496 cambridge-3.9.8/cambridge/dicts/dict.py
--rw-r--r--   0        0        0    44386 2024-05-24 04:32:32.407192 cambridge-3.9.8/cambridge/dicts/webster.py
--rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.8/cambridge/errors.py
--rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.8/cambridge/log.py
--rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.8/cambridge/main.py
--rw-r--r--   0        0        0     2561 2024-03-13 08:59:30.744980 cambridge-3.9.8/cambridge/utils.py
--rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.8/pyproject.toml
--rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.8/requirements.txt
--rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.8/screenshots/cambridge.png
--rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.8/screenshots/fzf.png
--rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.8/screenshots/webster.png
--rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.8/PKG-INFO
+-rw-r--r--   0        0        0       72 2024-03-03 06:01:31.364439 cambridge-3.9.9/.gitignore
+-rw-r--r--   0        0        0    32422 2022-09-14 04:27:11.000000 cambridge-3.9.9/LICENSE
+-rw-r--r--   0        0        0     4122 2024-03-06 13:40:28.754758 cambridge-3.9.9/README.md
+-rw-r--r--   0        0        0      266 2024-05-25 07:32:51.334686 cambridge-3.9.9/cambridge/__init__.py
+-rw-r--r--   0        0        0    10189 2024-05-25 07:09:06.355266 cambridge-3.9.9/cambridge/args.py
+-rw-r--r--   0        0        0     2306 2024-04-02 14:57:17.675678 cambridge-3.9.9/cambridge/cache.py
+-rw-r--r--   0        0        0     1769 2024-05-23 14:16:50.775853 cambridge-3.9.9/cambridge/color.py
+-rw-r--r--   0        0        0     3159 2024-05-24 02:25:10.074112 cambridge-3.9.9/cambridge/console.py
+-rw-r--r--   0        0        0    18593 2024-05-25 07:09:06.358931 cambridge-3.9.9/cambridge/dicts/cambridge.py
+-rw-r--r--   0        0        0     5597 2024-05-25 07:09:06.361275 cambridge-3.9.9/cambridge/dicts/dict.py
+-rw-r--r--   0        0        0    44396 2024-05-25 07:28:19.803107 cambridge-3.9.9/cambridge/dicts/webster.py
+-rw-r--r--   0        0        0      770 2024-03-11 05:51:25.317401 cambridge-3.9.9/cambridge/errors.py
+-rw-r--r--   0        0        0      599 2024-03-05 14:25:39.642688 cambridge-3.9.9/cambridge/log.py
+-rw-r--r--   0        0        0      682 2024-03-05 14:25:39.643531 cambridge-3.9.9/cambridge/main.py
+-rw-r--r--   0        0        0     2561 2024-05-25 07:09:06.369628 cambridge-3.9.9/cambridge/utils.py
+-rw-r--r--   0        0        0      731 2024-03-03 06:01:31.379053 cambridge-3.9.9/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-03-03 06:01:31.380018 cambridge-3.9.9/requirements.txt
+-rw-r--r--   0        0        0   430578 2024-03-06 13:51:33.866712 cambridge-3.9.9/screenshots/cambridge.png
+-rw-r--r--   0        0        0   338780 2023-08-21 11:28:38.010650 cambridge-3.9.9/screenshots/fzf.png
+-rw-r--r--   0        0        0   228507 2023-11-10 15:57:56.401249 cambridge-3.9.9/screenshots/webster.png
+-rw-r--r--   0        0        0     4827 1970-01-01 00:00:00.000000 cambridge-3.9.9/PKG-INFO
```

### Comparing `cambridge-3.9.8/LICENSE` & `cambridge-3.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/README.md` & `cambridge-3.9.9/README.md`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/args.py` & `cambridge-3.9.9/cambridge/args.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import sqlite3
 import logging
 import argparse
 import sys
+import os
+import subprocess
 
 from .cache import (
     get_response_words,
     get_random_words,
     delete_word,
 )
+from .console import c_print
 from .log import logger
 from .utils import OP, DICT
 from .dicts import webster, cambridge
 from .__init__ import __version__
 
 def parse_args():
     parser = argparse.ArgumentParser(
@@ -189,27 +192,56 @@
             if "cambridge" in i[1]:
                 print(f'{OP.DELETED.name} "{word}" from {DICT.CAMBRIDGE.name} in cache successfully')
             else:
                 print(f'{OP.DELETED.name} "{word}" from {DICT.MERRIAM_WEBSTER.name} in cache successfully')
     else:
         print(f'{OP.NOT_FOUND.name} "{word}" in cache')
 
-def print_word(entry, cols=40, print_dict_name=True):
-    if (not isinstance(entry, tuple)) or len(entry) < 2:
-        print("not valid")
+
+def print_word(index, entry):
+    cols = os.get_terminal_size().columns
+    text = entry[0]
+    text_len = len(text)
 
     if "cambridge" in entry[1]:
-        dict_name = DICT.CAMBRIDGE.name
+        dict_name = "CAMBRIDGE"
+    else:
+        dict_name = "WEBSTER"
+
+    if index % 2 == 0:
+        print(f"\033[37;;40m{index+1:6d}|{text}", end="")
+        print(f"\033[37;;40m{dict_name:>{cols-text_len-7}}\033[0m")
+
     else:
-        dict_name = DICT.MERRIAM_WEBSTER.name
+        c_print(f"#[#4A7D95]{index+1:6d}|{text}", end="")
+        c_print(f"#[#4A7D95]{dict_name:>{cols-text_len-7}}")
 
-    if print_dict_name:
-        print(f"{entry[0]:<{cols}}", dict_name)
+
+def is_tool(name):
+    """Check whether `name` is on $PATH and marked as executable."""
+
+    from shutil import which
+    return which(name) is not None
+
+
+def fzf(data, con, cur):
+    choices = {}
+    for entry in data:
+        choices[entry[0]] = entry[1]
+
+    c = "\n".join(choices.keys())
+    p1 = subprocess.Popen(["echo", c], stdout=subprocess.PIPE, text=True)
+    p2 = subprocess.Popen(["fzf", "--layout=reverse"], stdin=p1.stdout, stdout=subprocess.PIPE, text=True)
+    input_word = p2.communicate()[0].strip("\n")
+    if p2.returncode == 130 and input_word == "": # press ESC, not word selected, quit out of fzf
+        exit()
+    if "merrian" in choices[input_word]:
+        webster.search_webster(con, cur, input_word)
     else:
-        print(f"{entry[0]}")
+        cambridge.search_cambridge(con, cur, input_word)
 
 
 def list_words(args, con, cur):
     # The subparser i.e. the sub-command isn't in the namespace of args
 
     if args.delete:
         to_delete = args.delete
@@ -221,31 +253,48 @@
 
     elif args.random:
         try:
             data = get_random_words(cur)
         except sqlite3.OperationalError:
             logger.error("You may haven't searched any word yet")
         else:
-            for entry in data:
-                print_word(entry)
+            if not is_tool("fzf"):
+                print()
+                for index, entry in enumerate(data):
+                    print_word(index, entry)
+                print()
+            else:
+                fzf(data, con, cur)
 
     else:
         try:
             data = get_response_words(cur)
         except sqlite3.OperationalError:
             logger.error("You may haven't searched any word yet")
         else:
             if args.time:
-                data.sort(reverse=False, key=lambda tup: tup[2])
-                for entry in data:
-                    print_word(entry)
+                if not is_tool("fzf"):
+                    data.sort(reverse=False, key=lambda tup: tup[2])
+                    print()
+                    for index, entry in enumerate(data):
+                        print_word(index, entry)
+                    print()
+                else:
+                    data.sort(reverse=True, key=lambda tup: tup[2])
+                    fzf(data, con, cur)
             else:
                 data.sort()
-                for entry in data:
-                    print_word(entry, print_dict_name=False)
+                if not is_tool("fzf"):
+                    print()
+                    for index, entry in enumerate(data):
+                        print_word(index, entry)
+                    print()
+                else:
+                    fzf(data, con, cur)
+
 
 def search_word(args, con, cur):
     """
     The function is triggered when a user searches a word or phrase on terminal.
     First checks the args having "verbose" in it or not, if so, the debug mode will be turned on.
     Then it checks which dictionary is intended, and then calls respective dictionary function.
     """
```

### Comparing `cambridge-3.9.8/cambridge/cache.py` & `cambridge-3.9.9/cambridge/cache.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/color.py` & `cambridge-3.9.9/cambridge/color.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/console.py` & `cambridge-3.9.9/cambridge/console.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/dicts/cambridge.py` & `cambridge-3.9.9/cambridge/dicts/cambridge.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/dicts/dict.py` & `cambridge-3.9.9/cambridge/dicts/dict.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/dicts/webster.py` & `cambridge-3.9.9/cambridge/dicts/webster.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,15 +696,15 @@
                 continue
 
             if elm_attr == "sub-content-thread":
                 sub_content_thread(elm, ancestor_attr, num_label_count) # example under the meaning
                 has_badge = False
                 continue
 
-            if elm_attr == "ca" or elm_attr == "dx-jump":
+            if elm_attr == "ca":
                 extra(elm, ancestor_attr)
                 continue
 
             if elm_attr == "unText":
                 unText_simple(elm, ancestor_attr, num_label_count, has_badge)
                 continue
 
@@ -836,15 +836,15 @@
         if attr is not None:
             if elm.tag == "span" and "fw-bold ure" in attr:
                 c_print(f"#[bold {w_col.wf}]{elm.text}", end = " ")
                 continue
 
             if elm.tag == "span" and "fw-bold fl" in attr:
                 next_sibling = elm.getnext()
-                c_print(f"#[yellow]{elm.text}", end = "")
+                c_print(f"#[{w_col.eh_word_type}]{elm.text}", end = "")
                 continue
 
             if "ins" in attr:
                 print("", end="")
                 print_class_ins(elm)
                 continue
 
@@ -950,52 +950,57 @@
 
 
 # --- parse class "dictionary-entry-[number]" --- #
 def dictionary_entry(node):
     """Print one entry of the word and its attributes like plural types, pronounciations, tenses, etc."""
 
     print()
-
     for elm in node.iterchildren():
-        try:
-            if elm.attrib["class"]:
-                if "row entry-header" in elm.attrib["class"]:
-                    row_entry_header(elm)
-
-                if elm.attrib["class"] == "row headword-row header-ins":
-                    row_headword_row_header_ins(elm)
-
-                if elm.attrib["class"] == "row headword-row header-vrs":
-                    row_headword_row_header_vrs(elm)
-
-                if elm.attrib["class"] == "vg":
-                    vg(elm)
-
-                if "entry-uros" in elm.attrib["class"]:
-                    for i in elm.iterchildren():
-                        entry_uros(i)
-                        print()
-
-                if elm.attrib["class"] == "dxnls":
-                    dxnls(elm)
-
-                if elm.attrib["class"] == "mt-3":
-                    badge = elm.getchildren()[0] # class "lbs badge mw-badge-gray-100 text-start text-wrap d-inline"
-                    print_header_badge(badge.text, end="\n")
-
-                if elm.attrib["class"] == "cxl-ref":
-                    text = list(elm.itertext())
-                    print_meaning_content(": ", end="")
-                    for t in text:
-                        t = t.strip()
-                        if t:
-                            print_meaning_content(t, end=" ")
+        elm_attr = elm.get("class")
+        if elm_attr is not None:
+            if "row entry-header" in elm_attr:
+                row_entry_header(elm)
+                continue
 
-        except:
-            continue
+            if elm_attr == "row headword-row header-ins":
+                row_headword_row_header_ins(elm)
+                continue
+
+            if elm_attr == "row headword-row header-vrs":
+                row_headword_row_header_vrs(elm)
+                continue
+
+            if elm_attr == "vg":
+                vg(elm)
+                continue
+
+            if "entry-uros" in elm_attr:
+                for i in elm.iterchildren():
+                    entry_uros(i)
+                    print()
+                continue
+
+            if elm_attr == "dxnls":
+                dxnls(elm)
+                continue
+
+            if elm_attr == "mt-3":
+                badge = elm.getchildren()[0] # class "lbs badge mw-badge-gray-100 text-start text-wrap d-inline"
+                print_header_badge(badge.text, end="\n")
+                continue
+
+            if elm_attr == "cxl-ref":
+                text = list(elm.itertext())
+                print_meaning_content(": ", end="")
+                for t in text:
+                    t = t.strip()
+                    if t:
+                        print_meaning_content(t, end=" ")
+                print()
+                continue
 
 
 ##############################
 # --- print abstractions --- #
 ##############################
 
 def print_meaning_badge(text, end=" "):
```

### Comparing `cambridge-3.9.8/cambridge/errors.py` & `cambridge-3.9.9/cambridge/errors.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/log.py` & `cambridge-3.9.9/cambridge/log.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/main.py` & `cambridge-3.9.9/cambridge/main.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/cambridge/utils.py` & `cambridge-3.9.9/cambridge/utils.py`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/pyproject.toml` & `cambridge-3.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/screenshots/cambridge.png` & `cambridge-3.9.9/screenshots/cambridge.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/screenshots/fzf.png` & `cambridge-3.9.9/screenshots/fzf.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/screenshots/webster.png` & `cambridge-3.9.9/screenshots/webster.png`

 * *Files identical despite different names*

### Comparing `cambridge-3.9.8/PKG-INFO` & `cambridge-3.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cambridge
-Version: 3.9.8
+Version: 3.9.9
 Summary: cambridge is a terminal version of Cambridge Dictionary.
 Home-page: https://github.com/KateWang2016/cambridge
 Keywords: dictionary, cambridge, webster, English, web scraping, python
 Author: Kate Wang
 Author-email: kate.wang2018@gmail.com
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

