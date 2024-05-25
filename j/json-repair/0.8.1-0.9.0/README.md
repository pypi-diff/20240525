# Comparing `tmp/json_repair-0.8.1.tar.gz` & `tmp/json_repair-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_repair-0.8.1.tar", last modified: Mon Feb 12 09:34:55 2024, max compression
+gzip compressed data, was "json_repair-0.9.0.tar", last modified: Sat Feb 24 16:11:25 2024, max compression
```

## Comparing `json_repair-0.8.1.tar` & `json_repair-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:34:55.980186 json_repair-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-12 09:34:46.000000 json_repair-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-12 09:34:55.980186 json_repair-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-02-12 09:34:46.000000 json_repair-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-12 09:34:46.000000 json_repair-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 09:34:55.980186 json_repair-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:34:55.980186 json_repair-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:34:55.980186 json_repair-0.8.1/src/json_repair/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-12 09:34:46.000000 json_repair-0.8.1/src/json_repair/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13263 2024-02-12 09:34:46.000000 json_repair-0.8.1/src/json_repair/json_repair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:34:55.980186 json_repair-0.8.1/src/json_repair.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-12 09:34:55.000000 json_repair-0.8.1/src/json_repair.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-12 09:34:55.000000 json_repair-0.8.1/src/json_repair.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 09:34:55.000000 json_repair-0.8.1/src/json_repair.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-12 09:34:55.000000 json_repair-0.8.1/src/json_repair.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 09:34:55.980186 json_repair-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9270 2024-02-12 09:34:46.000000 json_repair-0.8.1/tests/test_json_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-02-12 09:34:46.000000 json_repair-0.8.1/tests/test_performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:11:25.110144 json_repair-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-24 16:11:14.000000 json_repair-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-24 16:11:25.110144 json_repair-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-02-24 16:11:14.000000 json_repair-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-02-24 16:11:14.000000 json_repair-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 16:11:25.110144 json_repair-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:11:25.106144 json_repair-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:11:25.106144 json_repair-0.9.0/src/json_repair/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-24 16:11:14.000000 json_repair-0.9.0/src/json_repair/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13373 2024-02-24 16:11:14.000000 json_repair-0.9.0/src/json_repair/json_repair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:11:25.110144 json_repair-0.9.0/src/json_repair.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-24 16:11:25.000000 json_repair-0.9.0/src/json_repair.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-24 16:11:25.000000 json_repair-0.9.0/src/json_repair.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 16:11:25.000000 json_repair-0.9.0/src/json_repair.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-24 16:11:25.000000 json_repair-0.9.0/src/json_repair.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:11:25.110144 json_repair-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-02-24 16:11:14.000000 json_repair-0.9.0/tests/test_json_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20554 2024-02-24 16:11:14.000000 json_repair-0.9.0/tests/test_performance.py
```

### Comparing `json_repair-0.8.1/LICENSE` & `json_repair-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `json_repair-0.8.1/PKG-INFO` & `json_repair-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_repair
-Version: 0.8.1
+Version: 0.9.0
 Summary: A package to repair broken json strings
 Author-email: Stefano Baccianella <4247706+mangiucugna@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Stefano Baccianella
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `json_repair-0.8.1/README.md` & `json_repair-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `json_repair-0.8.1/pyproject.toml` & `json_repair-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "json_repair"
-version = "0.8.1"
+version = "0.9.0"
 license = {file = "LICENSE"}
 authors = [
   { name="Stefano Baccianella", email="4247706+mangiucugna@users.noreply.github.com" },
 ]
 description = "A package to repair broken json strings"
 keywords = ["JSON", "REPAIR", "LLM", "PARSER"]
 readme = "README.md"
```

### Comparing `json_repair-0.8.1/src/json_repair/json_repair.py` & `json_repair-0.9.0/src/json_repair/json_repair.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,21 +241,24 @@
         number_chars = set("0123456789-.eE")
         char = self.get_char_at()
         while char and char in number_chars:
             number_str += char
             self.index += 1
             char = self.get_char_at()
         if number_str:
-            if "." in number_str or "e" in number_str or "E" in number_str:
-                return float(number_str)
-            elif number_str == "-":
-                # If there is a stray "-" this will throw an exception, throw away this character
-                return self.parse_json()
-            else:
-                return int(number_str)
+            try:
+                if "." in number_str or "e" in number_str or "E" in number_str:
+                    return float(number_str)
+                elif number_str == "-":
+                    # If there is a stray "-" this will throw an exception, throw away this character
+                    return self.parse_json()
+                else:
+                    return int(number_str)
+            except ValueError:
+                return number_str
         else:
             # This is a string then
             return self.parse_string()
 
     def parse_boolean_or_null(self) -> Union[bool, str, None]:
         # <boolean> is one of the literal strings 'true', 'false', or 'null' (unquoted)
         boolean_map = {"true": (True, 4), "false": (False, 5), "null": (None, 4)}
```

### Comparing `json_repair-0.8.1/src/json_repair.egg-info/PKG-INFO` & `json_repair-0.9.0/src/json_repair.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_repair
-Version: 0.8.1
+Version: 0.9.0
 Summary: A package to repair broken json strings
 Author-email: Stefano Baccianella <4247706+mangiucugna@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Stefano Baccianella
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `json_repair-0.8.1/tests/test_json_repair.py` & `json_repair-0.9.0/tests/test_json_repair.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,14 +187,18 @@
 
     # Test with whitespace
     assert repair_json(' { "key" : "value" } ') == '{"key": "value"}'
 
     # Test with null values
     assert repair_json('{"key": null}') == '{"key": null}'
 
+    # Test with numeric-like values
+    assert repair_json('{"key": 10-20}') == '{"key": "10-20"}'
+    assert repair_json('{"key": 1.1.1}') == '{"key": "1.1.1"}'
+
 
 def test_repair_json_corner_cases_generate_by_gpt_with_objects():
     # Test with nested JSON
     assert repair_json('{"key1": {"key2": [1, 2, 3]}}', True) == {
         "key1": {"key2": [1, 2, 3]}
     }
     assert repair_json('{"key1": {"key2": [1, 2, 3', True) == {
@@ -217,12 +221,16 @@
 
     # Test with whitespace
     assert repair_json(' { "key" : "value" } ', True) == {"key": "value"}
 
     # Test with null values
     assert repair_json('{"key": null}', True) == {"key": None}
 
+    # Test with numeric-like values
+    assert repair_json('{"key": 10-20}', True) == {"key": "10-20"}
+    assert repair_json('{"key": 1.1.1}', True) == {"key": "1.1.1"}
+
 def test_repair_json_skip_json_loads():
     assert repair_json('{"key": true, "key2": false, "key3": null}', skip_json_loads=True) == '{"key": true, "key2": false, "key3": null}'
     assert repair_json('{"key": true, "key2": false, "key3": null}', return_objects=True, skip_json_loads=True) == {"key": True, "key2": False, "key3": None}
     assert repair_json('{"key": true, "key2": false, "key3": }', skip_json_loads=True) == '{"key": true, "key2": false, "key3": ""}'
     assert repair_json('{"key": true, "key2": false, "key3": }', return_objects=True, skip_json_loads=True) == {"key": True, "key2": False, "key3": ""}
```

### Comparing `json_repair-0.8.1/tests/test_performance.py` & `json_repair-0.9.0/tests/test_performance.py`

 * *Files identical despite different names*

