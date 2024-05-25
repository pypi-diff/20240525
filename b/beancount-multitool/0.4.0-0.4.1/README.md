# Comparing `tmp/beancount_multitool-0.4.0.tar.gz` & `tmp/beancount_multitool-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_multitool-0.4.0.tar", max compression
+gzip compressed data, was "beancount_multitool-0.4.1.tar", max compression
```

## Comparing `beancount_multitool-0.4.0.tar` & `beancount_multitool-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.4.0/LICENSE
--rw-r--r--   0        0        0     2696 2024-05-24 04:29:10.491065 beancount_multitool-0.4.0/README.md
--rw-r--r--   0        0        0     1772 2024-05-24 03:24:29.912035 beancount_multitool-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      182 2024-05-23 01:27:44.241769 beancount_multitool-0.4.0/src/beancount_multitool/Institution.py
--rw-r--r--   0        0        0     5284 2024-05-24 04:10:42.855202 beancount_multitool-0.4.0/src/beancount_multitool/JABank.py
--rw-r--r--   0        0        0     2268 2024-05-24 03:31:45.263121 beancount_multitool-0.4.0/src/beancount_multitool/MappingDatabase.py
--rw-r--r--   0        0        0     4480 2024-05-24 03:32:40.768342 beancount_multitool-0.4.0/src/beancount_multitool/RakutenBank.py
--rw-r--r--   0        0        0     4781 2024-05-24 03:32:40.768228 beancount_multitool-0.4.0/src/beancount_multitool/RakutenCard.py
--rw-r--r--   0        0        0     5154 2024-05-24 04:06:12.816630 beancount_multitool-0.4.0/src/beancount_multitool/ShinseiBank.py
--rw-r--r--   0        0        0      454 2024-05-19 23:39:41.029470 beancount_multitool-0.4.0/src/beancount_multitool/__init__.py
--rw-r--r--   0        0        0      120 2024-05-20 00:15:30.523620 beancount_multitool-0.4.0/src/beancount_multitool/__main__.py
--rw-r--r--   0        0        0       22 2024-05-24 03:24:20.721033 beancount_multitool-0.4.0/src/beancount_multitool/__version__.py
--rw-r--r--   0        0        0     1475 2024-05-24 04:17:14.821049 beancount_multitool-0.4.0/src/beancount_multitool/as_transaction.py
--rw-r--r--   0        0        0     1684 2024-05-23 14:57:04.901452 beancount_multitool-0.4.0/src/beancount_multitool/cli.py
--rw-r--r--   0        0        0      421 2024-05-24 04:13:04.378795 beancount_multitool-0.4.0/src/beancount_multitool/get_beancount_config.py
--rw-r--r--   0        0        0      557 2024-05-24 03:18:42.671213 beancount_multitool-0.4.0/src/beancount_multitool/get_value.py
--rw-r--r--   0        0        0      654 2024-05-24 03:57:41.742099 beancount_multitool-0.4.0/src/beancount_multitool/read_config.py
--rw-r--r--   0        0        0      380 2024-05-24 04:16:15.921218 beancount_multitool-0.4.0/src/beancount_multitool/tests/test_get_beancount_config.py
--rw-r--r--   0        0        0      536 2024-05-24 04:02:22.544032 beancount_multitool-0.4.0/src/beancount_multitool/tests/test_get_value.py
--rw-r--r--   0        0        0      231 2024-05-24 03:52:22.609021 beancount_multitool-0.4.0/src/beancount_multitool/tests/test_read_config.py
--rw-r--r--   0        0        0     4052 1970-01-01 00:00:00.000000 beancount_multitool-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-05-13 10:19:52.000000 beancount_multitool-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1277 2024-05-25 12:35:01.002912 beancount_multitool-0.4.1/README.md
+-rw-r--r--   0        0        0     1834 2024-05-25 12:32:16.709954 beancount_multitool-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      182 2024-05-23 01:27:44.241769 beancount_multitool-0.4.1/src/beancount_multitool/Institution.py
+-rw-r--r--   0        0        0     5284 2024-05-24 04:10:42.855202 beancount_multitool-0.4.1/src/beancount_multitool/JABank.py
+-rw-r--r--   0        0        0     2268 2024-05-25 12:26:23.651681 beancount_multitool-0.4.1/src/beancount_multitool/MappingDatabase.py
+-rw-r--r--   0        0        0     4480 2024-05-24 03:32:40.768342 beancount_multitool-0.4.1/src/beancount_multitool/RakutenBank.py
+-rw-r--r--   0        0        0     4781 2024-05-24 03:32:40.768228 beancount_multitool-0.4.1/src/beancount_multitool/RakutenCard.py
+-rw-r--r--   0        0        0     5154 2024-05-24 04:06:12.816630 beancount_multitool-0.4.1/src/beancount_multitool/ShinseiBank.py
+-rw-r--r--   0        0        0      454 2024-05-19 23:39:41.029470 beancount_multitool-0.4.1/src/beancount_multitool/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-20 00:15:30.523620 beancount_multitool-0.4.1/src/beancount_multitool/__main__.py
+-rw-r--r--   0        0        0       22 2024-05-25 12:32:24.421178 beancount_multitool-0.4.1/src/beancount_multitool/__version__.py
+-rw-r--r--   0        0        0     1567 2024-05-25 09:42:51.099454 beancount_multitool-0.4.1/src/beancount_multitool/as_transaction.py
+-rw-r--r--   0        0        0     1684 2024-05-23 14:57:04.901452 beancount_multitool-0.4.1/src/beancount_multitool/cli.py
+-rw-r--r--   0        0        0      421 2024-05-24 04:13:04.378795 beancount_multitool-0.4.1/src/beancount_multitool/get_beancount_config.py
+-rw-r--r--   0        0        0      557 2024-05-24 03:18:42.671213 beancount_multitool-0.4.1/src/beancount_multitool/get_value.py
+-rw-r--r--   0        0        0      654 2024-05-24 03:57:41.742099 beancount_multitool-0.4.1/src/beancount_multitool/read_config.py
+-rw-r--r--   0        0        0      387 2024-05-24 07:53:23.172781 beancount_multitool-0.4.1/src/beancount_multitool/tests/test_get_beancount_config.py
+-rw-r--r--   0        0        0      553 2024-05-24 07:53:56.206848 beancount_multitool-0.4.1/src/beancount_multitool/tests/test_get_value.py
+-rw-r--r--   0        0        0      237 2024-05-24 07:53:33.405873 beancount_multitool-0.4.1/src/beancount_multitool/tests/test_read_config.py
+-rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 beancount_multitool-0.4.1/PKG-INFO
```

### Comparing `beancount_multitool-0.4.0/LICENSE` & `beancount_multitool-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/pyproject.toml` & `beancount_multitool-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-multitool"
-version = "0.4.0"
+version = "0.4.1"
 description = "A CLI tool that converts financial data to Beancount files"
 authors = ["Rick Lan <rlan@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rlan/beancount-multitool"
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -27,14 +27,15 @@
 click = "^8.1.7"
 tomli = { version = "^2.0.1", python = "<3.11" }
 tqdm = "^4.66.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0"
 pytest-cov = "^4.0"
+mkdocs-material = {extras = ["imaging"], version = "^9.5.24"}
 
 [tool.poetry.scripts]
 bean-mt = "beancount_multitool.cli:main"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
```

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/JABank.py` & `beancount_multitool-0.4.1/src/beancount_multitool/JABank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/MappingDatabase.py` & `beancount_multitool-0.4.1/src/beancount_multitool/MappingDatabase.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/RakutenBank.py` & `beancount_multitool-0.4.1/src/beancount_multitool/RakutenBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/RakutenCard.py` & `beancount_multitool-0.4.1/src/beancount_multitool/RakutenCard.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/ShinseiBank.py` & `beancount_multitool-0.4.1/src/beancount_multitool/ShinseiBank.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/as_transaction.py` & `beancount_multitool-0.4.1/src/beancount_multitool/as_transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,8 +52,10 @@
 
     output = "\n"
     output += f'{date.strftime("%Y-%m-%d")} * "{payee}" "{narration}"{tags_str}\n'
     for key, value in metadata.items():
         output += f'  {key}: "{value}"\n'
     output += f"  {source_account}\n"
     output += f"  {flag_str}{account}  {amount} {currency}\n"
+    for key, value in account_metadata.items():
+        output += f'    {key}: "{value}"\n'
     return output
```

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/cli.py` & `beancount_multitool-0.4.1/src/beancount_multitool/cli.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/get_value.py` & `beancount_multitool-0.4.1/src/beancount_multitool/get_value.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/read_config.py` & `beancount_multitool-0.4.1/src/beancount_multitool/read_config.py`

 * *Files identical despite different names*

### Comparing `beancount_multitool-0.4.0/src/beancount_multitool/tests/test_get_value.py` & `beancount_multitool-0.4.1/src/beancount_multitool/tests/test_get_value.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from beancount_multitool.get_value import get_value
 
 
 def test_get_value():
-    x = {"section": {"variable" : "value"}}
+    x = {"section": {"variable": "value"}}
 
     # okay
     assert get_value(x, "section", "variable") == "value"
 
     # variable does not exist
     try:
         get_value(x, "section", "unknown")
     except KeyError as e:
         print(e)
         assert True
     else:
-        assert False
+        assert AssertionError
 
     # section does not exist
     try:
         get_value(x, "unknown", "")
     except KeyError as e:
         print(e)
         assert True
     else:
-        assert False
+        assert AssertionError
```

