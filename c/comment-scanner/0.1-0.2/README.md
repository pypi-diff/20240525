# Comparing `tmp/comment_scanner-0.1.tar.gz` & `tmp/comment_scanner-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comment_scanner-0.1.tar", last modified: Sat May 25 09:20:37 2024, max compression
+gzip compressed data, was "comment_scanner-0.2.tar", last modified: Sat May 25 12:14:39 2024, max compression
```

## Comparing `comment_scanner-0.1.tar` & `comment_scanner-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-25 09:20:37.659173 comment_scanner-0.1/
--rw-rw-rw-   0        0        0      254 2024-05-25 09:20:37.659173 comment_scanner-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-03-03 16:55:29.000000 comment_scanner-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-25 09:20:37.585355 comment_scanner-0.1/comment_scanner/
--rw-rw-rw-   0        0        0       75 2024-05-25 09:18:24.000000 comment_scanner-0.1/comment_scanner/__init__.py
--rw-rw-rw-   0        0        0     3458 2024-05-25 09:18:28.000000 comment_scanner-0.1/comment_scanner/comment_scanner.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:20:37.651455 comment_scanner-0.1/comment_scanner/parsers/
--rw-rw-rw-   0        0        0        0 2024-02-29 17:55:20.000000 comment_scanner-0.1/comment_scanner/parsers/__init__.py
--rw-rw-rw-   0        0        0     2528 2024-05-25 09:18:31.000000 comment_scanner-0.1/comment_scanner/parsers/c_parser.py
--rw-rw-rw-   0        0        0     1542 2024-05-24 15:51:48.000000 comment_scanner-0.1/comment_scanner/parsers/common.py
--rw-rw-rw-   0        0        0     3643 2024-05-25 09:18:32.000000 comment_scanner-0.1/comment_scanner/parsers/js_parser.py
--rw-rw-rw-   0        0        0     2709 2024-05-25 09:18:33.000000 comment_scanner-0.1/comment_scanner/parsers/python_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-25 09:20:37.634430 comment_scanner-0.1/comment_scanner.egg-info/
--rw-rw-rw-   0        0        0      254 2024-05-25 09:20:36.000000 comment_scanner-0.1/comment_scanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-25 09:20:36.000000 comment_scanner-0.1/comment_scanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-25 09:20:36.000000 comment_scanner-0.1/comment_scanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-25 09:20:36.000000 comment_scanner-0.1/comment_scanner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-25 09:20:36.000000 comment_scanner-0.1/comment_scanner.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       25 2024-05-25 09:20:36.000000 comment_scanner-0.1/comment_scanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-25 09:20:36.000000 comment_scanner-0.1/comment_scanner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-25 09:20:37.659173 comment_scanner-0.1/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-25 09:19:54.000000 comment_scanner-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:14:39.092556 comment_scanner-0.2/
+-rw-rw-rw-   0        0        0     3729 2024-05-25 12:14:39.092556 comment_scanner-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3473 2024-05-25 12:12:46.000000 comment_scanner-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-25 12:14:38.954103 comment_scanner-0.2/comment_scanner/
+-rw-rw-rw-   0        0        0       89 2024-05-25 09:29:08.000000 comment_scanner-0.2/comment_scanner/__init__.py
+-rw-rw-rw-   0        0        0     3447 2024-05-25 10:45:57.000000 comment_scanner-0.2/comment_scanner/comment_scanner.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:14:39.084623 comment_scanner-0.2/comment_scanner/parsers/
+-rw-rw-rw-   0        0        0        0 2024-02-29 17:55:20.000000 comment_scanner-0.2/comment_scanner/parsers/__init__.py
+-rw-rw-rw-   0        0        0     2528 2024-05-25 09:18:31.000000 comment_scanner-0.2/comment_scanner/parsers/c_parser.py
+-rw-rw-rw-   0        0        0     1543 2024-05-25 12:13:22.000000 comment_scanner-0.2/comment_scanner/parsers/common.py
+-rw-rw-rw-   0        0        0     3643 2024-05-25 09:18:32.000000 comment_scanner-0.2/comment_scanner/parsers/js_parser.py
+-rw-rw-rw-   0        0        0     2709 2024-05-25 09:18:33.000000 comment_scanner-0.2/comment_scanner/parsers/python_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-25 12:14:39.035040 comment_scanner-0.2/comment_scanner.egg-info/
+-rw-rw-rw-   0        0        0     3729 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-25 09:20:36.000000 comment_scanner-0.2/comment_scanner.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       25 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-25 12:14:38.000000 comment_scanner-0.2/comment_scanner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-25 12:14:39.092556 comment_scanner-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      758 2024-05-25 12:13:59.000000 comment_scanner-0.2/setup.py
```

### Comparing `comment_scanner-0.1/comment_scanner/comment_scanner.py` & `comment_scanner-0.2/comment_scanner/comment_scanner.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             parser = MIME_MAP[mime]
             return parser.extract_comments(code.read())
         except common.Error as e:
             raise ParseError() from e
 
 
 def fetch_from_str(code: str, mime: Optional[str] = None
-                              ) -> List[common.Comment]:
+                   ) -> List[common.Comment]:
     """Extracts and returns comments from the given string
 
     Args:
       code: String      containing code to extract comments from
       mime: Optional MIME type for code (str).
     Returns:
       Python list of parsers.common.Comment in the order that they appear in the code
```

### Comparing `comment_scanner-0.1/comment_scanner/parsers/c_parser.py` & `comment_scanner-0.2/comment_scanner/parsers/c_parser.py`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.1/comment_scanner/parsers/common.py` & `comment_scanner-0.2/comment_scanner/parsers/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,11 +43,11 @@
         return self._line_number
 
     def is_multiline(self) -> bool:
         """Returns whether this comment was a multiline comment."""
         return self._multiline
 
     def __str__(self) -> str:
-        return self.text
+        return self._text
 
     def __repr__(self) -> str:
         return f'Comment({self._text}, {self._line_number}, {self._multiline})'
```

### Comparing `comment_scanner-0.1/comment_scanner/parsers/js_parser.py` & `comment_scanner-0.2/comment_scanner/parsers/js_parser.py`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.1/comment_scanner/parsers/python_parser.py` & `comment_scanner-0.2/comment_scanner/parsers/python_parser.py`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.1/comment_scanner.egg-info/SOURCES.txt` & `comment_scanner-0.2/comment_scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `comment_scanner-0.1/setup.py` & `comment_scanner-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md') as readme_file:
         return readme_file.read()
 
 
 setup(
     name='comment_scanner',
-    version='0.1',
+    version='0.2',
     install_requires=[
         'python-magic-bin>=0.4.14',
     ],
     description='Parse comments from various source code files',
     author='Faiz Alam',
     author_email='mohdfaizalam53@gmail.com',
     license='MIT',
```

